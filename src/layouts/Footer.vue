<template>
  <footer class="footer">
    <Register />
    <Social />
  </footer>
</template>

<script>
  import Register from '@/components/Register'
  import Social from '@/components/Social'
  
  export default {
    name: 'Footer',
    components: {
      Register,
      Social
    }
  }
</script>