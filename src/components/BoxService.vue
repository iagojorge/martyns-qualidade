<template>
  <div class="box">
    <img :src="imageSrc" alt="Image" class="box-image" />
    <h3 class="box-title">{{ title }}</h3>
    <p class="box-text">{{ text }}</p>
  </div>
</template>

<script>
export default {
  name: "BoxService",
  props: {
    imageSrc: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    text: {
      type: String,
      required: true
    }
  }
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500&display=swap');

.box {
  width: 300px;
  height: 575px;
  background-color: black;
  color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  padding-bottom: 20px;
  box-sizing: border-box;
  border-radius: 20px;
  overflow: hidden;
}

.box-image {
  width: 300px;
  height: 400px;
  object-fit: cover;
  margin-bottom: 30px; 
}

.box-title {
  font-family: 'Inter', sans-serif;
  font-size: 18px;
  font-weight: 500;
  text-align: center;
  margin: 0; 
}

.box-text {
  font-family: 'Inter', sans-serif;
  font-size: 12px;
  font-weight: 400;
  text-align: center;
  margin-top: 30px; 
}
</style>
