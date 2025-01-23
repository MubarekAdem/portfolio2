<script lang="ts">
	import {
		Instagram,
		Github,
		Linkedin,
		Plane,
		Mail,
		Twitter,
		PlaneIcon,
		LucidePlane,
		Send,
		Phone,
		Smile
	} from 'lucide-svelte';
	import logo from '$lib/assets/logo//DagmawiBabiLogo.png';

	import me from '$lib/assets/me/Me.png';
	import me2 from '$lib/assets/me/Me2.png';
</script>

<div class="border-dashed border-black pb-5">
	<div class="group flex items-center">
		<div
			class="flex flex-col gap-x-3 rounded border-zinc-300 px-2 py-2 pr-4 lg:flex-row xl:flex-row 2xl:flex-row"
		>
			<!-- TITLE -->
			<div class="flex items-center gap-x-2 md:flex lg:hidden xl:hidden 2xl:hidden">
				<div class="flex flex-col justify-center">
					<div class="text-xl font-semibold">Mubarek Adem</div>
					<span class="-mt-1">Website Developer</span>
				</div>
			</div>

			<!-- PROJECT IMAGE -->
			<div class="group/me h-56 w-[50%] cursor-pointer rounded md:h-56 lg:h-72 xl:h-72 2xl:h-72">
				<img src={me} alt="project" class="h-full w-full object-contain group-hover/me:hidden" />
				<img
					src={me2}
					alt="project"
					class="hidden h-full w-full object-contain group-hover/me:block"
				/>
			</div>

			<!-- PROJECT DETAILS -->
			<div class="flex w-full flex-col justify-center gap-y-4">
				<!-- TITLE -->
				<div class="hidden items-center gap-x-2 md:hidden lg:flex xl:flex 2xl:flex">
					<div class="flex flex-col justify-center">
						<div class="text-xl font-semibold">Mubarek Adem</div>
						<span class="-mt-1">Website Developer</span>
					</div>
				</div>

				<!-- DESCRIPTION -->
				<div class="flex flex-col gap-y-2">
					<p class="text-sm">
						Hello! My name is Mubarek and I’m a Full Stack Developer focused on building dynamic,
						scalable web applications. I create seamless end-to-end solutions, from responsive
						front-end interfaces to robust back-end systems, using modern frameworks and APIs to
						deliver fast, secure, and scalable results.
					</p>
				</div>

				<!-- CTA -->
				<div class="flex items-center gap-x-2">
					<!-- Social Links -->
					<div
						class="flex items-center justify-center gap-x-3 rounded-full border-zinc-300 py-1 text-sm transition-all hover:border-black"
					>
						<a href="https://www.t.me/MubarekA" target="_blank" rel="noopener noreferrer">
							<Send
								class="cursor-pointer text-sm text-zinc-700 hover:scale-125 hover:text-cyan-500"
								size={20}
							/>
						</a>
						<a
							href="https://www.linkedin.com/in/Mubarek-adem"
							target="_blank"
							rel="noopener noreferrer"
						>
							<Linkedin
								class="cursor-pointer text-sm text-zinc-700 hover:scale-125 hover:text-blue-500"
								size={20}
							/>
						</a>
						<a
							href="https://www.instagram.com/m.u.b.a.r.e.k_a"
							target="_blank"
							rel="noopener noreferrer"
						>
							<Instagram
								class="cursor-pointer text-sm text-zinc-700 hover:scale-125 hover:text-pink-600"
								size={20}
							/>
						</a>
						<a href="https://www.x.com/beatus_ad" target="_blank" rel="noopener noreferrer">
							<Twitter
								class="cursor-pointer text-sm text-zinc-700 hover:scale-125 hover:text-blue-500"
								size={20}
							/>
						</a>
						<a href="https://www.github.com/mubarekadem" target="_blank" rel="noopener noreferrer">
							<Github
								class="hover:text-black-500 cursor-pointer text-sm text-zinc-700 hover:scale-125"
								size={20}
							/>
						</a>
						<a href="mailto:mubarekadem001@gmail.com" target="_blank" rel="noopener noreferrer">
							<Mail
								class="cursor-pointer text-sm text-zinc-700 hover:scale-125 hover:text-green-500"
								size={20}
							/>
						</a>
					</div>

					<!-- Download CV Button -->
					<a
						href="https://drive.google.com/file/d/1dYtqi91taWfYkmv-W54JHdYXB_sP9G8k/view?usp=drive_link"
						class="rounded-full border border-black bg-black px-4 py-2 text-sm font-semibold text-white transition-all hover:bg-white hover:text-black"
					>
						Download CV
					</a>
				</div>
			</div>
		</div>
	</div>
</div>
