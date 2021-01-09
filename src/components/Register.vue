<template>
  <div class="register">
    <div class="content">
      <h3 class="title"
        v-text="title"
      ></h3>
      <p class="text"
        v-text="text"
      ></p>
    </div>
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
</template>

<script>
  export default {
    name: 'Register',
    data() {
      return {
        title: 'Get early access today',
        text: 'It only takes a minute to sign up and our free starter tier is extremely generous. If you have any questions, our support team would be happy to help you.',
        placeholder: 'email@example.com',
        btn: 'Get Started For Free'
      }
    },
  }
</script>