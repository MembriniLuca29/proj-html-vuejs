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
</div>
</template>

<style lang="scss" scoped>
.black-bar{
    display: flex;
    justify-content: space-between;
    width: 70%;
    background-color: #353637;
    padding: 0 15%;
    color: rgb(168, 165, 165);
    span:hover{
        text-decoration: underline;
        cursor: pointer;
    }
}
/*barra in position fix */
.fix-bar{
    position: fixed;
    display: flex;
    padding: 30px 15%;
    
    width: 70%;
    background-color: rgba(0, 0, 0, 0.7);
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
        font-weight: bold;
        font-weight: 900;
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
</style>