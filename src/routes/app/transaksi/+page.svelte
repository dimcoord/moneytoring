<script>
    import TabelTransaksi from "../../../components/TabelTransaksi.svelte";
    import ModalTransaksi from "../../../components/modals/ModalTransaksi.svelte";
</script>

<div class="flex justify-between mb-6">
    <h1 class="mb-2">Laporan Transaksi</h1>
    <ModalTransaksi />
    <!-- <a href="/app/produk/form" class="bg-merva font-bold text-white max-h-12 w-32 p-3 rounded-md" data-sveltekit-reload>Tambah Data</a> -->
</div>

<div class="mb-6">
    <h1 class="mb-6"><h1 class="font-normal inline">Total Transaksi Bulan April:</h1> Rp26.450.000</h1>
</div>

<TabelTransaksi />