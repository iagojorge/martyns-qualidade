<template>
  <section id="contato" class="section">
    <div class="content">
      <div class="text-h2">
        <h2>
          Para mais informações sobre nossos serviços e como podemos ajudar no
          seu projeto, entre em contato conosco. Estamos prontos para oferecer
          soluções personalizadas e atender todas as suas necessidades de
          inspeção e qualificação de soldas.
        </h2>
      </div>
      <div class="button-group">
        <a href="https://wa.me/5527998969507?text=Gostaria%20de%20fazer%20um%20or%C3%A7amento" class="btn-secondary" target="_blank" rel="noopener noreferrer">
          <img src="@/assets/phone.svg" alt="Phone Icon" class="btn-icon" />
          (27) 9 9896 9507
        </a>
        <a href="mailto:comercial@martynsqualidade.com.br" class="btn-primary" target="_blank" rel="noopener noreferrer">
          <img src="@/assets/email.svg" alt="Email Icon" class="btn-icon" />
          comercial@martynsqualidade.com.br
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppAbout",
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@400;500;900&display=swap");

body {
  font-family: "Inter", sans-serif;
}

.section {
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.content {
  max-width: 900px;
  margin-top: 300px;
  text-align: center;
}

.text-h2 {
  max-width: 700px;
  margin: 0 auto;
  text-align: left;
  margin-bottom: 100px;
}

h1 {
  font-size: 32px;
  color: #4e6fe0;
  font-weight: 900;
  text-align: center;
}

h2 {
  font-size: 16px;
  font-weight: 500;
  color: #333;
  margin-top: 20px;
  text-align: left;
}

.button-group {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
  margin-top: 20px;
}

.btn-primary, .btn-secondary {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 250px;
  height: 50px;
  border: none;
  border-radius: 38px;
  font-size: 16px;
  text-decoration: none;
  cursor: pointer;
}

.btn-primary {
  background-color: #4e6fe0;
  color: white;
  width: 350px;
}

.btn-secondary {
  background-color: #25D366;
  color: white;
  margin-right: 80px;
}

.btn-primary:hover, .btn-secondary:hover {
  opacity: 0.8;
}

.btn-icon {
  width: 24px; 
  height: 24px;
  margin-right: 10px;
}
</style>
