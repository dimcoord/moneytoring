<script>
    import { Table, TableBody, TableBodyCell, TableBodyRow, TableHead, TableHeadCell, Checkbox, TableSearch } from 'flowbite-svelte';
</script>

<Table>
    <TableHead>
      <TableHeadCell class="font-extrabold text-base">Nama Kasir</TableHeadCell>
      <TableHeadCell class="font-extrabold text-base">Jumlah Transaksi</TableHeadCell>
    </TableHead>
    <TableBody tableBodyClass="divide-y">
      <TableBodyRow>
        <TableBodyCell>Diding Ridwan</TableBodyCell>
        <TableBodyCell>430</TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>Ateng Surateng</TableBodyCell>
        <TableBodyCell>411</TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>Otang Komari</TableBodyCell>
        <TableBodyCell>320</TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>Jihan Sulaeman</TableBodyCell>
        <TableBodyCell>312</TableBodyCell>
      </TableBodyRow>
      <TableBodyRow>
        <TableBodyCell>Naring Fitriani</TableBodyCell>
        <TableBodyCell>444</TableBodyCell>
      </TableBodyRow>
    </TableBody>
  </Table>