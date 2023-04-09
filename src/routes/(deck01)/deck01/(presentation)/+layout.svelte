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
		{ route: '/deck01/final', title: 'Final Slide' }
	];

	onMount(async () => {
		if (browser) {
			await import('@lottiefiles/lottie-player');
		}
	});
</script>

<Deck notesURL="./notes">
	<slot />
</Deck>
