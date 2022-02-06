<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import Icons from "./components/Icons.vue";
</script>

<template>
  <nav class="navbar">
    <div class="container">
      <div class="logo">Flexbox</div>
      <ul class="nav">
        <li>
          <a href="#">Home</a>
        </li>
        <li>
          <a href="#">About</a>
        </li>
        <li>
          <a href="#">Contact</a>
        </li>
      </ul>
    </div>
  </nav>
  <header class="header">
    <div class="container">
      <div>
        <h1>Flexbox Layout Module</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore, ex
          quas voluptas animi eveniet esse rerum quisquam ab nam error nesciunt
          deserunt voluptatem beatae iusto, delectus voluptate eum perspiciatis
          quidem.
        </p>
      </div>
      <div class="icons">
        <Icons />
        <Icons />
        <Icons />
        <Icons />
      </div>
    </div>
  </header>
  <section class="boxes">
    <div class="container">
      <div class="box">
        <h2><i class="fas fa-arrows-alt-v"></i>Aligment & Space</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis
          nihil obcaecati nisi cumque magnam eveniet quidem modi. Architecto
          culpa dolorum accusantium, obcaecati cum quo est mollitia magni
          exercitationem itaque consectetur!
        </p>
      </div>
      <div class="box">
        <h2><i class="fas fa-arrows-alt"></i>Tricky Positioning</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis
          nihil obcaecati nisi cumque magnam eveniet quidem modi. Architecto
          culpa dolorum accusantium, obcaecati cum quo est mollitia magni
          exercitationem itaque consectetur!
        </p>
      </div>
      <div class="box">
        <h2><i class="fas fa-mobile"></i>Responsive Design</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis
          nihil obcaecati nisi cumque magnam eveniet quidem modi. Architecto
          culpa dolorum accusantium, obcaecati cum quo est mollitia magni
          exercitationem itaque consectetur!
        </p>
      </div>
    </div>
  </section>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@700&family=Poppins:wght@400;700&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Poppins", sans-serif;
  font-size: 16px;
  line-height: 1.5;
  color: #333;
  background: #a1c3ff;
}

h1,
h2 {
  margin-bottom: 15px;
}

ul {
  list-style-type: none;
}

.container {
  max-width: 1000px;
  margin: 0 auto;
  padding: 0 30px;
}

.navbar {
  background: #3474e6;
  color: #fff;
  height: 60px;
}

.navbar .logo {
  font-size: x-large;
  font-weight: bold;
}

.navbar a {
  color: #fff;
  text-decoration: none;
  font-size: 18px;
  font-weight: bold;
}

.navbar a:hover {
  color: lightblue;
}

.navbar .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100%;
}

.navbar ul {
  display: flex;
}

.navbar ul li {
  margin-left: 20px;
}

.header {
  background-color: #0151cc;
  color: #fff;
  min-height: 400px;
}

.header h1 {
  font-size: 3rem;
  font-weight: bold;
  line-height: 1.2;
}

.header .icons {
  display: grid;
  grid-template-columns: 1fr 1fr;
  min-width: 300px;
}

svg path {
  fill: cyan; 
  opacity: 0.9;
}

.header .container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.boxes .container {
  display: flex;
  
}
</style>
