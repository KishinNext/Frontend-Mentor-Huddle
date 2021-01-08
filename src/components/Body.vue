<template>
  <article>
      <div class="left">
          <img src="..\images\illustration-mockups.svg" alt="vcv">
      </div>
      <div class="right">
            <h1>Build The Community <br> Your Fans Will Love</h1>
            <p>Huddle re-imagines the way we biuld communities. You have a voice
                , bur so does your audience. Create connections with toyur users as you engage in geniune discussion.
            </p>
            <div class="button"><router-link to="/" class="router">Register</router-link></div>
      </div>
  </article>
</template>

<script>
import { gsap } from "gsap";
export default {
    mounted:function(){
        var tl = gsap.timeline({ defaults: {duration: 1} } );
        tl.from('.left',{ease:"power2.out", opacity:0})
        tl.from('.right',{ease:"power2.out", y:-200, opacity:0})
        tl.from('.button',{ease:"bounce.out", y:-200, opacity:0})
    }
}
</script>

<style>
@media only screen and (min-width: 0px){
    article{ 
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }
    article .left img{
        height: 40%;
        position: relative;
        margin: 3em;
        width: 100%;
    }
    article .right{
        margin-left: 3em;
        margin-top: 1.5em;
        position: relative;
        color: white;
        display: flex;
        flex-direction: column;
        align-items: center;
     
    }
    article .right h1{
        font-family: 'Poppins', sans-serif;
        letter-spacing: 0px;
        font-size: 2em;
        text-align: center;
    }
    article .right p{
        font-family: 'Open Sans', sans-serif;
        letter-spacing: 0.2px;
        font-size: medium;
        text-align: center;
    }


    .button{
        border-radius: 2em;
        width: 11em;
        height: 3em;
        border: 0;
        outline: none;
        padding: 0;
        box-shadow: 1px 1px 10px #000000;
        background-color: white;
        margin-top: 2em;
        
    }

    .button:active{
        border-radius: 2em;
        width: 11em;
        height: 3em;
        border: 0;
        outline:none;
        box-shadow: 1px 1px 10px #000000;
        background-color: #E980E7;
        transition: 0.1s linear;
    }


    .button .router{
        position: absolute; 
        border-radius: 2em;
        border: 0;
        padding: 0.7em;
        width: 8em;
        text-decoration: none;
        color: #674BB1;;
        font-family: 'Poppins', sans-serif;
        font-size: 1.2em;
        text-align: center;
        letter-spacing: 0.2px;
    }

    .button .router:active{

        position: absolute; 
        border-radius: 2em;
        border: 0;
        padding: 0.7em;
        width: 8em;
        text-decoration: none;
        color: white;
        font-family: 'Poppins', sans-serif;
        font-size: 1.2em;
        text-align: center;
        letter-spacing: 0.2px;  
    }

}

@media only screen and (min-width: 768px){
    article{
        margin-top: 3em;
        margin-left: 3.8em;
        margin-right: 3.1em;
        margin-bottom: 0em;
        padding: 0;   
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        
    }
    article .left img{
        height: 33em;
        margin: 0;
        width: auto;
        position: relative;
    }
    article .right{
        margin-left: 3em;
        margin-top: 1.5em;
        position: relative;
        color: white;
        align-items: flex-start;
     
    }
    article .right h1{
        font-family: 'Poppins', sans-serif;
        letter-spacing: 0px;
        font-size: 2em;
        text-align: left;
    }
    article .right p{
        font-family: 'Open Sans', sans-serif;
        letter-spacing: 0.2px;
        font-size: medium;
        text-align: left;
    }


    .button{
        border-radius: 2em;
        width: 11em;
        height: 3em;
        border: 0;
        outline: none;
        padding: 0;
        box-shadow: 1px 1px 10px #000000;
        background-color: white;
        margin-top: 2em;
        
    }

    .button:active{
        border-radius: 2em;
        width: 11em;
        height: 3em;
        border: 0;
        outline:none;
        box-shadow: 1px 1px 10px #000000;
        background-color: #E980E7;
        transition: 0.1s linear;
    }


    .button .router{
        position: absolute; 
        border-radius: 2em;
        border: 0;
        padding: 0.7em;
        width: 8em;
        text-decoration: none;
        color: #674BB1;;
        font-family: 'Poppins', sans-serif;
        font-size: 1.2em;
        text-align: center;
        letter-spacing: 0.2px;
    }

    .button .router:active{

        position: absolute; 
        border-radius: 2em;
        border: 0;
        padding: 0.7em;
        width: 8em;
        text-decoration: none;
        color: white;
        font-family: 'Poppins', sans-serif;
        font-size: 1.2em;
        text-align: center;
        letter-spacing: 0.2px;  
    }
}
</style>