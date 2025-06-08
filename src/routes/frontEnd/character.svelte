
<script>
	import Character1 from '$lib/image/character1.png';
	import Character2 from '$lib/image/Character2.png';
	import Character3 from '$lib/image/Character3.png';
	import Character4 from '$lib/image/Character4.png';
	import Character5 from '$lib/image/character5.png';

    const character = [
		{ image: Character1, alt: 'Character1', name: 'MAGNUS' },
		{ image: Character2, alt: 'Character2', name: 'KAMUI' },
		{ image: Character3, alt: 'Character3', name: 'AZEROTH' },
		{ image: Character4, alt: 'Character4', name: 'MALCOLM' },
		{ image: Character5, alt: 'Character5', name: 'VULKAN' }
	];
</script>

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