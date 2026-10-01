<script lang="ts">
	import Header from '$lib/components/Header.svelte';
	import Footer from '$lib/components/Footer.svelte';
	const steps = [
		{
			number: '01',
			title: 'Upload your plans',
			text: 'Start with your project plan set and supporting documents.'
		},
		{
			number: '02',
			title: 'PlanSmart reviews them',
			text: 'The system reviews the submitted plans and identifies items that need attention.'
		},
		{
			number: '03',
			title: 'Review the findings',
			text: 'See the findings organized into a clear, reviewable format.'
		},
		{
			number: '04',
			title: 'Get the report',
			text: 'Receive a structured review report you can use before submission.'
		}
	];
</script>

<svelte:head>
	<title>How It Works | PlanSmartAI</title>
	<meta
		name="description"
		content="See how PlanSmartAI reviews project plans and produces a clear review report before submission."
	/>
</svelte:head>
<Header />
<!-- HERO -->
<section class="bg-white px-6 pb-20 pt-16 sm:px-8 lg:px-12 lg:pb-28 lg:pt-24">
	<div class="mx-auto max-w-6xl text-center">
		<p class="mb-4 text-xs font-semibold uppercase tracking-[0.2em] text-[#8b6b32]">
			HOW PLANSMART WORKS
		</p>

		<h1 class="mx-auto max-w-4xl text-4xl font-semibold tracking-[-0.03em] text-black sm:text-5xl lg:text-6xl">
			From plan set to review-ready report.
		</h1>

		<p class="mx-auto mt-6 max-w-2xl text-base leading-7 text-neutral-600 sm:text-lg">
			See the complete process from the moment a project is submitted to the final review report.
		</p>
	</div>
</section>

<!-- VIDEO -->
<section class="bg-[#111111] px-6 py-16 sm:px-8 lg:px-12 lg:py-24">
	<div class="mx-auto max-w-6xl">
		<div class="mb-10 max-w-2xl">
			<p class="text-xs font-semibold uppercase tracking-[0.2em] text-[#d4a84b]">
				SEE IT IN ACTION
			</p>

			<h2 class="mt-3 text-3xl font-semibold tracking-tight text-white sm:text-4xl">
				Watch the process from start to finish.
			</h2>

			<p class="mt-4 leading-7 text-neutral-400">
				Follow a real project through the PlanSmart review process.
			</p>
		</div>

		<!-- VIDEO PLACEHOLDER -->
		<div class="relative aspect-video overflow-hidden border border-white/10 bg-neutral-900">
			<div class="absolute inset-0 flex flex-col items-center justify-center text-center">
				<div class="mb-5 flex h-16 w-16 items-center justify-center rounded-full border border-[#d4a84b] text-[#d4a84b]">
					<svg viewBox="0 0 24 24" class="ml-1 h-6 w-6 fill-current">
						<path d="M8 5v14l11-7z" />
					</svg>
				</div>

				<p class="text-sm font-medium uppercase tracking-wider text-white">
					Process Video Placeholder
				</p>

				<p class="mt-2 text-sm text-neutral-500">
					Final walkthrough video will be placed here
				</p>
			</div>
		</div>
	</div>
</section>

<!-- PROCESS -->
<section class="bg-white px-6 py-20 sm:px-8 lg:px-12 lg:py-28">
	<div class="mx-auto max-w-6xl">
		<div class="max-w-2xl">
			<p class="text-xs font-semibold uppercase tracking-[0.2em] text-[#8b6b32]">
				THE PROCESS
			</p>

			<h2 class="mt-3 text-3xl font-semibold tracking-tight text-black sm:text-4xl">
				One workflow. Four clear steps.
			</h2>
		</div>

		<div class="mt-14 grid gap-px overflow-hidden border border-neutral-200 bg-neutral-200 md:grid-cols-2 lg:grid-cols-4">
			{#each steps as step}
				<div class="bg-white p-7 lg:p-8">
					<span class="text-sm font-semibold text-[#8b6b32]">
						{step.number}
					</span>

					<h3 class="mt-10 text-lg font-semibold text-black">
						{step.title}
					</h3>

					<p class="mt-3 text-sm leading-6 text-neutral-600">
						{step.text}
					</p>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- INPUT / OUTPUT -->
<section class="bg-[#f5f4f1] px-6 py-20 sm:px-8 lg:px-12 lg:py-28">
	<div class="mx-auto max-w-6xl">
		<div class="text-center">
			<p class="text-xs font-semibold uppercase tracking-[0.2em] text-[#8b6b32]">
				FROM INPUT TO OUTPUT
			</p>

			<h2 class="mx-auto mt-3 max-w-3xl text-3xl font-semibold tracking-tight text-black sm:text-4xl">
				See what goes in — and what comes out.
			</h2>

			<p class="mx-auto mt-4 max-w-2xl leading-7 text-neutral-600">
				Use the example project to understand how the review moves from the original plan set to the final deliverable.
			</p>
		</div>

		<div class="mt-14 grid gap-8 lg:grid-cols-2">

			<!-- PLAN SET -->
			<div>
				<div class="mb-4 flex items-center justify-between">
					<div>
						<p class="text-xs font-semibold uppercase tracking-[0.16em] text-neutral-500">
							INPUT
						</p>

						<h3 class="mt-1 text-xl font-semibold text-black">
							Project plan set
						</h3>
					</div>

					<span class="text-xs text-neutral-500">
						PDF
					</span>
				</div>

				<div class="flex aspect-[4/3] items-center justify-center border border-neutral-300 bg-white p-8 shadow-sm">
					<div class="w-full max-w-sm border border-neutral-300 bg-neutral-50 p-8 text-center">
						<div class="mx-auto mb-5 h-20 w-16 border border-neutral-400 bg-white shadow-sm">
							<div class="space-y-2 p-3">
								<div class="h-1 bg-neutral-300"></div>
								<div class="h-1 w-3/4 bg-neutral-300"></div>
								<div class="mt-5 h-8 border border-neutral-300"></div>
								<div class="h-1 bg-neutral-300"></div>
							</div>
						</div>

						<p class="text-sm font-semibold text-black">
							Moana East Building 24 × 36
						</p>

						<p class="mt-1 text-xs text-neutral-500">
							FULL PERMIT PLAN SET
						</p>

						<p class="mt-5 text-xs text-neutral-400">
							Plan preview placeholder
						</p>
					</div>
				</div>
			</div>

			<!-- REPORT -->
			<div>
				<div class="mb-4 flex items-center justify-between">
					<div>
						<p class="text-xs font-semibold uppercase tracking-[0.16em] text-neutral-500">
							OUTPUT
						</p>

						<h3 class="mt-1 text-xl font-semibold text-black">
							Review report
						</h3>
					</div>

					<span class="text-xs text-neutral-500">
						PDF
					</span>
				</div>

				<div class="flex aspect-[4/3] items-center justify-center border border-neutral-300 bg-white p-8 shadow-sm">
					<div class="w-full max-w-sm border border-neutral-300 bg-white p-7 shadow-md">
						<div class="border-b border-neutral-200 pb-4">
							<p class="text-xs font-semibold uppercase tracking-wider text-[#8b6b32]">
								PLANSMARTAI
							</p>

							<p class="mt-2 text-lg font-semibold text-black">
								Plan Review Report
							</p>

							<p class="mt-1 text-xs text-neutral-500">
								Moana East Building 24 × 36
							</p>
						</div>

						<div class="mt-5 space-y-3">
							<div class="h-2 w-full bg-neutral-200"></div>
							<div class="h-2 w-5/6 bg-neutral-200"></div>
							<div class="h-2 w-4/6 bg-neutral-200"></div>
							<div class="mt-5 h-10 border border-neutral-200"></div>
							<div class="h-10 border border-neutral-200"></div>
						</div>

						<p class="mt-5 text-center text-[10px] text-neutral-400">
							Final report preview placeholder
						</p>
					</div>
				</div>

				<div class="mt-5">
					<button
						class="inline-flex items-center justify-center bg-black px-6 py-3 text-sm font-semibold text-white transition hover:bg-neutral-800"
					>
						Download Sample Report
					</button>
				</div>
			</div>

		</div>
	</div>
</section>

<!-- FINDINGS -->
<section class="bg-white px-6 py-20 sm:px-8 lg:px-12 lg:py-28">
	<div class="mx-auto grid max-w-6xl gap-12 lg:grid-cols-[0.85fr_1.15fr] lg:items-center">

		<div>
			<p class="text-xs font-semibold uppercase tracking-[0.2em] text-[#8b6b32]">
				THE RESULT
			</p>

			<h2 class="mt-3 text-3xl font-semibold tracking-tight text-black sm:text-4xl">
				Findings that are easier to understand and act on.
			</h2>

			<p class="mt-5 leading-7 text-neutral-600">
				The final report brings the review into one place, giving the project team a clear view of the items identified during the process.
			</p>
		</div>

		<!-- FINDINGS IMAGE PLACEHOLDER -->
		<div class="border border-neutral-200 bg-[#f7f7f7] p-5">
			<div class="border border-neutral-300 bg-white p-6">
				<div class="flex items-center justify-between border-b border-neutral-200 pb-4">
					<div>
						<div class="h-3 w-28 bg-neutral-800"></div>
						<div class="mt-2 h-2 w-40 bg-neutral-200"></div>
					</div>

					<div class="h-8 w-8 rounded-full bg-neutral-100"></div>
				</div>

				<div class="mt-6 space-y-4">
					<div class="border border-neutral-200 p-4">
						<div class="flex justify-between">
							<div class="h-2 w-32 bg-neutral-300"></div>
							<div class="h-2 w-14 bg-[#d4a84b]"></div>
						</div>
						<div class="mt-3 h-2 w-full bg-neutral-100"></div>
						<div class="mt-2 h-2 w-4/5 bg-neutral-100"></div>
					</div>

					<div class="border border-neutral-200 p-4">
						<div class="h-2 w-40 bg-neutral-300"></div>
						<div class="mt-3 h-2 w-full bg-neutral-100"></div>
						<div class="mt-2 h-2 w-3/4 bg-neutral-100"></div>
					</div>

					<div class="border border-neutral-200 p-4">
						<div class="h-2 w-24 bg-neutral-300"></div>
						<div class="mt-3 h-2 w-full bg-neutral-100"></div>
						<div class="mt-2 h-2 w-2/3 bg-neutral-100"></div>
					</div>
				</div>
			</div>

			<p class="mt-4 text-center text-xs text-neutral-400">
				Findings/report screenshot placeholder
			</p>
		</div>
	</div>
</section>

<!-- CONTACT -->
<section class="bg-[#111111] px-6 py-20 sm:px-8 lg:px-12 lg:py-24">
	<div class="mx-auto grid max-w-6xl gap-12 lg:grid-cols-[0.8fr_1.2fr]">

		<div>
			<p class="text-xs font-semibold uppercase tracking-[0.2em] text-[#d4a84b]">
				NEXT STEP
			</p>

			<h2 class="mt-3 text-3xl font-semibold tracking-tight text-white sm:text-4xl">
				Ready to review a project?
			</h2>

			<p class="mt-5 max-w-md leading-7 text-neutral-400">
				Tell us a little about your project and we'll help you get started.
			</p>
		</div>

		<!-- CONTACT FORM UI ONLY -->
		<div class="bg-white p-6 sm:p-8">
			<div class="grid gap-5 sm:grid-cols-2">

				<label class="block">
					<span class="text-xs font-semibold uppercase tracking-wider text-neutral-500">
						Name
					</span>
					<input
						type="text"
						placeholder="Your name"
						class="mt-2 w-full border border-neutral-300 px-4 py-3 text-sm outline-none focus:border-black"
					/>
				</label>

				<label class="block">
					<span class="text-xs font-semibold uppercase tracking-wider text-neutral-500">
						Email
					</span>
					<input
						type="email"
						placeholder="you@company.com"
						class="mt-2 w-full border border-neutral-300 px-4 py-3 text-sm outline-none focus:border-black"
					/>
				</label>

				<label class="block sm:col-span-2">
					<span class="text-xs font-semibold uppercase tracking-wider text-neutral-500">
						Company
					</span>
					<input
						type="text"
						placeholder="Company name"
						class="mt-2 w-full border border-neutral-300 px-4 py-3 text-sm outline-none focus:border-black"
					/>
				</label>

				<label class="block sm:col-span-2">
					<span class="text-xs font-semibold uppercase tracking-wider text-neutral-500">
						Project details
					</span>
					<textarea
						rows="4"
						placeholder="Tell us about your project"
						class="mt-2 w-full resize-none border border-neutral-300 px-4 py-3 text-sm outline-none focus:border-black"
					></textarea>
				</label>

				<button
					class="bg-black px-6 py-3 text-sm font-semibold text-white transition hover:bg-neutral-800 sm:col-span-2"
				>
					Request a Review
				</button>

			</div>
		</div>
	</div>
</section>
<Footer/>
