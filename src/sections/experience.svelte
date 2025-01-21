<script>
	import EachExperience from '../components/each_experience.svelte';
	import SectionTitle from '../components/section_title.svelte';

	// Images
	import stem from '$lib/assets/experience/stemlogo.png';
	import cisco from '$lib/assets/experience/ciscologo.png';
	import bdu from '$lib/assets/experience/bdulogo.png';
	import ibex from '$lib/assets/experience/ibexlogo.png';

	let experiences = [
		{
			company: 'Fullstack Website Developer Intern',
			logo: ibex,
			role: 'Fullstack Web Developer Intern',
			date: '2024 July — 2024 October',
			responsibilities: [''],
			description: [
				'A Fullstack Web Developer Intern at Ibex Technologies and Promotion, gaining hands-on experience in building and maintaining web applications, working with both front-end and back-end technologies to deliver innovative solutions.'
			]
		}
		// {
		// 	company: 'Bahir dar STEM Center',
		// 	logo: stem,
		// 	role: '',
		// 	date: '2018 - 2021',
		// 	responsibilities: [''],
		// 	description: [
		// 		'I completed high school at the Bahir Dar STEM Incubation Center, where I developed a strong passion for technology and innovation.'
		// 	]
		// },
		// {
		// 	company: 'Cisco CCNA , Addis Ababa University',
		// 	logo: cisco,
		// 	role: '',
		// 	date: '2023 December — 2024 March',
		// 	responsibilities: [''],
		// 	description: [
		// 		'A CISCO CCNA-certified professional with expertise in networking, focused on designing, configuring, and managing network systems to support business operations.'
		// 	]
		// },
		// {
		// 	company: 'ALX AiCE - Career Essentials',
		// 	logo: alx,
		// 	role: '',
		// 	date: '2024 May — 2024 July',
		// 	responsibilities: [''],
		// 	description: [
		// 		'A graduate of the ALX AICE Career Essentials program, specializing in artificial intelligence, with a focus on developing skills in AI technologies, problem-solving, and professional communication for a career in AI-driven industries.'
		// 	]
		// }
		// {
		// 	company: 'Artificial Intelligence and Robotics Center of Excellence',
		// 	logo: '',
		// 	role: 'Backend and DevOps Engineer',
		// 	date: 'February 2022 - Present',
		// 	responsibilities: [
		// 		'Deployed, secured and maintained multiple web apps',
		// 		'Wrote automating code to backup, log and maintain multiple projects',
		// 		'Write modern, performant, maintainable code for a diverse array of internal projects'
		// 	],
		// 	description: [
		// 		"I was a member of AASTU's Center of Excellence. It's a research and development program where I've developed multiple complex softwares and apps."
		// 	]
		// },
		// {
		// 	company: 'Arif Events',
		// 	logo: '',
		// 	role: 'web and mobile fullstack dev',
		// 	date: 'July - September 2019',
		// 	responsibilities: [
		// 		'Built new event management related features',
		// 		'Improved and maintained existing features'
		// 	],
		// 	description: [
		// 		'ArifEvents was my first internship where I worked on multiple projects and features.'
		// 	]
		// }
	];
</script>

<div class="pb-10">
	<SectionTitle title={'Experience'} />
	<div class="pl-10">
		<div class="h-7 border-l border-dashed border-zinc-900"></div>
	</div>

	{#each experiences as experience}
		<EachExperience {experience} />
	{/each}
</div>
