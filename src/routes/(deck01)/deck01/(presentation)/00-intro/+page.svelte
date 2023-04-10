<script>
	import './intro.css';
	import { addSteps } from '$lib/addsteps';
</script>

<div class="flex h-screen max-h-screen flex-col justify-center bg-gray-900">

	<h1
		class="max-w-5/6 mx-10 my-2 text-center font-sans text-5xl font-black leading-none tracking-tighter text-white"
	>
		Welcome to <span class="text-green-400">Mike's Presentation</span>
	</h1>
	<div
		class="max-w-4/6 mx-auto mt-8 text-center font-sans text-2xl font-normal leading-relaxed text-gray-400"
	>
		<p>
			Created with <span class="text-[#fff6a9] text-shadow-neon">PreSveltation</span>,
			
			<iconify-icon
				icon="logos:svelte-kit"
				class="text-2xl"
			/>
			and <iconify-icon icon="logos:tailwindcss" class="text-2xl" /> .
		</p>
		<p />
	</div>


	<div class="mx-auto mt-8 w-4/6 text-center font-sans text-lg font-normal text-blue-400">
		Press <kbd>m</kbd> to open an overview of all slides, and
		<kbd>s</kbd> to open the speaker view / notes. Use
		<kbd>&larr</kbd>
		and <kbd>&rarr</kbd> to move through the slides, and enter full screen mode by pressing
		<kbd>F11</kbd>.
	</div>

	<div class="mt-8 text-center text-lg text-gray-400">
		(These demo slides are currently not mobile friendly)
	</div>
</div>
