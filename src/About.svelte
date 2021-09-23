<script>
    import SectionTitle from './components/SectionTitle.svelte';
</script>

<div class="about">
    <SectionTitle titleName="ABOUT" />

    <div class="about-me">
        <p>I’m a Comp Sci grad from Cal State Long Beach. I enjoy programming and creating apps. I’d love to be part of a team where I can apply my skills and challenge myself.</p>
    </div>
</div>

<style>
    .about {
        padding: 3rem 1rem;
    }

    .about-me {
        background-color: var(--about-bg-color);
        width: 259px;
        height: 112px;
        padding: 11px 22px;
        border-radius: 2rem 0 2rem 2rem;
        display: flex;
        justify-content: center;
        align-items: center;
        margin-left: 39px;;
    }
</style>