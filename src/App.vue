<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html, body {
  width: 100vw;
  height: 100vh;

  font-family: 'Roboto', sans-serif;
}

:root {
  --white: #f6f6f6;
  --dark: #333333;
  --blue-light: rgba(45, 116, 213, 1);
  --blue: rgba(11, 27, 103, 0.98);
  --green: #398087;
  
  --bordered: solid 1px rgba(255, 255, 255, 0.5);
  --color-transparent: rgba(255, 255, 255, 0.1);
}

#app {
  width: 100%;
  height: 100%;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  gap: 3px;
  background: var(--dark);
}

.btn {
  width: 40px;
  height: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
  
  font-weight: 600;
  color: var(--white);
  border: var(--bordered);
  background: var(--color-transparent);
  border-radius: 3px;
  transition: all 0.3s;
}

.btn:active {
  transition: all 0.3s;
  background: rgba(255,255,255, 0.5);
}

</style>
