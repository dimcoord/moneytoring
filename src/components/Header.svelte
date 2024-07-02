<script>
    import { Button, Dropdown, DropdownItem } from 'flowbite-svelte';
    import { ChevronDownOutline } from 'flowbite-svelte-icons';

    let cabang = {
        bdgKenanganIndah: "Bandung - Jl. Kenangan Indah",
        bdgCisarantenKidul: "Bandung - Jl. Cisaranten Kidul",
        jktSouthQuarter: "Jakarta - Gedung South Quarter"
    }
    let cabangDipilih = cabang.bdgKenanganIndah;
</script>

<header class="w-[99%] mx-1 h-[4.5rem] bg-white flex items-center">
    <div id="dropdown" class="text-lg ml-10">
        <span>Pilih Cabang: </span>
        <Button class="bg-merva min-w-72 py-2">{cabangDipilih}</Button>
            <!-- <div id="dropdown-content" class="absolute bg-gray-200 z-10 text-center opacity-0 transition ease-in"> -->
            <Dropdown>
                <DropdownItem class="hover:bg-gray-200" on:click={() => (cabangDipilih = cabang.bdgKenanganIndah)}>{cabang.bdgKenanganIndah}</DropdownItem>
                <DropdownItem class="hover:bg-gray-200" on:click={() => (cabangDipilih = cabang.bdgCisarantenKidul)}>{cabang.bdgCisarantenKidul}</DropdownItem>
                <DropdownItem class="hover:bg-gray-200" on:click={() => (cabangDipilih = cabang.jktSouthQuarter)}>{cabang.jktSouthQuarter}</DropdownItem>
            </Dropdown>
            <!-- </div> -->
    </div>
</header>

<!-- <style>
    #dropbtn:hover #dropdown-content {
        opacity: 1;
    }
</style> -->