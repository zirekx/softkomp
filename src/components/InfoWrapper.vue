<template>
   <div class="wrapper-info">
    <div class="about-us-container">
   <h2>Kim jesteśmy?</h2>
    <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc suscipit molestie egestas. 
        Donec nunc tortor, congue et enim vel, placerat faucibus turpis. 
        Duis et magna mattis, accumsan lorem vitae, porttitor sem. 
        Suspendisse scelerisque placerat neque sed pretium. 
        Maecenas consectetur erat libero, tempus bibendum eros cursus et. Aenean at sagittis dui. 
        Vestibulum consectetur non mauris et malesuada. Morbi dapibus mattis eros a elementum. 
        Pellentesque ullamcorper sit amet purus at viverra. Aliquam iaculis dolor vitae eros lobortis,
        in cursus massa egestas. Sed mollis pretium mauris, a eleifend leo. 
        Cras pharetra turpis ut tortor lacinia placerat. Curabitur ac venenatis felis. Mauris auctor,
        diam ut commodo aliquam, nisl erat placerat ipsum, vel hendrerit leo urna eget velit. 
        Donec pulvinar laoreet orci eu auctor. Nulla metus lacus, sagittis et malesuada sed, ornare at eros.
    </p>
    <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc suscipit molestie egestas. 
        Donec nunc tortor, congue et enim vel, placerat faucibus turpis. 
        Duis et magna mattis, accumsan lorem vitae, porttitor sem. 
        Suspendisse scelerisque placerat neque sed pretium. 
        Maecenas consectetur erat libero, tempus bibendum eros cursus et. Aenean at sagittis dui. 
        Vestibulum consectetur non mauris et malesuada. Morbi dapibus mattis eros a elementum. 
        Pellentesque ullamcorper sit amet purus at viverra. Aliquam iaculis dolor vitae eros lobortis,
        in cursus massa egestas. Sed mollis pretium mauris, a eleifend leo. 
        Cras pharetra turpis ut tortor lacinia placerat. Curabitur ac venenatis felis. Mauris auctor,
        diam ut commodo aliquam, nisl erat placerat ipsum, vel hendrerit leo urna eget velit. 
        Donec pulvinar laoreet orci eu auctor. Nulla metus lacus, sagittis et malesuada sed, ornare at eros.
    </p>
    <button>Więcej</button>
    </div>
    <div class="shorts-container">
    <div class="shorts">
        <i class="fa fa-solid fa-angle-right arrow"></i>
        <span class = "short-text">Księgowość</span>
    </div>
    <div class="shorts">
        <i class="fa fa-solid fa-angle-right arrow"></i>
        <span class = "short-text">Księgowość</span>
    </div>
    <div class="shorts">
        <i class="fa fa-solid fa-angle-right arrow"></i>
        <span class = "short-text">Księgowość</span>
    </div>
    <div class="shorts">
        <i class="fa fa-solid fa-angle-right arrow"></i>
        <span class = "short-text">Księgowość</span>
    </div>
    <div class="shorts">
        <i class="fa fa-solid fa-angle-right arrow"></i>
        <span class = "short-text">Księgowość</span>
    </div>
    <div class="shorts">
        <i class="fa fa-solid fa-angle-right arrow"></i>
        <span class = "short-text">Księgowość</span>
    </div>
    <div class="shorts">
        <i class="fa fa-solid fa-angle-right arrow"></i>
        <span class = "short-text">Księgowość</span>
    </div>
    </div>
    </div>
</template>
<script>
export default {
  name: "infowrapper",
};
</script>
<style scoped lang="scss">
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css");
$background: url("@/assets/about-us-background.jpg");

.wrapper-info{
    width:100vw;
    height:100vh;
    padding-left:5%;
    padding-right:5%;
    padding-top:5%;
    background-image: $background;
    background-repeat: no-repeat;
    background-size: 100% 100%;
}
.about-us-container{
    width:50%;
    text-align:left;
    padding:5em;
    color:White;
    float:left;
}
.shorts{
    width:100%;
    float:left;
    
}
.shorts-container{
    width:20%;
    float:left;
    padding:5em;
    
  position: relative;
  top: 40%;
  transform: translateY(-50%);
  
    
}
.about-us-container h2{
    font-family: "Raleway";
    font-size:3vw;
    padding-bottom:5%;
}
.about-us-container p{
    font-family:"Poppins";
    font-size:0.7vw;
    color:#c0c0c0;
    padding-bottom:3%;
}
button{
    float:left;
    width:40%;
    height:2.3vw;
    background-color:#13b76f;
    font-family:'Inter', sans-serif;
    color:White;
    border:0.1vw solid #13b76f;
    border-radius:0.15vw;
    font-size:0.7vw;
    margin-top:5%;
    margin-bottom:5%;
}
button:hover{
    cursor:pointer;
    background-color:white;
    color:black;
}
.arrow:before{
  font-family: "FontAwesome"; 
	font-weight: 400;
	content: "\f105";  
    color:#13b76f;
}
.arrow{
text-align: center;
display: inline;
font-size:0.8vw;
}
.short-text{
    width:70%;
    color:white;
    font-size:0.7vw;
    font-family:"Poppins";
    padding:1em;
    font-weight:700;
    text-transform:uppercase;
    text-align:center;
    cursor:pointer;
}

.shorts{
   padding:10%;
  position: relative;
}
.shorts span:after{
  content: '';
  position: absolute;
  width: 100%;
  transform: scaleX(0);
  height: 2px;
  bottom: 0;
  left: 0;
  background-color: #13b76f;
  transform-origin: bottom right;
  transition: transform 0.35s ease-out;
  
}
.shorts span:hover:after{
transform: scaleX(1);
  transform-origin: bottom left;
}
</style>