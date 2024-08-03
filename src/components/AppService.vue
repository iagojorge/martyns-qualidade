<template>
  <section id="servicos" class="section">
    <h1>Serviços</h1>
    <div class="box-container">
      <BoxService
        :imageSrc="require('@/assets/inspec.webp')"
        title="inspeção de soldas"
        text="Utilizamos técnicas avançadas para garantir a integridade das soldas, identificando possíveis falhas e garantindo a segurança das estruturas."
      />
      <BoxService
        :imageSrc="require('@/assets/qualifica.png')"
        title="Qualificação de Soldadores"
        text="Qualificação de Soldadores pela norma ASME IX, AWS D1.1, dentre outras. Fornecemos local para Qualificação, EPIS, consumíveis e corpos de prova."
      />
      <BoxService
        :imageSrc="require('@/assets/procedimento.webp')"
        title="Qualificação de Procedimentos"
        text="Desenvolvemos e validamos procedimentos de soldagem para garantir a conformidade com as normas técnicas."
      />
      <BoxService
        :imageSrc="require('@/assets/terceir.webp')"
        title="Terceirização de Mão de Obra"
        text="Oferecemos profissionais especializados para atender demandas temporárias ou permanentes de nossos clientes."
      />
      <BoxService
        :imageSrc="require('@/assets/tinta.png')"
        title="Inspeção de Pintura"
        text="Verificamos a qualidade e aderência das pinturas industriais, garantindo a proteção adequada das superfícies."
      />
      <BoxService
        :imageSrc="require('@/assets/ultrasom.jpg')"
        title="Inspeção por Ultrassom Phased Array"
        text="Utilizamos tecnologia de ultrassom avançada para detectar descontinuidades internas em materiais."
      />
      <BoxService
        :imageSrc="require('@/assets/liquido.png')"
        title="Inspeção por Líquidos Penetrantes"
        text="Aplicamos métodos de líquidos penetrantes para identificar fissuras e defeitos superficiais."
      />
      <BoxService
        :imageSrc="require('@/assets/particula.png')"
        title="Inspeção por Partículas Magnéticas"
        text="Realizamos inspeções magnéticas para detectar descontinuidades superficiais e subsuperficiais em materiais ferromagnéticos."
      />
    </div>
  </section>
</template>

<script>
import BoxService from "./BoxService.vue";
export default {
  name: "AppAbout",
  components: {
    BoxService,
  },
};
</script>

<style scoped>
h1 {
  font-size: 32px;
  color: #4e6fe0;
  font-weight: 900;
  text-align: center;
}

.section {
  height: 180vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  padding-top: 110px;
}

.box-container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 30px;
  justify-content: center;
  margin-top: 110px;
}
</style>
