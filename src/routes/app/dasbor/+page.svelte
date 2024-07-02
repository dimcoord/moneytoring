<script>
    import Datepicker from '../../../components/Datepicker.svelte';
    import Cards from '../../../components/Cards.svelte';
    import TabelKasir from '../../../components/TabelKasir.svelte';
    import TabelProduk from '../../../components/TabelProduk.svelte';
</script>

<div>
    <h1 class="font-bold text-4xl mb-6">Dasbor Penjualan</h1>
    <div class="h-12 w-72 bg-white mb-6">
        <Datepicker />
    </div>
    <div class="flex flex-wrap flex-1 justify-between mb-12">
        <Cards />
    </div>
    <div class="grid grid-cols-2 gap-24">
        <div class="flex flex-col flex-wrap flex-1">
            <span class="font-medium text-lg mb-4">5 Produk Terlaris</span>
            <TabelProduk />
        </div>
        <div class="flex flex-col flex-wrap flex-1">
            <span class="font-medium text-lg mb-4">5 Penjualan Per Kasir Tertinggi</span>
            <TabelKasir />
        </div>
    </div>
</div>