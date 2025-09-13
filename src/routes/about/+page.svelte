<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Operator first",
			description: "We understand operator networks from the inside because we are operators. This gives us unique insight into building infrastructure that actually works."
		},
		{
			title: "Signal over noise",
			description: "High-quality, curated deal flow beats volume every time. We focus on connecting the right people at the right moment."
		},
		{
			title: "Build relationships, not spreadsheets",
			description: "Technology should eliminate admin overhead so angels and founders can focus on what matters—building connections and great companies."
		}
	];
</script>

<SecondaryHero
	title="Fundraising without gatekeepers"
	subtitle="Real access through real operators"
	imageSrc="/generated/image-two-founders-collaborating-in-a-modern-w.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"We saw too many high-potential founders struggling to raise money—not because they lacked talent, but because they weren't plugged into the right networks. And we saw angels wasting hours every week on Slack threads, spreadsheets, and scouting that went nowhere. We knew there was a better way.",
		"We started connecting technical founders and operator angels through the networks we trusted. What started as a handful of introductions grew fast—so we built the infrastructure investors actually needed: curated access, streamlined deal reviews, and tools that reduce admin overhead by 80%.",
		"Today, Execution gives angels consistent, high-signal deal flow from AI-native technical teams. Founders get access to capital without giving up control. Investors get to focus on what really matters—building relationships and backing companies early. We're just getting started."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Our team."
	subtitle="Operators building infrastructure for modern angel investing."
	stakeholders={[
		{
			name: "Bob Deforce",
			position: "Co-Founder",
			bio: "Building the infrastructure that connects technical founders with the right investors.",
			image: "/generated/image-a-young-business-executive-with-a-confid.webp"
		},
		{
			name: "Jaime Vico van Berkel",
			position: "Co-Founder",
			bio: "Leveraging operator networks to streamline angel investing and deal sourcing.",
			image: "/generated/image-a-tech-entrepreneur-with-a-thoughtful-ex.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to transform how you invest?"
	subtitle="Join the operator network"
	description="Stop wasting 80% of your time on admin work. Get curated deal flow from technical founders building AI startups, streamlined through exclusive operator networks. Angels get focused relationship-building. Founders get capital without losing control."
/>
