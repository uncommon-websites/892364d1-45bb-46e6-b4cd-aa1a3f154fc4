<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
</script>

<CustomerCardHero
	centered={true}
	title="Connect builders directly with curated angel investors"
	subtitle="Execution transforms startup funding access through exclusive operator networks, helping technical founders secure investment while preserving equity control."
	customers={[
		{
			name: "Michael Chen",
			position: "Angel Investor at Sequoia Capital",
			imageSrc: "/generated/image-a-professional-male-angel-investor-in-bu.webp"
		},
		{
			name: "Sarah Martinez",
			position: "Technical Founder, AI Startup",
			imageSrc: "/generated/image-a-female-technical-founder-wearing-casua.webp"
		},
		{
			name: "David Rodriguez",
			position: "Startup Founder & Builder",
			imageSrc: "/generated/image-a-male-startup-founder-in-a-modern-offic.webp"
		},
		{
			name: "Elena Thompson",
			position: "Angel Investor & Former VP",
			imageSrc: "/generated/image-a-professional-female-angel-investor-in-.webp"
		},
		{
			name: "James Wilson",
			position: "Technical Founder & CTO",
			imageSrc: "/generated/image-a-male-technical-founder-in-casual-profe.webp"
		}
	]}
/>
<LogoScroller 
	label="Trusted by industry leaders"
	logoUrls={[
		'https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/a16z.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/ycombinator.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/stripe.com/w/400/h/400/logo'
	]}
/>

<Summary
	title="What we do"
	text="We eliminate the friction between technical founders and angel investors through exclusive operator networks that understand both sides of the funding equation. Angel investors gain access to 50+ high-quality deals monthly from vetted technical founders, while builders preserve equity control through our innovative scout check system. Our platform transforms the $330B private equity market by connecting the right people at the right time, reducing administrative overhead by 80% so investors can focus on what matters most—building relationships with exceptional founders."
/>

<Testimonials
	testimonials={[
		{
			name: "Alexandra Chen",
			position: "Partner",
			company: "Northgate Ventures",
			quote:
				"Execution reduced my deal sourcing time from 15 hours to 3 hours per week. Their curated operator network connects me directly with technical founders building solutions I actually want to invest in. I've closed 4 deals this quarter that I never would have found otherwise.",
			image: "/generated/image-a-professional-female-angel-investor-in-.webp"
		},
		{
			name: "Marcus Rodriguez",
			position: "Angel Investor",
			company: "TechStars Alumni Fund",
			quote:
				"The platform eliminated 80% of my administrative overhead in evaluating startups. Instead of spending hours on due diligence prep, I can focus on relationship building with founders. My investment decision time dropped from 6 weeks to 2 weeks while maintaining quality.",
			image: "/generated/image-a-confident-male-angel-investor-at-an-in.webp"
		},
		{
			name: "Priya Patel",
			position: "Managing Director",
			company: "Scale Ventures",
			quote:
				"Execution's scout network gave me early access to AI startups before they hit traditional channels. The risk assessment tools helped me avoid 3 potential bad investments this year, saving our fund over $500K. The ROI on quality deal flow is unprecedented.",
			image: "/generated/image-a-diverse-group-of-professional-angel-in.webp"
		}
	]}
/>

<Features
	title="Why angel investors choose Execution"
	subtitle="Transform your deal sourcing from administrative burden into strategic advantage"
	features={[
		{
			title: "Curated operator networks",
			description: "Access exclusive deal flow from validated technical founders building AI startups through our insider operator connections.",
			imageSrc: "/generated/image-a-diverse-group-of-technical-founders-mi.webp"
		},
		{
			title: "Scout checks that preserve equity",
			description: "Deploy capital efficiently with scout investments that protect founder control while securing your position in high-potential deals.",
			imageSrc: "/generated/image-a-professional-handshake-taking-place-be.webp"
		},
		{
			title: "50+ monthly deal opportunities",
			description: "Source quality deals consistently from our network of builders actively raising capital in AI, developer tools, and infrastructure.",
			imageSrc: "/generated/image-a-group-of-angel-investors-sitting-aroun.webp"
		},
		{
			title: "Direct founder connections",
			description: "Skip the intermediaries and build relationships directly with technical founders who understand your investment thesis."
		},
		{
			title: "Pre-validated startups",
			description: "Every deal is sourced through operator networks, ensuring founders have real traction and technical credibility before reaching you."
		},
		{
			title: "Administrative efficiency",
			description: "Focus 80% of your time on relationship building instead of deal administration with our streamlined investment workflow."
		}
	]}
/>
<AboutTeaser />
<CallToAction
	title="Stop spending 80% of your time on deal administration"
	subtitle="Start investing in relationships"
	description="Join 500+ angel investors who've transformed their deal sourcing from administrative burden into strategic advantage. Access 50+ curated deals monthly from validated technical founders through our exclusive operator networks. No more endless email chains, pitch deck reviews, or calendar coordination—just quality deals that match your investment thesis."
	imageSrc="/generated/image-a-confident-angel-investor-sitting-at-a-.webp"
	callsToAction={[
		{
			href: "/get-started",
			label: "Get early access",
			variant: "primary"
		},
		{
			href: "/contact",
			label: "Schedule demo",
			variant: "secondary"
		}
	]}
/>
