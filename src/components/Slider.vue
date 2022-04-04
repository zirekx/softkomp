<template>
<div id="slider">
    <div class="slider-text-zone"> 
        <span class="above-heading-title">Lorem Ipsum</span>
        <h2>Example Title</h2>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit.
            Lorem ipsum dolor sit amet, consectetur adipiscing elit.
            Lorem ipsum dolor sit amet, consectetur adipiscing elit.
        </p>
        <button>Oferta</button>
        <div class="slider-link-container">
            <span class="slider-link-1">Facebook</span>
            <span class="slider-link-separator">/</span>
            <span class="slider-link-2">Instagram</span>
            <span class="slider-link-separator">/</span>
            <span class="slider-link-3">Twitter</span>
            
        </div>
        <div class="expierience-slider-heading">
            <span class="number-heading-slider">9</span>
            <span class="title-heading-slider">Lat doświadczenia</span>
        </div>
        <div class="expierience-slider-heading">
            <span class="number-heading-slider">50</span>
            <span class="title-heading-slider">Zadowolonych klientów</span>
        </div>
    </div>
    <div class="slider-image-spot">
        <img src="@/assets/banner-image.jpeg">
    
    </div>

    <div class="slider-navigation-panel">
<div class="sbn sbn01">
		
		<ul>
			<li><a class="is-active" href="#">1</a></li>
			<li><a href="#">2</a></li>
			<li><a href="#">3</a></li>
			<li><a href="#">4</a></li>
			<li><a href="#">5</a></li>
		</ul>
</div>
  <img class="arrowDown" :src="arrowDown" />
    </div>
</div>    



</template>

<script>

export default {
  name: "slider",
  data(){
    return {
      sliderCircle: require('@/assets/circle.svg'),
      arrowDown: require('@/assets/arrow-down.svg')
    }
  }
  
};

//FontAwesome


</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@800&display=swap');
</style>
<style scoped>


#slider{
    padding-top:10%;
    padding-right:5%;
    padding-left: 5%;
    margin-top:4.19%;
    height:100vh;
    width:auto;
    background: #C04848;  /* fallback for old browsers */
    background: linear-gradient(rgb(7, 17, 26), rgb(0, 0, 0,0.8)), url("@/assets/banner-image.jpeg");  /* Chrome 10-25, Safari 5.1-6 */
    background: linear-gradient(rgb(7, 17, 26), rgb(0, 0, 0,0.7)), url("@/assets/banner-image.jpeg"); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
    background-size: cover;
    max-width:100%;
overflow:auto;
}
.slider-image-spot img{
    width:100%;
    height:100%;
}

.slider-text-zone{
    float:left;
    max-width:20%;
    margin-left:15%;
}
.slider-image-spot{
    max-width:40%;
    float:left;
    padding-left:10%;
}
.slider-navigation-panel{
    float:right;
    max-width:1%;
    position: relative;
    height:100%;  
    top: 50%;
    -webkit-transform: translateY(-50%);
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
}
.above-heading-title{
    width:100%;
    float:left;
    color:#13b76f;
    font-family: 'Inter', sans-serif;
    text-transform:uppercase;
    font-weight:Bold;
    font-size:0.5vw;
    letter-spacing:2px;
}
h2{
    width:100%;
    float:left;
    color:White;
    font-family: 'Raleway', sans-serif;
    font-size:2.5vw;
    font-weight:bold;
}
p{
    max-width:80%;
    float:left;
    color:#c0c0c0;
;
    font-family: 'Poppins', sans-serif;
    font-size:0.7vw;
    margin-top:5%;
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
    transform:scale(0.95);
    background-color:White;
    color:black;
    border:1px solid black;
    cursor:pointer;

}


.slider-link-container{
    width:100%;
    float:left;
}
.slider-link-container span{
    padding:0.2vw;
    font-family: 'Poppins', sans-serif;
    color:#c0c0c0;
    font-size:0.65vw;
    font-weight:600;

}
.expierience-slider-heading{
    margin-top:5%;
    width:50%;
    float:left;
}
.number-heading-slider{
    width:100%;
    float:left;
    
    color:white;
    font-family:'Inter', sans-serif;
    font-size:3vw;
}
.title-heading-slider{
    width:100%;
    float:left;
    color:White;
    font-family: 'Poppins', sans-serif;
    font-size:0.7vw;
}
.slider-navigation-panel svg {


}
</style>
<style scoped lang="scss">
.sbn {
	width: 47.5%;
	height: 280px;
	padding-top: 80px;
	border-top: 1px solid #fff;
	box-sizing: border-box;
}
.sbn:nth-of-type(odd) {
	float: left;
}
.sbn:nth-of-type(even) {
	float: right;
}
.sbn:nth-of-type(1),
.sbn:nth-of-type(2) {
	height: 200px;
	padding-top: 0;
	border-top: none;
}
.sbn p {
	font-size: 20px;
	margin-bottom: 40px;
}

@media screen and (max-width: 800px) {
	.sbn-list {
		margin: 80px 40px 0;
	}
	.sbn {
		width: auto;
		float: none !important;
	}
	.sbn:nth-of-type(2) {
		height: 280px;
		padding-top: 80px;
		border-top: 1px solid #13b76f;
	}
	ul li {
		margin: 0 .7em !important;
	}
	.sbn13 ul li {
		width: 26px;
		margin: 0 .6em !important;
	}
}


ul {
	list-style: none;
	text-align: center;
}
ul li {
	display: inline-block;
	margin: 0 1em;
}
ul li a {
	display: inline-block;
	width:0.7vw;
	height: 0.7vw ;
	font-size: 0;
	text-indent: 100%;
	white-space: nowrap;
	overflow: hidden;
	outline: none;
	box-sizing: border-box;
	transition: .2s ease-in-out;
}


.sbn01 ul li a {
	border: 2px solid #13b76f;
	border-radius: 50%;
}
.sbn01 ul li a:hover,
.sbn01 ul li a.is-active {
	background-color: #13b76f;
}


.sbn02 ul li a {
	border: 2px solid #fff;
	border-radius: 50%;
}

.arrowDown{
filter: invert(99%) sepia(4%) saturate(0%) hue-rotate(52deg) brightness(113%) contrast(100%);
width:3vw;

}

</style>

