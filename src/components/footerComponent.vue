<script>
export default {
  name: 'footerComponent'
}

</script>

<template>
  <footer>
    <p> &copy; 2022 </p>
    <img class="logo" src="../assets/Logo.png" alt="">
    <p> All Rights Reserved</p>   
  </footer>
</template>

<style scoped>

footer{
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 0.3em;
  align-items: center;
  background: #000000;
  max-width: 84.3rem;
  width: 100%;
  height: 4.5em;
  text-align: center;
  
}
footer p {
  font-family: 'Helvetica Neue';
  font-style: normal;
  font-weight: 500;
  font-size: 0.9rem;
  color: #6A6A6A;
}
.logo {
    height: 1.1rem;
    margin-top: -0.4em;
}
nav a {
  
  line-height: 2.3em;
}
@media screen and (max-width:768px) {
  footer {
    width: 48rem;
  }
}
</style>
