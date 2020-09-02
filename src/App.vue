<template>
  <div id="app">
   <Main/>
  </div>
</template>

<script>
import Main from './components/Main.vue'

export default {
  name: 'App',
  components: {
    Main
  }
}
</script>

<style>
* {
    margin: 0;
    padding: 0;
   }
body {
  top: 0;
  left: 0;
  margin: 0 auto;
  padding: 0;
  font-family: 'Merriweather Sans', sans-serif;
}
.grids {
  display: grid;
  grid-template-columns: 1fr 1fr;
  background: url(./assets/QhXoJnF.jpg) ; 
  background-size: cover;
  height: 100vh;
}
.main-body {
   
  text-align: center;
  margin-top: 200px;
}
.main-body h1 {
  color: #ffffff;
  font-weight: bold;
  font-size: 65px;
}
.main-body h3 {
  font-size: 30px;
  background-color: #ffffff;
  background-image: linear-gradient(45deg, #60ff75, #136c0a, #002b12);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent; 
  -moz-background-clip: text;
  -moz-text-fill-color: transparent;
}
.main-body-links {
margin-top: 20px;
}
.main-body .main-body-links a{
  text-decoration: none;
  margin: 30px;
  font-size: 20px;
  color: #136c0a;
  font-weight: bold;

}
.main-body .main-body-image img {
  width: 100%;
}
.main-body-image {
 
margin-top: 10%;

}
.main-body .main-body-links a:hover{
  text-decoration-line: underline;
 }
   @media only screen and (max-width: 850px) {  
    .grids {
      grid-template-columns: 1fr;
    }
    .main-body {
      margin-top: 50px;
    }
    .main-body-image {
      text-align: center;
      justify-self: center;
      width: 70%;
    margin-top: 30px;

}
  } 
</style>
