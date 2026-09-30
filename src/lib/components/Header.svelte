<script lang="ts">
    import logo from '$lib/assets/logo-black-300x109-Photoroom.png';
</script>

<header class="w-full border-b border-[#d4a84b] bg-black">
    <div
        class="mx-auto flex max-w-[1280px] items-center gap-[36px] px-8 py-[18px]
               max-[1100px]:gap-[22px] max-[1100px]:px-6 max-[1100px]:py-4
               max-[800px]:px-5 max-[800px]:py-[15px]"
    >
        <!-- LOGO -->
        <a
            href="/"
            class="flex shrink-0 items-center"
            aria-label="PlanSmart home"
        >
            <img
                src={logo}
                alt="PlanSmartAI"
                class="block h-auto w-[180px]
                       max-[1100px]:w-[160px]
                       max-[800px]:w-[155px]"
            />
        </a>

        <!-- MAIN NAVIGATION -->
        <nav
            class="flex flex-1 items-center gap-[26px]
                   max-[1100px]:gap-[18px]
                   max-[800px]:hidden"
            aria-label="Main navigation"
        >
            <a
                href="#product"
                class="whitespace-nowrap text-[14px] font-medium text-white transition-colors duration-200 hover:text-[#d4a84b]
                       max-[1100px]:text-[13px]"
            >
                Product
            </a>

            <a
                href="#how-it-works"
                class="whitespace-nowrap text-[14px] font-medium text-white transition-colors duration-200 hover:text-[#d4a84b]
                       max-[1100px]:text-[13px]"
            >
                How it works
            </a>

            <a
                href="#use-cases"
                class="whitespace-nowrap text-[14px] font-medium text-white transition-colors duration-200 hover:text-[#d4a84b]
                       max-[1100px]:text-[13px]"
            >
                Use cases
            </a>

            <a
                href="#plans"
                class="whitespace-nowrap text-[14px] font-medium text-white transition-colors duration-200 hover:text-[#d4a84b]
                       max-[1100px]:text-[13px]"
            >
                Plans
            </a>

            <a
                href="#enterprise"
                class="whitespace-nowrap text-[14px] font-medium text-white transition-colors duration-200 hover:text-[#d4a84b]
                       max-[1100px]:text-[13px]"
            >
                Enterprise
            </a>
        </nav>

        <!-- RIGHT SIDE -->
        <div
            class="flex shrink-0 items-center gap-[18px]
                   max-[800px]:hidden"
        >
            <span
                class="whitespace-nowrap text-[12px] text-white
                       max-[1100px]:hidden"
            >
                Part of <strong class="font-bold text-white">2BuildAI</strong>
            </span>

            <a
                href="#login"
                class="whitespace-nowrap text-[14px] font-semibold text-white no-underline transition-colors duration-200 hover:text-[#d4a84b]"
            >
                Log in
            </a>

            <a
                href="#signup"
                class="inline-flex items-center justify-center whitespace-nowrap rounded-lg border border-[#d4a84b] bg-[#d4a84b] px-[18px] py-[10px] text-[14px] font-semibold text-white no-underline transition-colors duration-200 hover:bg-[#d4a84b] hover:text-black"
            >
                Sign up
            </a>
        </div>
    </div>
</header>

