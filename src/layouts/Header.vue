<template>
  <header class="header">
    <h1 class="title">
      <img class="logo" src="@/assets/images/logo.svg" alt="Fylo">
    </h1>
    <Navigation />
  </header>
</template>

<script>
  import Navigation from '@/components/Navigation'
  
  export default {
    name: 'Header',
    components: { 
      Navigation 
    },
  }
</script>