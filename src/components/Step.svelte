<script>
    export let step;
    export let githubLink;
    export let liveLink;
</script>

<div class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-violet-700 text-center group hover:border-violet-400 duration-200">
    <div class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200">
        <i class={step.icon} />
    </div>

    <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">
        {step.name}
    </h3>

    <slot />

    <div class="project-image">
        <img src={step.imageUrl} alt={step.name} class="w-full h-auto rounded-lg" />
    </div>

    <div class="flex justify-between gap-4 mt-4">
        <a href={githubLink} target="_blank" class="button github-button">
            <i class="fa-solid fa-robot mr-2"></i>
            GitHub
        </a>
        <a href={liveLink} target="_blank" class="button live-button">
            <i class="fa-solid fa-bolt mr-2"></i>
            Live
        </a>
    </div>
</div>

<style>
    .button {
        padding: 0.5rem 1rem;
        border-radius: 0.25rem;
        transition: background-color 0.2s;
    }
    .github-button {
        background-color: #24292e;
        color: white;
    }
    .live-button {
        background-color: #0366d6;
        color: white;
    }
    .button:hover {
        opacity: 0.8;
    }
</style>