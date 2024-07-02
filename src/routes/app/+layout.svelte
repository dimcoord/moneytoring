<script>
  import "../../app.css"
  import Sidebar from "../../components/Sidebar.svelte";
  import Header from "../../components/Header.svelte";
</script>

<Sidebar />
<main class="min-h-screen bg-gray-100 ml-[18.5rem]">
  <Header />
  <div class="m-16">
    <slot />
  </div>
</main>
