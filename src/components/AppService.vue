<template>
    <section id="sobre-nos" class="section">
      <h1>Serviços</h1>
      <div class="box-container">
        <BoxService
          :imageSrc="require('@/assets/qualifica.png')"
          title="Qualificação de Soldadores"
          text="Qualificação de Soldadores pela norma ASME IX, AWS D1.1, dentre outras. Fornecemos local para Qualificação, EPIS, consumíveis e corpos de prova."
        />
        <BoxService
          :imageSrc="require('@/assets/qualifica.png')"
          title="Qualificação de Soldadores"
          text="Qualificação de Soldadores pela norma ASME IX, AWS D1.1, dentre outras. Fornecemos local para Qualificação, EPIS, consumíveis e corpos de prova."
        />
        <BoxService
          :imageSrc="require('@/assets/qualifica.png')"
          title="Qualificação de Soldadores"
          text="Qualificação de Soldadores pela norma ASME IX, AWS D1.1, dentre outras. Fornecemos local para Qualificação, EPIS, consumíveis e corpos de prova."
        />
        <BoxService
          :imageSrc="require('@/assets/qualifica.png')"
          title="Qualificação de Soldadores"
          text="Qualificação de Soldadores pela norma ASME IX, AWS D1.1, dentre outras. Fornecemos local para Qualificação, EPIS, consumíveis e corpos de prova."
        />
        <BoxService
          :imageSrc="require('@/assets/qualifica.png')"
          title="Qualificação de Soldadores"
          text="Qualificação de Soldadores pela norma ASME IX, AWS D1.1, dentre outras. Fornecemos local para Qualificação, EPIS, consumíveis e corpos de prova."
        />
        <BoxService
          :imageSrc="require('@/assets/qualifica.png')"
          title="Qualificação de Soldadores"
          text="Qualificação de Soldadores pela norma ASME IX, AWS D1.1, dentre outras. Fornecemos local para Qualificação, EPIS, consumíveis e corpos de prova."
        />
        <BoxService
          :imageSrc="require('@/assets/qualifica.png')"
          title="Qualificação de Soldadores"
          text="Qualificação de Soldadores pela norma ASME IX, AWS D1.1, dentre outras. Fornecemos local para Qualificação, EPIS, consumíveis e corpos de prova."
        />
        <BoxService
          :imageSrc="require('@/assets/qualifica.png')"
          title="Qualificação de Soldadores"
          text="Qualificação de Soldadores pela norma ASME IX, AWS D1.1, dentre outras. Fornecemos local para Qualificação, EPIS, consumíveis e corpos de prova."
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
  .section {
    height: 200vh;
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
  