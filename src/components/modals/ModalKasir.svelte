<script>
    import { Button, Modal, Label, Input, Select } from 'flowbite-svelte';
    import { cabang } from '../../data'
    let formModal = false;
    let selected = '';
    let cabangModal = [
    { value: 'bdg-ck', name: `${cabang.bdgCisarantenKidul}` },
    { value: 'bdg-ki', name: `${cabang.bdgKenanganIndah}` },
    { value: 'jkt-gsq', name: `${cabang.jktSouthQuarter}` }
  ];
</script>

<Button color="blue" class="bg-merva h-12" on:click={() => (formModal = true)}>Tambah Data</Button>

<Modal bind:open={formModal} size="xs" autoclose={false} class="w-full">
    <form class="flex flex-col space-y-6" action="#">
      <h3 class="mb-4 text-xl font-medium text-gray-900 dark:text-white">Form Kasir</h3>
      <Label class="space-y-2">
        <span>Kode Kasir</span>
        <Input type="text" name="text" placeholder="Contoh: KCP-01" required />
      </Label>
      <Label class="space-y-2">
        <span>Nama Kasir</span>
        <Input type="text" name="text" placeholder="Contoh: Asep Priyadi" required />
      </Label>
      <Label class="space-y-2">
        <span>Cabang</span>
        <Select class="mt-2" items={cabangModal} bind:value={selected} />
      </Label>
      <Label class="space-y-2">
        <span>Kata Sandi</span>
        <Input type="password" name="password" placeholder="•••••" required />
      </Label>
      <Button color="blue" type="submit" class="w-full bg-merva">Simpan</Button>
    </form>
</Modal>