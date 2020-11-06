<template>
  <div id="app" class="container">
      <Menu />
      <Main />  
      <About />
      <Services />
      <Portfolio />
      <Contact />   
  </div>
</template>

<script>
import Menu from './components/Menu.vue'
import Main from './components/Main.vue'
import About from './components/About.vue'
import Services from './components/Services.vue'
import Portfolio from './components/Portfolio.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    Menu,
    Main,
    About,
    Services,
    Portfolio,
    Contact
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Blinker&display=swap');

html {
    scroll-behavior: smooth;
  }
  
  body {
    margin: 0;
    padding: 0;
    position: relative;
    -webkit-font-smoothing: antialiased;
    overflow: hidden;
    background-color:#161616;
    font-family: 'Blinker', sans-serif;
  }
  
  h1 {
    font-size: 60px;
    color: #e23a6e;
    margin-bottom: 10px;
    text-shadow: 0px 1px 1px #000;
  }
  
  p {
    color: rgba(255, 255, 255, 0.8);
  }
  
  .navbar {
    position: fixed;
    bottom: 0;
    border-top: 2px solid #161616;
    background: #202020;
    width: 100vw;
    height: 50px;
    z-index: 100;
  }
  
  .nav-links {
    display: flex;
    justify-content: space-around;
    height: 40px;
    align-items: center;
  }
  
  a {
    text-decoration: none;
    color: #F27121;
    font-weight:bold;
    font-size: 18px;
    position: relative;
    height: 50px;
    width: 150px;
    flex-basis: 150px;
    flex-grow: 1;
    text-align: center;
    padding-top: 17px;
    box-sizing: border-box;
  }

  .lead{
      font-size: 24px;
      line-height:32px;
  }
  
  a:hover,
  a:active,
  a:focus {
    background: #F27121;
    color:#202020;
  }
  
  .section {
    background: #161616;
    position: relative;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .top-deco {
    width: 300px;
    height: 150px;
    background: #8A2387;  /* fallback for old browsers */
    background: -webkit-linear-gradient(to right, #F27121, #E94057, #8A2387);  
    background: linear-gradient(to right, #F27121, #E94057, #8A2387);
    position: absolute;
    top: -10px;
    clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
    transform: rotate(180deg);
  }

  .deco-1{
      display:none;
  }
  
  .section:nth-child(odd) {
    background: #8A2387;  /* fallback for old browsers */
    background: -webkit-linear-gradient(to right, #F27121, #E94057, #8A2387); 
    background: linear-gradient(to right, #F27121, #E94057, #8A2387);
  }
  
  .section:nth-child(odd) .top-deco {
    background: #161616;
  }
  
  .section:nth-child(odd) h1 {
    color: #fff;
  }
  
  .section:nth-child(odd) p {
    color: rgba(255, 255, 255, 0.8);
  }
  
  .section:nth-child(odd) .icon {
    color: #fa96b5;
  }
  
  .center {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
  }
  
  .icon {
    font-size: 55px;
    color: #fff;
    position: absolute;
    top: 36%;
    left: 41%;
    transform: rotate(180deg);
  }
  
  .fa-smile {
    font-size: 60px;
  }
  
  .three .icon {
    left: 42%;
  }
  
  .five .icon {
    left: 38%;
  }

  .one img{
      width:720px;
      margin-bottom: 20px;
  }
  
</style>
