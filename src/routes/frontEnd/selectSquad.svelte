<script>
	import Icon1 from '$lib/image/Icon1.png';
	import Icon2 from '$lib/image/Icon2.png';
	import Icon3 from '$lib/image/Icon3.png';
	import Hero from '$lib/image/Hero1.png';
	import Arrow from '$lib/image/Arrow-right.png';
    import Hexagon from '$lib/image/Hexagon.png';

	const selection = [
		{ image: Icon1, alt: 'Icon1', title: 'Gameplay and Features' },
		{ image: Icon2, alt: 'Icon2', title: 'Items and Collectibles' },
		{ image: Icon3, alt: 'Icon3', title: 'Heroes and Game Locations' }
	];
</script>

<div class="flex flex-col items-center  max-2xl:text-center lg:mt-10 2xl:grid 2xl:grid-cols-2">
	<div class="flex w-full flex-col max-xl:text-center">
		<div>
			<h1 class="my-10 text-2xl font-bold tracking-widest xl:text-4xl">
				Unleash your survival Instincts in a futuristic apocalypse
			</h1>
			<p class="mb-4 font-semibold text-gray-500">
				Engage in heart-pounding combat across ruined cityscapes and war-torn landscapes
			</p>
			<div class="mb-5">
				<button class="angled-button bg-[#2d42df] text-white">Buy Game</button>
				<button class="angled-button border border-[#2d42df] bg-white text-[#2d42df]"
					>Learn More</button
				>
			</div>
		</div>
		<div class="mt-10 flex max-md:flex-col max-md:items-center max-2xl:justify-center max-2xl:gap-2 lg:gap-4">
			{#each selection as { image, alt, title }}
				<div
					class="flex flex-col w-full max-md:size-50  2xl:h-56 2xl:w-50  justify-between rounded-xl border-3 border-blue-600 p-4"
				>
					<div class="flex flex-col items-center gap-5 text-center">
						<img src={image} {alt} class="size-10" />
						<p class="mx-2 text-sm font-semibold">{title}</p>
					</div>
					<div class="flex justify-end">
						<button><img src={Arrow} alt="arrow" /></button>
					</div>
				</div>
			{/each}
		</div>
	</div>
	<div class="relative flex justify-center">
		<img
			src={Hexagon}
			alt="hexagon"
			class="absolute top-20 left-1/2 z-0 -translate-x-1/2 2xl:h-[650px] 2xl:w-[650px]"
		/>

		<img src={Hero} alt="hero" class="relative z-10 2xl:bottom-20 2xl:h-[909px] 2xl:w-[630px]" />
	</div>
</div>
