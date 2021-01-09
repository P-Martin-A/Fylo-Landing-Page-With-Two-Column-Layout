<template>
  <div class="about">
    <div class="images">
      <img class="image" src="@/assets/images/illustration-2.svg" alt="">
    </div>
    <div class="content">
      <div class="texts">
        <h3 class="title"
          v-text="title"
        ></h3>
        <p class="text"
          v-text="text_fisrt"
        ></p>
        <p class="text"
          v-text="text_second"
        ></p>
      </div>
      <div class="go">
        <a class="btn" href="#"
          v-text="btn"
        >
        </a>
        <img class="image" src="@/assets/images/icon-arrow.svg" alt="Arrow">
      </div>
      <div class="info">
        <div class="box">
          <img class="quotes" src="@/assets/images/icon-quotes.svg" alt="Quotes">
          <p class="text"
            v-text="text_third"
          ></p>
          <div class="person">
            <img class="image" src="@/assets/images/avatar-testimonial.jpg" alt="Person">
            <div class="texts">
              <h4 class="avatar"
                v-text="avatar"
              ></h4>
              <span class="stack"
                v-text="stack"
              ></span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'About',
    data() {
      return {
        title: 'Stay productive, wherever you are',
        text_fisrt: 'Never let location be an issue when accessing your files. Fylo has you covered for all of your file storage needs.',
        text_second: 'Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required!',
        btn: 'See how Fylo works',
        text_third: 'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
        avatar: 'Kyle Burton',
        stack: 'Founder & CEO, Huddle'
      }
    },
  }
</script>