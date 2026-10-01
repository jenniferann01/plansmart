<script lang="ts">
	import Header from '$lib/components/Header.svelte';
	import Footer from '$lib/components/Footer.svelte';

	const steps = [
		{
			number: '01',
			title: 'Upload your plans',
			text: 'Start with the complete PDF plan set for your project.'
		},
		{
			number: '02',
			title: 'PlanSmart reviews the set',
			text: 'The review checks the submitted drawings for items that may need attention before submission.'
		},
		{
			number: '03',
			title: 'Review what was found',
			text: 'Findings are organized by sheet so your team can see where each item belongs.'
		},
		{
			number: '04',
			title: 'Get your review report',
			text: 'Use the report to work through findings before the plans reach the permit desk.'
		}
	];
</script>

<svelte:head>
	<title>How It Works | PlanSmartAI</title>
	<meta
		name="description"
		content="See how PlanSmartAI takes a project plan set from upload to a clear review report before submission."
	/>
</svelte:head>

<Header />

<!-- HERO -->
<section class="bg-white px-6 pb-20 pt-20 sm:px-8 lg:px-12 lg:pb-28 lg:pt-28">
	<div class="mx-auto max-w-7xl">
		<div class="max-w-4xl">
			<p class="mb-5 text-xs font-semibold uppercase tracking-[0.22em] text-[#a07a32]">
				HOW PLANSMART WORKS
			</p>

			<h1
				class="max-w-4xl text-5xl font-medium leading-[1.02] tracking-[-0.045em] text-black sm:text-6xl lg:text-7xl"
			>
				From plan set to
				<span class="text-neutral-400">review-ready.</span>
			</h1>

			<p class="mt-7 max-w-2xl text-lg leading-8 text-neutral-600 sm:text-xl">
				PlanSmart reviews your project drawings, organizes what needs attention, and gives
				your team a clear report before submission.
			</p>
		</div>

		<div class="mt-12 flex flex-wrap items-center gap-x-8 gap-y-3 border-t border-neutral-200 pt-6">
			<span class="text-sm font-medium text-black">Upload</span>
			<span class="text-neutral-300">→</span>
			<span class="text-sm text-neutral-500">Review</span>
			<span class="text-neutral-300">→</span>
			<span class="text-sm text-neutral-500">Find</span>
			<span class="text-neutral-300">→</span>
			<span class="text-sm text-neutral-500">Resolve</span>
		</div>
	</div>
</section>

<!-- VIDEO / DEMO -->
<section class="bg-[#111111] px-6 py-20 sm:px-8 lg:px-12 lg:py-28">
	<div class="mx-auto max-w-7xl">
		<div class="grid gap-12 lg:grid-cols-[0.65fr_1.35fr] lg:items-end">
			<div>
				<p class="text-xs font-semibold uppercase tracking-[0.22em] text-[#d4a84b]">
					SEE IT IN ACTION
				</p>

				<h2
					class="mt-4 text-4xl font-medium leading-tight tracking-[-0.035em] text-white sm:text-5xl"
				>
					See the review happen.
				</h2>

				<p class="mt-5 max-w-md text-base leading-7 text-neutral-400">
					Follow a project from the original drawing set through the PlanSmart review process.
				</p>
			</div>

			<div
				class="relative aspect-video overflow-hidden border border-white/10 bg-[#191919]"
			>
				<!-- VIDEO PLACEHOLDER -->
				<div class="absolute inset-0">
					<div
						class="absolute left-[10%] top-[14%] h-px w-[80%] bg-white/10"
					></div>

					<div
						class="absolute left-[10%] top-[28%] h-px w-[65%] bg-white/10"
					></div>

					<div
						class="absolute bottom-[25%] left-[10%] h-px w-[72%] bg-white/10"
					></div>

					<div
						class="absolute right-[14%] top-[18%] h-[55%] w-px bg-white/10"
					></div>
				</div>

				<div class="absolute inset-0 flex items-center justify-center">
					<div
						class="flex h-20 w-20 items-center justify-center rounded-full bg-[#d4a84b] text-black transition hover:scale-105"
					>
						<svg viewBox="0 0 24 24" class="ml-1 h-7 w-7 fill-current">
							<path d="M8 5v14l11-7z" />
						</svg>
					</div>
				</div>

				<div class="absolute bottom-5 left-5">
					<p class="text-xs font-medium uppercase tracking-[0.18em] text-white/60">
						PLANSMARTAI DEMO
					</p>
				</div>

				<div class="absolute bottom-5 right-5">
					<p class="text-xs text-white/40">
						Video placeholder
					</p>
				</div>
			</div>
		</div>
	</div>
</section>

<!-- PROCESS -->
<section class="bg-white px-6 py-20 sm:px-8 lg:px-12 lg:py-28">
	<div class="mx-auto max-w-7xl">
		<div class="grid gap-10 lg:grid-cols-[0.55fr_1.45fr]">
			<div>
				<p class="text-xs font-semibold uppercase tracking-[0.22em] text-[#a07a32]">
					THE WORKFLOW
				</p>

				<h2
					class="mt-4 max-w-md text-4xl font-medium leading-tight tracking-[-0.035em] text-black sm:text-5xl"
				>
					Four steps between your drawings and your review.
				</h2>
			</div>

			<div class="border-t border-neutral-200">
				{#each steps as step}
					<div
						class="grid gap-5 border-b border-neutral-200 py-8 sm:grid-cols-[80px_1fr] sm:gap-8"
					>
						<div class="text-sm font-semibold tracking-[0.12em] text-[#a07a32]">
							{step.number}
						</div>

						<div class="max-w-2xl">
							<h3 class="text-2xl font-medium tracking-tight text-black">
								{step.title}
							</h3>

							<p class="mt-3 max-w-xl text-base leading-7 text-neutral-600">
								{step.text}
							</p>
						</div>
					</div>
				{/each}
			</div>
		</div>
	</div>
</section>

<!-- REAL PROJECT -->
<section class="bg-[#f4f2ed] px-6 py-20 sm:px-8 lg:px-12 lg:py-28">
	<div class="mx-auto max-w-7xl">
		<div class="max-w-3xl">
			<p class="text-xs font-semibold uppercase tracking-[0.22em] text-[#a07a32]">
				FROM DRAWINGS TO FINDINGS
			</p>

			<h2
				class="mt-4 text-4xl font-medium leading-tight tracking-[-0.035em] text-black sm:text-5xl"
			>
				Don't just explain the workflow.
				<span class="text-neutral-500">Show the work.</span>
			</h2>

			<p class="mt-5 max-w-2xl text-base leading-7 text-neutral-600">
				Use a real project plan set to show what PlanSmart starts with — and what the review
				produces.
			</p>
		</div>

		<div class="mt-14 grid gap-6 lg:grid-cols-2">
			<!-- INPUT -->
			<div>
				<div class="mb-4 flex items-end justify-between">
					<div>
						<p class="text-xs font-semibold uppercase tracking-[0.18em] text-neutral-500">
							01 / INPUT
						</p>

						<h3 class="mt-2 text-2xl font-medium tracking-tight text-black">
							The plan set
						</h3>
					</div>

					<span class="text-xs text-neutral-500">PDF</span>
				</div>

				<div
					class="group relative aspect-[4/3] overflow-hidden border border-neutral-300 bg-white p-6"
				>
					<div class="absolute inset-6 border border-neutral-200 bg-[#fafafa]">
						<div class="absolute inset-6 border border-neutral-300 bg-white shadow-sm">
							<div class="border-b border-neutral-200 px-5 py-4">
								<div class="flex items-center justify-between">
									<div>
										<div class="h-2 w-32 bg-neutral-800"></div>
										<div class="mt-2 h-1.5 w-20 bg-neutral-300"></div>
									</div>

									<div class="text-[9px] uppercase tracking-wider text-neutral-400">
										A-1
									</div>
								</div>
							</div>

							<div class="p-5">
								<div class="grid grid-cols-3 gap-3">
									<div class="col-span-2 h-28 border border-neutral-300">
										<div class="m-4 h-px bg-neutral-300"></div>
										<div class="mx-4 mt-8 h-px bg-neutral-200"></div>
										<div class="mx-4 mt-8 h-px bg-neutral-200"></div>
									</div>

									<div class="space-y-3">
										<div class="h-8 border border-neutral-200"></div>
										<div class="h-8 border border-neutral-200"></div>
										<div class="h-8 border border-neutral-200"></div>
									</div>
								</div>
							</div>
						</div>
					</div>

					<div class="absolute bottom-8 left-8">
						<p class="text-xs font-medium uppercase tracking-[0.16em] text-neutral-500">
							Moana East Building
						</p>

						<p class="mt-1 text-sm font-medium text-black">
							24 × 36 · Full Permit Plan Set
						</p>
					</div>
				</div>
			</div>

			<!-- OUTPUT -->
			<div>
				<div class="mb-4 flex items-end justify-between">
					<div>
						<p class="text-xs font-semibold uppercase tracking-[0.18em] text-neutral-500">
							02 / OUTPUT
						</p>

						<h3 class="mt-2 text-2xl font-medium tracking-tight text-black">
							The review report
						</h3>
					</div>

					<span class="text-xs text-neutral-500">PDF</span>
				</div>

				<div
					class="relative aspect-[4/3] overflow-hidden border border-neutral-300 bg-white p-6"
				>
					<div
						class="absolute left-[12%] right-[12%] top-[8%] bottom-[-18%] border border-neutral-300 bg-white p-6 shadow-[0_12px_40px_rgba(0,0,0,0.08)]"
					>
						<div class="flex items-start justify-between border-b border-neutral-200 pb-5">
							<div>
								<p class="text-[9px] font-semibold uppercase tracking-[0.18em] text-[#a07a32]">
									PLANSMARTAI
								</p>

								<p class="mt-2 text-xl font-medium tracking-tight text-black">
									Plan Review Report
								</p>

								<p class="mt-1 text-xs text-neutral-500">
									Moana East Building 24 × 36
								</p>
							</div>

							<div class="text-right">
								<p class="text-[9px] uppercase tracking-wider text-neutral-400">
									REVIEW
								</p>

								<p class="mt-1 text-xs font-medium text-black">
									PSA SAMPLE
								</p>
							</div>
						</div>

						<div class="mt-6 grid grid-cols-3 gap-3">
							<div class="border border-neutral-200 p-3">
								<p class="text-[9px] uppercase text-neutral-400">Findings</p>
								<p class="mt-2 text-lg font-medium text-black">—</p>
							</div>

							<div class="border border-neutral-200 p-3">
								<p class="text-[9px] uppercase text-neutral-400">Sheets</p>
								<p class="mt-2 text-lg font-medium text-black">—</p>
							</div>

							<div class="border border-neutral-200 p-3">
								<p class="text-[9px] uppercase text-neutral-400">Status</p>
								<p class="mt-2 text-lg font-medium text-[#a07a32]">Review</p>
							</div>
						</div>

						<div class="mt-6 space-y-3">
							<div class="border border-neutral-200 p-4">
								<div class="flex justify-between">
									<div class="h-2 w-32 bg-neutral-300"></div>
									<div class="h-2 w-12 bg-[#d4a84b]"></div>
								</div>

								<div class="mt-3 h-1.5 w-full bg-neutral-100"></div>
								<div class="mt-2 h-1.5 w-4/5 bg-neutral-100"></div>
							</div>

							<div class="border border-neutral-200 p-4">
								<div class="h-2 w-40 bg-neutral-300"></div>

								<div class="mt-3 h-1.5 w-full bg-neutral-100"></div>
								<div class="mt-2 h-1.5 w-3/4 bg-neutral-100"></div>
							</div>
						</div>
					</div>

					<p class="absolute bottom-5 left-0 right-0 text-center text-xs text-neutral-400">
						Sample report preview
					</p>
				</div>

				<div class="mt-5">
					<button
						type="button"
						class="inline-flex items-center gap-3 bg-black px-6 py-3 text-sm font-semibold text-white transition hover:bg-[#d4a84b] hover:text-black"
					>
						Download sample report

						<svg viewBox="0 0 20 20" class="h-4 w-4 fill-current">
							<path d="M10 2v10.17l3.59-3.58L15 10l-5 5-5-5 1.41-1.41L9 12.17V2h1zM3 17h14v2H3v-2z" />
						</svg>
					</button>
				</div>
			</div>
		</div>
	</div>
</section>

<!-- FINDINGS -->
<section class="bg-white px-6 py-20 sm:px-8 lg:px-12 lg:py-28">
	<div class="mx-auto max-w-7xl">
		<div class="grid gap-14 lg:grid-cols-[0.7fr_1.3fr] lg:items-center">
			<div>
				<p class="text-xs font-semibold uppercase tracking-[0.22em] text-[#a07a32]">
					WHAT YOU SEE
				</p>

				<h2
					class="mt-4 text-4xl font-medium leading-tight tracking-[-0.035em] text-black sm:text-5xl"
				>
					Every finding has a place.
				</h2>

				<p class="mt-5 max-w-md text-base leading-7 text-neutral-600">
					Instead of a long list with no context, findings are connected back to the project
					and the sheet where they were identified.
				</p>
			</div>

			<!-- FINDINGS UI -->
			<div class="border border-neutral-200 bg-[#f7f7f5] p-4 sm:p-6">
				<div class="border border-neutral-200 bg-white">
					<div class="flex items-center justify-between border-b border-neutral-200 px-5 py-4">
						<div>
							<p class="text-[9px] font-semibold uppercase tracking-[0.18em] text-[#a07a32]">
								PLANSMARTAI
							</p>

							<p class="mt-1 text-sm font-medium text-black">
								Review Findings
							</p>
						</div>

						<span class="text-xs text-neutral-400">
							Sample
						</span>
					</div>

					<div class="divide-y divide-neutral-200">
						<div class="grid gap-4 p-5 sm:grid-cols-[70px_1fr_auto] sm:items-start">
							<span class="text-xs font-semibold text-neutral-400">A-1</span>

							<div>
								<p class="text-sm font-medium text-black">
									Documentation review item
								</p>

								<p class="mt-1 text-xs leading-5 text-neutral-500">
									Review the identified item before submission.
								</p>
							</div>

							<span class="text-[10px] font-semibold uppercase tracking-wider text-[#a07a32]">
								Review
							</span>
						</div>

						<div class="grid gap-4 p-5 sm:grid-cols-[70px_1fr_auto] sm:items-start">
							<span class="text-xs font-semibold text-neutral-400">A-2</span>

							<div>
								<p class="text-sm font-medium text-black">
									Sheet coordination item
								</p>

								<p class="mt-1 text-xs leading-5 text-neutral-500">
									See the associated sheet and finding details.
								</p>
							</div>

							<span class="text-[10px] font-semibold uppercase tracking-wider text-[#a07a32]">
								Review
							</span>
						</div>

						<div class="grid gap-4 p-5 sm:grid-cols-[70px_1fr_auto] sm:items-start">
							<span class="text-xs font-semibold text-neutral-400">M-1</span>

							<div>
								<p class="text-sm font-medium text-black">
									Plan review item
								</p>

								<p class="mt-1 text-xs leading-5 text-neutral-500">
									Additional context is provided within the report.
								</p>
							</div>

							<span class="text-[10px] font-semibold uppercase tracking-wider text-[#a07a32]">
								Review
							</span>
						</div>
					</div>
				</div>

				<p class="mt-4 text-center text-xs text-neutral-400">
					Findings interface placeholder
				</p>
			</div>
		</div>
	</div>
</section>

<!-- CTA -->
<section class="bg-[#111111] px-6 py-20 sm:px-8 lg:px-12 lg:py-28">
	<div class="mx-auto max-w-7xl">
		<div class="grid gap-10 lg:grid-cols-[1fr_auto] lg:items-end">
			<div>
				<p class="text-xs font-semibold uppercase tracking-[0.22em] text-[#d4a84b]">
					READY WHEN YOU ARE
				</p>

				<h2
					class="mt-4 max-w-3xl text-4xl font-medium leading-tight tracking-[-0.035em] text-white sm:text-5xl lg:text-6xl"
				>
					Know what needs attention
					<span class="text-neutral-500">before you submit.</span>
				</h2>

				<p class="mt-6 max-w-xl text-base leading-7 text-neutral-400">
					Start with your project plans and see what PlanSmart can find.
				</p>
			</div>

			<div class="lg:pb-1">
				<button
					type="button"
					class="inline-flex items-center justify-center bg-[#d4a84b] px-7 py-4 text-sm font-semibold text-black transition hover:bg-white"
				>
					Start a free review
				</button>

				<p class="mt-3 text-center text-xs text-neutral-500">
					No card required to start
				</p>
			</div>
		</div>
	</div>
</section>

<Footer />