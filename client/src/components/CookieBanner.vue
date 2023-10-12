<template>
  <div class="cookie-wrapper">
    <p>Dev and its partners use cookies and similar technologies to provide you with a better experience</p>
    <p>By accepting all cookies, you agree to our use of cookies to deliver and maintain our services and site, improve the quality of dev</p>
    <div class="cookie-actions">
      <button @click="accept()">Accept all</button>
      <button @click="deny()">Deny non-essential</button>
    </div>
  </div>
</template>

<script setup>
import {ref} from 'vue'

function accept(){
  console.log('accepting cookies')
}

function deny(){
  console.log('denying cookies')
}

</script>

<style scoped>

.cookie-wrapper{
  position: absolute;
  bottom: 0px;
  left: 50%;
  transform: translateX(-50%);
  height: fit-content;
  width: 100%;
  box-shadow: 0px 2px 10px grey;
  border-radius: 10px;
  padding: 15px 0px;
  margin: 0;
}

.cookie-actions{
}

button{
  background-color: rgb(129, 169, 253);
  color: rgb(247, 247, 247);
  margin: 0px 5px;
}

</style>