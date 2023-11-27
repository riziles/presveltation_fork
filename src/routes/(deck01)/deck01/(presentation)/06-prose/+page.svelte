<script lang="ts">
	import Test from './Test.md'
</script>

<svelte:head>
	<link rel="stylesheet" href="/katex.min.css">
	<link rel="stylesheet" href="/atom-dark.css">
</svelte:head>

<div class="flex h-screen w-screen flex-col items-center justify-center bg-gray-900">
<div class="flex flex-col items-center gap-8 text-2xl md:flex-row md:gap-20">
	<article class="prose prose-li:marker:text-emerald-200 prose-invert">
		<Test />
	</article>
</div>
</div>


