<script>
import { store } from '../store.js';

export default {
    name:"footerComponent",
  data() {
    return {
      store
    };
  },
  
  };
</script>

<template>
<div class="main-footer-background">
  <div class="section-footer-container">
    <div class="section-footer lower">
      <img src="../assets/img/avada-drivers-logo-2x-300x58.png" alt="">
      <p>Avada Driving school is the right choice for experienced drivers looking for a refresher course, or the brand new driver wanting to pass first time.</p>
    </div>
    <div class="section-footer">
      <h4>CONTACT DETAILS</h4>
      <div class="info-detail">
        <p><i class="fa-solid fa-house-chimney"></i> 12345 North main street, <br>
        <span class="space">New York, NY 555555</span></p>
        <p><i class="fa-solid fa-phone-flip"></i> 1.800.555.6789</p>
        <p><i class="fa-solid fa-envelope"></i> info@your-domain.com</p>
        <p><i class="fa-solid fa-link"></i> Theme-fusion.com</p>
      </div>
    </div>
    <div class="section-footer">
      <h4>COURSES</h4>
      <div>
        <h3 class="green-text"><i class="fa-solid fa-circle-arrow-right green-text"></i> Pass Plus</h3>
        <h3 class="green-text"><i class="fa-solid fa-circle-arrow-right green-text"></i> Intensive Course</h3>
        <h3 class="green-text"><i class="fa-solid fa-circle-arrow-right green-text"></i> Automatic</h3>
        <h3 class="green-text"><i class="fa-solid fa-circle-arrow-right green-text"></i> Instructor Training</h3>
      </div>
    </div>
    <div class="section-footer">
      <div class="grid-img"><img  src="../assets/img/footer-ad-grid-400x357.png" alt=""></div>
      <button>BOOK NOW</button>
    </div>
</div>
</div>
<div class="info-footer">
  <p>© Copyright 2012 - 2020| Avada Theme by <span class="green-text">ThemeFusion </span> | All Rights Reserved | Powered by <span class="green-text">WorldPress</span></p>
  <p><i class="fa-brands fa-facebook"></i><i class="fa-brands fa-twitter"></i><i class="fa-brands fa-youtube"></i><i class="fa-brands fa-instagram"></i></p>
</div>
</template>

<style lang="scss" scoped>
.main-footer-background{
  background-image: url(../assets/img/footer-background-color.jpg);
.section-footer-container{
  padding: 50px;
  width: 70%;
  display: flex;
  justify-content: space-evenly;
  margin: 0 auto;
  color: #929AA3;

  .lower{
    margin-top: 40px;
    
  }
  .section-footer{
    width: calc(100% / 4);
    padding: 20px 10px;
    line-height: 30px;
    margin-left: 70px;
    h4{
      color: white;
      font-size: 1.5rem;
    }
    .space{
      margin-left: 40px;
    }
    i{
      margin-right: 10px;
      font-size: 1.4rem;
      color:#F6F6F6 ;
    }
    .green-text{
      color: #7ABC64;
    }
   
    .grid-img{
      height: 300px;
      width: 100%;
      background-image: url(../assets/img/footer-ad-grid.png);
      
    }
    button{
      height: 50px;
        padding: 0px 30px;
        background-color: #7ABC64;
        border-radius: 20px;
        color: white;
        border: 5px solid transparent;
        font-weight: bolder;
      }
      button:hover{
        background-color: white;
        color:#7ABC64 ;
        padding: 0px 30px;
        border: 5px solid #7ABC64;
        cursor: pointer;
  }
  }
}

}
.info-footer{
  position: relative;
  
  background-color: #494C4E;
  width: 100%;
  height: 100px;
  color: white;
  display: flex;
  justify-content: space-evenly;
  p{
    padding-top: 20px;
    color: #929AA3;
  i{
    padding: 0 5px;
    color: white;
  }
  i:hover{
    cursor: pointer;
    color: blue;
  }
  .green-text{
    color: #7ABC64;
  }
}
}
</style>