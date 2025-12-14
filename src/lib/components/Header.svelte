<script lang="ts">
	import { ArrowUpRight } from 'lucide-svelte';
</script>

<header class="w-full px-4 md:px-8 py-6 flex items-center justify-between text-[10px] font-medium tracking-wide uppercase border-b border-transparent fixed top-0 left-0 z-50 bg-[#F4F4F2]/90 backdrop-blur-sm transition-all duration-300">
	<div class="flex-1">
		<a href="/" class="block">
			<svg width="80" height="76" viewBox="0 0 112 106" fill="none" xmlns="http://www.w3.org/2000/svg" class="h-8 w-auto">
				<path d="M111.712 30.2285V0C92.366 0 73.5034 6.52934 59.961 17.8952L56.3336 20.7972L52.7062 17.8952C38.922 6.52934 20.3013 0 0.955078 0V30.2285C0.955078 38.4506 3.85704 46.1891 8.6936 52.7184C3.85704 59.2478 0.955078 66.9863 0.955078 75.2085V105.437C20.3013 105.437 39.1639 98.9076 52.7062 87.5417L56.3336 84.6397C46.9023 79.0777 41.0985 69.1627 41.0985 58.0387V47.3983C41.0985 36.516 46.9023 26.3592 56.3336 20.7972C65.7649 26.3592 71.5688 36.516 71.5688 47.3983V58.0387C71.5688 68.9209 65.7649 79.0777 56.3336 84.6397L59.961 87.5417C73.7452 98.9076 92.366 105.437 111.712 105.437V75.2085C111.712 66.9863 108.81 59.2478 103.974 52.7184C108.81 46.1891 111.712 38.4506 111.712 30.2285Z" fill="#201B21"/>
			</svg>
		</a>
	</div>

	<nav class="hidden md:flex items-center gap-12 text-gray-500">
		<a href="#about" class="hover:text-black transition-colors">About</a>
		<a href="#work" class="hover:text-black transition-colors">Work</a>
		<a href="#directors" class="hover:text-black transition-colors">Directors</a>
		<a href="#services" class="hover:text-black transition-colors">Services</a>
		<a href="#contact" class="hover:text-black transition-colors">Contact</a>
	</nav>

	<div class="flex-1 flex justify-end items-center gap-6 md:gap-8">
		<a href="#directors" class="flex items-center gap-1 hover:opacity-70 transition-opacity">
			<ArrowUpRight size={14} />
			DIRECTORS
		</a>
		<a href="#contact" class="flex items-center gap-1 hover:opacity-70 transition-opacity">
			<ArrowUpRight size={14} />
			CONTACT
		</a>
	</div>
</header>
