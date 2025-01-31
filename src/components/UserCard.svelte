<script>
    const {userinfo} = $props();
</script>
<div class="p-2 border-2 border-zinc-200 flex gap-2 rounded-md m-2 h-40 w-92 hover:border-zinc-400 transition-all">
    <div class="w-32 h-32 rounded-full border-2 border-zinc-200">
        
    </div>
    <div class="flex flex-col gap-2 pb-2">
        <p>{userinfo.name}</p>
        <p>{userinfo.email}</p>
        <p>{userinfo.phone}</p>
        <p class="mt-auto">Status: <span class={userinfo.status == "Active" ? "text-green-700" : "text-red-700"}>{userinfo.status}</span></p>
    </div>
</div>