<script>
    import Main from "./Main/Main.svelte";
    import Navbar from "./navbar/navbar.svelte"
    import Footer from "./footer/footer.svelte";
</script>
<div class="wrapper">
      <Navbar/>
      <Main/>
      <Footer/>
</div>

<style>
  .wrapper {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }


</style>
