<script>
    import SectionTitle from './components/SectionTitle.svelte';
</script>

<div class="about">
    <SectionTitle titleName="ABOUT" />
    <div class="blob">
        <svg width="192" height="176" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
            <path fill="#F17300" d="M36.4,-48.1C49.4,-40.7,63.7,-33,69.1,-21.3C74.6,-9.5,71.2,6.3,64.9,19.6C58.6,33,49.3,44,37.9,54.4C26.6,64.8,13.3,74.7,1.5,72.7C-10.3,70.6,-20.7,56.7,-36.3,47.6C-51.9,38.6,-72.8,34.5,-73.7,25.4C-74.6,16.3,-55.5,2.2,-49.2,-15.6C-42.9,-33.4,-49.3,-55,-43.2,-64.6C-37.1,-74.2,-18.5,-71.8,-3.4,-67.1C11.7,-62.4,23.4,-55.4,36.4,-48.1Z" transform="translate(100 100)" />
        </svg>
    </div>
    <div class="about-me">
        <p>I’m a Computer Science graduate from Cal-State Long Beach. I enjoy programming and creating apps. I’d love to be part of a team where I can apply my skills and challenge myself.</p>
        <br>
        <p>I'm well versed in a handful of languages, but consider myself a backend engineer. Currently working on refining my frontend skills so that I can become a fullstack engineer.</p>
    </div>
</div>

<style>
    .about {
        padding: 3rem 1rem;
        position: relative;
    }

    .blob {
        position: absolute;
        z-index: -1;
        top: 0;
        left: -2.875rem;
        transform: scale(1.3);
    }

    .about-me {
        background-color: var(--about-bg-color);
        width: 16.1875rem;
        height: max-content;
        padding: 0.6875rem 1.375rem;
        border-radius: 2rem 0 2rem 2rem;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-left: 2.4375rem;
    }

    @media only screen and (device-width: 280px) and (device-height: 653px) {
        .about-me {
            width: 10.3rem;
        }
    }

    /* GALAXY S5 */
    @media only screen 
           and (device-width: 360px)
           and (device-height: 640px) {
        .about-me {
            margin-left: 1.5625rem;
        }
    }
    
    @media only screen and (min-width: 393px) {
        .about-me {
            margin-left: 3.625rem;
        }
    }
    
    /* PIXEL 2 */
    @media only screen and (min-width: 411px) {
        .about-me {
            margin-left: 4.75rem;
        }
    }

    @media only screen and (min-width: 512px) and (min-height: 717px) {
        .about {
            padding: 3rem 2rem;
        }

        .about-me {
            margin-left: 3.8rem;
            width: 21.3rem;
        }
    }

    @media only screen and (min-width: 540px) and (min-height: 720px) {
        .about {
            padding: 3rem 2rem;
        }

        .about-me {
            margin-left: 3.8rem;
            width: 23.3rem;
        }
    }

    @media only screen and (min-width: 717px) and (min-height: 512px) {
        .about {
            padding: 3rem 2rem;
        }

        .about-me {
            width: 34.1875rem;
            margin-left: 4rem;
        }
    }
    
    @media only screen and (min-width: 720px) and (min-height: 540px) {
        .about {
            padding: 3rem 2rem;
        }

        .about-me {
            width: 32.1875rem;
            margin-left: 6rem;
        }
    }

    @media only screen and (min-width: 768px) {
        .about {
            padding: 3rem 3rem 0;
        }

        .about-me {
            margin-left: 3.25rem;
            width: 36rem;
        }

        .blob {
            transform: scale(1.5);
            top: -1rem;
            left: -3rem;
        }

        p {
            font-size: 1.25rem;
        }
    }

    @media only screen and (min-width: 800px) and (min-height: 112px) {
        .about-me {
            margin-left: 17.25rem;
        }
    }

    @media only screen 
           and (min-width: 1024px)
           and (min-height: 1366px) {

        .about {
            padding: 3rem 3.5rem;
        }

        .about-me {
            margin-left: 30rem;
        }
    }

    @media only screen and (min-width: 1024px) and (min-height: 768px) {
        .about-me {
            margin-left: 31rem;
        }
    }

    @media only screen and (min-width: 1024px) {
        .about {
            padding: 3.5rem 13rem;
        }

        .about-me {
            margin-left: 5rem;
            width: 30rem;
        }

        .blob {
            top: 1rem;
            left: 8rem;
        }
    }

    @media only screen and (min-width: 1280px) and (min-height: 632px) {
        .about {
            padding: 3.5rem 13rem;
        }

        .about-me {
            margin-left: 15rem;
        }

        .blob {
            top: 1rem;
            left: 8rem;
        }
    }

    @media only screen and (min-width: 1366px) and (min-height: 1024px) {
        .about {
            padding: 3.5rem 13rem;
        }

        .about-me {
            margin-left: 31rem;
        }

        .blob {
            top: 1rem;
            left: 8rem;
        }
    }

    @media only screen and (min-width: 1440px) {
        .about-me {
            margin-left: 22rem;
            width: 39rem;
        }

        p {
            font-size: 1.25rem;
        }
    }

    @media only screen and (min-width: 1632px) and (min-height: 939px) {
        .about-me {
            margin-left: 23rem;
            width: 48rem;
        }
    }
</style>