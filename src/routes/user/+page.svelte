<script>

</script>
<main class="flex flex-col p-4 flex-1">
    <div class="border rounded-md flex p-4 gap-4 bg-gradient-to-r from-yellow-300 to-yellow-100 border-yellow-500">
        <img class="rounded-md border border-yellow-500" src="https://randomuser.me/api/portraits/men/75.jpg" alt="Profile picture">
        <div>
            <p class="text-3xl mb-2">Minta Admin</p>
            <p>Role : Administrator</p>
            <p>Contacts : mintaadmin@logipro.hu (+36300000000)</p>
            <p class="mt-2">Status : <span class="text-green-500 font-bold">Active</span></p>
        </div>
    </div>
    <div class="flex border-2 border-zinc-300 rounded p-2 mt-2 gap-2">
        <div class="flex flex-col gap-2">
            <p>Contacts:</p>
            <div class="flex gap-1 justify-between">
                <p>Email:</p>
                <input type="email" placeholder="Email" class="border border-zinc-300 rounded p-2 w-96 ml-16" value="mindtaadmin@logipro.hu">
            </div>
            <div class="flex gap-1 justify-between">
                <p class="mr-1">Phone Number:</p>
                <input type="text" placeholder="Phone Number" class="border border-zinc-300 rounded p-2 w-96" value="+36300000000">
            </div>
        </div>
        <div class="flex flex-col gap-2 ml-auto mr-auto">
            <p>Personal information:</p>
            <div class="flex gap-1 justify-between">
                <p>Name:</p>
                <input type="text" placeholder="Name" class="border border-zinc-300 rounded p-2 w-96" value="Minta Admin">
            </div>
            <div class="flex gap-1 justify-between">
                <p>Address:</p>
                <input type="text" class="border border-zinc-300 rounded p-2 w-96" placeholder="Address" value="0000, Talfajakoz, Margit utca 2">
            </div>
        </div>
    </div>
</main>