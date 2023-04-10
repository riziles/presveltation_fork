<script lang="ts">
	import { onMount } from 'svelte';
	import { browser } from '$app/environment';

	import 'animate.css';
	import 'iconify-icon';

	import { slides } from '$lib/stores';
	import Deck from '$lib/Deck.svelte';

	$slides = [
		{ route: '/deck01/00-intro', title: 'Introduction', notes: true },
		{ route: '/deck01/01-animations', title: 'Animations with Animate.CSS' },
		{ route: '/deck01/02-lottie', title: 'Lottie-Player' },
		{ route: '/deck01/03-animate-tailwind', title: 'Tailwind Transitions' },
		{ route: '/deck01/04-code', title: 'Code Blocks' },
		{ route: '/deck01/05-math', title: 'Math' },
		{ route: '/deck01/06-prose', title: 'Markdown' },
		{ route: '/deck01/07-DSA-con', title: 'DSA-con' },
		{ route: '/deck01/08-Mario', title: 'Its so over' },
		{ route: '/deck01/final', title: 'Final Slide' },
		{ route: '/deck01/final2', title: 'Final Slide 2' },
		{ route: '/deck01/final3', title: 'Final Slide 3' },
		{ route: '/deck01/final4', title: 'Final Slide 4' },
		{ route: '/deck01/final5', title: 'Final Slide 5' },
		{ route: '/deck01/final6', title: 'Final Slide 6' }
	];

	onMount(async () => {
		if (browser) {
			await import('@lottiefiles/lottie-player');
		}
	});
</script>

<Deck notesURL="/deck01/notes">
	<slot />
</Deck>
