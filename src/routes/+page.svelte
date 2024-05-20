<div class="wrapper">
  <ul class="navbar">
    <img src="#" alt="logo" />
    <div class="navbar-items">
      <li>HOME</li>
      <li>SERVICES</li>
      <li>PROJECTS</li>
      <li>COMPANY</li>
      <li>CARREER</li>
    </div>
  </ul>
  <footer class="footer">
    <section class="footer-section">
      <div class="footer-container">
        <h3>Ciavolella S.r.l</h3>
        <p>Via Di Biasio, 144 03043 - Cassino (Fr), Italy</p>
        <p>+39 0776 311097</p>
        <a href="#">info@ciavolella.com </a>
        <p>P.IVA 02831730607</p>
      </div>
      <div class="footer-container">
        <h3>Naviga</h3>
        <p>Services</p>
        <p>Projects</p>
        <p>About</p>
        <p>Carreer</p>
        <p>Contact</p>
      </div>
      <div class="footer-container">
        <h3>Lavora con nol</h3>
        <p>
          Ciavolella engineering è sempre alla ricerca di persone appassionate,
          dinamiche, aperte alla collaborazione e al confronto con voglia di
          cimentarsi in un ambiente nuovo e in crescita.
        </p>
        <p><a href="#">Clicca aqui</a> e scopri le posizioni aperte.</p>
      </div>
    </section>
    <div class="footer-copyright">© 2021 - Ciavolella srl - All rights reserved. </div>
  </footer>
</div>

<style>
  .wrapper {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }

  .navbar {
    display: flex;
    justify-content: space-between;
    padding: 40px 100px;
    margin: 0;
    box-shadow: 0 0 10px #000;
  }

  .navbar-items {
    display: flex;
    gap: 40px;
  }

  .footer {
    display: grid;
    grid-template-columns: 1fr;
    background-color: #f5f5f5;
    padding: 40px;
    gap: 30px;
  }

  .footer-section {
    display: flex;
    justify-content: center;
    margin-inline: auto;
  }

  .footer-container {
    width: 200px;
  }

  .footer-copyright {
    text-align: center;
  }
</style>
