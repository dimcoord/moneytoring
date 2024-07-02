<script>
    import { Table, TableBody, TableBodyCell, TableBodyRow, TableHead, TableHeadCell, Checkbox, TableSearch } from 'flowbite-svelte';
</script>

<Table>
    <TableHead>
      <TableHeadCell class="font-extrabold text-base">#</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">No. Transaksi</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Tanggal</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Total Transaksi</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Aksi</TableHeadCell>
    </TableHead>
    <TableBody tableBodyClass="divide-y">
      <TableBodyRow>
        <TableBodyCell>1</TableBodyCell>
        <TableBodyCell>0005</TableBodyCell>
        <TableBodyCell>09 April 2024</TableBodyCell>
        <TableBodyCell>Rp456.000</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-merva min-w-8 min-h-8 rounded-md text-white mr-6">A</button>
            <button class="bg-yellow-400 min-w-8 min-h-8 rounded-md text-white mr-6">C</button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => confirm("Apakah Anda Yakin?")}>B</button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>2</TableBodyCell>
        <TableBodyCell>0004</TableBodyCell>
        <TableBodyCell>08 Maret 2024</TableBodyCell>
        <TableBodyCell>Rp222.500</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-merva min-w-8 min-h-8 rounded-md text-white mr-6">A</button>
            <button class="bg-yellow-400 min-w-8 min-h-8 rounded-md text-white mr-6">C</button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => confirm("Apakah Anda Yakin?")}>B</button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>3</TableBodyCell>
        <TableBodyCell>0003</TableBodyCell>
        <TableBodyCell>07 Februari 2024</TableBodyCell>
        <TableBodyCell>Rp144.000</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-merva min-w-8 min-h-8 rounded-md text-white mr-6">A</button>
            <button class="bg-yellow-400 min-w-8 min-h-8 rounded-md text-white mr-6">C</button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => confirm("Apakah Anda Yakin?")}>B</button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>4</TableBodyCell>
        <TableBodyCell>0002</TableBodyCell>
        <TableBodyCell>06 Januari 2024</TableBodyCell>
        <TableBodyCell>Rp423.000</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-merva min-w-8 min-h-8 rounded-md text-white mr-6">A</button>
            <button class="bg-yellow-400 min-w-8 min-h-8 rounded-md text-white mr-6">C</button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => confirm("Apakah Anda Yakin?")}>B</button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>5</TableBodyCell>
        <TableBodyCell>0001</TableBodyCell>
        <TableBodyCell>05 Desember 2023</TableBodyCell>
        <TableBodyCell>Rp900.000</TableBodyCell>
        <TableBodyCell>
          <div class="flex justify-center">
            <button class="bg-merva min-w-8 min-h-8 rounded-md text-white mr-6">A</button>
            <button class="bg-yellow-400 min-w-8 min-h-8 rounded-md text-white mr-6">C</button>
            <button class="bg-red-600 min-w-8 min-h-8 rounded-md text-white"
            on:click={() => confirm("Apakah Anda Yakin?")}>B</button>
          </div>
        </TableBodyCell>
      </TableBodyRow>
    </TableBody>
  </Table>