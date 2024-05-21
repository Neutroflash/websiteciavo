<script>
    import Services from "./Services/services.svelte";
</script>
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
  <section class="services">
      <Services/>
  </section>
  <section class="contacts">
    <h1>CONTACTS</h1>
    <div class="contacts-items">
      <div>
        <p>Thank you for your interest in our engineering services .</p>
        <p>
          If you wish to send us a message, please do not hesitate to fill out
          the fields below.
        </p>
        <p>
          We will be happy to get back to you as soon as possible, for any
          information or to provide you with a free quotation.
        </p>
      </div>
      <form class="contact-form">
        <div class="form-group">
          <input
            type="text"
            id="name"
            name="name"
            placeholder="Name"
            required
          />
        </div>
        <div class="form-group">
          <input
            type="email"
            id="email"
            name="email"
            placeholder="Email"
            required
          />
        </div>
        <div class="form-group">
          <input
            type="text"
            id="subject"
            name="subject"
            placeholder="Subject"
            required
          />
        </div>
        <div class="form-group">
          <textarea
            id="message"
            name="message"
            rows="4"
            placeholder="Message"
            required
          ></textarea>
        </div>
        <button type="submit">Send</button>
      </form>
      <div>
        <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d1046.9459941116936!2d13.820555358382034!3d41.48758998178449!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x133abc089b8c4c15%3A0x5fb42dfd780a245a!2sCiavolella%20srl!5e0!3m2!1sit!2spe!4v1716248324205!5m2!1sit!2spe" width="400" height="300" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        <div>
          <h2>Ciavolella S.r.l</h2>
        </div>
      </div>
    </div>
  </section>
  <footer class="footer">
    <section class="footer-section">
      <div class="footer-container">
        <h3>Ciavolella S.r.l</h3>
        <div class="container-items">
          <p>Via Di Biasio, 144 03043 - Cassino (Fr), Italy</p>
          <p>+39 0776 311097</p>
          <a href="#">info@ciavolella.com </a>
          <p>P.IVA 02831730607</p>
        </div>
      </div>
      <div class="footer-container">
        <h3>Naviga</h3>
        <div class="container-items">
          <p>Services</p>
          <p>Projects</p>
          <p>About</p>
          <p>Carreer</p>
          <p>Contact</p>
        </div>
      </div>
      <div class="footer-container">
        <h3>Lavora con nol</h3>
        <div class="container-items">
          <p>
            Ciavolella engineering è sempre alla ricerca di persone
            appassionate, dinamiche, aperte alla collaborazione e al confronto
            con voglia di cimentarsi in un ambiente nuovo e in crescita.
          </p>
          <p><a href="#">Clicca aqui</a> e scopri le posizioni aperte.</p>
        </div>
      </div>
    </section>
    <div class="footer-copyright">
      © 2021 - Ciavolella srl - All rights reserved.
    </div>
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

  .container-items {
    display: flex;
    flex-direction: column;
    gap: 10px;
    margin-top: 20px;
  }

  .contacts {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    margin-inline: auto;
    padding: 40px 50px;
  }

  .contacts-items {
    display: flex;
    flex-direction: column;
    gap: 30px;
  }

  .contact-form .form-group {
  margin-bottom: 15px;
}

.contact-form input,
.contact-form textarea {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
  font-size: 16px;
}

.contact-form input:focus,
.contact-form textarea:focus {
  outline: none;
  border-color: #007bff;
}

.contact-form button {
  right: 0;
  padding: 10px;
  border: none;
  border-radius: 4px;
  background-color: #007bff;
  color: #fff;
  font-size: 16px;
  cursor: pointer;
}

.contact-form button:hover {
  background-color: #0056b3;
}
</style>
