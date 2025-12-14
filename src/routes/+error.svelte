<script lang="ts">
	import { page } from "$app/state";
</script>

<div class="min-h-screen bg-[#F4F4F2] text-[#1A1A1A] font-sans flex items-center justify-center px-4">
	<div class="text-center">
		<h1 class="text-8xl md:text-9xl font-thin tracking-tighter mb-4 uppercase">{page.status}</h1>
		<p class="text-sm uppercase tracking-wide font-medium mb-8 text-gray-500">{page.error?.message ?? "Something went wrong."}</p>
		<a href="/" class="inline-block bg-[#1A1A1A] text-white px-10 py-4 rounded-full text-[10px] font-bold uppercase tracking-widest hover:bg-primary-500 transition-colors">
			Return Home
		</a>
	</div>
</div>
