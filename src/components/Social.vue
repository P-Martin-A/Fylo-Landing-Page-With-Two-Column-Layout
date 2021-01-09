<template>
  <div class="social">
    <div class="contact">
      <img class="logo" src="@/assets/images/logo-white.svg" alt="Fylo">
      <div class="phone">
        <img class="image" src="@/assets/images/icon-phone.svg" alt="Phone">
        <span
          v-text="phone.text"
        ></span>
      </div>
      <div class="email">
        <img class="image" src="@/assets/images/icon-email.svg" alt="Email">
        <span
          v-text="email.text"        
        ></span>
      </div>
    </div>
    <div class="lists">
      <ul class="list"
        v-for="(items, index) of lists" 
        :key="index"
      >
        <li class="item"
          v-for="(link, index) of items" 
          :key="index"
        >
          <a class="link" href="#"
            v-text="link"
          ></a>
        </li>
      </ul>
    </div>
    <div class="socials">
      <img class="image" src="@/assets/images/facebook.svg" alt="Facebook">
      <img class="image" src="@/assets/images/twitter.svg" alt="Twitter">
      <img class="image" src="@/assets/images/instagram.svg" alt="Instagram">
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Social',
    data() {
      return {
        phone: {
          text: 'Phone: +1-543-123-4567<'
        },
        email: {
          text: 'example@fylo.com'
        },
        lists: [
          [
            'About Us', 'Jobs', 'Press', 'Blog'
          ],
          [
            'Contact Us', 'Terms', 'Privacy'
          ]
        ]
      }
    },
  }
</script>