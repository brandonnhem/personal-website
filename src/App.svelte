<script>
	import Heading from './Heading.svelte';
	import Projects from './Projects.svelte';
	import About from './About.svelte';
	import Experience from './Experience.svelte';
	import Contact from './Contact.svelte';
</script>

<Heading />
<Projects />
<About />
<section>
	<div class="blob">
        <svg width="106" height="119" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
            <path fill="#F17300" d="M37.9,-54.9C47.7,-45.2,53,-32.1,54.8,-19.4C56.7,-6.8,55.1,5.3,50,14.7C44.8,24.1,36,30.7,27,37C18.1,43.3,9.1,49.2,-0.8,50.3C-10.7,51.5,-21.5,47.9,-27.6,40.7C-33.8,33.6,-35.3,22.8,-39.7,12.2C-44.1,1.6,-51.3,-8.7,-50.4,-17.9C-49.5,-27.1,-40.4,-35.1,-30.6,-44.8C-20.9,-54.6,-10.4,-66,1.8,-68.6C14.1,-71.1,28.2,-64.7,37.9,-54.9Z" transform="translate(100 100)" />
        </svg>
    </div>
	<Experience />
	<Contact />
</section>

<style>
	section {
		position: relative;
		overflow: hidden;
	}
	
	.blob {
        position: absolute;
        left: 85vw;
        top: 42vh;
        transform: scale(1.6);
        z-index: 3;
    }
</style>