<script>
    import AppHeader from './components/AppHeader.vue';
    import AppMain from './components/AppMain.vue';
    import AppMainBottom from './components/AppMainBottom.vue';
    import AppFooterTop from './components/AppFooterTop.vue';
    
    export default {
      components:{
        AppHeader,
        AppMain,
        AppMainBottom,
        AppFooterTop,
        
      } 
    }
</script>
<template>
  <div>
    <AppHeader/>
    <AppMain/>
    <AppMainBottom/>
    <AppFooterTop/>
   
  </div>
</template>
<style lang="scss">
  @use './styles/generals.scss' as *;
  
</style>