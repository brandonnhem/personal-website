<header>
    <div class="intro">
        <h1>Hello! My name is</h1>
        <h1 class="h1-special">Brandon.</h1>
        <div class="blob">
            <svg width="135" height="165"viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
                <path fill="#F17300" d="M37.4,-49.5C48.7,-43.3,58.1,-32.6,61.1,-20.5C64,-8.4,60.6,5.1,56.5,18.6C52.4,32.1,47.7,45.7,38.2,52.5C28.7,59.4,14.3,59.5,3,55.4C-8.4,51.3,-16.8,43,-31.2,37.8C-45.6,32.5,-66.1,30.3,-70.2,21.8C-74.4,13.3,-62.3,-1.5,-56.8,-18.4C-51.3,-35.4,-52.3,-54.4,-43.9,-61.6C-35.6,-68.7,-17.8,-64,-2.4,-60.8C13.1,-57.5,26.2,-55.8,37.4,-49.5Z" transform="translate(100 100)" />
            </svg>
        </div>
    </div>
</header>

<style>
    header {
        display: flex;
        justify-content: center;
        overflow: hidden;
    }

    .intro {
        text-align: center;
        margin: 6rem 0 1rem;
        position: relative;
    }

    .h1-special {
        font-weight: 900;
    }

    .blob {
        position: absolute;
        top: -9.25rem;
        left: 13rem;
        transform: scale(1.5) rotate(38deg);
    }

    @media only screen and (min-width: 768px) {
        header {
            margin-bottom: 9rem;
        }

        .blob {
            top: -9rem;
            left: 24rem;
            transform: scale(1.9) rotate(38deg);
        }
    }

    @media only screen 
           and (min-width: 1024px)
           and (min-height: 1366px) {
        .blob {
            left: 32rem;
        }
    }

    @media only screen
           and (min-width: 1024px) 
           and (min-height: 768px) {
        header {
            margin-bottom: 15rem;
        }

        .blob {
            left: 33rem;
        }
    }

    @media only screen and (min-width: 1366px) and (min-height: 1024px) {
        .intro {
            margin: 10rem 0 1rem;
        }

        .blob {
            top: -12rem;
        }
    }

    @media only screen and (min-width: 1280px) and (min-height: 632px) {
        .intro {
            margin: 8rem 0 1rem;
        }

        header {
            margin-bottom: 14rem;
        }
    }
</style>