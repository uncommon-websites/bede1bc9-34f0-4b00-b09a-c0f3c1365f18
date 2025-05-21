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
			title: "Innovation",
			description: "Constantly challenging the status quo to create better solutions."
		},
		{
			title: "Integrity",
			description: "Building trust through transparent actions and honest communication."
		},
		{
			title: "Impact",
			description: "Measuring our success by the positive change we create for our clients."
		}
	];
</script>

<SecondaryHero
	title="S3, now a local file system"
	subtitle="Skip the slowdowns—maximize GPU utilization and move fast with instant, POSIX-compatible cloud storage"
	imageSrc="/mockups/airport-screen-1747844124326.png"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Hunter Leath spent nearly a decade building cloud storage systems at Amazon and running storage infrastructure at Netflix. During that time, he saw the same problem again and again: companies were paying millions for GPUs, only to leave them sitting idle—waiting for data to load. Whether it was training models, running CI jobs, or processing massive files, moving data from S3 into fast local storage was a daily pain. Sync scripts, slow filesystems, and clunky transfers held teams back—and made compute painfully inefficient.",
		"Regatta Storage was born to fix this. Instead of forcing teams to wrestle with temporary storage or complex syncing setups, Regatta makes S3 feel like a local POSIX file system—with zero changes to application code. It turns any S3-compatible bucket into a local disk: read and write files instantly, process huge datasets in place, and keep cloud and local storage automatically in sync. With Regatta, teams can ship faster, scale smarter, and finally use expensive compute resources the way they were meant to be used.",
		"Our mission is simple: bring world-class data infrastructure to anyone working with large datasets—no matter the size of their company. The best engineering teams in the world shouldn't be the only ones with fast, efficient, scalable storage pipelines. Regatta makes local-speed cloud storage accessible to every data and AI team building the future."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Founder"
	subtitle="Built by a storage engineer who knows the pain firsthand."
	stakeholders={[
		{
			name: "Hunter Leath",
			position: "Founder & CEO",
			bio: "Hunter spent 8 years building Amazon's Elastic File System, then led Netflix's cloud storage team. Now he’s building Regatta Storage to finally solve the data bottlenecks that slow down modern workloads.",
			image: "/generated/image-a-professional-headshot-of-a-male-startu.webp"
		}
	]}
/>




<!-- CTA Section -->
<CallToAction
  title="Join us to build the backbone of cloud data."
  subtitle="Be part of a high-talent team solving the hard problems in data movement, infrastructure, and scale."
  description="Ready to help end slow data transfers and wasted GPUs? Reach out if you want to build foundational infrastructure, join the team, or invest in the future of cloud storage."
/>
"
	subtitle="Let's create something amazing"
	description="Join the companies already leveraging our expertise to transform their digital presence and achieve their business goals."
/>
