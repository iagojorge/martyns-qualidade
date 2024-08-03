<template>
    <section id="footer" class="section">
      <div class="logo">
        <img src="@/assets/logo.png" alt="Martyns Qualidade Logo" />
        <h2>© 2024 Martyns Qualidade. Todos os direitos reservados.</h2>
        <h2>Endereço: Rua Edmundo Gonçalves Ferreira, 250 - Porto das Laranjeiras - Serra - ES</h2>
      </div>
      <div class="info">
        <div class="page">
          <h1>Páginas</h1>
          <a href="#home" class="footer-link">Home</a>
          <a href="#servicos" class="footer-link">Serviços</a>
          <a href="#sobre-nos" class="footer-link">Sobre-Nós</a>
          <a href="#contato" class="footer-link">Contato</a>
        </div>
        <div class="contact">
          <h1>Contato</h1>
          <a href="mailto:comercial@martynsqualidade.com.br" class="footer-link">E-mail</a>
          <a href="https://wa.me/5527998969507?text=Gostaria%20de%20fazer%20um%20or%C3%A7amento" class="footer-link">Whatsapp</a>
        </div>
      </div>
    </section>
  </template>
  
  
  <script>
  export default {
    name: "AppFooter",
  };
  </script>
  
  <style scoped>
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@800;300&display=swap");

.section {
  background-color: #4e6fe0;
  min-height: 291px;
  display: flex;
  justify-content: space-between;
  padding: 20px;
  color: #ffffff;
}

.logo {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
  width: 50%;
  gap: 50px; 
}

.logo img {
  height: 50px;
}

.info {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  width: 20%;
}

.page, .contact {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
  gap: 5px; 
}

.page h1, .contact h1 {
  font-family: 'Inter', sans-serif;
  font-weight: 800;
  font-size: 20px;
  margin-bottom: 18px; 
  color: #ffffff; 
}

.page a, .contact a {
  font-family: 'Inter', sans-serif;
  font-weight: 300;
  font-size: 14px;
  color: #ffffff;
  text-decoration: none;
  background-color: transparent;
  padding: 5px 10px;
  border-radius: 5px;
  transition: background-color 0.3s, color 0.3s;
}

.page a:hover, .contact a:hover {
  background-color: #ffffff;
  color: #4e6fe0;
}

.contact{
  margin-right: 100px;
}

.logo h2 {
    font-family: 'Inter', sans-serif;
    font-weight: 300;
    font-size: 14px;
    color: #ffffff; 
  }
</style>

  