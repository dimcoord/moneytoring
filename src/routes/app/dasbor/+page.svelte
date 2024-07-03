<script>
    import Datepicker from '../../../components/Datepicker.svelte';
    import Cards from '../../../components/Cards.svelte';
    import TabelProdukDasbor from '../../../components/TabelProdukDasbor.svelte';
    import TabelKasirDasbor from '../../../components/TabelKasirDasbor.svelte';
</script>

<div>
    <h1 class="mb-6">Dasbor Penjualan</h1>
    <div class="h-10 w-72 bg-white mb-6">
        <Datepicker />
    </div>
    <div class="flex justify-between mb-12">
        <Cards />
    </div>
    <div class="grid grid-cols-2 gap-24">
        <div class="flex flex-col">
            <span class="font-medium text-lg mb-4">5 Produk Terlaris</span>
            <TabelProdukDasbor />
        </div>
        <div class="flex flex-col">
            <span class="font-medium text-lg mb-4">5 Penjualan Per Kasir Tertinggi</span>
            <TabelKasirDasbor />
        </div>
    </div>
</div>