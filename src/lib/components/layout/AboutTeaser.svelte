<!--
@component AboutTeaser
An engaging founder story teaser that builds personal connection and company credibility.
-->
<script lang="ts">
	// Types
	type TeamMember = {
		name: string;
		role: string;
		image: string;
	};

	// Components
	import Button from "../ui/Button.svelte";
	import ScrollText from "./sub/ScrollText.svelte";

	// State
	let sectionRef: HTMLElement;

	let props = $props();

	// Data
	const teamMember: TeamMember = {
		name: "Bob Deforce",
		role: "Co-Founder",
		image: "/generated/image-a-professional-startup-founder-sitting-a.webp"
	};
</script>

<section bind:this={sectionRef} {...props}>
	<div class="section-px section-py container mx-auto">
		<div class="relative mx-auto grid max-w-4xl place-items-center gap-16">
			<ScrollText
				class="text-title1 text-center"
				text={`"We watched talented founders spend 80% of their time fundraising just to raise tiny checks. So we built a way to flip the model—where capital chases execution, not the other way around."`}
			/>

			<!-- Team Member & CTA Section -->
			<div class="grid items-center gap-8">
				<div class="flex items-center justify-center gap-6">
					<img
						src={teamMember.image}
						alt={teamMember.name}
						class="size-16 rounded-full object-cover ring-2 ring-gray-100"
					/>
					<div class="text-center sm:text-left">
						<div class="text-callout font-medium">{teamMember.name}</div>
						<div class="text-caption text-emphasis-low">{teamMember.role}</div>
						<div class="text-caption text-emphasis-low mt-1">Former operator, now connecting builders with capital</div>
					</div>
					<Button 
						href="/about" 
						variant="secondary" 
						size="sm" 
						class="ml-8 transition-all hover:scale-105"
					>
						Read our story
					</Button>
				</div>
			</div>

			<!-- Context hint -->
			<div class="text-center">
				<p class="text-body text-emphasis-medium max-w-2xl">
					From sitting on both sides of the funding table to building the platform we wished existed—discover how we're transforming the $330B private equity market for technical founders and angel investors.
				</p>
			</div>
		</div>
	</div>
</section>
