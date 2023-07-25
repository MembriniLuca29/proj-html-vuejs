<script>
import { store } from '../store.js';

export default {
  data() {
    return {
      store
    };
  },
  
  };
</script>

<template>
  <div class="big-container">
<div class="start-learning horizzontal">
  <div >
    <h2>
      Start Learning to Drive Today
    </h2>
    <h6>Give us a call to schedule your first driving lesson </h6>
  </div>
  <div><p ><i class="fa-solid fa-phone-flip"></i>  <span class="phone">1-800-555-555</span></p></div>
</div>
<div class="invisible-backgorund">
  <img src="../assets/img/promise-background.jpg" alt="" >
  <img src="../assets/img/latestnews-bottom-800x70.png" alt=""  class="triangle">
</div>
<div class="course-container">
  <div class="courses">
    <div class="corner">
      <span class="text">NEW</span>
    </div>
      <h2>Courses</h2>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elitesentium voluptatum iusto voluptatem fugit, quas illum. Ratione q</p>
      <button>COURSE INFORMATION</button>
    </div>
    <div class="type-course">
      <div><img src="" alt="">
      <h5>Pass Plus</h5>
      <button class="learn-more-button">LEARN MORE</button>
    </div>
      <div><img src="" alt="">
      <h5></h5>
      <button class="learn-more-button">LEARN MORE</button>
    </div>
      <div><img src="" alt="">
      <h5></h5>
      <button class="learn-more-button">LEARN MORE</button>
    </div>
    </div>
  </div>
</div>
</template>

<style lang="scss" scoped>

.big-container{
  position: relative;
  .horizzontal{
  background-image: url(../assets/img/horizontal-cta-background.jpg);
  width: 100%;
  height: 250px;
  background-position: center;
  display: flex;
  justify-content: space-around;
  align-items: center;
  font-size: 2rem;
  color: white;
  background-size: cover;
  div{
    margin: 0 10%;
    h2{
      margin: 10px 0;
    }
    h6{
      margin: 0;
      font-size: 1.3rem;
    }
  }
  i{
    padding-right: 15px;
  }
  .phone:hover{
    cursor: pointer;
    text-decoration: underline;
  }
}
/*sfondo semitrasparente */
.invisible-backgorund {
  position: absolute;
  width: 100%;
  top: -200px;
  z-index: -1;
  img{
    width: 100%;
    max-height: 1100px;
    object-fit: contain;
  }
  .triangle{
  position: relative;
  top: -10px;
    filter: invert(9%);
  }

  /*zona corsi */
 
}
.course-container{
    width: 100%;
    display: flex;
    justify-content: space-around;
    
    .courses {
    text-align: center;
    width: 400px;
    height: 400px;
    background-color: white;
    border-radius: 20px;
    position: relative;
    top: -30px;
    align-items: center;

    .corner {
      position: absolute;
      rotate: 270deg;
      top: 0;
      left: 0;
      width: 0;
      height: 0;
      border-radius: 0 20px 0 0;
      border-style: solid;
      border-width: 0px 80px 80px 0px;
      border-color: transparent #7ABC64  transparent #7ABC64;

      .text {
        color: white;
        font-weight: bold;
        transform: rotate(45deg);
        position: absolute;
        top: 20px;
        left: 35px;
      }
    }
    h2{
      font-size: 2.5rem;
      padding-top: 15px;
    }
    p{
      font-size: 1.3rem;
      color: rgb(168, 165, 165) ;
      padding: 10px 30px;
      line-height: 35px
    }
    button{
        padding: 10px 30px;
        background-color: #7ABC64;
        border-radius: 20px;
        color: white;
        border: 5px solid transparent;
        font-weight: bolder;
      }
      button:hover{
        background-color: white;
        color:#7ABC64 ;
        padding: 10px 30px;
        border: 5px solid #7ABC64;
        cursor: pointer;
  }
    .type-course{
      display: flex;
      width: 40%;
    }
  }
}
}
</style>