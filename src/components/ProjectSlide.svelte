<script>
    export let projectName;
    export let githubLink;
    export let liveLink;
    export let backgroundLink;
    let svgSize = 20;
    if (window.innerWidth >= 1024) {
        svgSize = 30;
    }
</script>

<div class="project-slide" style="background-image: linear-gradient(180deg, rgba(0, 0, 0, 0.175) 0%, rgba(0, 0, 0, 0.7) 100%), url({backgroundLink});">
    <h2>{projectName}</h2>
    
    {#if liveLink !== undefined}
        <div class="links">
            <a href="{liveLink}">
                <svg width="{svgSize}" height="{svgSize}" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M17.001 20H6.00098C4.89641 20 4.00098 19.1046 4.00098 18V7C4.00098 5.89543 4.89641 5 6.00098 5H10.001V7H6.00098V18H17.001V14H19.001V18C19.001 19.1046 18.1055 20 17.001 20ZM11.701 13.707L10.291 12.293L16.584 6H13.001V4H20.001V11H18.001V7.415L11.701 13.707Z" fill="#FFFFFF"></path>
                </svg>
            </a>
            <a href="{githubLink}">
                <svg width="{svgSize}" height="{svgSize}" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M12.026 2C7.13295 1.99937 2.96183 5.54799 2.17842 10.3779C1.395 15.2079 4.23061 19.893 8.87302 21.439C9.37302 21.529 9.55202 21.222 9.55202 20.958C9.55202 20.721 9.54402 20.093 9.54102 19.258C6.76602 19.858 6.18002 17.92 6.18002 17.92C5.99733 17.317 5.60459 16.7993 5.07302 16.461C4.17302 15.842 5.14202 15.856 5.14202 15.856C5.78269 15.9438 6.34657 16.3235 6.66902 16.884C6.94195 17.3803 7.40177 17.747 7.94632 17.9026C8.49087 18.0583 9.07503 17.99 9.56902 17.713C9.61544 17.207 9.84055 16.7341 10.204 16.379C7.99002 16.128 5.66202 15.272 5.66202 11.449C5.64973 10.4602 6.01691 9.5043 6.68802 8.778C6.38437 7.91731 6.42013 6.97325 6.78802 6.138C6.78802 6.138 7.62502 5.869 9.53002 7.159C11.1639 6.71101 12.8882 6.71101 14.522 7.159C16.428 5.868 17.264 6.138 17.264 6.138C17.6336 6.97286 17.6694 7.91757 17.364 8.778C18.0376 9.50423 18.4045 10.4626 18.388 11.453C18.388 15.286 16.058 16.128 13.836 16.375C14.3153 16.8651 14.5612 17.5373 14.511 18.221C14.511 19.555 14.499 20.631 14.499 20.958C14.499 21.225 14.677 21.535 15.186 21.437C19.8265 19.8884 22.6591 15.203 21.874 10.3743C21.089 5.54565 16.9181 1.99888 12.026 2Z" fill="#FFFFFF"></path>
                </svg>
            </a>
        </div>
    {:else}
        <div class="links one-link">
            <a href="{githubLink}">
                <svg width="{svgSize}" height="{svgSize}" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M12.026 2C7.13295 1.99937 2.96183 5.54799 2.17842 10.3779C1.395 15.2079 4.23061 19.893 8.87302 21.439C9.37302 21.529 9.55202 21.222 9.55202 20.958C9.55202 20.721 9.54402 20.093 9.54102 19.258C6.76602 19.858 6.18002 17.92 6.18002 17.92C5.99733 17.317 5.60459 16.7993 5.07302 16.461C4.17302 15.842 5.14202 15.856 5.14202 15.856C5.78269 15.9438 6.34657 16.3235 6.66902 16.884C6.94195 17.3803 7.40177 17.747 7.94632 17.9026C8.49087 18.0583 9.07503 17.99 9.56902 17.713C9.61544 17.207 9.84055 16.7341 10.204 16.379C7.99002 16.128 5.66202 15.272 5.66202 11.449C5.64973 10.4602 6.01691 9.5043 6.68802 8.778C6.38437 7.91731 6.42013 6.97325 6.78802 6.138C6.78802 6.138 7.62502 5.869 9.53002 7.159C11.1639 6.71101 12.8882 6.71101 14.522 7.159C16.428 5.868 17.264 6.138 17.264 6.138C17.6336 6.97286 17.6694 7.91757 17.364 8.778C18.0376 9.50423 18.4045 10.4626 18.388 11.453C18.388 15.286 16.058 16.128 13.836 16.375C14.3153 16.8651 14.5612 17.5373 14.511 18.221C14.511 19.555 14.499 20.631 14.499 20.958C14.499 21.225 14.677 21.535 15.186 21.437C19.8265 19.8884 22.6591 15.203 21.874 10.3743C21.089 5.54565 16.9181 1.99888 12.026 2Z" fill="#FFFFFF"></path>
                </svg>
            </a>
        </div>
    {/if}
</div>

<style>
    .project-slide {
        width: 7.375rem;
        height: 13.9375rem;
        border-radius: 0.9375rem;
        background-size: 7.375rem 13.9375rem;
        background-repeat: no-repeat;
        margin-right: 1.875rem;
        flex-shrink: 0;
    }

    h2 {
        color: hsl(100, 100%, 100%);
        margin: 0 0.5rem;
        padding-top: 8.0625rem;
    }

    .links {
        margin: 0 0 0.75rem 3.875rem;
    }

    .one-link {
        margin: 0 0 0.75rem 5.5rem;
    }

    @media only screen and (min-width: 768px) {
        .project-slide {
            margin-right: 2.5rem;
        }
    }

    @media only screen and (min-width: 1024px) and (min-height: 1366px) {
        .project-slide {
            width: 9.5625rem;
            height: 17.9375rem;
            margin-right: 4rem;
            background-size: 9.5625rem 17.9375rem;
        }

        h2 {
            font-size: 1.5rem;
            margin: 3.5rem 1rem 0;
        }

        .links {
            margin: 0 0 1rem 5rem;
        }

        .one-link {
            margin: 0 0 1rem 7rem;
        }
    }

    @media only screen and (min-width: 1024px) and (min-height: 768px) {
        .project-slide {
            margin-right: 3.5rem;
        }
    }

    @media only screen and (min-width: 1366px) and (min-height: 1024px) {
        .project-slide {
            width: 9.5625rem;
            height: 17.9375rem;
            margin-right: 4rem;
            background-size: 9.5625rem 17.9375rem;
        }

        h2 {
            font-size: 1.5rem;
            margin: 3.5rem 1rem 0;
        }

        .links {
            margin: 0 0 1rem 5rem;
        }

        .one-link {
            margin: 0 0 1rem 7rem;
        }
    }

    @media only screen and (min-width: 1280px) and (min-height: 632px) {
        .project-slide {
            width: 9.5625rem;
            height: 17.9375rem;
            margin-right: 6rem;
            background-size: 9.5625rem 17.9375rem;
        }

        h2 {
            font-size: 1.5rem;
            margin: 3.5rem 1rem 0;
        }

        .links {
            margin: 0 0 1rem 5rem;
        }

        .one-link {
            margin: 0 0 1rem 7rem;
        }
    }

    @media only screen and (min-width: 1024px) {
        .project-slide {
            width: 9.5625rem;
            height: 17.9375rem;
            margin-right: 5rem;
            background-size: 9.5625rem 17.9375rem;
        }

        h2 {
            font-size: 1.5rem;
            margin: 3.5rem 1rem 0;
        }

        .links {
            margin: 0 0 1rem 5rem;
        }

        .one-link {
            margin: 0 0 1rem 7rem;
        }
    }

    @media only screen and (min-width: 1440px) {
        h2 {
            font-size: 2rem;
            margin: 2rem 1rem 0;
        }
    }
</style>