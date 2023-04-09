<script lang="ts">
	import { goto } from '$app/navigation';
	import { page } from '$app/stores';
	import { slides, currSlide } from '$lib/stores';
	import { onMount, onDestroy } from 'svelte';

	

	currSlide.update(n => 0)

	onMount(() => {
		goto('deck01/00-intro');
	});
	

</script>


<slot />