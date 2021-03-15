<script>
	import { sun } from '@modern-dev/daylight';

	const date = new Date();
	const lat = 47.62965;
	const long = -122.321281;

	console.log(sun.getTimes(date, lat, long).astronomicalDawn);
</script>

<main class="grid grid-cols-1 w-full min-h-full">
	<hr />
</main>

<style>
	main {
		grid-template-rows: repeat(24, minmax(0, 1fr));
		background: linear-gradient(
			180deg,
			rgba(0, 0, 0, 1) 0%,
			rgba(9, 9, 121, 1) 50%,
			rgba(5, 17, 201, 1) 100%
		);
	}
</style>
