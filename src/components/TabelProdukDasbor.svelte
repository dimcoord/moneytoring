<script>
    import { Table, TableBody, TableBodyCell, TableBodyRow, TableHead, TableHeadCell, Checkbox, TableSearch } from 'flowbite-svelte';
</script>

<Table>
    <TableHead>
      <TableHeadCell class="font-extrabold text-base">Nama Produk</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Jumlah Terjual</TableHeadCell>
    </TableHead>
    <TableBody tableBodyClass="divide-y">
      <TableBodyRow>
        <TableBodyCell>Kecap Bango</TableBodyCell>
        <TableBodyCell>430</TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>Beras Pandan</TableBodyCell>
        <TableBodyCell>411</TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>Minyak Bimoli</TableBodyCell>
        <TableBodyCell>320</TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>Mie Indomie</TableBodyCell>
        <TableBodyCell>312</TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>Frutang</TableBodyCell>
        <TableBodyCell>444</TableBodyCell>
      </TableBodyRow>
    </TableBody>
  </Table>