<script lang="ts">
	import Advantage from './Advantage.svelte';

	const advantages: { title: string; content: string }[] = [
		{
			title: 'Hybrid Platform',
			content:
				'Cryeator appears to be a hybrid platform that combines aspects of both web2 and web3, providing a seamless experience for users to interact and transact with content using a unified interface.'
		},

		{
			title: 'Simplified Web3 Interaction',
			content:
				'Cryeator aims to simplify the process of interacting with web3 applications and decentralized platforms by integrating the wallet and website functionalities, allowing users to perform various actions with minimal clicks.'
		},

		{
			title: 'Cryeator SIB (Spend In Behalf)',
			content:
				'This feature enables a content creator to delegate the spending of their earnings to another specified address. This allows the creator to authorize a designated address to access and utilize the earnings from their content without requiring direct intervention from the creator.'
		},

		{
			title: 'Cryeator Dislike',
			content:
				'The platform introduces a unique concept where disliking content results in the burning of tokens, creating scarcity. The disliked content will also owe the same amount that was used to dislike it. The owed amount can be repaid through subsequent likes received by the content, effectively offsetting the dislike.'
		},

		{
			title: 'Future Marketplace',
			content:
				'Cryeator has plans to incorporate a marketplace that facilitates direct transactions between buyers and sellers, allowing users to purchase content with a single click.'
		},
		{
			title: 'Enhanced Financial Flexibility and Delegation',
			content:
				'The SIB (Spend In Behalf) function in Cryeator empowers content creators to delegate the authority to access and manage their earnings to specific addresses. This feature provides enhanced financial flexibility, allowing creators to streamline financial operations and delegate financial responsibilities to trusted entities.'
		}
	];
</script>

<div class="w-full flex flex-col gap-10 px-6">
    <div class="mt-16 md:mt-0">
        <h2 class="text-4xl lg:text-5xl font-bold lg:tracking-tight">Discover the Key Benefits of Cryeator</h2>
        <p class="text-lg mt-4 text-slate-600">
            Explore the advantages that Cryeator offers, revolutionizing the way content creators and
            fans interact.
        </p>
    </div>
    <div class="grid sm:grid-cols-2 md:grid-cols-3 mt-16 gap-16">
        {#each advantages as advantage, index}
            <Advantage {advantage} />
        {/each}
    </div>
</div>