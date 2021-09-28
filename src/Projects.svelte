<script>
    import SectionTitle from './components/SectionTitle.svelte';
    import ProjectSlide from './components/ProjectSlide.svelte';
</script>

<section>
    <svg id="wave" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
        <path fill="#DBE4EE" fill-opacity="1" d="M0,192L34.3,186.7C68.6,181,137,171,206,160C274.3,149,343,139,411,128C480,117,549,107,617,112C685.7,117,754,139,823,170.7C891.4,203,960,245,1029,272C1097.1,299,1166,309,1234,277.3C1302.9,245,1371,171,1406,133.3L1440,96L1440,320L1405.7,320C1371.4,320,1303,320,1234,320C1165.7,320,1097,320,1029,320C960,320,891,320,823,320C754.3,320,686,320,617,320C548.6,320,480,320,411,320C342.9,320,274,320,206,320C137.1,320,69,320,34,320L0,320Z"></path>
    </svg>
    <div class="projects">
        <SectionTitle titleName="PROJECTS"/>
        <div class="carousel">
            <ProjectSlide projectName="Carpool App" 
                          githubLink="https://github.com/byteMe-CSULB/710" 
                          backgroundLink="/images/710.png" />
            <ProjectSlide projectName="Server Match" 
                          githubLink="https://github.com/CECS-445-Project/ServerMatch"
                          backgroundLink="/images/server_match.png" />
            <ProjectSlide projectName="Tip Calc-ulator" 
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
            <svg id="arrow" width="16" height="16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
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
        .cta-btn {
            margin: 0.8125rem 2rem 1rem 11.0625rem;
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
        .cta-btn {
            margin: 0.8125rem 2rem 1rem 14.0625rem;
        }

        #wave {
            top: -5.375rem;
        }
    }
</style>