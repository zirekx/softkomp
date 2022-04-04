<template>
  <div class="header">
    
    <img class = "nav-logo" src = "https://www.soft-komp.pl/wp-content/uploads/2021/10/logo_260.png" loading="lazy" alt = "Logo">

    <nav class="navbar">
      <ul class="main-menu">
        <li class="nav_menu-item"><p>Oferta</p></li>
        <li class="nav_menu-item"><p>Strony WWWW</p></li>
        <li class="nav_menu-item"><p>O nas</p></li>
        <li class="nav_menu-item"><p>Aktualizacje</p></li>
      </ul>
      <div class="hamburger">
                <span class="bar"></span>
                <span class="bar"></span>
                <span class="bar"></span>
            </div>
    </nav>
    <img class="aeroadmin-download" src= "https://www.soft-komp.pl/wp-content/uploads/2021/10/aeroadmin_logo.png" loading="lazy" alt = "Aeroadmin">
    
  </div>
</template>

<script>
export default {
  name: "header",
};
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Anonymous+Pro:wght@700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Anonymous+Pro:wght@700&family=Raleway:wght@100&display=swap');

.header{
  background-color:#07111a;
  padding-right:5%;
  padding-left: 5%;
  color:white;
  width:100%;
  max-height:80px;
  padding-top:1%;
  padding-bottom:1%;
  display:flex;
  align-items:center;
  position:fixed;
  top:0;
  margin:0;
  box-sizing: border-box;
  z-index: 2;

  
}
.aeroadmin-download{
width:10%;
float:right;
}
ul{
  list-style-type: none;
  margin: 0;
  padding: 0;
  
  
  
}
li{
  float:left;
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-transform:uppercase;
  font-family: 'Raleway', sans-serif;
  font-size:14px;
  font-weight:800;
  
}
.nav-logo{
  width:10%;
  float:left;
}
.navbar{
  width:50%;
  margin: 0 auto;

}
.nav_menu-item{
   display: inline-block;
  position: relative;
  cursor:pointer;
}
.nav_menu-item p:after{
  content: '';
  position: absolute;
  width: 100%;
  transform: scaleX(0);
  height: 2px;
  bottom: 0;
  left: 0;
  background-color: #13b76f;
  transform-origin: bottom right;
  transition: transform 0.25s ease-out;
  
}
.nav_menu-item p:hover:after{
transform: scaleX(1);
  transform-origin: bottom left;
}
</style>
<style scoped>
@media screen and (max-width: 1200px) {
  li {
     font-size: 1vw;;
  }
}



</style>