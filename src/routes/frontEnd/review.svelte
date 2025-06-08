<script>
    
	const questions = [
		'Is "Shadowfall Chronicles" a single-player or multiplayer game?',
		'What sets the factions apart, and can I switch between them?',
		'How does the crafting system work in the game?',
		'Will my decisions affect the games outcome, and are there multiple endings?',
		'What content can I expect with the upcoming expansions?'
	];
</script>

<div class="flex flex-col items-center gap-8">
    <div class="text-center">
        <h6 class="mb-4 text-xl md:text-3xl font-bold">
            Unveiling Clarity: <br />
            Your Questions Answered
        </h6>
        <p class="max-md:text-sm">
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
        <p class="md:text-xl font-bold">Still have a question?</p>
        <p>Feel free to reach out for clarification and inquiries.</p>
        <button class="angled-button bg-[#2d42df] text-white">Contact us</button>
    </div>
</div>