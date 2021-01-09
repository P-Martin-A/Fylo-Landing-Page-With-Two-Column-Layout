<template>
  <div class="hero">
    <div class="images">
      <img class="image" src="@/assets/images/illustration-1.svg" alt="Hero">
    </div>
    <div class="content">
      <h2 class="title"
        v-text="title"
      ></h2> 
      <p class="text"
        v-text="text"
      ></p>
      <form class="form">
        <div class="form-group">
          <input type="text"
            :placeholder="placeholder"
          >
          <button type="submit"
            v-text="btn"
          ></button>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Hero', 
    data() {
      return {
        title: 'All your files in one secure location, accessible anywhere.',
        text: 'Fylo stores your most important files in one secure location. Access them wherever you need, share and collaborate with friends, family, and co-workers.',
        placeholder: 'Enter your email',
        btn: 'Get Started'        
      }
    },
  }
</script>