<script lang="ts">
	import { addSteps } from '$lib/addsteps';

	let classP = 'text-blue-400';
</script>

<div class="flex h-screen w-screen flex-col items-center justify-center bg-gray-900 text-2xl">
	<h2 class="m-6 text-6xl font-bold text-white">Conclusion:</h2>

	<div use:addSteps={[{ steps: '1', classes: classP }]}>
		<p>At the end of the day, I really don't think it matters.</p>
	</div>

	<div use:addSteps={[{ steps: '2', classes: classP }]}>
		<p>Wherever you go is gonna be the best high school on the gosh darn planet,</p>
	</div>
	<div use:addSteps={[{ steps: '3', classes: classP }]}>
		<p>because you are there.</p>
	</div>
	<div use:addSteps={[{ steps: '4', classes: classP }]}>
		<p>And it's not because of how smart you are</p>
	</div>
	<div use:addSteps={[{ steps: '5', classes: classP }]}>
		<p>or how many boys want to date you</p>
	</div>
	<div use:addSteps={[{ steps: '6', classes: classP }]}>
		<p>or how good your walkovers are.</p>
	</div>
	<div use:addSteps={[{ steps: '7', classes: classP }]}>
		<p>You're just great, and we love you, and we're proud of you.</p>
	</div>
</div>
