<script>
    import { Button, Modal, Label, Input, Checkbox } from 'flowbite-svelte';
    let formModal = false;
</script>

<Button color="blue" class="bg-merva h-12" on:click={() => (formModal = true)}>Tambah Data</Button>

<Modal bind:open={formModal} size="xs" autoclose={false} class="w-full">
    <form class="flex flex-col space-y-6" action="#">
      <h3 class="mb-4 text-xl font-medium text-gray-900 dark:text-white">Form Produk</h3>
      <Label class="space-y-2">
        <span>Kode Produk</span>
        <Input type="text" name="text" placeholder="Contoh: KCP-01" required />
      </Label>
      <Label class="space-y-2">
        <span>Nama Produk</span>
        <Input type="text" name="text" placeholder="Contoh: Kecap Manis" required />
      </Label>
      <Label class="space-y-2">
        <span>Harga Beli Produk</span>
        <Input type="number" name="number" placeholder="Contoh: 20000" required />
      </Label>
      <Label class="space-y-2">
        <span>Harga Jual Produk</span>
        <Input type="number" name="number" placeholder="Contoh: 35000" required />
      </Label>
      <Label class="space-y-2">
        <span>Jumlah Produk</span>
        <Input type="number" name="number" placeholder="Contoh: 12" required />
      </Label>
      <Button color="blue" type="submit" class="w-full bg-merva">Simpan</Button>
    </form>
</Modal>