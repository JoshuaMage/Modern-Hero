<script>
	import Icon1 from '$lib/image/Icon1.png';
	import Icon2 from '$lib/image/Icon2.png';
	import SelectSquad from './frontEnd/selectSquad.svelte';
	import SelectedHero from './frontEnd/selectedHero.svelte';
	import Character from './frontEnd/character.svelte';
	import Pricing from './frontEnd/pricing.svelte';
	import Review from './frontEnd/review.svelte';
	import GameTitle from '$lib/image/gameTitle.png';

	import Logo from '$lib/image/Logo.png';

	import Footer from '$lib/footer.svelte';

</script>

<div class="flex h-full w-full justify-center overflow-hidden px-4">
	<div class="flex h-full w-full flex-col gap-20 lg:items-center 2xl:w-[1435px]">
		<img src={GameTitle} alt="shadowfall" class="absolute max-xl:hidden" />
		<SelectSquad />

		<SelectedHero />

		<Character />

		<Pricing />

		<Review />

		<Footer />
	</div>
</div>
