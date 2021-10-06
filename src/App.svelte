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
        left: 20rem;
        top: 23rem;
        transform: scale(1.6);
        z-index: 3;
    }

	/* GALAXY S5 */
	@media only screen and (min-width: 360px) {
		.blob {
			top: 22rem;
			left: 19rem;
		}
	}

	/* IPHONE 6/7/8 */
	@media only screen and (min-width: 375px) {
		.blob {
			top: 22rem;
		}
	}

	/* IPHONE X */
	@media only screen
		   and (min-width: 375px)
		   and (min-height: 812px) {
		.blob {
			top: 22rem;
			left: 20rem;
		}
	}
	
	@media only screen and (min-width: 393px) {
        .blob {
			left: 21rem;
		}
    }

	/* PIXEL 2 */
	@media only screen and (min-width: 411px) {
		.blob {
			top: 22rem;
			left: 22rem;
		}
	}
	
	/* PIXEL 2 XL */
	@media only screen
	       and (min-width: 411px)
		   and (min-height: 823px) {
		.blob {
			top: 22rem;
			left: 22rem;
		}
	}

	/* IPHONE 6+/7+/8+ */
	@media only screen and (min-width: 414px) {
		.blob {
			top: 23rem;
			left: 22rem;
		}
	}

	@media only screen and (min-width: 768px) {
		.blob {
			top: 31rem;
			left: 44rem;
			transform: scale(1.9);
		}
	}

	@media only screen and (min-width: 768px) and (min-height: 1366px) {
		.blob {
			top: 35.875rem;
			left: 60.25rem;
		}
	}

	@media only screen and (min-width: 800px) and (min-height: 1112px) {
		.blob {
			left: 46.125rem;
		}
	}

	@media only screen and (min-width: 1024px) and (min-height: 768px) {
		.blob {
			top: 33rem;
			left: 60rem;
		}
	}

	@media only screen and (min-width: 1024px) {
		.blob {
			top: 31rem;
			left: 49rem;
		}
	}
	
	@media only screen and (min-width: 1024px) and (min-height: 1366px) {
		.blob {
			top: 34rem;
			left: 49rem;
		}
	}
	
	@media only screen and (min-width: 1280px) and (min-height: 632px) {
		.blob {
			top: 31rem;
			left: 64rem;
		}
	}
	
	@media only screen and (min-width: 1366px) and (min-height: 1024px) {
		.blob {
			top: 31rem;
			left: 68rem;
		}
	}

	@media only screen and (min-width: 1440px) {
		.blob {
			top: 31rem;
			left: 74rem;
		}
	}

	@media only screen and (min-width: 1632px) and (min-height: 939px) {
		.blob {
			left: 87rem;
		}
	}
</style>