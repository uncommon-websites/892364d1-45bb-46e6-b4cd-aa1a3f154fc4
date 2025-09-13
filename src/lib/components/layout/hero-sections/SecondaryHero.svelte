<script lang="ts">
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";

	let {
		title,
		subtitle,
		imageSrc = "https://www.unc.mn/image-placeholder.svg",
		...rest
	}: {
		title: string;
		subtitle: string;
		imageSrc: string;
		[key: string]: any;
	} = $props();
</script>

<header class="relative bg-gray-900 dark:bg-gray-950" {...rest}>
	<div class="absolute inset-0 bg-gradient-to-br from-purple-900/20 to-orange-900/20"></div>
	<div class="relative container mx-auto section-px">
		<!-- Hero Content -->
		<div class="py-24 lg:py-32 grid gap-16 lg:grid-cols-2 lg:gap-24 items-center">
			<div class="space-y-8">
				<div class="space-y-4">
					<h1 class="text-4xl lg:text-5xl xl:text-6xl font-bold text-white leading-tight">
						{title}
					</h1>
					<p class="text-xl lg:text-2xl text-gray-300 font-medium">
						{subtitle}
					</p>
				</div>
			</div>
			
			<!-- Hero Image -->
			<div class="aspect-video overflow-hidden rounded-2xl bg-gray-800 border border-gray-700">
				<img
					class="h-full w-full object-cover"
					src={imageSrc}
					alt="Execution team collaborating in modern workspace"
				/>
			</div>
		</div>
	</div>
</header>
