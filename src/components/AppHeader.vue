<template>
  <header>
    <div class="header-container">
      <div class="logo">
        <img src="@/assets/logo.png" alt="Martyns Qualidade Logo">
      </div>
      <nav>
        <a href="#home" :class="{ active: currentSection === 'home' }" @click="scrollToSection('home')">Home</a>
        <a href="#servicos" :class="{ active: currentSection === 'servicos' }" @click="scrollToSection('servicos')">Serviços</a>
        <a href="#sobre-nos" :class="{ active: currentSection === 'sobre-nos' }" @click="scrollToSection('sobre-nos')">Sobre Nós</a>
        <a href="#contato" :class="{ active: currentSection === 'contato' }" @click="scrollToSection('contato')">Contato</a>
      </nav>
      <a href="https://wa.me/5527998969507?text=Gostaria%20de%20fazer%20um%20or%C3%A7amento" class="cta" target="_blank" rel="noopener noreferrer">Faça um Orçamento</a>
    </div>
  </header>
</template>

<script>
export default {
  name: 'AppHeader',
  data() {
    return {
      currentSection: 'home'
    };
  },
  methods: {
    scrollToSection(section) {
      this.currentSection = section;
      const element = document.getElementById(section);
      if (element) {
        element.scrollIntoView({ behavior: 'smooth' });
      }
    }
  }
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap');

body {
  font-family: 'Inter', sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  color: #333;
}

header {
  background-color: #fff;
  border-bottom: 1px solid #ddd;
  padding: 10px 20px;
  width: 98%;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 1000;
}

.header-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  display: flex;
  align-items: center;
}

.logo img {
  height: 50px;
  margin-right: 10px;
}

.logo span {
  font-size: 14px;
  color: #333;
}

nav {
  display: flex;
  gap: 20px;
}

nav a {
  text-decoration: none;
  color: #333;
  font-size: 16px;
  position: relative;
  padding-bottom: 5px;
}

nav a::after {
  content: '';
  display: block;
  width: 0;
  height: 2px;
  background: #4E6FE0;
  transition: width 0.3s;
  position: absolute;
  bottom: 0;
  left: 0;
}

nav a:hover::after,
nav a.active::after {
  width: 100%;
}

nav a.active {
  color: #4E6FE0;
  font-weight: bold;
}

.cta {
  background-color: #4E6FE0;
  color: #fff;
  padding: 10px 20px;
  border-radius: 20px;
  text-decoration: none;
  font-size: 16px;
}

.cta:hover {
  background-color: #4E6FE0;
}
</style>
