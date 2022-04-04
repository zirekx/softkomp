<template>
    <div class="offer-list">
        <div class="left_panel-offer">
            <ul class="c-links" >
              <li class="btn--corners">
                <a href="#" data-number="WWW">Strony</a>
              </li>
            </ul>
            <p class="heading-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut efficitur cursus massa, vel varius nisl porttitor sed. 
              Pellentesque quis est sagittis, facilisis justo vitae, posuere ante. 
              Proin risus orci, tristique luctus rutrum eu, commodo quis sapien. 
              Donec et lectus nisl. Sed laoreet pulvinar ultricies. 
              Donec imperdiet lectus quis ante sollicitudin, id scelerisque lorem tristique. 
              Phasellus nibh nunc, venenatis vitae tincidunt ac, pharetra quis nibh. 
              Phasellus sodales tempus neque eget auctor. 
            </p>
          <div class="user-info">
            <div class="avatar-user-info">
              <div class="page">
                <div class="page__container">
                    <div class="page__demo">
                      <a href="#0" class="mask mask_type2 mask_type2-a2 page__tile">
                        <img src="https://images.unsplash.com/photo-1569466896818-335b1bedfcce?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=80" class="mask__img" alt="The avatar of Stas Melnikov">
                      </a>
                    </div>   
                    <span class="page__caption">Wojtek</span>    
                </div>
             </div>
             <span class="proffesion-user-info">Fullstack Web Developer <br /> Seo Specialist <br />  IT Specialist</span>
            </div>
            <div class="quote-container-user-info">
              <p class="quote-user-info">“Google only loves you when everyone else loves you first.”</p>
            </div>
          </div>
        </div>
        
        <div class="right_panel-offer">
          <div class = "row">
            <div class = "column"><div class="bb"><img width="50px" class="bb-popup" src="@/assets/redirect-icon.png" /><img class="img-offer" src = "//blog.codepen.io/wp-content/uploads/2012/06/Button-White-Large.png" /></div><p> Tworzenie i Projektowanie Stron WWW </p> </div>
            <div class = "column"><div class="bb"><img class="img-offer" src = "//blog.codepen.io/wp-content/uploads/2012/06/Button-White-Large.png" /></div><p> Pozycjonowanie SEO </p> </div>
            <div class = "column"> <div class="bb"><img class="img-offer" src = "//blog.codepen.io/wp-content/uploads/2012/06/Button-White-Large.png" /></div><p> Optymalizacja stron WWW </p></div>
          </div>
          <div class = "row">
            <div class = "column"><div class="bb"><img class="img-offer" src = "//blog.codepen.io/wp-content/uploads/2012/06/Button-White-Large.png" /></div><p> Hosting WWW </p> </div>
            <div class = "column"><div class="bb"><img class="img-offer" src = "//blog.codepen.io/wp-content/uploads/2012/06/Button-White-Large.png" /></div><p> Sklepy E-Commerce </p></div>
            <div class = "column"> <div class="bb"><img class="img-offer" src = "//blog.codepen.io/wp-content/uploads/2012/06/Button-White-Large.png" /></div><p> Social Mediami </p></div>
          </div>
        </div>
        
    </div>

</template>


<script>
export default {
  name: "offers",
};

</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Delius+Swash+Caps&display=swap');
.offer-list{
  
    width:100vw;
    height:100vh;
    padding-left:5%;
    padding-right:5%;
    padding-top:10%;
    
    
}
.left_panel-offer{
    width:25%;   
    float:left;
    background-color:#0e1111;
    
}
.right_panel-offer{
    width:75%;
    float:left;
    padding-left:5%;
}
.column {
  float: left;
  width: 33.33%;
  
}
.row{
  margin-bottom:5%;
}
.row:after {
  content: "";
  display: table;
  clear: both;
}
.column {
  float: left;
  color:White;
  
}
@media screen and (max-width: 600px) {
  .column {
    width: 100%;
  }
}

.left, .right {
  width: 25%;
}

.middle {
  width: 50%;
}
.heading-text{
  padding-top:5%;
  width:100%;
  float:left;
  color:#c0c0c0;
  font-family: 'Poppins', sans-serif;
  font-size:0.7vw;
  text-align:center;
}

.avatar-user-info{
   float:left;
   width:30%;
}
.proffesion-user-info{
width:100%;
float:left;
text-align:center;
font-family: 'Poppins', sans-serif;
color:White;
font-size:0.55em;
}
.quote-container-user-info{

float:left;
  width:70%;
  height:300px;
  padding-left:5%;
  overflow: hidden; 
  
}
.quote-user-info{
  
  position: relative;
  top: 40%;
  -webkit-transform: translateY(-50%);
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
  color:white;
  font-size:1.1vw;
  font-family: 'Delius Swash Caps', cursive;
}

.column p{
  width:100%;
  text-align:center;
  font-family: 'Poppins', sans-serif;
  padding-top:3%;
  color:White;
  font-size:0.8vw;
  
}






</style>
<style scoped lang="scss">
$bg-color: #0e1111;
$accent-color: #13b76f;
@mixin v-h-center {
  
  
  
}
.o-title--primary {
  font-size: 3em;
  font-family: 'Poppins', sans-serif;
  font-weight: 400;
  text-align: center;
  color: white;
  @include v-h-center;
  margin-top: -1.5em;
}

.c-links {
  margin: 0;
  padding: 0;
  text-align: center;
  @include v-h-center;
  
}

$border-width: 0.15vw;
$padding-width: 3px;
$corner-size: 2.4vw;

.btn--corners {
  position: relative;
  display: inline-block;
  margin: 0;
  padding: $padding-width;
  font-size: 3vw;
  text-align: center;
  vertical-align: top;
  font-weight: 400;
  border: $border-width solid $accent-color;
}

.btn--corners:not(:last-child) {
  margin-right: 2px;
}

.btn--corners::before,
.btn--corners::after {
  content: "";
  position: absolute;
  background-color: $bg-color;
  z-index: 0;
  transition: 200ms ease-in;
  transform-origin: center center;
}

.c-links:target .btn--corners::before,
.c-links:target .btn--corners::after {
  background-color: rgba(0, 0, 0, 0.6);
  transition-duration: 600ms;
}

.btn--corners::before {
  width: calc(100% + #{$border-width} * 2 - #{$corner-size});
  height: calc(100% + #{$border-width} * 2);
  top: -$border-width;
  left: 50%;
  transform: translateX(-50%);
}

.btn--corners::after {
  height: calc(100% + #{$border-width} * 2 - #{$corner-size});
  width: calc(100% + #{$border-width} * 2);
  left: -$border-width;
  top: 50%;
  transform: translateY(-50%);
}

.btn--corners:hover::before {
  width: 0;
}

.btn--corners:hover::after {
  height: 0;
}

.btn--corners a {
  position: relative;
  display: inline-block;
  color: white;
  text-transform: uppercase;
  text-decoration: none;
  line-height: 1em;
  font-size: 0.7em;
  font-family: 'Raleway', sans-serif;
  font-weight:500;
  padding: 5px 20px;
  margin: 0 2px;
  z-index: 1;
}

.btn--corners a::after {
  content: attr(data-number);
  display: block;
  font-family: Lora;
  font-style: italic;
}

.btn--primary {
  background: $accent-color;
  color: #979c9c;
  padding: 10px 40px;
  text-decoration: none;
  @include v-h-center;
  margin-top: 6em;
}

</style>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Play:wght@700&display=swap');


.mask{
  --uiMaskClipPath: var(--maskClipPath);

  box-sizing: var(--maskBoxSizing, border-box);
  display: var(--maskDisplay, inline-flex);
  padding: var(--maskStrokeThickness, 3px);
  clip-path: var(--uiMaskClipPath);
  background-color: var(--maskStrokeColor, currentColor);
}

.mask__img{
  max-width: 100%;
  display: block;
  clip-path: var(--uiMaskClipPath);
}

.mask, 
.mask__img{
  transition: clip-path var(--maskAnimationDuration, .2s) var(--maskAnimationTimingFunction, ease-out);
}



.mask_type1{
  --maskClipPath: polygon(0 10%, 10% 0, 90% 0, 100% 10%, 100% 90%, 90% 100%, 10% 100%, 0 90%);
}

.mask_type2{
  --maskClipPath: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
}

.mask_type3{
  --maskClipPath: polygon(0 10%, 10% 10%, 10% 0, 90% 0, 90% 10%, 100% 10%, 100% 90%, 90% 90%, 90% 100%, 10% 100%, 10% 90%, 0 90%);
}

.mask_type4{
  --maskClipPath: polygon(0 50%, 50% 0, 100% 50%, 50% 100%);
}



.mask_type1-a1{
  --maskAnimationDuration: .4s;
}

.mask_type1:hover, 
.mask_type1:focus{
  --maskClipPath: polygon(0 0, 100% 0, 100% 10%, 100% 100%, 90% 100%, 0% 100%, 0% 90%, 0% 10%);
}



.mask_type2-a1{
  --maskAnimationDuration: .4s;
}

.mask_type2:hover, 
.mask_type2:focus{
  --maskClipPath: polygon(100% 0, 100% 50%, 100% 100%, 0 100%, 0% 50%, 0 0);
}



.mask_type3-a1{
  --maskAnimationDuration: .5s
}

.mask_type3:hover, 
.mask_type3:focus{
  --maskClipPath: polygon(90% 0, 100% 0, 100% 10%, 100% 90%, 100% 100%, 90% 100%, 10% 100%, 0 100%, 0 90%, 0 10%, 0 0, 10% 0);
}


.mask_type4:hover, 
.mask_type4:focus{
  --maskClipPath: polygon(0 0, 100% 0, 100% 100%, 0 100%);
}



.mask_type1-a2{
  --maskAnimationDuration: .5s;
}

.mask_type1-a2:hover, 
.mask_type1-a2:focus{
  --maskClipPath: polygon(0 0, 90% 0, 100% 0, 100% 90%, 100% 100%, 10% 100%, 0 100%, 0 10%); 
}



.mask_type2-a2{
  --maskAnimationDuration: .9s;
  --maskAnimationTimingFunction: cubic-bezier(1, 0.18, 0, 1.14);
}



.mask{
  --maskStrokeColor: #13b76f;
  --maskStrokeThickness: 0.1vw;
  width:10vw;
  height:10vw;
}



.page{
  height:100%;
  box-sizing: border-box;
  width: 30%;
  padding: 1.5rem;
  margin: auto;  
  text-align: center;
  justify-content: center;
  display: grid; 
  grid-gap: 3rem; 
  grid-template-columns: repeat(auto-fit, 15rem);
}

.page__caption{
  display: inline-block; 
  padding: .5rem 2rem;
  border:1px solid #13b76f;
  font-family: 'Play', sans-serif;
  font-weight:400;
  
  font-size: 1rem; 
  color: white; 
  text-transform: uppercase;
  margin-top:5%;
}

.page__demo{ 
  margin-top: 1.5rem; 
  width:100%;
}

.page__tile{ 
  width: 9rem; 
  height: 9rem; 
}
.page__container{
  width:100%;
}

</style>
<style scoped lang="scss">
$anime-time: 8s;

$box-size: 200px;
$clip-distance: .05;
$clip-size: $box-size * (1 + $clip-distance * 2);
$path-width: 2px;

$main-color: #13b76f;

$codepen-logo-path: url('//blog.codepen.io/wp-content/uploads/2012/06/Button-White-Large.png');

%full-fill {
  
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
}

.bb {
  position: relative;
  width: 10.3vw;
  height: 10.3vw;
  margin: auto;
  color: $main-color;
  box-shadow: inset 0 0 0 1px rgba($main-color, .5);
  text-align: center;

}
.img-offer{
  max-width:8vw;
  
   position: absolute;
   left: 50%;
   top: 50%;
   transform: translate(-50%, -50%);
   opacity:1;
    transition:opacity 3s; 
  
}
.bb-popup{
  visibility:hidden;
  opacity : 0; transition:opacity 1s; 
}
.bb:hover .bb-popup{
visibility:visible;
opacity : 1;
}
.bb:hover .img-offer{
  visibility:hidden;
  opacity:0;
}
/////


</style>