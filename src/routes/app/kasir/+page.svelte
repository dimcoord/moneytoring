<script>
    import TabelKasir from "../../../components/TabelKasir.svelte";
    import ModalKasir from "../../../components/modals/ModalKasir.svelte";
</script>

<div class="flex justify-between mb-6">
    <h1 class="mb-6">Kelola Kasir</h1>
    <ModalKasir />
    <!-- <a href="/app/kasir/form" class="bg-merva font-bold text-white max-h-12 w-32 p-3 rounded-md" data-sveltekit-reload>Tambah Data</a> -->
</div>

<TabelKasir />

