<script>
    import SVG from './svg.svelte';
    const Footer = [
		{
			title: 'Modern Hero',
			content: [
				'Our meni is celebration of flavors from aournd the world, crafted with care and creativity by our talented'
			],
			custom: true 
		},
		{
			title: 'Quik Links',
			list: ['Home', 'Our Menu', 'Reservation', 'About us', 'Chefs Details']
		},
		{
			title: 'Food Menu',
			list: ['Fast-food', 'Italian Food', 'Thai food', 'Bengali food', "Chef's food"]
		},
		{
			title: 'Contact Us',
			list: ['Mariveles Bataan Philippines', '123 (456) 789', 'jdelrosario2121@gmail.com']
		}
	];
</script>

<div class="text-black">
    <div class="flex  w-full 2xl:w-[1600px] flex-col justify-center">
        <hr />
        <div class="flex max-lg:flex-col max-2xl:justify-around 2xl:justify-between items-center gap-8 py-10">
            <h6 class="text-2xl font-bold tracking-wider">Subscribe for Daily Update</h6>
            <div class="flex gap-2">
                <input type="email" placeholder="Enter Email Address" class="border p-2" />
                <button class="border p-2 bg-[#2563eb] text-white"> Subscribe Now</button>
            </div>
        </div>

        <div class="grid 2xl:grid-cols-4 min-md:grid-cols-2 gap-4  w-full   mx-auto ">
            {#each Footer as section}
                <div class="flex flex-col max-md:p-2 {section.custom ? 'gap-4' : 'items-center'}">
                    <div>
                        <h6 class="{section.custom ? 'text-2xl' : ''} font-bold ">{section.title}</h6>
                    </div>
                    <div >
                        {#if section.content}
                            {#each section.content as paragraph}
                                <p class="2xl:w-80 max-md:px-0 max-2xl:px-20 text-black text-xs">{paragraph}</p>
                            {/each}
                        {/if}

                        {#if section.list}
                            <ul class="mt-4  flex flex-col gap-2 text-black">
                                {#each section.list as item}
                                    <li class="text-sm">{item}</li>
                                {/each}
                            </ul>
                        {/if}
                        <div class="mt-5  flex justify-center items-center">
                            {#if section.custom}
                                <SVG />
                            {/if}
                        </div>
                    </div>
                </div>
            {/each}
        </div>
        <hr class="mt-20" />
        <div class="m-8 flex max-md:flex-col max-md:gap-4 justify-between">
            <p class="text-xl">copyright @joshua2025 | All Rights Reserved</p>
            <p class="text-lg">Designed by Joshua</p>
        </div>
    </div>
</div>