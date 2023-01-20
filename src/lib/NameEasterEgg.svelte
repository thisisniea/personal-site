<script lang="ts">
    const words = [
        "chia",
        "via",
        "korea",
        "tortilla",
        "pizzeria",
        "idea"
    ]

    let currentWord = 'niea';

    const homeRotate = '0deg';
    const homeSkew = '0deg';

    $: rotate = homeRotate;
    $: skew = homeSkew;
    $: scale = 1;

    $: hoverCount = 0;

    let isAnimating = false;

    function hover() {
        if (isAnimating) return;
        isAnimating = true;
        hoverCount++;

        rotate = 5 - Math.random() * 10 + 'deg';
        skew = 15 - Math.random() * 30 + 'deg';
        scale = 1.1;

        setTimeout(() => {
            rotate = homeRotate;
            skew = homeSkew;
            scale = 1;

            if (hoverCount < 5) {
                setTimeout(() => {
                    isAnimating = false;
                }, 50);
            } else {
                setTimeout(() => {
                    const lastWord = currentWord;
                    while (currentWord === lastWord)
                        currentWord = words[Math.floor(Math.random() * words.length)];

                    setTimeout(() => {
                        hoverCount = 0;
                        isAnimating = false;
                    }, 100);
                }, 100);
            }            
        }, 50);
    }
</script>

<span class={$$props.class}>
    <em class:exploding={hoverCount >= 5} on:mouseenter={hover} style={`--skew: ${skew}; --rotate: ${rotate}; --scale: ${scale}`}>{currentWord}</em>.me
</span>

<style lang="postcss">
    span {
        margin-right: auto;
        user-select: none;
        transform: skewX(-15deg);
    }

    em {
        font-weight: bold;
        font-style: italic;
        transform: skewX(var(--skew)) rotate(var(--rotate)) scale(var(--scale));
        display: inline-block;

        transition: transform 0.05s ease-in-out;
    }

    em.exploding {
        animation: explode 0.25s normal;
    }

    @keyframes explode {
        0% {
            filter: blur(0);
            opacity: 1;
        }
        10% {
            filter: blur(0px);
            opacity: 1;
        }
        30% {
            filter: blur(5px);
            opacity: 0.9;
        }
        50% {
            filter: blur(10px);
            opacity: 0;
        }
        100% {
            filter: blur(0px);
            opacity: 1;
        }
    }
</style>