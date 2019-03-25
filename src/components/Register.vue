<template>
<div class="limitClass" align="center">
    <div   class="BorderClass">
         <img height="125" weight="125" style="border-radius:40px" src="https://i.pinimg.com/736x/ab/d0/1d/abd01dddab053fe07194bae291c44434--copy.jpg" >
         <title>Register</title>
        <h1 style="font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;">Register</h1>
        <div class="userClass" >
            <br>
            <form v-on:submit.prevent="registerUser">
    
                <br>
                <input type="text"  class="inputClass" v-model="user.name" placeholder="UserName" >
                <br>
                <input type="password"  class="inputClass" v-model="user.password" placeholder="Password"  >
                <br>
                 <input type="password"  class="inputClass" v-model="user.confirmpassword" placeholder="ConfirmPassword"  >
                <br>
                <button type="submit" class="butClass" v-on:submit.prevent="registerUser"> Register</button>
            
            </form>
        </div>
    </div>
</div>
</template>

<script>
export default {
    data(){
        return{
            user:{
            }
        }
    },
    methods:{
       registerUser(){
         console.log("UserName:" + this.user.name + " Password: " + this.user.password );
            var fileText = new Blob([this.user.name + " " + this.user.password], { type: "application/json" });
             var textURL = window.URL.createObjectURL(fileText);
             var downloadLink = document.createElement("a");
            downloadLink.download = "myJson.json";
            downloadLink.innerHTML = "";
            downloadLink.href = textURL;
            document.body.appendChild(downloadLink);
            downloadLink.click();
           this.user={}
        }
    }
}
</script>

<style >
    body{
        background-image: url("http://www.fondosni.com/images/2011-12-04/lindo%20paisaje%20en%20blanco%20y%20negro-547130.jpg");
        background-repeat: no-repeat;
        
    }
    .BorderClass{
    height: 550px;
   width: 500px;
  border-radius: 20px;
  overflow: hidden;
  padding: 55px 55px 37px 55px;
    text-align: center;
    background: #9152f8;
  background: -webkit-linear-gradient(top,#4e4e4e4e, #E4E4E4);
  background: -o-linear-gradient(top, #4e4e4e4e, #E4E4E4);
  background: -moz-linear-gradient(top, #4e4e4e4e, #E4E4E4);
  background: linear-gradient(top, #4e4e4e4e, #E4E4E4);
}

.limitClass{
    content: "";
  display: block;
  position: absolute;
  z-index: -5;
  width: 100%;
  height: 100%;
  top: 60px;
  left: 0;
}

h1{
    text-shadow: 5px;
    font-size: 40px;
    
}

.inputClass{
    font-family: comic;
    color: #333333;
    line-height: 1.2;
    font-size: 18px;
    display: block;
    width: 100%;
    background: transparent;
    height: 60px;
    padding: 0 20px;
    padding: 1px 0px;
        padding: 1px;
    border-width: 2px;
    border-radius: 10px;
}

img{
    border-image: 20px;
}

.butClass{
background-color:whitesmoke;
    border-radius: 70px;
    color:black;
    padding: 15px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    position: relative;
    top: 10px;
    left: 0 px;
    background-color: #4e4e4e4e;    
    
}

b{
        font-style: comic;
        display: inline;
    font-size: 20px;
    color: #555555;
    line-height: 1.5;
    padding-left: 26px;
}
input::-webkit-input-placeholder {
    color:black;
    font-weight: bold;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    
    
}
input::-moz-placeholder {
    color: black;
    font-weight: bold;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}
h1{
    color:black;
    font-family: comic;
}
</style>
 