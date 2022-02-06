<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import TheIcon from "./components/TheIcon.vue";
import TheMenu from "./components/TheMenu.vue";
</script>

<template>
  <nav class="navbar">
    <div class="container">
      <div class="logo">Flexbox</div>
      <div class="menu">
        <TheMenu />
      </div>
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
          Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Exercitationem aliquid tempore numquam ratione alias eum optio quam
          dolor distinctio minima?
        </p>
      </div>
      <div class="icons">
        <TheIcon />
        <TheIcon />
        <TheIcon />
        <TheIcon />
      </div>
    </div>
  </header>
  <section class="boxes">
    <div class="container">
      <div class="box">
        <h2><i class="fas fa-arrows-alt-v"></i>Aligment & Space</h2>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Facere,
          reiciendis.
        </p>
      </div>
      <div class="box">
        <h2><i class="fas fa-arrows-alt"></i>Tricky Positioning</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit, id.
        </p>
      </div>
      <div class="box">
        <h2><i class="fas fa-mobile-alt"></i>Responsive Design</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quia, iure.
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
  display: flex;
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
  margin: 20px 0;
}

.header .icons svg path {
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
  justify-content: space-between;
}

.box {
  flex: 1;
  background: #0851cc;
  color: #fff;
  border-radius: 10px;
  margin: 20px 10px;
  box-shadow: 0 3px 5px rgba(0, 0, 0, 0.6);
  padding: 15px 20px;
}

.box i {
  margin-right: 10px;
}

.menu {
  display: none;
  width: 30px;
  cursor: pointer;
}

@media (max-width: 768px) {
  .header .container {
    flex-direction: column;
    padding-top: 20px;
    text-align: center;
  }

  .boxes .container {
    display: block;
    text-align: center;
  }

  .navbar ul {
    display: none;
  }

  .navbar .menu {
    display: block;
  }
}
</style>
