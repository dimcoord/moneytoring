<script>
    import { Button, Modal } from 'flowbite-svelte';
    let defaultModal = false;
    import { cabang } from  "../data"
    
    let cabangDipilih = cabang.bdgKenanganIndah;
</script>

<header class="w-[99%] mx-1 h-[4.5rem] bg-white flex items-center">
    <div id="dropdown-container" class="text-lg ml-10">
        <span>Pilih Cabang: </span>
        <button on:click={() => (defaultModal = true)}
        class="text-black bg-merva-100 hover:bg-merva-200 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center inline-flex items-center" type="button">
            {cabangDipilih} 
            <svg class="w-2.5 h-2.5 ms-3" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 10 6">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m1 1 4 4 4-4"/>
            </svg>
        </button>
                
        <Modal title="Pilih Cabang" bind:open={defaultModal} autoclose>
            <p class="text-base leading-relaxed text-center text-gray-500 dark:text-gray-400">Silahkan pilih cabang yang akan dimonitor!</p>
            <svelte:fragment slot="footer">
            <div class="grid grid-cols-3 grid-rows-2 gap-4">
                <Button color="blue" class="text-black bg-merva-100 hover:bg-merva-200 mb-4"
                on:click={() => (cabangDipilih = cabang.bdgKenanganIndah)}
                >{cabang.bdgKenanganIndah}</Button>
                <Button color="blue" class="text-black bg-merva-100 hover:bg-merva-200 mb-4"
                on:click={() => (cabangDipilih = cabang.bdgCisarantenKidul)}
                >{cabang.bdgCisarantenKidul}</Button>
                <Button color="blue" class="text-black bg-merva-100 hover:bg-merva-200 mb-4"
                on:click={() => (cabangDipilih = cabang.jktSouthQuarter)}
                >{cabang.jktSouthQuarter}</Button>
                <Button color="alternative" class="col-span-3">Tidak jadi</Button>
            </div>
            </svelte:fragment>
        </Modal>
            <!-- <Dropdown>
                <DropdownItem class="hover:bg-gray-200" on:click={() => (cabangDipilih = cabang.bdgKenanganIndah)}>{cabang.bdgKenanganIndah}</DropdownItem>
                <DropdownItem class="hover:bg-gray-200" on:click={() => (cabangDipilih = cabang.bdgCisarantenKidul)}>{cabang.bdgCisarantenKidul}</DropdownItem>
                <DropdownItem class="hover:bg-gray-200" on:click={() => (cabangDipilih = cabang.jktSouthQuarter)}>{cabang.jktSouthQuarter}</DropdownItem>
            </Dropdown> -->
    </div>
</header>