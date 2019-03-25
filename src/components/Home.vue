<template>
    <div>
        <img  class="logoClass2" src="https://media.istockphoto.com/vectors/music-record-studio-black-and-white-logo-template-with-sound-retro-vector-id1034907326">
        <img class="logoClass" src="https://i.pinimg.com/736x/ab/d0/1d/abd01dddab053fe07194bae291c44434--copy.jpg">
        <div class="borderClass">
            <h1>Welcome to Life Sound</h1>
            <h2>where your heart dances</h2>
            <router-link class="inClass1" tag="li" to="/Register">Sing up now</router-link>
            <router-link class="inClass2" tag="li" to="/Login" >Login</router-link>
            <div class="muestra1">
                <img class="img1" height="350" width="350" src="https://images.pexels.com/photos/114820/pexels-photo-114820.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940">
                
                <img class="img2" height="350" width="350" src="https://images.pexels.com/photos/416831/pexels-photo-416831.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style>
 body{
     background-image: url("https://i.pinimg.com/originals/92/4b/ff/924bffc69c0b12c535b1553bab1bc205.jpg");
    
 }

 .logoClass{
     height: 100px;
     width: 100px;
     opacity: 0.85;
     top:200px;
     position:absolute; 
     top: 4px;
     right: 10px;
     border-radius: 50px;
 }
  .logoClass2{
     height: 100px;
     width: 100px;
     opacity: 0.85;
     top:200px;
     position:absolute; 
     top: 4px;
     right: 1410px;
     border-radius: 50px;
 }
 h1 {
     position: absolute;
     color:white;
     bottom: 400px;
    right: 500px;
    font-size: 50px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    border-color: black;
    border-radius: 20px;
 }
  h2 {
     position: absolute;
     color:white;
     bottom: 370px;
    right: 590px;
    font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 30px;
    border-color: black;
 }
 .inClass2{
     position: absolute;
    color:white;
    bottom: 320px;
    right: 550px;
    font-size: 20px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    border-color: black;
      border-radius: 20px;
    list-style:none;
        border: 10px solid salmon;
    background-color: salmon;
 }
 .inClass1{
    position: absolute;
    color:white;
    bottom: 320px;
    right: 900px;
    font-size: 20px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    border-radius: 20px;
    list-style:none;
    border: 8px solid salmon;
    background-color: salmon;
 }
 .img1{
     position: absolute;
     bottom: -250px;
     right: 1000px;
  border-radius: 10px;
  overflow: hidden;
  padding: 20px 15px 15px 20px;
    text-align: center;
   background-color: white;
   justify-content: center;
  align-items: center;
 }
 .img2{
          position: absolute;
     bottom: -250px;
     right: 200px;
  border-radius: 10px;
  overflow: hidden;
  padding: 20px 15px 15px 20px;
    text-align: center;
   background-color: white;
   justify-content: center;
  align-items: center;
 }

</style>
