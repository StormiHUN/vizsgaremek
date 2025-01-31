<script>
// @ts-nocheck

    import UserCard from "../../components/UserCard.svelte";

    const temp = [
        {
            name : "Minta Admin",
            email : "mintaadmin@logipro.hu",
            phone : "06300000000",
            status : "Active"
        },
        {
            name : "Kamion Karcsi",
            email : "kamionkarcsi@logipro.hu",
            phone : "06300000001",
            status : "Inactive"
        },
        {
            name : "Logi Lajos",
            email : "logilajos@logipro.hu",
            phone : "06300000002",
            status : "Inactive"
        },
        {
            name : "Minta Admin",
            email : "mintaadmin@logipro.hu",
            phone : "06300000000",
            status : "Active"
        },
        {
            name : "Kamion Karcsi",
            email : "kamionkarcsi@logipro.hu",
            phone : "06300000001",
            status : "Inactive"
        },
        {
            name : "Logi Lajos",
            email : "logilajos@logipro.hu",
            phone : "06300000002",
            status : "Inactive"
        },
        {
            name : "Minta Admin",
            email : "mintaadmin@logipro.hu",
            phone : "06300000000",
            status : "Active"
        },
        {
            name : "Kamion Karcsi",
            email : "kamionkarcsi@logipro.hu",
            phone : "06300000001",
            status : "Inactive"
        },
        {
            name : "Logi Lajos",
            email : "logilajos@logipro.hu",
            phone : "06300000002",
            status : "Inactive"
        },
        {
            name : "Minta Admin",
            email : "mintaadmin@logipro.hu",
            phone : "06300000000",
            status : "Active"
        },
        {
            name : "Kamion Karcsi",
            email : "kamionkarcsi@logipro.hu",
            phone : "06300000001",
            status : "Inactive"
        },
        {
            name : "Logi Lajos",
            email : "logilajos@logipro.hu",
            phone : "06300000002",
            status : "Inactive"
        }
    ]

    let sorting = "None"

    async function setSorting(param) {
        if(sorting == param) return
        sorting = param
        console.log(sorting)
    }

</script>

<main class="mx-auto my-4 flex flex-col border-2 border-zinc-200 rounded-md p-4 gap-2">
    <div class="border-2 border-zinc-200 rounded-md p-2 flex">
        <div class="flex w-1/2">
            <input class="p-2 border-2 border-r-0 border-zinc-200 rounded-l-md w-4/6 hover:bg-zinc-100 transition-all" type="text" placeholder="Search for">
            <button class="p-2 border-2 border-zinc-200 rounded-r-md hover:bg-zinc-300 hover:border-zinc-400 hover:border-l-2 hover:text-zinc-700 transition-all">Search</button>
        </div>
        <div class="flex gap-2">
            <p class="content-center">Sort to: </p>
            <input class="border-2 border-zinc-200 rounded-full p-2 focus:border-zinc-400 focus:border-2" type="button" value="Name" on:click={() => setSorting("Name")}>
            <input class="border-2 border-zinc-200 rounded-full p-2 focus:border-zinc-400 focus:border-2" type="button" value="None" on:click={() => setSorting("None")}>
            <input class="border-2 border-zinc-200 rounded-full p-2 focus:border-zinc-400 focus:border-2" type="button" value="Status" on:click={() => setSorting("Status")}>
        </div>
    </div>
    <div class=" grid grid-cols-4 gap-2 border-2 border-zinc-200 rounded-md">
        {#each temp as info}
        <UserCard userinfo={info}/>
        {/each}
    </div>
</main>
