<template>
  <div class="app">
    <Header />
    <main>
      <router-view />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";

export default {
  components: {
    Header,
    Footer,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  list-style: none;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
  color: #345;
}
body {
  background: url("./assets/pattern.svg");
}
img {
  max-lines: 100%;
  display: block;
}
.btn {
  display: block;
  padding: 10px 30px;
  background: #87f;
  border-radius: 4px;
  color: #fff;
  text-align: center;
  font-size: 1rem;
  box-shadow: 0 4px 8px rgba(30, 60, 90, 0.2);
  transition: all 0.3s;
  cursor: pointer;
}
.btn:hover {
  background-attachment: #65d;
  transform: scale(1.1);
}
.app {
  display: flex;
  min-height: 100vh;
  flex-flow: column;
}
main {
  flex: 1;
}
</style>
