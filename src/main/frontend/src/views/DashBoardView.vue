<script setup>
import dashboardAside from '../components/dashboard/dashboardAside.vue';
import Header from '../components/Header.vue';
import SpecimenList from '../components/dashboard/specimentList.vue';
</script>

<template>
  <main>
    <div class="header">
      <Header/>
    </div>

  <div class="container">
    <dashboardAside />
    <div class="specimentList">
      <SpecimenList/>
    </div>
  </div>

  </main>
</template>

<style lang="scss" scoped>
 @use "./src/sass/styles.scss" as *;
 
 main{
    background: $background-page;
    background-repeat: no-repeat;
    background-size: cover ;
        .header {
          padding-top: 30px;
          margin: 0 auto;    
        }
    
        .container{
          display: flex;
          flex-direction: row;
          margin-top: 5vh;
          margin-left: 4em;

            .specimentList  {
              margin-left: 4em;
            }
        }

        
  }

    



</style>