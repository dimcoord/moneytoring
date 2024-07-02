<script>
    import { Table, TableBody, TableBodyCell, TableBodyRow, TableHead, TableHeadCell, Checkbox, TableSearch } from 'flowbite-svelte';
</script>

<Table>
    <TableHead>
      <TableHeadCell class="font-extrabold text-base">#</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Kode Produk</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Nama Produk</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Harga Jual</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Jumlah Produk</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Aksi</TableHeadCell>
    </TableHead>
    <TableBody tableBodyClass="divide-y">
      <TableBodyRow>
        <TableBodyCell>1</TableBodyCell>
        <TableBodyCell>KCP01</TableBodyCell>
        <TableBodyCell>Kecap Bango</TableBodyCell>
        <TableBodyCell>Rp2.000</TableBodyCell>
        <TableBodyCell>25</TableBodyCell>
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
        <TableBodyCell>KCP01</TableBodyCell>
        <TableBodyCell>Kecap ABC</TableBodyCell>
        <TableBodyCell>Rp2.500</TableBodyCell>
        <TableBodyCell>15</TableBodyCell>
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
        <TableBodyCell>BRS01</TableBodyCell>
        <TableBodyCell>Beras Pandan Wangi</TableBodyCell>
        <TableBodyCell>Rp14.000</TableBodyCell>
        <TableBodyCell>32</TableBodyCell>
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
        <TableBodyCell>MIE01</TableBodyCell>
        <TableBodyCell>Mie Sedap</TableBodyCell>
        <TableBodyCell>Rp23.000</TableBodyCell>
        <TableBodyCell>12</TableBodyCell>
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
        <TableBodyCell>MNM01</TableBodyCell>
        <TableBodyCell>Minuman Aqua</TableBodyCell>
        <TableBodyCell>Rp9.000</TableBodyCell>
        <TableBodyCell>25</TableBodyCell>
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