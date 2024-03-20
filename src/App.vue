<script>
export default {
  data(){
    return{
      title:'Titolo globale Vite',
      p: 'primo paragrafo Vite',
      title2: 'Titolo scope Vite',
      p2: 'paragrafo css scope'
    }
  }
}
</script>

<template>
  <div class="container-md d-flex">
    <!-- container css globale -->
    <div class="box box1">
      <h1>{{ title }}</h1>
      <p>{{ p }}</p>
    </div>
    <!-- container css scoped -->
    <div class="box box2">
      <h1>{{ title2 }}</h1>
      <p>{{ p2 }}</p>
    </div>
  </div>
</template>

<style scoped>
  .box.box2 h1{
    color: rgb(145, 49, 235);
  }

  .box.box2 p{
    color: rgb(24, 211, 211);
    font-size: 1.7rem;
  }

</style>