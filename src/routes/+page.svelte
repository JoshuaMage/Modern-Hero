<script>
	import Icon1 from '$lib/image/Icon1.png';
	import Icon2 from '$lib/image/Icon2.png';
	import Icon3 from '$lib/image/Icon3.png';
	import Hero from '$lib/image/Hero1.png';
	import GameTitle from '$lib/image/gameTitle.png';
	import Arrow from '$lib/image/Arrow-right.png';
	import Hexagon from '$lib/image/Hexagon.png';
	import Character1 from '$lib/image/character1.png';
	import Character2 from '$lib/image/Character2.png';
	import Character3 from '$lib/image/Character3.png';
	import Character4 from '$lib/image/Character4.png';
	import Character5 from '$lib/image/character5.png';

	import Hero2 from '$lib/image/hero2.png';
	import Circle from '$lib/image/circle.png';

	import Logo from '$lib/image/Logo.png';

	import Footer from '$lib/footer.svelte';

	const selection = [
		{ image: Icon1, alt: 'Icon1', title: 'Gameplay and Features' },
		{ image: Icon2, alt: 'Icon2', title: 'Items and Collectibles' },
		{ image: Icon3, alt: 'Icon3', title: 'Heroes and Game Locations' }
	];

	const character = [
		{ image: Character1, alt: 'Character1', name: 'MAGNUS' },
		{ image: Character2, alt: 'Character2', name: 'KAMUI' },
		{ image: Character3, alt: 'Character3', name: 'AZEROTH' },
		{ image: Character4, alt: 'Character4', name: 'MALCOLM' },
		{ image: Character5, alt: 'Character5', name: 'VULKAN' }
	];

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

	const questions = [
		'Is "Shadowfall Chronicles" a single-player or multiplayer game?',
		'What sets the factions apart, and can I switch between them?',
		'How does the crafting system work in the game?',
		'Will my decisions affect the games outcome, and are there multiple endings?',
		'What content can I expect with the upcoming expansions?'
	];
</script>

<div class="flex h-full w-full justify-center px-4">
	<div class="mx-4 flex w-full flex-col gap-20 lg:items-center 2xl:w-[1435px]">
		<img src={GameTitle} alt="shadowfall" class="absolute max-xl:hidden" />
		<div class="flex flex-col items-center max-2xl:text-center lg:mt-10 2xl:grid 2xl:grid-cols-2">
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
				<div class="mt-10 flex max-2xl:justify-center max-2xl:gap-2 lg:gap-5">
					{#each selection as { image, alt, title }}
						<div
							class="flex h-56 w-50 flex-col justify-between rounded-xl border-3 border-blue-600 p-4"
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

				<img
					src={Hero}
					alt="hero"
					class="relative z-10 2xl:bottom-20 2xl:h-[909px] 2xl:w-[630px]"
				/>
			</div>
		</div>

		<div class="grid justify-center gap-2 2xl:grid-cols-3">
			<div
				class="m mt-10 grid items-center max-2xl:grid-cols-2 max-xl:gap-2 max-lg:flex max-lg:flex-col lg:gap-5 2xl:w-80 2xl:grid-rows-2"
			>
				<div
					class="flex h-[315px] w-[410px] flex-col items-center gap-6 rounded-xl border-3 border-blue-600 p-4"
				>
					<img src={Icon2} alt="Hero2" class="size-10" />
					<p class="mx-2 text-center font-semibold">Intense Survival Gameplay</p>

					<p class="text-center text-sm text-gray-500">
						Test your skills and instincts as you navigate through hostile environments, scavenge
						for resources, and make crucial choices to survive in a world on the brink of collapse.
					</p>
				</div>
				<div
					class="flex h-[315px] w-[410px] flex-col items-center gap-6 rounded-xl border-3 border-blue-600 p-4"
				>
					<img src={Icon2} alt="Hero2" class="size-10" />
					<p class="mx-2 text-center font-semibold">Cooperative Multiplayer</p>

					<p class="text-center text-sm text-gray-500">
						Join forces with friends or other players in cooperative multiplayer mode. Tackle
						challenging missions together, coordinate strategies, and combine your unique abilities.
					</p>
				</div>
			</div>

			<div class="relative flex justify-center">
				<img src={Hero2} alt="hero2" class="z-1 2xl:h-[888px] 2xl:w-[685px]" />
				<img src={Circle} alt="circle" class="absolute bottom-1 2xl:size-[647px]" />
			</div>

			<div class="ml-10 flex flex-col items-center justify-center 2xl:w-80">
				<div
					class="flex h-[315px] w-[410px] flex-col items-center gap-6 rounded-xl border-3 border-blue-600 p-4"
				>
					<img src={Icon2} alt="Hero2" class="size-10" />
					<p class="mx-2 text-center font-semibold">Tactical Combat and Customization</p>

					<p class="text-center text-sm text-gray-500">
						Engage in adrenaline-pumping combat encounters, utilizing a range of futuristic weapons,
						gadgets, and abilities. Customize your play style, strategize your approach, and
						outmaneuver enemies for tactical advantage.
					</p>
				</div>
			</div>
		</div>

		<div class="flex flex-col items-center justify-center">
			<div class="mb-10 text-center">
				<h2 class="text-2xl font-bold text-blue-500">From Outcast To Legends</h2>
				<p>Witness the rise of unlikely heroes who defy the odds and challenge fate.</p>
			</div>

			<!-- Custom 3x3 grid with center character -->
			<div class="grid gap-4 text-center min-lg:grid-cols-2 xl:grid-cols-3 xl:grid-rows-3">
				<!-- Top-left -->
				<div class="character-border">
					<img src={character[0].image} alt={character[0].alt} />
					<p class="text-center font-bold">{character[0].name}</p>
				</div>

				<!-- Empty top-center -->
				<div class="max-xl:hidden"></div>

				<!-- Top-right -->
				<div class="character-border">
					<!-- Content -->
					<img src={character[1].image} alt={character[1].alt} class="mx-auto mb-2" />
					<p class="text-center font-bold">{character[1].name}</p>
				</div>

				<!-- Empty middle-left -->
				<div class="max-xl:hidden"></div>

				<!-- Center image -->
				<div class="character-border">
					<img src={character[2].image} alt={character[2].alt} />
					<p class="text-center font-bold">{character[2].name}</p>
				</div>

				<!-- Empty middle-right -->
				<div class="max-xl:hidden"></div>

				<!-- Bottom-left -->
				<div class="character-border">
					<img src={character[3].image} alt={character[3].alt} />
					<p class="text-center font-bold">{character[3].name}</p>
				</div>

				<!-- Empty bottom-center -->
				<div class="max-xl:hidden"></div>

				<!-- Bottom-right -->
				<div class="character-border">
					<img src={character[4].image} alt={character[4].alt} />
					<p class="text-center font-bold">{character[4].name}</p>
				</div>
			</div>
		</div>

		<div class="flex h-full w-full flex-col gap-10 py-10 text-center">
			<div>
				<h2 class="mb-4 text-4xl font-bold text-[#2563eb]">
					Invest in Your Survival: <br /> Pricing Tiers
				</h2>
				<p class="text-2xl">
					Explore Our Pricing Options Tailored to Your Gameplay Goals and Preferences
				</p>
			</div>
			<div class="flex items-center justify-around max-xl:flex-col max-xl:gap-8">
				{#each pricing as { image, plan, title, Price, button, p1, p2, p3, p4, p5 }}
					<div class="w-[535px] rounded-2xl border-4 border-[#2563eb] p-12">
						<div class="flex w-full flex-col items-center gap-4 py-5">
							<img src={image} alt="Icon1" />
							<h6 class="text-lg">{title}</h6>
						</div>
						<hr class="border border-[#2563eb]" />
						<div class="flex flex-col gap-8 py-8">
							<h5 class="text-2xl font-bold">$ {Price}</h5>
							<button class="bg-[#2563eb] p-2 px-6 text-white">{button}</button>
						</div>
						<hr class="border border-[#2563eb]" />
						<ul class="flex flex-col gap-7 py-6 text-start text-sm font-thin tracking-wide">
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

		<div class="flex flex-col items-center gap-8">
			<div class="text-center">
				<h6 class="mb-4 text-3xl font-bold">
					Unveiling Clarity: <br />
					Your Questions Answered
				</h6>
				<p>
					Navigate Through Frequently Asked Questions to Enhance <br /> Your Understanding of Shadowfall
					Chronicles
				</p>
			</div>
			<div>
				<div class="flex flex-col gap-4 py-4">
					{#each questions as question}
						<div class="rounded-xl border border-white shadow-md shadow-black">
							<p class="flex justify-between gap-2 p-4">
								{question} <span class="text-2xl font-bold">+</span>
							</p>
						</div>
					{/each}
				</div>
			</div>
			<div class="flex flex-col gap-6 text-center">
				<p class="text-xl font-bold">Still have a question?</p>
				<p>Feel free to reach out for clarification and inquiries.</p>
				<button class="angled-button bg-[#2d42df] text-white">Contact us</button>
			</div>
		</div>
		<!-- 
		<div class="w-screen bg-[#2563eb] text-white">
			<div class="grid max-xl:grid-cols-1 max-xl:grid-rows-3 max-xl:justify-center xl:grid-cols-4 p-10 gap-5 xl:place-items-center">
	
			  <div class="flex flex-col items-center  2xl:items-start text-center">
				<h6 class="flex text-2xl font-bold tracking-wider gap-2 mb-2 px-4">
				  <img src={Logo} alt="logo" /> Modern Hero
				</h6>
				<p class="text-xs">Experience the game that will change your the way you play.</p>
			  </div>
		  
		
			  <div class="col-span-2 flex flex-col items-center text-center  text-sm" >
				<p class="tracking-wide mb-4 font-semibold">
				  Subscribe to stay tuned for latest updates. Let's do it!
				</p>
				<div class="flex gap-2">
				  <input type="email" placeholder="Enter Your Email Address" class="bg-white text-black p-3 text-xs" />
				  <button class="font-bold text-black bg-white p-3 text-xs">Subscribe</button>
				</div>
			  </div>
		  
	
			  <div class="flex flex-col items-center text-center">
				<p class="font-semibold tracking-wider mb-4 text-xs">Follow Us</p>
				<div class="flex gap-4">
				  <Svg />
				</div>
			  </div>
		  
			</div>

			<hr >

			<div class="m-8 flex max-md:flex-col max-md:gap-4 justify-between">
				<p class="">copyright @joshua2025 | All Rights Reserved</p>
				<p class="text-lg">Designed by Joshua</p>
			</div>
		  </div> -->
		<Footer />
	</div>
</div>
