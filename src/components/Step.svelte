<script>
    export let step;
</script>

<a
    href={step.href}
    target="_blank"
    class="p-4 sm:p-6 md:p-8 flex flex-col justify-between gap-4 rounded-lg border border-solid border-violet-700 text-center group cursor-pointer hover:border-violet-400 duration-200 h-full"
>
    <div
        class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200"
    >
        {#if step.type === "fa"}
            <i class={step.icon + " text-4xl sm:text-5xl md:text-6xl mb-5"}/>
        {:else}
            <img
                src={step.icon}
                alt={step.name}
                class="object-contain w-14 h-14 sm:w-16 sm:h-16 md:w-20 md:h-20 -translate-y-2"
                onerror="this.style.display='none'"
            />
        {/if}
    </div>
    <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">{step.name}</h3>
    <slot />

    
    <div class="flex flex-1 gap-4 items-end">
        <div
            class="ml-auto cursor-pointer hover:text-slate-950 duration-200 rounded-sm relative after:absolute after:top-0 after:h-0 after:right-full after:w-full after:h-full after:bg-white after:duration-200 hover:after:translate-x-full after:z-[1] overflow-hidden"
        >
            <p class="relative z-[4]">Go to &rarr;</p>
        </div>
    </div>
</a>
