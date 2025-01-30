<script>

</script>
<main class="flex min-h-screen max-h-screen flex-1">   
    <!--Information window-->
    <div class="flex flex-col lg:grid lg:grid-cols-2 lg:grid-rows-2 p-4 gap-4 flex-1">

        <!--Shipments information-->
        <div class="border-2 rounded-lg p-4 flex flex-col gap-4">
            <h2 class="text-4xl font-semibold">423 Shipments</h2>
            
            <div class="flex gap-4">
                <h3 class="flex-1 text-center">
                    <span class="text-3xl block">107</span> Active
                </h3>
                <div class="max-w-1 flex-1 bg-zinc-200"></div>
                <h3 class="flex-1 text-center">
                    <span class="text-3xl block">177</span> Pending
                </h3>
                <div class="max-w-1 flex-1 bg-zinc-200"></div>
                <h3 class="flex-1 text-center">
                    <span class="text-3xl block">139</span> Completed
                </h3>
            </div>
            
            <div class="overflow-y-scroll flex flex-1 border-2 rounded-lg relative">
                <table class="flex-1">
                    <thead class="top-0 sticky bg-zinc-300 text-left">
                        <tr>
                            <th>Route ID</th>
                            <th>License plate</th>
                            <th>Content</th>
                            <th>Start time</th>
                            <th>From ➡ To</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>001</td>
                            <td>ABC123</td>
                            <td>General Cargo</td>
                            <td>08:00 AM</td>
                            <td>New York ➡ Boston</td>
                        </tr>
                        <tr>
                            <td>002</td>
                            <td>XYZ789</td>
                            <td>Electronics</td>
                            <td>09:00 AM</td>
                            <td>San Francisco ➡ Los Angeles</td>
                        </tr>
                        <tr>
                            <td>003</td>
                            <td>DEF456</td>
                            <td>Furniture</td>
                            <td>10:00 AM</td>
                            <td>Miami ➡ Orlando</td>
                        </tr>
                        <tr>
                            <td>004</td>
                            <td>GHI012</td>
                            <td>Textiles</td>
                            <td>11:00 AM</td>
                            <td>Chicago ➡ Detroit</td>
                        </tr>
                        <tr>
                        <td>005</td>
                        <td>JKL345</td>
                        <td>Food</td>
                        <td>12:00 PM</td>
                        <td>Houston ➡ Dallas</td>
                    </tr>
                    <tr>
                        <td>006</td>
                        <td>MNO678</td>
                        <td>Machinery</td>
                        <td>01:00 PM</td>
                        <td>Seattle ➡ Portland</td>
                    </tr>
                    <tr>
                        <td>007</td>
                        <td>PQR901</td>
                        <td>Automobile Parts</td>
                        <td>02:00 PM</td>
                        <td>Philadelphia ➡ Pittsburgh</td>
                    </tr>
                    <tr>
                        <td>008</td>
                        <td>STU234</td>
                        <td>Books</td>
                        <td>03:00 PM</td>
                        <td>Phoenix ➡ Tucson</td>
                    </tr>
                    <tr>
                        <td>009</td>
                        <td>VWX567</td>
                        <td>Medicines</td>
                        <td>04:00 PM</td>
                        <td>Austin ➡ San Antonio</td>
                    </tr>
                    <tr>
                        <td>010</td>
                        <td>YZA890</td>
                        <td>Electronics</td>
                        <td>05:00 PM</td>
                        <td>Nashville ➡ Memphis</td>
                    </tr>
                    <tr>
                        <td>011</td>
                        <td>BCD123</td>
                        <td>Clothing</td>
                        <td>06:00 PM</td>
                        <td>Charlotte ➡ Raleigh</td>
                    </tr>
                    <tr>
                        <td>012</td>
                        <td>EFG456</td>
                        <td>Tools</td>
                        <td>07:00 PM</td>
                        <td>Kansas City ➡ St. Louis</td>
                    </tr>
                    <tr>
                        <td>013</td>
                        <td>HIJ789</td>
                        <td>Jewelry</td>
                        <td>08:00 PM</td>
                        <td>Denver ➡ Colorado Springs</td>
                    </tr>
                    <tr>
                        <td>014</td>
                        <td>KLM012</td>
                        <td>Office Supplies</td>
                        <td>09:00 PM</td>
                        <td>Atlanta ➡ Savannah</td>
                    </tr>
                    <tr>
                        <td>015</td>
                        <td>NOP345</td>
                        <td>Home Appliances</td>
                        <td>10:00 PM</td>
                        <td>Las Vegas ➡ Reno</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
    <!--Notifications-->
    <div class="border-2 row-span-2 rounded-lg p-4 flex flex-col">
        <h2 class="text-4xl font-semibold">Notifications</h2>
        <div class="flex-1 overflow-y-auto mt-4">
            {#each new Array(5) as i}
            <div class="flex p-2 gap-2 items-center bg-yellow-100 border border-yellow-200 rounded mb-2 mr-2 hover:bg-yellow-200 hover:border-yellow-300 transition-all">
                <div class="rounded-full bg-zinc-100 p-4 border-zinc-300 border">MT</div>
                <div class="flex-1">
                    <h3 class="font-semibold">@MinTamás</h3>
                    <p>Requested new password</p>
                </div>
                <div>2024.12.01</div>
            </div>
            <div class="flex p-2 gap-2 items-center bg-green-100 border border-green-200 rounded mb-2 mr-2 hover:bg-green-200 hover:border-green-300 transition-all">
                <div class="rounded-full bg-zinc-100 p-4 border-zinc-300 border">‎ LL ‎ </div>
                <div class="flex-1">
                    <h3 class="font-semibold">@LogiLajos</h3>
                    <p>Created new job</p>
                </div>
                <div>2024.12.01</div>
            </div>
            <div class="flex p-2 gap-2 items-center bg-red-100 border border-red-200 rounded mb-2 mr-2 hover:bg-red-200 hover:border-red-300 transition-all">
                <div class="rounded-full bg-zinc-100 p-4 border-zinc-300 border">‎ KK </div>
                <div class="flex-1">
                    <h3 class="font-semibold">@KamionKarcsi</h3>
                    <p>Experienced vehicle malfunction</p>
                </div>
                <div>2024.12.01</div>
            </div>
            {/each}
        </div>
    </div>
    
    <!--Audit log-->
    <div class="flex flex-col border-2 rounded-lg p-4">
        <div class="flex justify-between">
            <h2 class="text-4xl font-semibold">Audit log</h2>
            <button
            class="p-2 bg-zinc-100 rounded-lg hover:bg-zinc-300 transition-all"
            >Clear</button
            >
        </div>
        <div class="flex-1 overflow-y-auto mt-4">
            {#each new Array(10) as i}
            <div class="flex p-2 gap-2 items-center hover:bg-zinc-200 transition-all rounded-md mr-2">
                <div class="rounded-full bg-zinc-100 p-4">MT</div>
                <div class="flex-1">
                    <h3 class="font-semibold">@MinTamás</h3>
                    <p>Started shipment 013</p>
                </div>
                <div>2024.11.21</div>
            </div>
            {/each}
        </div>
    </div>
</div>
</main>
