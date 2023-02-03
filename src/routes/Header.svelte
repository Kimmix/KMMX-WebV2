<script>
	import logo from '../asset/svg/logo_fill_mono.svg';
</script>

<header>
	<div class="corner">
		<a href="#">
			<img src={logo} alt="KMMX Logo" />
		</a>
	</div>
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		position: sticky;
    top: 0;
    z-index: 999;
	}

	.corner {
		width: 3em;
		height: 3em;
	}

	.corner a {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
		transition: scale 500ms ease-out;
	}

	.corner img {
		width: 2em;
		height: 2em;
		object-fit: contain;
	}

	.corner a:hover img {
		fill: var(--acc2b-color) !important;
	}
	.corner a:hover {
		scale: 1.2;
	}

</style>
