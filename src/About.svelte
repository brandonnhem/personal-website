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
        <p>I’m a Comp Sci grad from Cal State Long Beach. I enjoy programming and creating apps. I’d love to be part of a team where I can apply my skills and challenge myself.</p>
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
        top: 0px;
        left: -46px;
        transform: scale(1.3);
    }

    .about-me {
        background-color: var(--about-bg-color);
        width: 16.1875rem;
        height: 7rem;
        padding: 0.6875rem 1.375rem;
        border-radius: 2rem 0 2rem 2rem;
        display: flex;
        justify-content: center;
        align-items: center;
        margin-left: 2.4375rem;
    }
</style>