<script>
    import Icon2 from '$lib/image/Icon2.png';
    import Hero2 from '$lib/image/hero2.png';
	import Circle from '$lib/image/circle.png';
</script>

<div  class="grid 2xl:grid-cols-3 justify-center gap-2 ">
    <div
        class="grid max-2xl:grid-cols-2 2xl:grid-rows-2 max-lg:flex max-lg:flex-col items-center max-xl:gap-2  lg:gap-5 2xl:w-80  "
    >
        <div
            class="flex h-[315px] w-96 md:w-[410px] flex-col items-center gap-6 rounded-xl border-3 border-blue-600 p-4"
        >
            <img src={Icon2} alt="Hero2" class="size-10" />
            <p class="mx-2 text-center font-semibold">Intense Survival Gameplay</p>

            <p class="text-center text-sm text-gray-500">
                Test your skills and instincts as you navigate through hostile environments, scavenge
                for resources, and make crucial choices to survive in a world on the brink of collapse.
            </p>
        </div>
        <div
            class="flex h-[315px] w-96 md:w-[410px] flex-col items-center gap-6 rounded-xl border-3 border-blue-600 p-4"
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

    <div class="md:ml-10 flex flex-col items-center md:justify-center 2xl:w-80">
        <div
            class="flex h-[315px] w-96 md:w-[410px] flex-col items-center gap-6 rounded-xl border-3 border-blue-600 p-4"
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