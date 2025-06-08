<script>
	import Icon1 from '$lib/image/Icon1.png';

	const pricing = [
		{
			image: Icon1,
			plan: 'Basic Plan',
			title: 'Survivors Starter Pack',
			Price: '29.99/mo',
			button: 'Buy Game',
			p1: 'Access to the full game with all core features.',
			p2: 'Single-player mode available.',
			p3: 'Limited selection of character customization options.',
			p4: 'Exclusive in-gameL "Rockies Rations supply pack',
			p5: 'Feature text goes here'
		},
		{
			image: Icon1,
			plan: 'Pro Plan',
			title: 'Apocalypse Conqueror Bundle',
			Price: '40.99/mo',
			button: 'Buy Game',
			p1: 'All features of the Basic Plan included.',
			p2: 'Unlock access to multiplayer mode, team up with friends.',
			p3: 'Extensive range of character customization choices.',
			p4: 'Exclusive in-game items: "Veterans Arsenal" weapon pack.',
			p5: 'Priority access to upcoming expansions and updates.'
		}
	];
</script>

<div class="flex h-full w-full flex-col gap-10 py-10 text-center">
	<div>
		<h2 class="mb-4 max-md:text-2xl lg:text-4xl font-bold text-[#2563eb]">
			Invest in Your Survival: <br /> Pricing Tiers
		</h2>
		<p class="max-md:text-lg md:text-2xl">
			Explore Our Pricing Options Tailored to Your Gameplay Goals and Preferences
		</p>
	</div>
	<div class="flex items-center justify-around max-xl:flex-col max-xl:gap-8">
		{#each pricing as { image, plan, title, Price, button, p1, p2, p3, p4, p5 }}
			<div class="lg:w-[535px] rounded-2xl border-4 border-[#2563eb] max-md:p-6 lg:p-12">
				<div class="flex w-full flex-col items-center gap-4 py-5">
					<img src={image} alt="Icon1" />
					<h6 class="max-md:text-base lg:text-lg">{title}</h6>
				</div>
				<hr class="border border-[#2563eb]" />
				<div class="flex flex-col gap-4 lg:gap-8 max-md:py-4 lg:py-8">
					<h5 class="max-md:text-xl lg:text-2xl font-bold">$ {Price}</h5>
					<button class="bg-[#2563eb] p-2 px-6 text-white">{button}</button>
				</div>
				<hr class="border border-[#2563eb]" />
				<ul class="flex flex-col gap-4 lg:gap-7 py-6 text-start text-sm font-thin tracking-wide">
					<li><span class="ml-1 font-bold text-[#2563eb]">&#10003;</span> {p1}</li>
					<li><span class="ml-1 font-bold text-[#2563eb]">&#10003;</span> {p2}</li>
					<li><span class="ml-1 font-bold text-[#2563eb]">&#10003;</span> {p3}</li>
					<li><span class="ml-1 font-bold text-[#2563eb]">&#10003;</span> {p4}</li>
					<li><span class="ml-1 font-bold text-[#2563eb]">&#10003;</span> {p5}</li>
				</ul>
			</div>
		{/each}
	</div>
</div>
