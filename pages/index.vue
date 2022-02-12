<template>
  <div class="root">
    <div class="top">
      <div class="top_content">
        <img src="/img.png" alt="" />
        <h1>Masuda Takumi</h1>
      </div>
    </div>
    <div class="skills">
      <h1>Skills</h1>
      <div class="lng">
        <h2>Language</h2>
        <p>HTML/CSS/Sass（A)</p>
        <p>JavaScript（B）</p>
        <p>TypeScript（C）</p>
        <p>Python（A）</p>
        <p>Go（C）</p>
      </div>
      <div class="fw">
        <h2>FrameWork</h2>
        <p>Vue.js/Nuxt.js（A)</p>
        <p>Express（B）</p>
        <p>Flask（A)</p>
        <p>Django（C)</p>
      </div>
    </div>
    <div class="links">
      <h1>Links</h1>
      <div class="link">
        <div class="link_button" @click="to('https://twitter.com/takumi_mas')">
          Twitter
        </div>
        <div
          class="link_button button_r"
          @click="to('https://github.com/takumimas')"
        >
          Github
        </div>
        <div
          class="link_button"
          @click="to('https://www.wantedly.com/id/takumimas')"
        >
          Wantedly
        </div>
        <div class="link_button button_r" @click="to('https://masublog.net/')">
          Blog
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Zen+Kaku+Gothic+Antique&display=swap:wght@800");
.top {
  width: 100vw;
  height: 100vh;
  background-image: url("/bg.png");
  background-size: cover;
}
.top_content {
  text-align: center;
  font-size: 3rem;
  color: white;
  padding-top: 200px;
  font-family: "Zen Kaku Gothic Antique", sans-serif;
}
.top_content img {
  width: 140px;
}
.skills {
  width: 100vw;
  min-height: 100vh;
  background-color: #0dbf9e;
  text-align: center;
  padding-top: 40px;
  padding-bottom: 40px;
}
.skills h1 {
  color: white;
  font-size: 2.5rem;
  font-family: "Zen Kaku Gothic Antique", sans-serif;
}
.lng {
  width: 400px;
  height: 270px;
  background-color: #f7b521;
  margin: auto;
  margin-top: 20px;
  color: white;
  padding: 10px 40px;
}
.lng h2 {
  font-family: "Zen Kaku Gothic Antique", sans-serif;
  font-size: 1.5rem;
}
.lng p {
  font-size: 1.2rem;
  margin-top: 10px;
  font-family: "Zen Kaku Gothic Antique", sans-serif;
  text-align: left;
}
.fw {
  width: 400px;
  height: 240px;
  background-color: #077bc5;
  margin: auto;
  margin-top: 20px;
  color: white;
  padding: 10px 40px;
}
.fw h2 {
  font-family: "Zen Kaku Gothic Antique", sans-serif;
  font-size: 1.5rem;
}
.fw p {
  font-size: 1.2rem;
  margin-top: 10px;
  font-family: "Zen Kaku Gothic Antique", sans-serif;
  text-align: left;
}
.links {
  width: 100vw;
  min-height: 100vh;
  text-align: center;
  background-color: #f7b521;
  margin: auto;
  color: white;
  padding: 30px 40px;
}
.links h1 {
  color: white;
  font-size: 2.5rem;
  font-family: "Zen Kaku Gothic Antique", sans-serif;
}
.link {
  width: 400px;
  height: 350px;
  margin: auto;
  margin-top: 40px;
  background-color: #0dbf9e;
  padding: 20px;
}
.link_button {
  width: 250px;
  height: 60px;
  background-color: #077bc5;
  margin: auto;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 15px;
  font-family: "Zen Kaku Gothic Antique", sans-serif;
}

.button_r {
  background-color: #d72678;
}
</style>

<script>
export default {
  methods: {
    to(link) {
      location.href = link;
    },
  },
};
</script>