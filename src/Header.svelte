<script lang="ts">
	let menuIsOpened: boolean = false;
	function toggleMenu() {
		menuIsOpened = !menuIsOpened;
	}
</script>

<header
	class="astronav-sticky-header sticky top-0 border-b z-20 transition-all is-active py-2 bg-white/80 border-gray-200 backdrop-blur-lg"
>
	<div class="max-w-screen-xl mx-auto px-5">
		<div
			class="flex flex-col lg:flex-row justify-between items-center relative z-10"
			data-astro-transition-scope="astro-o7bz76pi-1"
		>
			<div class="flex w-full lg:w-auto items-center justify-between">
				<a
					href="/"
					class="text-lg flex items-center transition focus-visible:ring-2 focus-visible:ring-offset-2 focus-visible:ring-indigo-500 focus-visible:outline-none focus-visible:shadow-outline-indigo rounded-full px-2 -ml-2"
					><span class="font-bold text-indigo-600">Cryeator</span></a
				>
				<div class="block lg:hidden">
					<button on:click={toggleMenu}
						><svg
							fill="currentColor"
							class="w-4 h-4 text-gray-800"
							width="24"
							height="24"
							viewBox="0 0 24 24"
							xmlns="http://www.w3.org/2000/svg"
							><title>Toggle Menu</title><path
								class={' ' + (menuIsOpened ? '' : 'hidden')}
								fill-rule="evenodd"
								clip-rule="evenodd"
								d="M18.278 16.864a1 1 0 01-1.414 1.414l-4.829-4.828-4.828 4.828a1 1 0 01-1.414-1.414l4.828-4.829-4.828-4.828a1 1 0 011.414-1.414l4.829 4.828 4.828-4.828a1 1 0 111.414 1.414l-4.828 4.829 4.828 4.828z"
							/><path
								class={' ' + (menuIsOpened ? 'hidden' : '')}
								fill-rule="evenodd"
								d="M4 5h16a1 1 0 010 2H4a1 1 0 110-2zm0 6h16a1 1 0 010 2H4a1 1 0 010-2zm0 6h16a1 1 0 010 2H4a1 1 0 010-2z"
							/></svg
						></button
					>
				</div>
			</div>
			<nav class={'w-full lg:w-auto mt-2 lg:flex lg:mt-0 ' + (menuIsOpened ? '' : 'hidden')}>
				<ul class="flex flex-col lg:flex-row lg:gap-3">
					<li>
						<a
							href="/pricing"
							class="flex lg:px-3 py-2 text-sm text-gray-600 hover:text-indigo-600 focus-visible:ring-2 focus-visible:ring-offset-2 transition focus-visible:ring-indigo-500 focus-visible:outline-none focus-visible:shadow-outline-indigo rounded-full"
							>Pricing</a
						>
					</li>
					<li>
						<a
							href="/about"
							class="flex lg:px-3 py-2 text-sm text-gray-600 hover:text-indigo-600 focus-visible:ring-2 focus-visible:ring-offset-2 transition focus-visible:ring-indigo-500 focus-visible:outline-none focus-visible:shadow-outline-indigo rounded-full"
							>About</a
						>
					</li>
					<li>
						<a
							href="/blog"
							class="flex lg:px-3 py-2 text-sm text-gray-600 hover:text-indigo-600 focus-visible:ring-2 focus-visible:ring-offset-2 transition focus-visible:ring-indigo-500 focus-visible:outline-none focus-visible:shadow-outline-indigo rounded-full"
							>Blog</a
						>
					</li>
					<li>
						<a
							href="/contact"
							class="flex lg:px-3 py-2 text-sm text-gray-600 hover:text-indigo-600 focus-visible:ring-2 focus-visible:ring-offset-2 transition focus-visible:ring-indigo-500 focus-visible:outline-none focus-visible:shadow-outline-indigo rounded-full"
							>Contact</a
						>
					</li>
				</ul>
				<div class="lg:hidden flex items-center mt-3 gap-4">
					<a
						href="#"
						class="rounded-full text-center transition focus-visible:ring-2 focus-visible:ring-offset-2 focus-visible:ring-indigo-500 focus-visible:outline-none focus-visible:shadow-outline-indigo w-full px-5 py-2 bg-gray-100 hover:bg-gray-200 border-2 border-transparent"
						>Log in</a
					><a
						href="#"
						class="rounded-full text-center transition focus-visible:ring-2 focus-visible:ring-offset-2 focus-visible:ring-indigo-500 focus-visible:outline-none focus-visible:shadow-outline-indigo w-full px-5 py-2 bg-indigo-600 text-white hover:bg-indigo-800"
						>View Whitepaper</a
					>
				</div>
			</nav>

			<div>
				<div class="hidden lg:flex items-center gap-4">
					<a
						href="#"
						class="text-sm px-2 py-1 transition focus-visible:ring-2 focus-visible:ring-offset-2 focus-visible:ring-indigo-500 focus-visible:outline-none focus-visible:shadow-outline-indigo rounded-full"
						>Log in</a
					><a
						href="#"
						class="rounded-full text-center transition focus-visible:ring-2 focus-visible:ring-offset-2 focus-visible:ring-indigo-500 focus-visible:outline-none focus-visible:shadow-outline-indigo px-4 py-2 text-sm bg-indigo-600 text-white hover:bg-indigo-800 inline-flex items-center group gap-px"
						><span>View Whitepaper</span></a
					>
				</div>
			</div>
		</div>
	</div>
</header>
