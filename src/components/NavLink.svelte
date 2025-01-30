<script>
    const {href, children} = $props();
</script>
<div class="p-2 hover:bg-zinc-50 rounded-r-lg border-l border-l-zinc-200 transition-all">
    <a {href}>{@render children()}</a>
</div>