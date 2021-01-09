<template>
  <nav class="navigation">
    <ul class="list">
      <li class="item"
        v-for="(item, index) of items" 
        :key="index"
      >
        <a class="link" href="#"
          v-text="item"
        ></a>
      </li>
    </ul>
  </nav>
</template>

<script>
  export default {
    name: 'HelloWorld',
    data() {
      return {
        items: ['Features', 'Team', 'Sign In']
      }
    },
  }
</script>