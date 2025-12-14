<script lang="ts">
	import Header from "$lib/components/Header.svelte";
	import { ArrowUpRight, ArrowRight } from 'lucide-svelte';

	const services = [
		{ id: '01', name: 'MUSIC VIDEOS' },
		{ id: '02', name: 'COMMERCIALS & BRANDED CONTENT' },
		{ id: '03', name: 'EDITING / VFX / COLOR / FINISHING' },
		{ id: '04', name: 'PHOTOGRAPHY & SOCIAL CONTENT' },
		{ id: '05', name: 'NFT CREATION & DEPLOYMENT' },
		{ id: '06', name: 'FULL-SERVICE PRODUCTION' },
		{ id: '07', name: 'CREATIVE DIRECTION' }
	];

	const directors = [
		{ name: 'EDGAR ESTEVES', role: 'FOUNDER & DIRECTOR', img: '/generated/image-confident-latino-male-director-in-his-30-1765714406717-5.webp' },
		{ name: 'NIKITA VILCHINSKI', role: 'DIRECTOR', img: '/generated/image-professional-male-cinematographer-in-his-1765714408827-6.webp' },
		{ name: 'ANASTASIA DELMARK', role: 'DIRECTOR', img: '/generated/image-talented-female-director-in-her-20s-with-1765714410944-7.webp' },
		{ name: 'ARSENI NOVO', role: 'DIRECTOR', img: '/generated/image-creative-male-director-in-his-30s-with-f-1765714413066-8.webp' },
		{ name: 'GEERTEN HARMENS', role: 'DIRECTOR', img: '/generated/image-professional-male-cinematographer-in-his-1765714415271-9.webp' },
		{ name: 'JUAN FELIPE ZULETA', role: 'DIRECTOR', img: '/generated/image-young-latino-male-director-in-his-20s-wi-1765714417377-10.webp' },
		{ name: 'PAOLA OSSA', role: 'DIRECTOR', img: '/generated/image-latina-female-director-in-her-30s-with-c-1765714419561-11.webp' },
		{ name: 'CARLY GIBERT', role: 'DIRECTOR', img: '/generated/image-young-female-director-in-her-20s-with-cr-1765714421850-12.webp' }
	];
</script>

<div class="min-h-screen bg-[#F4F4F2] text-[#1A1A1A] font-sans selection:bg-primary-500 selection:text-white overflow-x-hidden">
	<Header />

	<main>
		<!-- Hero Section -->
		<section class="pt-12 md:pt-20 pb-10 px-4 md:px-8">
			<div class="flex flex-col md:flex-row justify-between items-start mb-12 md:mb-24 relative">
				<div class="max-w-[200px] text-[10px] leading-relaxed uppercase tracking-wide font-medium mt-2">
					<p>Blank Square is a canvas for artists to create culture-defining content through full-service production and diverse creative collaboration.</p>
				</div>
				<h1 class="text-[14vw] md:text-[9rem] lg:text-[11rem] leading-[0.8] font-thin tracking-tighter text-right mt-8 md:mt-0 uppercase">
					Artist <br />
					Visions
				</h1>
			</div>

			<!-- Hero Images -->
			<div class="grid grid-cols-5 gap-2 md:gap-4 mb-8 h-[30vh] md:h-[50vh]">
				<div class="overflow-hidden h-full">
					<img src="/generated/image-professional-music-video-production-on-s-1765714395483-0.webp" alt="Music video production" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
				<div class="overflow-hidden h-full">
					<img src="/generated/image-behind-the-scenes-of-a-music-video-shoot-1765714398119-1.webp" alt="Behind the scenes" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
				<div class="overflow-hidden h-full">
					<img src="/generated/image-cinematic-shot-of-a-music-artist-in-dram-1765714400263-2.webp" alt="Cinematic shot" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
				<div class="overflow-hidden h-full">
					<img src="/generated/image-film-crew-setting-up-professional-camera-1765714402419-3.webp" alt="Film crew" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
				<div class="overflow-hidden h-full">
					<img src="/generated/image-vibrant-music-video-scene-with-colorful--1765714404642-4.webp" alt="Vibrant production" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
			</div>

			<div class="flex flex-col md:flex-row justify-between items-start">
				<span class="text-[10px] uppercase tracking-wide font-medium mt-4 hidden md:block">Scroll</span>
				<h1 class="text-[14vw] md:text-[9rem] lg:text-[11rem] leading-[0.8] font-thin tracking-tighter text-right w-full uppercase">
					To Culture-<br />
					Defining Content
				</h1>
			</div>
		</section>

		<!-- Services Section -->
		<section class="py-20 md:py-32" id="services">
			<div class="flex justify-center mb-16 md:mb-24">
				<span class="text-[10px] font-bold uppercase tracking-widest">Services</span>
			</div>

			<div class="border-t border-gray-300">
				{#each services as service}
					<div class="group border-b border-gray-300 py-6 md:py-10 px-4 md:px-8 flex items-center justify-between hover:bg-white transition-colors cursor-pointer">
						<span class="text-[10px] font-medium text-gray-500 w-8 md:w-12">/{service.id}</span>
						<h2 class="text-2xl md:text-5xl lg:text-6xl font-thin tracking-tight group-hover:italic transition-all duration-300 uppercase">{service.name}</h2>
						<div class="flex items-center gap-1 text-[10px] font-medium uppercase opacity-0 group-hover:opacity-100 transition-opacity translate-x-[-10px] group-hover:translate-x-0 duration-300">
							<ArrowUpRight size={12} />
							Learn More
						</div>
					</div>
				{/each}
			</div>
		</section>

		<!-- Directors Section -->
		<section class="py-20 px-4 md:px-8 bg-[#F4F4F2]" id="directors">
			<div class="flex flex-col md:flex-row justify-between items-start mb-16 md:mb-24">
				<h2 class="text-4xl md:text-6xl font-light tracking-tight mb-8 md:mb-0 uppercase">Our Directors</h2>
				<div class="max-w-xs text-[10px] leading-relaxed uppercase tracking-wide font-medium text-right md:text-left">
					<p>A diverse roster of visionary directors from around the world, united by their commitment to authentic storytelling and cultural impact.</p>
				</div>
			</div>

			<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-x-4 gap-y-12 md:gap-y-16">
				{#each directors as director}
					<div class="group cursor-pointer">
						<div class="aspect-[3/4] overflow-hidden mb-4 bg-gray-200">
							<img src={director.img} alt={director.name} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
						</div>
						<h3 class="text-xs font-bold uppercase tracking-wide mb-1">{director.name}</h3>
						<p class="text-[10px] text-gray-500 uppercase tracking-wide mb-3">{director.role}</p>
						<div class="inline-flex items-center gap-1 text-[10px] font-medium uppercase opacity-0 group-hover:opacity-100 transition-opacity">
							<ArrowUpRight size={10} />
							View Reel
						</div>
					</div>
				{/each}
				
				<!-- Join Us Card -->
				<div class="flex flex-col justify-between h-full min-h-[300px] border border-gray-300 p-8 bg-[#F4F4F2] hover:bg-white transition-colors cursor-pointer group">
					<div class="flex justify-center items-center flex-1">
						<ArrowRight size={48} class="text-gray-300 group-hover:text-black transition-colors" />
					</div>
					<div>
						<h3 class="text-xs font-bold uppercase tracking-wide mb-1 leading-relaxed">Opening doors for<br/>diverse creatives</h3>
						<div class="inline-flex items-center gap-1 text-[10px] font-medium uppercase mt-4">
							<ArrowUpRight size={10} />
							Join Us
						</div>
					</div>
				</div>
			</div>
		</section>

		<!-- About Section -->
		<section class="py-20 px-4 md:px-8" id="about">
			<div class="flex flex-col lg:flex-row mb-16 gap-12 lg:gap-24">
				<div class="flex-1">
					<h2 class="text-4xl md:text-6xl font-light tracking-tight uppercase">About Blank Square</h2>
				</div>
				<div class="flex-1">
					<h2 class="text-3xl md:text-5xl font-light tracking-tight mb-8 text-left uppercase leading-tight">A canvas for artists<br/>to create</h2>
					<div class="grid grid-cols-1 md:grid-cols-2 gap-8 text-[10px] leading-relaxed uppercase tracking-wide font-medium">
						<p>Founded by Edgar Esteves, a Venezuelan immigrant who lived undocumented for nearly three decades, Blank Square transforms artist visions into culture-defining content through authentic storytelling and diverse creative collaboration.</p>
						<p>From music videos for multi-platinum artists like Nicki Minaj, Doja Cat, and Lil Wayne to major brand campaigns for Nike, Puma, and Ford, we deliver full-service production with proven ROI. Based in Los Angeles, we're capturing the $5B music video market while opening doors for diverse creatives.</p>
					</div>
					<a href="#work" class="inline-flex items-center gap-1 text-[10px] font-medium uppercase mt-8 hover:opacity-60 transition-opacity">
						<ArrowUpRight size={10} />
						View Work
					</a>
				</div>
			</div>

			<div class="flex flex-col md:flex-row gap-4 h-[50vh] md:h-[70vh]">
				<div class="w-full md:w-[60%] h-full bg-gray-200 overflow-hidden">
					<img src="/generated/image-large-professional-film-production-studi-1765714424075-13.webp" alt="Production studio" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
				</div>
				<div class="w-full md:w-[40%] h-full flex flex-col gap-4">
					<div class="flex-1 bg-gray-200 overflow-hidden">
						<img src="/generated/image-film-editing-suite-with-multiple-monitor-1765714426168-14.webp" alt="Editing suite" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
					</div>
					<div class="flex-1 flex gap-4">
						<div class="flex-1 bg-gray-200 overflow-hidden">
							<img src="/generated/image-professional-camera-equipment-and-lighti-1765714428343-15.webp" alt="Camera equipment" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
						</div>
						<div class="flex-1 bg-gray-200 overflow-hidden">
							<img src="/generated/image-green-screen-studio-setup-with-professio-1765714430449-16.webp" alt="Green screen studio" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
						</div>
					</div>
				</div>
			</div>
		</section>

		<!-- CTA Section -->
		<section class="py-32 px-4 md:px-8 bg-[#1A1A1A] text-white text-center" id="contact">
			<span class="text-[10px] font-medium uppercase tracking-widest mb-6 block opacity-80">Let's Create Together</span>
			<h2 class="text-4xl md:text-6xl lg:text-8xl font-thin tracking-tight mb-12 uppercase">
				Ready to bring your<br />
				vision to life?
			</h2>
			<a href="mailto:info@blanksquare.com" class="inline-block bg-white text-[#1A1A1A] px-10 py-4 rounded-full text-[10px] font-bold uppercase tracking-widest hover:bg-primary-500 hover:text-white transition-colors">
				Get In Touch
			</a>
		</section>

		<!-- Bottom Gallery -->
		<div class="grid grid-cols-2 md:grid-cols-5 h-[60vh]" id="work">
			<div class="overflow-hidden">
				<img src="/generated/image-dynamic-music-video-scene-with-dancer-pe-1765714432538-17.webp" alt="Music video production" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
			<div class="overflow-hidden">
				<img src="/generated/image-cinematic-commercial-shoot-with-brand-pr-1765714434654-18.webp" alt="Commercial production" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
			<div class="overflow-hidden">
				<img src="/generated/image-hip-hop-artist-performing-for-camera-in--1765714436699-19.webp" alt="Hip-hop video" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
			<div class="overflow-hidden">
				<img src="/generated/image-fashion-forward-music-video-scene-with-v-1765714438930-20.webp" alt="Fashion video" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
			<div class="overflow-hidden hidden md:block">
				<img src="/generated/image-behind-the-scenes-of-major-music-video-p-1765714441114-21.webp" alt="Behind the scenes" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
		</div>

		<!-- Footer Marquee -->
		<div class="overflow-hidden py-6 border-b border-gray-200">
			<div class="whitespace-nowrap animate-marquee flex">
				<span class="text-4xl md:text-6xl lg:text-8xl font-thin tracking-tight mx-4 uppercase">A canvas for artists to create — Culture-defining content — A canvas for artists to create — </span>
				<span class="text-4xl md:text-6xl lg:text-8xl font-thin tracking-tight mx-4 uppercase">A canvas for artists to create — Culture-defining content — A canvas for artists to create — </span>
			</div>
		</div>
	</main>

	<footer class="px-4 md:px-8 py-12 text-[10px] font-medium uppercase tracking-wide">
		<div class="flex flex-col md:flex-row justify-between items-start md:items-end gap-12 md:gap-8">
			<div class="flex flex-col gap-3">
				<a href="#about" class="hover:opacity-60">About</a>
				<a href="#work" class="hover:opacity-60">Work</a>
				<a href="#directors" class="hover:opacity-60">Directors</a>
				<a href="#services" class="hover:opacity-60">Services</a>
				<a href="#contact" class="hover:opacity-60">Contact</a>
			</div>

			<div class="text-left md:text-center">
				<p class="text-lg md:text-2xl font-normal tracking-tight mb-6">INFO@BLANKSQUARE.COM</p>
				<p class="text-lg tracking-widest">LOS ANGELES, CA</p>
			</div>

			<div class="flex flex-col gap-3 text-left md:text-right">
				<a href="https://instagram.com/blanksquare" target="_blank" rel="noopener" class="hover:opacity-60">Instagram</a>
				<a href="#privacy" class="hover:opacity-60">Privacy Policy</a>
			</div>
		</div>

		<div class="flex flex-col md:flex-row justify-between items-center mt-20 pt-8 border-t border-gray-200 text-[10px] text-gray-400 gap-4">
			<p>© BLANK SQUARE. ALL RIGHTS RESERVED</p>
			<div class="flex items-center gap-1">
				<svg width="60" height="57" viewBox="0 0 112 106" fill="none" xmlns="http://www.w3.org/2000/svg" class="h-6 w-auto opacity-40">
					<path d="M111.712 30.2285V0C92.366 0 73.5034 6.52934 59.961 17.8952L56.3336 20.7972L52.7062 17.8952C38.922 6.52934 20.3013 0 0.955078 0V30.2285C0.955078 38.4506 3.85704 46.1891 8.6936 52.7184C3.85704 59.2478 0.955078 66.9863 0.955078 75.2085V105.437C20.3013 105.437 39.1639 98.9076 52.7062 87.5417L56.3336 84.6397C46.9023 79.0777 41.0985 69.1627 41.0985 58.0387V47.3983C41.0985 36.516 46.9023 26.3592 56.3336 20.7972C65.7649 26.3592 71.5688 36.516 71.5688 47.3983V58.0387C71.5688 68.9209 65.7649 79.0777 56.3336 84.6397L59.961 87.5417C73.7452 98.9076 92.366 105.437 111.712 105.437V75.2085C111.712 66.9863 108.81 59.2478 103.974 52.7184C108.81 46.1891 111.712 38.4506 111.712 30.2285Z" fill="currentColor"/>
				</svg>
			</div>
			<p>2024</p>
		</div>
	</footer>
</div>

<style>
	@keyframes marquee {
		0% { transform: translateX(0); }
		100% { transform: translateX(-50%); }
	}
	.animate-marquee {
		animation: marquee 30s linear infinite;
	}
</style>

