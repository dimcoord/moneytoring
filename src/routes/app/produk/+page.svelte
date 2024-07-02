<script>
    import TabelProduk from "../../../components/TabelProduk.svelte";
</script>

<div class="flex justify-between mb-6">
    <h1 class="mb-6">Produk</h1>
    <a href="/app/produk/form" class="bg-merva font-bold text-white max-h-12 w-32 p-3 rounded-md" data-sveltekit-reload>Tambah Data</a>
</div>

<TabelProduk />