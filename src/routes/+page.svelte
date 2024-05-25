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

  .footer {
    display: grid;
    grid-template-columns: 1fr;
    background-color: #f5f5f5;
    padding: 40px;
    gap: 30px;
  }


</style>
