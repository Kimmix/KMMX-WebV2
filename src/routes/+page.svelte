<script>
	import Title from "./kmmx-main/title.svelte";
	import Intro from "./kmmx-main/intro.svelte";
	import Cinematic from "./kmmx-main/cinematic.svelte";
</script>

<svelte:head>
	<title>KMMX</title>
	<meta name="description" content="KMMX Protogen" />
</svelte:head>
<!-- <Intro /> -->
<section>
	<Title />
	<Cinematic />
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
</style>
