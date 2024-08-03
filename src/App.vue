<template>
  <div id="app">
    <AppHeader />
    <AppHome />
    <AppService/>
    <AppAbout/>
    <AppContact/>
    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppHome from './components/AppHome.vue';
import AppService from './components/AppService.vue';
import AppAbout from './components/AppAbout.vue';
import AppContact from './components/AppContact.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppHome,
    AppContact,
    AppService,
    AppAbout,
    AppFooter
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;900&display=swap');

body {
  font-family: 'Inter', sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  color: #333;
}
</style>
