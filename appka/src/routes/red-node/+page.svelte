<script lang="ts">
	import { onMount } from 'svelte';

	type ModeredData = {
		robottoolnumber: number | null;
		downtime: number | null;
		currentNumber: number | null;
		cycletime: number | null;
		machineauto: boolean | null;
	};

	let message: ModeredData | null = null;
	let ws: WebSocket;

	onMount(() => {
		ws = new WebSocket('ws://10.184.152.201:1880/studentdata/eqc8');

		ws.onopen = () => {
			console.log('WebSocket connected');
		};

		ws.onmessage = (event) => {
			console.log('Prijatá správa:', event.data);
			try {
				const data = JSON.parse(event.data);
				console.log('Parsed data:', data);

				message = {
					robottoolnumber: data.robottoolnumber ?? null,
					downtime: data.downtime ?? null,
					currentNumber: data.currentNumber ?? null,
					cycletime: data.cycletime ?? null,
					machineauto: data.machineauto ?? null
				};
			} catch (error) {
				console.error('Parsing error:', error);
			}
		};

		ws.onerror = (error) => {
			console.error('WebSocket error:', error);
		};

		ws.onclose = () => {
			console.log('WebSocket closed');
		};
	});
</script>

<div class="pl-90 mt-40">
	<article
		class="w-300 h-150 flex flex-col items-center justify-center rounded-2xl border-4 border-black bg-gray-800 p-6 text-emerald-300"
	>
		<main>
			<h1 class="mb-10 text-center text-4xl font-bold">DÁTA</h1>
			<div class="mt-4 space-y-2 text-center text-2xl">
				{#if message}
					<p>RobotToolNumber : {message.robottoolnumber}</p>
					<p>DownTime : {message.downtime}</p>
					<p>CurrentNumber : {message.currentNumber}</p>
					<p>CycleTime : {message.cycletime}</p>
					<p>MachineAuto : {message.machineauto ? 'Áno' : 'Nie'}</p>
				{:else}
					<p>Čakám na údaje...</p>
				{/if}
			</div>
		</main>
	</article>
</div>
