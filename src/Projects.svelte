<script>
    import SectionTitle from './components/SectionTitle.svelte';
    import ProjectSlide from './components/ProjectSlide.svelte';
</script>

<section>
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
        <path fill="#DBE4EE" fill-opacity="1" d="M0,192L34.3,186.7C68.6,181,137,171,206,160C274.3,149,343,139,411,128C480,117,549,107,617,112C685.7,117,754,139,823,170.7C891.4,203,960,245,1029,272C1097.1,299,1166,309,1234,277.3C1302.9,245,1371,171,1406,133.3L1440,96L1440,320L1405.7,320C1371.4,320,1303,320,1234,320C1165.7,320,1097,320,1029,320C960,320,891,320,823,320C754.3,320,686,320,617,320C548.6,320,480,320,411,320C342.9,320,274,320,206,320C137.1,320,69,320,34,320L0,320Z"></path>
    </svg>
    <div class="projects">
        <SectionTitle titleName="PROJECTS"/>
        <div class="carousel">
            <ProjectSlide projectName="Github Grabber" 
                          githubLink="https://github.com/brandonnhem/github-profile-grabber"
                          liveLink="https://github-grabber.vercel.app/" 
                          backgroundLink="/images/mobile_light.png" />
        </div>
    </div>
</section>

<style>
    .projects {
        padding: 1rem;
        background-color: var(--project-bg-color);
    }

    section {
        position: relative;
        margin-top: 5rem;
    }

    svg {
        position: absolute;
        top: -5rem;
    }
</style>