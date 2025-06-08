<script>
	import '../app.css';
	import Logo from '$lib/image/Logo.png';
	import VectorLine from '$lib/image/Vector Line.png';

	let { children } = $props();
	let showMenu = $state(false);
</script>


	<nav class="relative flex h-20 items-center justify-between 2xl:justify-around 2xl:mx-40">
		<a href="/" class="flex gap-2 text-3xl font-bold">
			<img src={Logo} alt="Logo" /> MODERNHERO
		</a>

		<div class="max-lg:hidden gap-5 flex justify-center mr-40">
			<a href="/">Home</a>
			<a href="/">About</a>
			<a href="/">Contact Us</a>
		</div>

		<button
			class="text-3xl focus:outline-none lg:hidden mx-4"
			onclick={() => (showMenu = !showMenu)}
			aria-label="Toggle Menu"
		>
			☰
		</button>

		<button class="angled-button hidden lg:inline text-white bg-[#2d42df]">Buy Game</button>

		{#if showMenu}
			<ul class="absolute top-full right-0 left-0 z-50 mt-2 flex max-md:flex-col justify-between gap-4 p-10 bg-black max-md:p-4 md:text-lg opacity-90 shadow-md lg:hidden text-white">
				<li class="transition-all duration-300 ease-in-out hover:text-2xl">
					<a href="/">Home</a>
				</li>
				<li class="transition-all duration-300 ease-in-out hover:text-2xl">
					<a href="/">About</a>
				</li>
				<li class="transition-all duration-300 ease-in-out hover:text-2xl">
					<a href="/">Contact Us</a>
				</li>
				<li class="transition-all duration-300 ease-in-out hover:text-2xl">
					<a href="/order">ORDER NOW <span>&#8594;</span></a>
				</li>
			</ul>
		{/if}
	</nav>
	<div class="flex justify-center">
		<img src={VectorLine} alt="VectorLine" />
	</div>


{@render children()}