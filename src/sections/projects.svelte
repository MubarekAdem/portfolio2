<script lang="ts">
	import { ExternalLink, Github, MoveDiagonal } from 'lucide-svelte';
	import EachProject_2 from '../components/each_project_2.svelte';
	import SectionTitles from '../components/section_title.svelte';
	import ExtraProjects from '../components/extra_projects.svelte';

	// Project Images

	import ecommerce from '$lib/assets/projects/ecommerce.png';
	import ZikrApp from '$lib/assets/projects/zikrapp.png';
	import RuthfulHearts from '$lib/assets/projects/RuthfulHearts.png';
	import BreakingNews from '$lib/assets/projects/breakingnews.png';
	import TelegramCommunityGallery from '$lib/assets/projects/TelegramCommunityGallery.jpg';
	import MyBible from '$lib/assets/projects/MyBible.png';
	import AASTUECSFApp from '$lib/assets/projects/AASTUECSFApp.png';
	import FidelPops from '$lib/assets/projects/FidelPops.jpg';
	import MenenArts from '$lib/assets/projects/MenenArts.png';
	import EthioDatasets from '$lib/assets/projects/EthioDatasets.png';
	import Projectify from '$lib/assets/projects/projectify.png';
	import StatiCall from '$lib/assets/projects/projectify.png';

	let Projects = [
		{
			title: 'Projectify',
			image: Projectify,
			description:
				'Projectify is an AI-powered platform designed to streamline project analysis, generate innovative ideas, and assist you in managing your projects effectively. By leveraging cutting-edge AI technologies, Projectify helps you save time, improve productivity, and achieve your goals seamlessly.',
			link: 'https://project-fy-tau.vercel.app/',
			code: 'https://github.com/MubarekAdem/project-analyser',
			tools: ['NextJS', 'Gemini', 'TailwindCSS']
		},
		{
			title: 'My E-Commerce ( ongoing )',
			image: ecommerce,
			description:
				'An intuitive and responsive e-commerce platform built to provide a seamless shopping experience. Featuring product management, user authentication, role-based access, secure checkout, and customer reviews, this project showcases modern web development practices using Next.js, Tailwind CSS, and a custom authentication system. Optimized for both desktop and mobile views, it offers a user-friendly interface for browsing, adding to cart, and making purchases.',
			link: 'https://e-commerce-store-three-blush.vercel.app/',
			code: 'https://github.com/MubarekAdem/e-commerce-store',
			tools: ['ReactJS', 'TailwindCSS', 'NodeJS', 'MongoDB']
		},
		{
			title: 'Fake News Generator',
			image: BreakingNews,
			description:
				"A fun and creative website that allows users to generate their own breaking news headlines. Inspired by breakyourownnews.com, this tool lets users customize headlines with various categories, making it easy to create and share unique, fictional news stories. Built with a user-friendly interface, it's designed for quick and engaging content creation.",
			link: 'https://breakingnewsgenerator.vercel.app/',
			code: 'https://github.com/MubarekAdem/breaking-news-generator',
			tools: ['NextJS', 'TailwindCSS']
		},
		{
			title: 'My-Zikr-App',
			image: ZikrApp,
			description:
				'An Islamic and enriching web application designed to enhance the daily practices of Muslims. Built with Next.js, My Zikr App provides users with features like Quran reading, tasbeeh counters for dhikr (remembrance of Allah), curated collections of duas (supplications), and authentic hadiths. With a sleek and intuitive interface, it ensures seamless navigation and a focused user experience. The app also plans to include more features, such as daily reminders, Islamic calendar integration and more.',
			link: 'https://my-zikr-app.vercel.app/',
			code: 'https://github.com/MubarekAdem/my-zikr-app',
			tools: ['NextJS', 'TailwindCSS']
		}
	];

	let extraProjects = [
		{
			title: 'Des Encryption algorithm',
			link: 'https://github.com/MubarekAdem/des-encryption-algoritm'
		},
		{
			title: 'Inventory Management',
			link: 'https://github.com/MubarekAdem/inventory-management'
		},
		{
			title: 'Joke API',
			link: 'https://github.com/MubarekAdem/inventory-management'
		}
		// {
		// 	title: 'TG Chat Analyzer',
		// 	link: 'https://chat-dagmawibabi.vercel.app/'
		// },
		// {
		// 	title: 'Lexicon',
		// 	link: 'https://github.com/dagmawibabi/Lexicon/releases/latest'
		// },
		// {
		// 	title: 'Survival Manual',
		// 	link: 'https://github.com/dagmawibabi/OfflineSurvivalManual/releases/latest'
		// },
		// {
		// 	title: 'I Am Ninja',
		// 	link: 'https://github.com/dagmawibabi/IAmNinja'
		// },
		// {
		// 	title: 'Beautiful OS',
		// 	link: 'https://github.com/dagmawibabi/beautifulelectronsurface'
		// }
	];

	// Additional projects omitted for brevity...
</script>

<div class="pb-10">
	<!-- AI/ML PROJECTS -->
	<div class="pb-10">
		<SectionTitles title={'Web Projects'} />
		{#each Projects as project}
			<EachProject_2 {project} />
		{/each}
	</div>

	<!-- CHRISTIAN PROJECTS -->
	<!-- <div class="pb-10">
		<SectionTitles title={'Christian Projects'} />
		{#each christianProjects as project}
			<EachProject_2 {project} />
		{/each}
	</div> -->

	<!-- SOCIAL PROJECTS -->
	<!-- <div class="pb-10">
		<SectionTitles title={'Social Projects'} />
		{#each socialProjects as project}
			<EachProject_2 {project} />
		{/each}
	</div> -->
	<!-- <div class="pb-10">
		<SectionTitles title={'Notable Projects'} />
		{#each notableProjects as project}
			<EachProject_2 {project} />
		{/each}
	</div> -->

	<!-- GAMES?? -->

	<!-- EXTRA PROJECTS -->
	<SectionTitles title={' Extra Projects'} />
	<ExtraProjects {extraProjects} />
</div>
