<script lang="ts">
	// Components
	import UseCases from "$lib/components/layout/UseCases.svelte";
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
</script>

<CustomerCardHero
  title="Your cloud storage, now local"
  subtitle="Regatta turns S3 into a fast, local file system—so your data is always ready when compute is."
  customers={[
    {
      name: "Dr. Emily Carter",
      position: "AI Research Engineer, Salesforce",
      imageSrc: "/generated/image-a-smiling-female-engineer-in-a-modern-wo.webp"
    },
    {
      name: "Marcus Lin",
      position: "CI/CD Developer, Depot",
      imageSrc: "/generated/image-a-confident-male-developer-at-his-workst.webp"
    },
    {
      name: "Alexis Reed",
      position: "Platform Lead, Neon",
      imageSrc: "/generated/image-a-professional-female-lead-in-a-bustling.webp"
    },
    {
      name: "Ryan Patel",
      position: "Observability Specialist, Axiom",
      imageSrc: "/generated/image-a-male-specialist-in-an-open-workspace-p.webp"
    },
    {
      name: "Priya Mukherjee",
      position: "Satellite Imagery Scientist, ValueSpace",
      imageSrc: "/generated/image-a-female-data-scientist-in-a-collaborati.webp"
    }
  ]}
  centered={false}
/>

<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		'https://logo.clearbit.com/nvidia.com',
		'https://logo.clearbit.com/salesforce.com',
		'https://logo.clearbit.com/zillow.com',
		'https://logo.clearbit.com/depot.dev'
	]}
/>

<Summary
	title="What we do"
	text="Regatta Storage makes S3 cloud storage work like a local file system, eliminating slow data transfers and keeping your GPUs busy. Get instant, POSIX-compatible access to huge datasets—without re-architecting your workflow. Simple, seamless performance for teams with real data needs."
/>

<Testimonials
	generating
	testimonials={[
		{
			name: "Jane Smith",
			position: "CTO",
			company: "Tech Innovations",
			quote:
				"Their cutting-edge automation boosted our productivity by 35%.\nThe intuitive interface reduced training time and improved team adoption.",
			image:
				"https://images.unsplash.com/photo-1571513722275-4b41940f54b8?q=80&w=3687&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
		},
		{
			name: "John Doe",
			position: "Director of Operations",
			company: "Global Solutions",
			quote:
				"Their robust security protocols gave us confidence in handling sensitive data.\nThe 24/7 support team resolved issues within hours, not days.",
			image:
				"https://images.unsplash.com/photo-1600603405959-6d623e92445c?q=80&w=3687&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
		},
		{
			name: "Sarah Johnson",
			position: "Product Manager",
			company: "Future Systems",
			quote:
				"The scalable platform grew seamlessly with our business needs.\nTheir customization options allowed us to tailor solutions perfectly to our workflows.",
			image:
				"https://images.unsplash.com/photo-1531123897727-8f129e1688ce?q=80&w=3687&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
		}
	]}
/>

<Features
	title="Why teams choose Regatta"
	subtitle={undefined}
	features={[
		{
			title: "Your files, instantly available",
			description: "Access cloud-hosted data as if it were local—no downloads, no sync lag, and no spinning up temp volumes just to get work done."
		},
		{
			title: "Local file system that runs on S3",
			description: "Regatta makes your S3 buckets behave like a POSIX-compliant local file system with full support for existing tools and pipelines."
		},
		{
			title: "Zero changes to your stack",
			description: "Drop-in replacement for EFS and EBS—plug into data-intensive applications without rearchitecting workloads or rewriting code."
		},
		{
			title: "GPUs never wait on data",
			description: "Stream massive datasets directly to your compute nodes so expensive resources don't sit idle during training, testing, or deploy."
		},
		{
			title: "Runs anywhere S3 does",
			description: "Compatible with all S3 and S3-like services, offering flexibility and portability with no vendor lock-in or region restrictions."
		},
		{
			title: "Built for scale, built by experts",
			description: "Designed by storage leaders from AWS and Netflix to handle multi-petabyte workloads with confidence, performance, and simplicity."
		}
	]}
/>

<UseCases
	title="Use Cases"
	subtitle="Real-world applications for your business needs"
	useCases={[
		{
			title: "Faster AI training and iteration",
			description: "Run ML training jobs and experiments without waiting for datasets to copy—access S3 storage at local speeds, so your GPUs stay busy, not idle.",
			image: "/generated/image-a-group-of-researchers-collaborating-in-.webp",
			link: {
				href: "/use-cases/ai-training-performance",
				label: "Learn more"
			}
		},
		{
			title: "Instant data for CI/CD pipelines",
			description: "Eliminate long build times and flaky tests caused by slow storage—give engineering teams direct, fast access to gigabytes of artifacts and dependencies.",
			image: "/generated/image-engineers-in-a-contemporary-office-setti.webp",
			link: {
				href: "/use-cases/faster-ci-cd",
				label: "Learn more"
			}
		},
		{
			title: "Faster analytics and observability",
			description: "Query and analyze huge volumes of cloud data in real time, keeping dashboards and platforms responsive for your users.",
			image: "/generated/image-a-team-of-professionals-in-a-bustling-of.webp",
			link: {
				href: "/use-cases/analytics-observability",
				label: "Learn more"
			}
		}
	]}
/>

<AboutTeaser
  quote="It kept bugging me—you shouldn’t need to copy all your data locally just to do fast compute in the cloud."
  name="Hunter Leath"
  title="Founder, Regatta Storage"
  image="/generated/image-a-founder-and-an-engineer-collaborating-.webp"
/>
<CallToAction
  title="Your GPUs shouldn’t wait on data"
  subtitle="Run at full speed with local-like cloud storage — no manual downloads, syncing, or re-architecting."
  description="Keep your workloads moving and your engineers happy. Regatta makes S3 feel like a local file system, so teams no longer wait on data transfers and GPUs never sit idle. Fast, reliable, and easy to deploy."
  imageSrc="/generated/image-a-smiling-cloud-infrastructure-engineer-.webp"
  callsToAction={[{ href: '/get-started', label: 'Try Regatta free', variant: 'primary' }]}
/>

