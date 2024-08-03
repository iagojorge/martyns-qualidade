<template>
  <section id="home" class="section">
    <img src="@/assets/banner.png" alt="banner" class="banner" />
    <div class="content">
      <h1>Martyns Qualidade - Excelência em Inspeção de Soldas</h1>
      <div class="text-h2">
        <h2>
          Fundada com o objetivo de contribuir para a garantia da Qualidade em
          Processos de Soldagem, Equipamentos e Fabricação, a Martyns Qualidade
          Inspeção & Soldas se destaca como uma referência no setor de Controle da
          Qualidade. Oferecemos serviços de parceria com mão de obra
          especializada, Certificada ABENDI e FBTS, dentre outras, para atender as
          demandas mais rigorosas de nossos clientes.
        </h2>
      </div>
      <div class="button-group">
        <button class="btn-primary" @click="scrollToSection('sobre-nos')">Saiba mais sobre nós</button>
        <a href="https://wa.me/5527998969507?text=Gostaria%20de%20fazer%20um%20or%C3%A7amento" class="btn-image" target="_blank" rel="noopener noreferrer">
          <img src="@/assets/zap.png" alt="Button Image" />
        </a>
        <img src="@/assets/pet.png" alt="pet" class="pet-image"/>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppHome",
  methods: {
    scrollToSection(sectionId) {
      const section = document.getElementById(sectionId);
      if (section) {
        section.scrollIntoView({ behavior: 'smooth' });
      }
    }
  }
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;900&display=swap');

body {
  font-family: 'Inter', sans-serif;
}

.banner {
  width: 100%;
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
  margin-top: 50px;
  text-align: center;
}

.text-h2 {
  max-width: 700px;
  margin: 0 auto;
  text-align: left; 
}

h1 {
  font-size: 32px;
  color: #4E6FE0;
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

.btn-primary {
  background-color: #4E6FE0;
  color: white;
  width: 300px;
  height: 50px;
  border: none;
  border-radius: 38px;
  font-size: 16px;
  cursor: pointer;
}

.btn-primary:hover {
  background-color: #4E6FE0;
}

.btn-image {
  background: none;
  border: none;
  cursor: pointer;
}

.btn-image img {
  width: 80px;
  height: 80px;
}

.pet-image {
  width: 205px;
  height: 300px;
}
</style>
