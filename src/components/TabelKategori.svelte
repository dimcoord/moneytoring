<script>
    import { Table, TableBody, TableBodyCell, TableBodyRow, TableHead, TableHeadCell, Checkbox, TableSearch } from 'flowbite-svelte';
</script>

<Table>
    <TableHead>
      <TableHeadCell class="font-extrabold text-base">#</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Kode Kategori</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Nama Kategori</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Aksi</TableHeadCell>
    </TableHead>
    <TableBody tableBodyClass="divide-y">
      <TableBodyRow>
        <TableBodyCell>1</TableBodyCell>
        <TableBodyCell>KCP</TableBodyCell>
        <TableBodyCell>Kecap</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-merva min-w-8 min-h-8 rounded-md text-white mr-6">A</button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => confirm("Apakah Anda Yakin?")}>B</button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>2</TableBodyCell>
        <TableBodyCell>BRS</TableBodyCell>
        <TableBodyCell>Beras</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-merva min-w-8 min-h-8 rounded-md text-white mr-6">A</button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => confirm("Apakah Anda Yakin?")}>B</button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>3</TableBodyCell>
        <TableBodyCell>MYK</TableBodyCell>
        <TableBodyCell>Minyak</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-merva min-w-8 min-h-8 rounded-md text-white mr-6">A</button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => confirm("Apakah Anda Yakin?")}>B</button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>4</TableBodyCell>
        <TableBodyCell>MIE</TableBodyCell>
        <TableBodyCell>Mie Instan</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-merva min-w-8 min-h-8 rounded-md text-white mr-6">A</button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => confirm("Apakah Anda Yakin?")}>B</button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>5</TableBodyCell>
        <TableBodyCell>MNM</TableBodyCell>
        <TableBodyCell>Minuman Kemasan</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-merva min-w-8 min-h-8 rounded-md text-white mr-6">A</button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => confirm("Apakah Anda Yakin?")}>B</button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
    </TableBody>
  </Table>