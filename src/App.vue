<template>
  <!-- <div id="nav">
    <router-link to="/">Home</router-link>
  </div> -->

  <router-view/>
</template>



<style>


@media only screen and (min-width: 100px){
    body{
    background-image: url('./images/bg-mobile.svg')  ;
    background-color: #674BB1; 
    background-repeat: no-repeat;
    background-size: cover;
    margin: 0;
    padding: 0;

    }
}
@media only screen and (min-width: 768px) {
  body{

    background-image: url('./images/bg-desktop.svg')  ;
    background-color: #674BB1;  
    background-repeat: no-repeat;
    background-size: inherit;
    margin: 0;
    padding: 0;

  }
}


</style>
