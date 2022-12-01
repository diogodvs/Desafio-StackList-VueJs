<template>
  <div class="h-full w-full bg-black-700 font-sans">
    <HeaderComponent></HeaderComponent>
    
    <div class=" text-white-900 m-auto justify-center h-[34.6rem] ">

      <HelloI18n></HelloI18n>
      <StackListComponent></StackListComponent>
      <LocaleSwitcher class="mt-40"></LocaleSwitcher>

    </div>
    
  </div>
  
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import LocaleSwitcher from './components/LocaleSwitcher.vue';
  import HelloI18n from './components/HelloI18n.vue';
  import StackListComponent from './components/StackListComponent.vue';
  
export default {
  name: 'App',
  components: {
    HeaderComponent,
    LocaleSwitcher,
    HelloI18n,
    StackListComponent  
  },  
}
</script>

<style>
#app {
  margin: 0;
  padding: 0;
}
</style>
