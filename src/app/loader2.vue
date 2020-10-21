<template>


    <div class="loader">

   
 
<img src="../assets/logos/long_logo.svg" alt="">
    
  
    <div class="half-circle"></div>
    <!-- <div class="line1"></div> -->
    <div class="half-circle2"></div>
      <!-- <div class="di1" "></div> -->
      <!-- <div class="di2"></div>  -->
    <div class="half-circle3"></div>



<div class="text">
      <span>Almost done..</span> <br>
    <span>Please wait, while we prepare the dashboard for you.</span>
</div>

   

</div>












  
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@900&display=swap");
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    display: block;
}
.text
{
  position: absolute;
  margin-top: 200px;
}
.text span

{
    display: block;
  font-family: "Roboto", sans-serif;
  font-size: 22px;
  color: rgb(105, 105, 105);



}
img 
{
  background: black;
  padding: 10px;
  margin-top:-300px;
  border-radius: 5px;

}
.loader
{
width: 100%;
position: fixed;
top: 0;
left: 0;
width: 100%;
height: 100vh;
background: rgb(255, 255, 255);
display: flex;
text-align: center;
align-items: center;
justify-content: center;

}

.line1
{
    width: 15px ;
    height: 10px;
    position: absolute;
    background:#d46204;
    border-radius: 20px;
    margin-top: 38px;
    
    
}
.di1,.di2
{
    height: 10px;
    width: 10px; 
    height: 10px;
    position: absolute;
    background:#d46204;
    border-radius: 20px; 

}
.di1 
{
    margin-top: -133px;
    margin-left: -35px;
     transform-origin: 20px 45px;
    -webkit-animation: spin 3s linear infinite;
    animation: spin1 3s round infinite;
    
}
.di2 
{
    margin-top: -85px;
    margin-left: 80px; 
}



.half-circle {
    height:100px;
    width: 50px;
    position: absolute;
    border-radius: 50px 0 0 50px;
    border-top: 10px solid#0055ff00;
    border-left: 10px solid #0055ff;
    border-bottom: 10px solid #0055ff;
    transform: rotate(-118deg);
    z-index: 2;
    
    margin-top: -50px;
     margin-left: -50px;
    transform-origin: 50px 50px;
    -webkit-animation: spin 3s linear infinite;
    animation: spin1 3s round infinite;
   
    
}



.half-circle:before,.half-circle:after{
    content: "";
    width: 5px;
    height: 10px;
    position: absolute;
    left: 7px;
    top: 2px;
    background:  #0055ff;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
    transform:  rotate(-45deg); 

  
}

.half-circle:after{
  bottom:2px;
  top: 80px;
  left: 39px;
  transform:  rotate(0deg); 

}




.half-circle2 
{
    height:100px;
    width: 50px;
    position: absolute;
    border-radius: 50px 0 0 50px;
    border-top: 10px solid #1b801b00;
    border-left: 10px solid #d46204;
    
    border-bottom: 10px solid  #1b801b00;
    
   
    margin-top: -50px;
    margin-left: -50px;
    z-index: 1;
    
    transform-origin: 50px 50px;
    -webkit-animation: spainSection 3s linear infinite;
    animation: spainSection 3s round infinite;
   
  
}

.half-circle2:before,.half-circle2:after{
    content: "";
    width: 5px;
    height: 10px;
    position: absolute;
    left: 17%;
    top: 2px;
    background:  #d46204;

    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
    transform:  rotate(-45deg); 
}
.half-circle2:after{
  bottom:2px;
  top: inherit;
  transform:  rotate(45deg); 
  left: 17%;

}








.half-circle3
{
    height:100px;
    width: 50px;
    position: absolute;
    border-radius: 50px 0 0 50px;
    border-top: 10px solid#ba540000;
    border-left: 10px solid #ba540000;
    border-bottom: 10px solid #d46204;
   
    margin-top: -50px;
    margin-left: -50px;


    transform-origin: 50px 50px;
    -webkit-animation: animationround 3s linear infinite;
    animation: animationround 3s round infinite;
   
      
}



.half-circle3:before,.half-circle3:after{
    content: "";
    width: 5px;
    height: 10px;
    position: absolute;
    left: 40px;
    top: 80px;
    background: #d46204;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
    transform:  rotate(0deg); 
}
.half-circle3:after{
  bottom:2px;
  top:65px;
  transform:  rotate(-135deg); 
  left: 10%;

}






/* circle 1  */

@-webkit-keyframes spin {
    0%   {
        -webkit-transform: rotate(0deg);
        -ms-transform: rotate(0deg);
        transform: rotate(0deg);
    }

    20%   {
        -webkit-transform: rotate(288deg);
        -ms-transform: rotate(288deg);
        transform: rotate(deg);
    }

    40%   {
        -webkit-transform: rotate(72deg);
        -ms-transform: rotate(72deg);
        transform: rotate(72deg);
    }
    60%   {
        -webkit-transform: rotate(216deg);
        -ms-transform: rotate(216deg);
        transform: rotate(216deg);
    }
    80% {
        -webkit-transform: rotate(288deg);
        -ms-transform: rotate(288deg);
        transform: rotate(288deg);
    }
    100% {
        -webkit-transform: rotate(360deg);
        -ms-transform: rotate(360deg);
        transform: rotate(360deg);
    }
}
@keyframes spin {
    0%   {
        -webkit-transform: rotate(0deg);
        -ms-transform: rotate(0deg);
        transform: rotate(0deg);
    }

    50%   {
        -webkit-transform: rotate(180deg);
        -ms-transform: rotate(180deg);
        transform: rotate(180deg);
    }

    /* 40%   {
        -webkit-transform: rotate(144deg);
        -ms-transform: rotate(144deg);
        transform: rotate(144deg);
    }
    60%   {
        -webkit-transform: rotate(216deg);
        -ms-transform: rotate(216deg);
        transform: rotate(216deg);
    }
    80% {
        -webkit-transform: rotate(288deg);
        -ms-transform: rotate(288deg);
        transform: rotate(288deg);
    } */
    100% {
        -webkit-transform: rotate(360deg);
        -ms-transform: rotate(360deg);
        transform: rotate(360deg);
    }
}


/* circle 2  */





@-webkit-keyframes spainSection {
    0%   {
        -webkit-transform: rotate(72deg);
        -ms-transform: rotate(72deg);
        transform: rotate(72deg);
    }

    20%   {
        -webkit-transform: rotate(144deg);
        -ms-transform: rotate(144deg);
        transform: rotate(144deg);
    } 

     40%   {
        -webkit-transform: rotate(216deg);
        -ms-transform: rotate(216deg);
        transform: rotate(216deg);
    }
    60%   {
        -webkit-transform: rotate(288deg);
        -ms-transform: rotate(288deg);
        transform: rotate(288deg);
    }
    80% {
        -webkit-transform: rotate(360deg);
        -ms-transform: rotate(360deg);
        transform: rotate(360deg);
    }
    100% {
        -webkit-transform: rotate(0deg);
        -ms-transform: rotate(0deg);
        transform: rotate(0deg);
    }
}
@keyframes spainSection {
    0%   {
        -webkit-transform: rotate(0deg);
        -ms-transform: rotate(0deg);
        transform: rotate(0deg);
    }

    20%   {
        -webkit-transform: rotate(-72deg);
        -ms-transform: rotate(-72deg);
        transform: rotate(-72deg);
    }

    40%   {
        -webkit-transform: rotate(-144deg);
        -ms-transform: rotate(-144deg);
        transform: rotate(-144deg);
    }
    60%   {
        -webkit-transform: rotate(-216deg);
        -ms-transform: rotate(-216deg);
        transform: rotate(-216deg);
    }
    80% {
        -webkit-transform: rotate(-288deg);
        -ms-transform: rotate(-288deg);
        transform: rotate(-288deg);
    }
    100% {
        -webkit-transform: rotate(-360deg);
        -ms-transform: rotate(-360deg);
        transform: rotate(-360deg);
    }
}



/* circle 3  */





@-webkit-keyframes animationround {
    0%   {
        -webkit-transform: rotate(0deg);
        -ms-transform: rotate(0deg);
        transform: rotate(0deg);
    }

    20%   {
        -webkit-transform: rotate(72deg);
        -ms-transform: rotate(72deg);
        transform: rotate(72deg);
    }

    40%   {
        -webkit-transform: rotate(144deg);
        -ms-transform: rotate(144deg);
        transform: rotate(144deg);
    }
    60%   {
        -webkit-transform: rotate(216deg);
        -ms-transform: rotate(216deg);
        transform: rotate(216deg);
    }
    80% {
        -webkit-transform: rotate(288deg);
        -ms-transform: rotate(288deg);
        transform: rotate(288deg);
    }
    100% {
        -webkit-transform: rotate(360deg);
        -ms-transform: rotate(360deg);
        transform: rotate(360deg);
    }
}
@keyframes animationround {
    0%   {
        -webkit-transform: rotate(0deg);
        -ms-transform: rotate(0deg);
        transform: rotate(0deg);
    }

    20%   {
        -webkit-transform: rotate(-72deg);
        -ms-transform: rotate(-72deg);
        transform: rotate(-72deg);
    }

    40%   {
        -webkit-transform: rotate(-144deg);
        -ms-transform: rotate(-144deg);
        transform: rotate(-144deg);
    }
    60%   {
        -webkit-transform: rotate(-216deg);
        -ms-transform: rotate(-216deg);
        transform: rotate(-216deg);
    }
    80% {
        -webkit-transform: rotate(-288deg);
        -ms-transform: rotate(-288deg);
        transform: rotate(-288deg);
    }
    100% {
        -webkit-transform: rotate(-360deg);
        -ms-transform: rotate(-360deg);
        transform: rotate(-360deg);
    }
}



</style>







