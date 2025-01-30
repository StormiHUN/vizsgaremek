<script>
    import ArrowRight from "svelte-material-icons/ArrowRight.svelte"
    const { label, children } = $props();
</script>

<details class="flex flex-col transition-all group">
    <summary
        class="appearance-none text-xl list-none flex items-center gap-1 hover:bg-zinc-50 p-2 rounded-md transition-all hover:border group-open:border-l group-open:rounded-l-none group-open:border group-open:bg-zinc-300"
    >
    <!-- {@html icon} -->
    {label}
    <ArrowRight class="transition-all ml-auto group-open:rotate-90"/>
    </summary>
    {@render children()}
</details>
