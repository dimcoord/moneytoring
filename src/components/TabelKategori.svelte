<script>
    import { Table, TableBody, TableBodyCell, TableBodyRow, TableHead, TableHeadCell, Checkbox, TableSearch } from 'flowbite-svelte';
    import { Button, Modal } from 'flowbite-svelte';
    import { ExclamationCircleOutline, TrashBinOutline, PenOutline } from 'flowbite-svelte-icons';
    let popupModal = false;
</script>

<Modal bind:open={popupModal} size="xs" autoclose>
  <div class="text-center">
    <ExclamationCircleOutline class="mx-auto mb-4 text-gray-400 w-12 h-12 dark:text-gray-200" />
    <h3 class="mb-5 text-lg font-normal text-gray-500 dark:text-gray-400">Apakah Anda yakin ingin menghapus kategori ini?</h3>
    <Button color="red" class="me-2">Ya, hapus</Button>
    <Button color="alternative">Tidak, jangan hapus</Button>
  </div>
</Modal>

<Table>
    <TableHead>
      <TableHeadCell class="font-extrabold text-base">#</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Kode Kategori</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Nama Kategori</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base text-center">Aksi</TableHeadCell>
    </TableHead>
    <TableBody tableBodyClass="divide-y">
      <TableBodyRow>
        <TableBodyCell>1</TableBodyCell>
        <TableBodyCell>KCP</TableBodyCell>
        <TableBodyCell>Kecap</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-yellow-400 min-w-8 min-h-8 rounded-md text-white mr-6"><PenOutline class="mx-auto" /></button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => (popupModal = true)}><TrashBinOutline class="mx-auto" /></button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>2</TableBodyCell>
        <TableBodyCell>BRS</TableBodyCell>
        <TableBodyCell>Beras</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-yellow-400 min-w-8 min-h-8 rounded-md text-white mr-6"><PenOutline class="mx-auto" /></button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => (popupModal = true)}><TrashBinOutline class="mx-auto" /></button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>3</TableBodyCell>
        <TableBodyCell>MYK</TableBodyCell>
        <TableBodyCell>Minyak</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-yellow-400 min-w-8 min-h-8 rounded-md text-white mr-6"><PenOutline class="mx-auto" /></button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => (popupModal = true)}><TrashBinOutline class="mx-auto" /></button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>4</TableBodyCell>
        <TableBodyCell>MIE</TableBodyCell>
        <TableBodyCell>Mie Instan</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-yellow-400 min-w-8 min-h-8 rounded-md text-white mr-6"><PenOutline class="mx-auto" /></button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => (popupModal = true)}><TrashBinOutline class="mx-auto" /></button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>5</TableBodyCell>
        <TableBodyCell>MNM</TableBodyCell>
        <TableBodyCell>Minuman Kemasan</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-yellow-400 min-w-8 min-h-8 rounded-md text-white mr-6"><PenOutline class="mx-auto" /></button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => (popupModal = true)}><TrashBinOutline class="mx-auto" /></button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
    </TableBody>
  </Table>