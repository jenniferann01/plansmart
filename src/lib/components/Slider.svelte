<script lang="ts">
	const officeScreens = [
		{
			title: 'Your review at a glance',
			description:
				'See the overall review status, findings and sheets that need attention from one place.'
		},
		{
			title: 'Every finding tied to a sheet',
			description:
				'Each finding connects back to the drawing sheet and explains exactly what needs attention.'
		},
		{
			title: 'See what was found',
			description:
				'Critical findings, warnings and informational items are organized so your team can focus on what matters.'
		},
		{
			title: 'Review the drawing context',
			description:
				'Open the relevant sheet and see the context behind each finding before making a correction.'
		},
		{
			title: 'Submission-ready output',
			description:
				'Bring resolved findings together into a clear review package before the plans go to the permit desk.'
		}
	];

	let currentScreen = $state(0);

	function previousScreen() {
		if (currentScreen > 0) {
			currentScreen -= 1;
		}
	}

	function nextScreen() {
		if (currentScreen < officeScreens.length - 1) {
			currentScreen += 1;
		}
	}

</script>

<section id="office-side" class="bg-[#111111] text-white">
	<div class="mx-auto max-w-7xl px-6 py-20 sm:px-8 lg:px-10 lg:py-28">

		<!-- Section heading -->
		<div class="flex flex-col gap-8 md:flex-row md:items-end md:justify-between">
			<div class="max-w-3xl">
				<p
					class="font-mono text-xs font-semibold uppercase tracking-[0.18em] text-[#d4a84b]"
				>
					AND THE OFFICE SIDE
				</p>

				<h2
					class="mt-4 max-w-2xl text-3xl font-extrabold leading-tight tracking-tight sm:text-4xl lg:text-5xl"
				>
					See PlanSmart in action.
				</h2>

				<p class="mt-5 max-w-2xl text-base leading-7 text-white/65 sm:text-lg">
					A closer look at the application your team uses after the drawings are uploaded.
				</p>
			</div>

			<!-- Navigation -->
			<div class="flex items-center gap-4">
				<button
					type="button"
					onclick={previousScreen}
					disabled={currentScreen === 0}
					aria-label="Previous screen"
					class="flex h-11 w-11 items-center justify-center rounded-full border border-white/20 text-white transition hover:border-[#d4a84b] hover:text-[#d4a84b] disabled:cursor-not-allowed disabled:opacity-30 disabled:hover:border-white/20 disabled:hover:text-white"
				>
					<svg
						width="20"
						height="20"
						viewBox="0 0 24 24"
						fill="none"
						stroke="currentColor"
						stroke-width="2.4"
						stroke-linecap="round"
						stroke-linejoin="round"
					>
						<path d="m15 18-6-6 6-6" />
					</svg>
				</button>

				<span class="min-w-[58px] text-center font-mono text-sm text-white/60">
					<span class="font-bold text-white">{currentScreen + 1}</span>
					/
					{officeScreens.length}
				</span>

				<button
					type="button"
					onclick={nextScreen}
					disabled={currentScreen === officeScreens.length - 1}
					aria-label="Next screen"
					class="flex h-11 w-11 items-center justify-center rounded-full border border-white/20 text-white transition hover:border-[#d4a84b] hover:text-[#d4a84b] disabled:cursor-not-allowed disabled:opacity-30 disabled:hover:border-white/20 disabled:hover:text-white"
				>
					<svg
						width="20"
						height="20"
						viewBox="0 0 24 24"
						fill="none"
						stroke="currentColor"
						stroke-width="2.4"
						stroke-linecap="round"
						stroke-linejoin="round"
					>
						<path d="m9 18 6-6-6-6" />
					</svg>
				</button>
			</div>
		</div>

		<!-- Screenshot placeholder -->
		<div
			class="mt-12 overflow-hidden rounded-2xl border border-white/10 bg-[#181818] shadow-2xl"
		>
			<div class="aspect-[16/8] min-h-[260px] bg-[#202020] p-3 sm:p-5 lg:p-7">
				<!-- Browser / application frame -->
				<div
					class="h-full overflow-hidden rounded-lg border border-white/10 bg-[#f5f5f3] text-[#111111] shadow-xl"
				>
					<!-- Fake browser bar -->
					<div class="flex h-9 items-center gap-2 border-b border-black/10 bg-white px-4">
						<div class="h-2.5 w-2.5 rounded-full bg-black/15"></div>
						<div class="h-2.5 w-2.5 rounded-full bg-black/15"></div>
						<div class="h-2.5 w-2.5 rounded-full bg-black/15"></div>

						<div
							class="ml-4 h-5 max-w-md flex-1 rounded bg-black/[0.04]"
						></div>
					</div>

					<!-- Fake PlanSmart application -->
					<div class="flex h-[calc(100%-2.25rem)]">

						<!-- Sidebar -->
						<aside class="hidden w-44 border-r border-black/10 bg-[#151515] p-4 text-white sm:block">
							<div class="font-bold tracking-tight">
								PlanSmart<span class="text-[#d4a84b]">AI</span>
							</div>

							<div class="mt-8 space-y-2">
								<div class="rounded bg-white/10 px-3 py-2 text-xs">
									Dashboard
								</div>
								<div class="px-3 py-2 text-xs text-white/45">
									Projects
								</div>
								<div class="px-3 py-2 text-xs text-white/45">
									Reviews
								</div>
								<div class="px-3 py-2 text-xs text-white/45">
									Reports
								</div>
							</div>
						</aside>

						<!-- Main application placeholder -->
						<div class="flex-1 overflow-hidden p-4 sm:p-6 lg:p-8">

							<div class="flex items-start justify-between gap-4">
								<div>
									<div class="h-3 w-20 rounded bg-black/10"></div>
									<div class="mt-2 h-6 w-48 rounded bg-black/15"></div>
								</div>

								<div class="rounded-full bg-[#d4a84b]/15 px-3 py-1.5 text-[10px] font-semibold text-[#80631e]">
									REVIEW IN PROGRESS
								</div>
							</div>

							<!-- Fake stats -->
							<div class="mt-6 grid grid-cols-2 gap-3 sm:grid-cols-4">
								<div class="rounded border border-black/10 bg-white p-3">
									<div class="h-2 w-14 rounded bg-black/10"></div>
									<div class="mt-2 h-5 w-8 rounded bg-black/15"></div>
								</div>

								<div class="rounded border border-black/10 bg-white p-3">
									<div class="h-2 w-14 rounded bg-black/10"></div>
									<div class="mt-2 h-5 w-8 rounded bg-black/15"></div>
								</div>

								<div class="rounded border border-black/10 bg-white p-3">
									<div class="h-2 w-14 rounded bg-black/10"></div>
									<div class="mt-2 h-5 w-8 rounded bg-black/15"></div>
								</div>

								<div class="rounded border border-black/10 bg-white p-3">
									<div class="h-2 w-14 rounded bg-black/10"></div>
									<div class="mt-2 h-5 w-8 rounded bg-black/15"></div>
								</div>
							</div>

							<!-- Fake findings -->
							<div class="mt-5 rounded border border-black/10 bg-white">
								<div class="border-b border-black/10 px-4 py-3">
									<div class="h-3 w-28 rounded bg-black/10"></div>
								</div>

								<div class="divide-y divide-black/5">
									<div class="flex items-center gap-3 px-4 py-3">
										<div class="h-2.5 w-2.5 rounded-full bg-red-400"></div>
										<div class="h-2.5 flex-1 rounded bg-black/10"></div>
										<div class="hidden h-2.5 w-20 rounded bg-black/10 sm:block"></div>
									</div>

									<div class="flex items-center gap-3 px-4 py-3">
										<div class="h-2.5 w-2.5 rounded-full bg-amber-400"></div>
										<div class="h-2.5 flex-1 rounded bg-black/10"></div>
										<div class="hidden h-2.5 w-20 rounded bg-black/10 sm:block"></div>
									</div>

									<div class="flex items-center gap-3 px-4 py-3">
										<div class="h-2.5 w-2.5 rounded-full bg-amber-400"></div>
										<div class="h-2.5 flex-1 rounded bg-black/10"></div>
										<div class="hidden h-2.5 w-20 rounded bg-black/10 sm:block"></div>
									</div>

									<div class="flex items-center gap-3 px-4 py-3">
										<div class="h-2.5 w-2.5 rounded-full bg-green-500"></div>
										<div class="h-2.5 flex-1 rounded bg-black/10"></div>
										<div class="hidden h-2.5 w-20 rounded bg-black/10 sm:block"></div>
									</div>
								</div>
							</div>

						</div>
					</div>
				</div>
			</div>

			<!-- Caption -->
			<div class="border-t border-white/10 px-6 py-6 sm:px-8">
				<div class="max-w-3xl">
					<h3 class="text-xl font-bold tracking-tight sm:text-2xl">
						{officeScreens[currentScreen].title}
					</h3>

					<p class="mt-2 text-sm leading-6 text-white/60 sm:text-base">
						{officeScreens[currentScreen].description}
					</p>
				</div>
			</div>
		</div>

		<!-- Placeholder notice -->
		<p class="mt-4 text-xs text-white/30">
			Placeholder interface — replace with actual PlanSmart application screenshots when available.
		</p>
	</div>
</section>