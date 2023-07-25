<script>
import { store } from '../store.js';

export default {
    name:"headerComponent",
  data() {
    return {
      store
    };
  },
  
  };
</script>

<template>
    

<div class="header-container">
    <div class="black-bar">
        <p>We have a 95% Successful Pass Rate!</p>
        <p><i class="fa-solid fa-phone-flip"></i> Give us a call to book yout tuition! <span>1-800-555-555</span></p>
    </div>
    <!-- fix bar -->
    <div class="fix-bar">
        <img src="../assets/img/avada-drivers-logo-2x-300x58.png" alt="AVADA DRIVING SCHOOL">
        <ul>
            <li ><a href="" class="active">HOME</a></li>
            <li><a href="">ABOUT</a></li>
            <li><a href="">PRICES</a></li>
            <li><a href="">COURSES</a><span>NEW</span></li>
            <li><a href="">LOCATION</a></li>
            <li><a href="">BLOG</a></li>
        </ul>
        <button type="button">BOOK NOW</button>
    </div>
    <div class="jumbotron">
        <div class="title">
            <h1>Drive with Avada</h1>
            <h5>We offer the finest driving tuition money can buy</h5>
        </div>
    </div>
    <div class="interactive-icon">
        <div><i class="fa-brands fa-algolia"></i></div>
        <h4>Demos</h4>
    </div>
    <div class="interactive-icon2">
        <div class="sale"><span >$</span>39</div>
        <h4>On sale</h4>
    </div>
</div>
</template>

<style lang="scss" scoped>
.black-bar{
    position: fixed;
    display: flex;
    justify-content: space-between;
    width: 70%;
    background-color: #353637;
    padding: 0 15%;
    color: rgb(168, 165, 165);
    z-index: 2;
    span:hover{
        text-decoration: underline;
        cursor: pointer;
    }
}
/*barra in position fix */
.fix-bar{
    z-index: 2;
    position: fixed;
    display: flex;
    padding: 30px 15%;
    margin-top: 50px;
    width: 70%;
    background-color: rgba(0, 0, 0, 0.4);
    color: white;
    align-items: center;
    
    img{
        padding-right: 30px;
    }

    ul{
        list-style: none;
        display: flex;
       
        li{
            display: flex;
            padding: 0 20px;
            font-weight: bolder;
            font-size: 1.2rem;
            align-items: center;
            font-weight: bolder;
            .active{
                color: #7ABC64;
                border-bottom: 2px solid #7ABC64;
            }
            span{
                margin-left: 10px;
                padding: 3px 5px;
                color: white;
                background-color: #7ABC64;
                border-radius: 5px;
                font-size: 0.8rem;
                margin-bottom: 10px;
            }
            span:hover{
                cursor: pointer;
            }
            a{
                color: white;
                text-decoration: none;
                padding-bottom: 10px;
            }
            a:hover{
                color:#7ABC64 ;
            }
        }
    }
    button{
        padding: 15px 35px;
        background-color: #7ABC64;
        border-radius: 30px;
        color: white;
        border: transparent;
        margin-left: 50px;
        margin-bottom:10px ;
    
    }
    button:hover{
        background-color: white;
        color:#7ABC64 ;
        padding: 10px 30px;
        border: 5px solid #7ABC64;
        cursor: pointer;
    }
}
/*jumbotron*/
.jumbotron{
    background-image: url(../assets/img/homepage-hero-background.jpg);
    height: 800px;
    max-width: 100%;
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    .title{
        position: relative;
        color: white;
        top: 45%;
        left: 20%;
        width: 800px;
        h1{
            font-size: 80px;
            padding: 0;
            margin: 0;
        }
        h5{
            font-size: 30px;
            padding: 0;
            margin: 0;
            font-weight: lighter;
        }
    }
}
.interactive-icon, .interactive-icon2{
    position: fixed;
    background-color: white;
    height: 65px;
    width: 65px;
    text-align: center;
    border-radius: 10px;
    z-index: 5;
    div{
        height: 60%;
        font-size: 1.8rem;
        padding: 3px;
    }
    h4{
        margin: 0;
        color: gr;
    }
    .sale{
        color:#7ABC64 ;
        span{
        font-size: 1.0rem;
        position: relative;
        top: -10px;
        }
    }
   
}
.interactive-icon{
    right: 20px;
    top: 160px;
}
.interactive-icon2{
    right: 20px;
    top: 260px;
}
.interactive-icon:hover,.interactive-icon2:hover{
        cursor: pointer;
        color: white;
        background-color: black;
    }
</style>