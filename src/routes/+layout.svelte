<script>
    import "../app.css";
    import AccountCogOutline from "svelte-material-icons/AccountCogOutline.svelte"
    import AccountGroupOutline from "svelte-material-icons/AccountGroupOutline.svelte"
    import DatabaseOutline from "svelte-material-icons/DatabaseOutline.svelte"
    import Truck from "svelte-material-icons/TruckOutline.svelte"
    import House from "svelte-material-icons/HomeOutline.svelte"
    import NavDropdown from "../components/NavDropdown.svelte";
    import NavLink from "../components/NavLink.svelte";
</script>

<div class="flex min-h-screen">
    <nav class="pr-4 m-4 border-r-2 min-w-64 flex flex-col gap-2 sticky top-0">
        <h1 class="text-3xl font-semibold mb-6">LogiPRO</h1>
        <div class="flex flex-col gap-2">
            <a href="/" class="text-2xl flex items-center gap-2 border border-white hover:bg-zinc-100 hover:border-zinc-200 transition-all rounded-md p-2"><House/>Home</a>
            <NavDropdown label="Users"> 
                <NavLink href="/users">
                    See users
                </NavLink>
                <NavLink href="/newuser">
                    New user
                </NavLink>
            </NavDropdown>
            <NavDropdown label="Shipments"> 
                <NavLink href="#">
                    See Shipments
                </NavLink>
                <NavLink href="#">
                    Shipments history
                </NavLink>
            </NavDropdown>
            <NavDropdown label="Database"> 
                <NavLink href="#">
                    Query
                </NavLink>
                <NavLink href="#">
                    Recent queries
                </NavLink>
                <NavLink href="#">
                    See raw data
                </NavLink>
            </NavDropdown>

        </div>
        <div
            class="mt-auto flex gap-2 border p-2 rounded-3xl items-center hover:border-zinc-400 transition-all"
        >
            <div class="rounded-full p-2 bg-zinc-200">MA</div>
            <div>
                <p>Minta Admin</p>
                <p class="text-sm text-zinc-400">Admin</p>
            </div>
            <a class="ml-auto" href="/user">
                <AccountCogOutline class="size-8"/>
            </a>
        </div>
    </nav>
    <slot />
</div>
