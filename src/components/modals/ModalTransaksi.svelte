<script>
    import { Button, Modal, Label, Input, Select } from 'flowbite-svelte';
    import { produk } from '../../data'
    let formModal = false;
    let selected = '';
    let produkModal = [
    { value: 'kcp-01', name: `${produk.kecap}` }
  ];
</script>

<Button color="blue" class="bg-merva h-12" on:click={() => (formModal = true)}>Tambah Data</Button>

<Modal bind:open={formModal} size="xs" autoclose={false} class="w-full">
    <form class="flex flex-col space-y-6" action="#">
      <h3 class="mb-4 text-xl font-medium text-gray-900 dark:text-white">Form Transaksi</h3>
      <div class="flex">
        <Label class="space-y-2 mr-4">
          <span>Produk</span>
          <Select class="mt-2" items={produkModal} bind:value={selected} />
        </Label>
        <Label class="space-y-2">
          <span>Jumlah Produk</span>
          <Input type="number" name="number" placeholder="Contoh: 12" required />
        </Label>
      </div>
      <div class="flex">
        <Button color="blue" type="submit" class="w-[40%] bg-merva mr-4">Simpan</Button>
        <Button color="blue" type="submit" class="w-[40%] bg-yellow-400">Tambah Produk</Button>
      </div>
    </form>
</Modal>