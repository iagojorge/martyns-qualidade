<template>
  <section id="sobre-nos" class="section">
    <div class="box">
      <h1>Inovação</h1>
      <h2>Investimos continuamente em tecnologia e capacitação.</h2>
    </div>
    <div class="box">
      <h1>Inovação</h1>
      <h2>Investimos continuamente em tecnologia e capacitação.</h2>
    </div>
    <div class="box">
      <h1>Inovação</h1>
      <h2>Investimos continuamente em tecnologia e capacitação.</h2>
    </div>
    <div class="box">
      <h1>Inovação</h1>
      <h2>Investimos continuamente em tecnologia e capacitação.</h2>
    </div>
    <div class="big-box">
      <h1>Nossa Visão</h1>
      <h2>
        Ser reconhecidos como a principal empresa de inspeção de soldas no
        mercado, valorizando a integridade, a qualidade e a satisfação do
        cliente em todos os nossos serviços.
      </h2>
    </div>
    <div class="big-box">
      <h1>Nossa Missão</h1>
      <h2>
        Comprometidos com a excelência, buscamos fornecer serviços de inspeção e
        qualificação que garantam a segurança e qualidade dos projetos de nossos
        clientes, promovendo a inovação e o desenvolvimento contínuo.
      </h2>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppAbout",
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@800;500&display=swap");

.section {
  background-color: #181717;
  min-height: 80vh;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  text-align: center;
  gap: 95px 120px; 
}

.box {
  width: 226px;
  height: 146px;
  text-align: left;
}

.big-box {
  width: 573px;
  height: 160px;
  text-align: center;
}

h1 {
  font-family: "Inter", sans-serif;
  font-weight: 800;
  font-size: 18px;
  color: #ffffff;
  margin-bottom: 10px;
}

h2 {
  font-family: "Inter", sans-serif;
  font-weight: 500;
  font-size: 12px;
  color: #616161;
  margin: 0;
}

.big-box h1 {
  text-align: center; 
}
</style>
