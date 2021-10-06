<script>
    import SectionTitle from './components/SectionTitle.svelte';
    import ProjectSlide from './components/ProjectSlide.svelte';

    let svgSize = 16;
    if (window.innerWidth >= 1024) {
        svgSize = 20;
    }
</script>

<section>
    {#if window.innerWidth >= 768}
        <svg id="big-wave" viewBox="0 0 1440 66" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M0 28.8L34.3 27.2597C68.6 25.6031 137 22.6969 206 19.5C274.3 16.3031 343 13.3969 411 10.2C480 7.00313 549 4.09688 617 5.55C685.7 7.00313 754 13.3969 823 22.6097C891.4 31.9969 960 44.2031 1029 52.05C1097.1 59.8969 1166 62.8031 1234 53.5903C1302.9 44.2031 1371 22.6969 1406 11.7403L1440 0.900002V66H1405.7C1371.4 66 1303 66 1234 66C1165.7 66 1097 66 1029 66C960 66 891 66 823 66C754.3 66 686 66 617 66C548.6 66 480 66 411 66C342.9 66 274 66 206 66C137.1 66 69 66 34 66H0V28.8Z" fill="#DBE4EE"/>
        </svg>
    {:else}
        <svg id="wave" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
            <path fill="#DBE4EE" fill-opacity="1" d="M0,192L34.3,186.7C68.6,181,137,171,206,160C274.3,149,343,139,411,128C480,117,549,107,617,112C685.7,117,754,139,823,170.7C891.4,203,960,245,1029,272C1097.1,299,1166,309,1234,277.3C1302.9,245,1371,171,1406,133.3L1440,96L1440,320L1405.7,320C1371.4,320,1303,320,1234,320C1165.7,320,1097,320,1029,320C960,320,891,320,823,320C754.3,320,686,320,617,320C548.6,320,480,320,411,320C342.9,320,274,320,206,320C137.1,320,69,320,34,320L0,320Z"></path>
        </svg>
    {/if}        
    <div class="projects">
        <SectionTitle titleName="PROJECTS"/>
        <div class="carousel">
            <ProjectSlide projectName="Carpool App" 
                          githubLink="https://github.com/byteMe-CSULB/710" 
                          backgroundLink="/images/710.png" />
            <ProjectSlide projectName="Server Match" 
                          githubLink="https://github.com/CECS-445-Project/ServerMatch"
                          backgroundLink="/images/server_match.png" />
            <ProjectSlide projectName="Tip Splitter" 
                          githubLink="https://github.com/brandonnhem/Tip-Calculator"
                          liveLink="https://brandonnhem.github.io/Tip-Calculator/"
                          backgroundLink="/images/splitter.png" />
            <ProjectSlide projectName="Github Grabber"
                          githubLink="https://github.com/brandonnhem/github-profile-grabber"
                          liveLink="https://github-grabber.vercel.app/" 
                          backgroundLink="/images/github_grabber.png" />
            <ProjectSlide projectName="Price Adjuster"
                          githubLink="https://github.com/brandonnhem/interactive-pricing-component-challenge"
                          liveLink="https://interactive-pricing-component-challenge.vercel.app/" 
                          backgroundLink="/images/interactive_pricing.png" />
            <ProjectSlide projectName="Simon Game" 
                          githubLink="https://github.com/brandonnhem/SimonGame"
                          liveLink="https://brandonnhem.github.io/SimonGame/" 
                          backgroundLink="/images/simon.png" />
        </div>
        <a class="cta-btn" href="https://github.com/brandonnhem/">
            <p>View More</p>
            <svg id="arrow" width="{svgSize}" height="{svgSize}" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M12 22C6.47967 21.9939 2.00606 17.5203 2 12V11.8C2.10993 6.30453 6.63459 1.92796 12.1307 2.00088C17.6268 2.07381 22.0337 6.56889 21.9978 12.0653C21.9619 17.5618 17.4966 21.9989 12 22ZM12 4C7.58172 4 4 7.58172 4 12C4 16.4183 7.58172 20 12 20C16.4183 20 20 16.4183 20 12C19.995 7.58378 16.4162 4.00496 12 4ZM10.55 17L9.136 15.585L12.671 12.05L9.136 8.515L10.55 7.1L15.5 12.05L10.551 17H10.55Z" fill="#FFFFFF"></path>
            </svg>
        </a>
    </div>
</section>

<style>
    .projects {
        padding: 0 1rem;
        background-color: var(--project-bg-color);
        height: 22.0625rem;
        z-index: 1;
    }

    section {
        position: relative;
        margin-top: 4.875rem;
    }

    #wave {
        position: absolute;
        top: -4.875rem;
        z-index: -1;
    }

    .carousel {
        padding-top: 1.8125rem;
        display: flex;
        flex-direction: row;
        position: relative;
        overflow-x: scroll;
        overflow-y: hidden;
    }

    .carousel::-webkit-scrollbar {
        width: 20px;
    }
    
    .carousel::-webkit-scrollbar-track {
        background-color: transparent;
    }
    
    .carousel::-webkit-scrollbar-thumb {
        background-color: rgb(185, 189, 190);
        border-radius: 20px;
        border: 6px solid transparent;
        background-clip: content-box;
    }
    
    .carousel::-webkit-scrollbar-thumb:hover {
        background-color: rgb(153, 167, 170);
    }

    .cta-btn {
        background-color: var(--icon-color);
        color: hsl(100, 100%, 100%);
        border-radius: 0.9375rem;
        padding: 0.5rem;
        display: inline-flex;
        justify-content: flex-start;
        align-content: center;
        margin: 0.8125rem 2rem 1rem 12.0625rem;
    }

    p {
        display: inline-block;
    }

    #arrow {
        margin: 0.125rem 0 0 0.375rem;
    }

    a {
        text-decoration: none;
        color: hsl(100, 100%, 100%);
    }

    @media only screen
           and (device-width: 360px)
           and (device-height: 640px) {
        .projects {
            padding: 0 1rem 1rem;
        }

        .cta-btn {
            margin: 0.8125rem 2rem 1rem 11.0625rem;
        }
    }

    @media only screen and (min-width: 375px) and (min-height: 667px) {
        .projects {
            padding: 0 1rem 1rem;
        }
    }

    @media only screen and (min-width: 393px) {
        .cta-btn {
            margin: 0.8125rem 2rem 1rem 13.5625rem;
            width: max-content;
        }

        #wave {
            top: -5.3125rem;
        }
    }

    @media only screen and (min-width: 411px) {
        .projects {
            padding: 0 1rem 1rem;
        }

        .cta-btn {
            margin: 0.8125rem 2rem 1rem 14.0625rem;
        }

        #wave {
            top: -5.375rem;
        }
    }

    @media only screen and (min-width: 768px) {
        #big-wave {
            position: absolute;
            top: -2.2rem;
            z-index: -1;
        }

        .projects {
            padding: 0 3rem 1rem;
        }

        .cta-btn {
            margin: 0.8125rem 2rem 1rem 32.875rem;
        }
    }

    @media only screen 
           and (min-width: 1024px)
           and (min-height: 1366px) {
        #big-wave {
            position: absolute;
            top: -2.9rem;
            z-index: -1;
        }

        section {
            margin-top: 13.5rem;
        }

        .projects {
            padding: 4rem 3.5rem;
        }

        .carousel {
            margin-left: 1.5rem;
        }

        .cta-btn {
            margin-left: 48rem;
        }
    }

    @media only screen 
           and (min-width: 800px) 
           and (min-height: 1112px) {
        #wave {
            top: -10.4rem;
        }

        .carousel {
            margin-left: 1.5rem;
        }
    }

    @media only screen 
           and (min-width: 1024px) 
           and (min-height: 768px) {
        #wave {
            top: -13.275rem;
        }

        .carousel {
            margin-left: 1.5rem;
        }

        .cta-btn {
            margin: 0.8125rem 2rem 1rem 44.875rem;
        }
    }

    @media only screen and (min-width: 1024px) {
        #big-wave {
            position: absolute;
            top: -2.9rem;
            z-index: -1;
        }   

        .projects {
            padding: 0 13rem 5rem;
        }

        .cta-btn {
            margin: 0.8125rem 2rem 1rem 27.875rem;
        }

        p {
            font-size: 1.25rem;
        }
    }

    @media only screen and (min-width: 1024px) and (min-height: 1366px) {
        .projects {
            padding: 0 13rem 5.5rem;
        }
    }

    @media only screen and (min-width: 1280px) and (min-height: 632px) {
        #wave {
            top: -16.575rem;
        }

        .projects {
            padding: 0 13rem 3.5rem;
        }

        .cta-btn {
            margin: 0.8125rem 2rem 1rem 42.875rem;
        }

        .carousel {
            margin-left: 1.5rem;
        }
    }

    @media only screen and (min-width: 1366px) and (min-height: 1024px) {
        #big-wave {
            top: -3.6rem;
        }

        .projects {
            padding: 0 13rem 5rem;
        }

        .cta-btn {
            margin: 0.8125rem 2rem 1rem 42.875rem;
        }
    }

    @media only screen and (min-width: 1440px) {
        #big-wave {
            top: -3.8rem;
        }

        .cta-btn {
            margin: 0.8125rem 2rem 1rem 54.875rem;
            border-radius: 2rem;
            padding: 0.8rem;
        }

        .projects {
            padding: 0 13rem 6.7rem;
        }

        p {
            font-size: 1.25rem;
        }
    }

    @media only screen and (min-width: 1632px) and (min-height: 939px) {
        #wave {
            top: -20.975rem;
        }

        .cta-btn {
            margin: 0.8125rem 2rem 1rem 66.875rem;
        }

        .projects {
            padding: 0 13rem 4.5rem;
        }
    }
</style>