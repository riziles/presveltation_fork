<script lang="ts">
	import { addSteps } from '$lib/addsteps';

	let classP = 'text-blue-400';
</script>

<div class="flex h-screen w-screen flex-col items-center justify-center bg-gray-900 text-2xl">
	<h2 class="m-6 text-6xl font-bold text-white">Conclusion:</h2>

	<div use:addSteps={[{ steps: '1', classes: classP }]}>
		<p>So don't stress out.</p>
	</div>
	<div use:addSteps={[{ steps: '2', classes: classP }]}>
		<p>Close your eyes, take a deep breath and ask the ancestors to guide you.</p>
	</div>
	<div use:addSteps={[{ steps: '3', classes: classP }]}>
		<p>And wherever you wind up,</p>
	</div>
	<div use:addSteps={[{ steps: '4', classes: classP }]}>
		<p>just try to make that place the best place it can be.</p>
	</div>
	<div use:addSteps={[{ steps: '5', classes: classP }]}>
		<p>And it will be.</p>
	</div>
</div>
