<script>
    import Services from "./Services/services.svelte";
    import Navbar from "./navbar/navbar.svelte"
    import Contact from "./contact/contact.svelte";
    import Footer from "./footer/footer.svelte";
</script>
<div class="wrapper">
      <Navbar/>
  <section class="services">
      <Services/>
  </section>
  <section class="contacts">
      <Contact/>
  </section>
  <footer class="footer">
      <Footer/>
  </footer>
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

  .contacts {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    margin-inline: auto;
    padding: 40px 50px;
  }

</style>
