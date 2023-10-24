<script lang="ts">
	import Advantages from './Advantages.svelte';
	import Cta from './Cta.svelte';
	import Footer from './Footer.svelte';
	import Header from './Header.svelte';
	import Hero from './Hero.svelte';
	import Podcast from './Podcast.svelte';
	import Roadmap from './Roadmap.svelte';
	import Socials from './Socials.svelte';
	import Team from './Team.svelte';

	const teams: { name: string; position: string; image: string }[] = [
		{
			name: 'John Osaretin',
			image: 'https://pbs.twimg.com/profile_images/1697025802406182912/FADRC21l_400x400.jpg',
			position: 'Founder & CEO'
		}
	];

	const data = [
		{
			name: 'team',
			value: 1500000000
		},
		{
			name: 'marketing',
			value: 500000000
		},
		{
			name: 'liquidity',
			value: 6000000000
		}
	];
</script>

<Header />
<div class="max-w-screen-xl mx-auto px-5">
	<Hero />

	<!-- <Podcast /> -->
	<Cta />
	<Advantages />

	<!-- <Chart {data}/> -->

	<Roadmap />
	<Team {teams} />
	<Socials />
</div>
<Footer/>
