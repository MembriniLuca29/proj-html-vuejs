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
      <div><img src="../assets/img/courses-passplus-200x200.jpg" alt="">
      <h5>Pass Plus</h5>
      <button class="learn-more-button">LEARN MORE</button>
    </div>
      <div><img src="../assets/img/course-intensive-200x200.jpg" alt="">
      <h5>Intensive Course</h5>
      <button class="learn-more-button">LEARN MORE</button>
    </div>
      <div><img src="../assets/img/courses-instructor-200x200.jpg" alt="">
      <h5>Instructor</h5>
      <button class="learn-more-button">LEARN MORE</button>
    </div>
    </div>
  </div>
  <!-- zona dati -->
  <div class="data-container">
    <div class="rate-container">
      <div class="hidden"><div class="grey-ball"></div></div>
      <div class="radius-95">
        
        <h2>95%</h2></div>
      <h4>PASS RATE</h4>
    </div>
    <div class="rate-container">
      <div class="radius-100"><h2>100%</h2></div>
      <h4>REFERRAL RATE</h4>
    </div>
    <div class="rate-container">
      <div class="radius-0">
        <div class="green-ball"></div>
        <h2>0%</h2></div>
      <h4>ACCIDENT RATE</h4>
    </div>
  </div>

  <!-- istructors -->
  <div class="instructor-container">
    <h3>Your Instructor</h3>
    <div class="instructor-info">
      <p>Lorem, ipsum sit amet consectetur adipisicing elit. Deserunt fugit ratione blanditiis quibusdam neque aspernatur eaque molestias, atque a illum.</p>
      <button>MORE ABOUT US</button>
    </div>
    <div class="data-container">
      <div class="info-instructor-container">
        <div><img src="../assets/img/instructor-mikehart-400x254.jpg" alt=""></div>
        <h5>Mike Hart</h5>
        <p><i class="fa-brands fa-facebook"></i><i class="fa-brands fa-twitter"></i><i class="fa-brands fa-instagram"></i><br>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Autem, inventore?</p>
      </div>
      <div class="info-instructor-container bigger">
        <div><img src="../assets/img/instructor-johnsmith-400x254.jpg" alt=""></div>
        <h5>John Smith</h5>
        <p><i class="fa-brands fa-facebook"></i><i class="fa-brands fa-twitter"></i><i class="fa-brands fa-instagram"></i><br>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Autem, inventore?</p>
      </div>
      <div class="info-instructor-container">
        <div><img src="../assets/img/instructor-angelahart-400x254.jpg" alt=""></div>
        <h5>Angela Hart</h5>
        <p><i class="fa-brands fa-facebook"></i><i class="fa-brands fa-twitter"></i><i class="fa-brands fa-instagram"></i><br>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Autem, inventore?</p>
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
  top: -250px;
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
    left: 140px;
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
  
  }
  .type-course{
      display: flex;
      width: 50%;
      div{
        width:calc((100% / 3) - 80px);
        margin: 80px 10px 0 10px;
        text-align: center;
        h5{
          color: #929AA3 ;
          font-size: 1.6rem;
          text-align: center;
          margin: 20px;
        }
        h5:hover{
          color: black;
        }
        button{
        background-color: white;
        color:#929AA3 ;
        padding: 10px 30px;
        border: 5px solid #929AA3;
        cursor: pointer;
        border-radius: 20px;
        }
        button:hover{
          color: black;
          border:5px solid black;
        }
      }
    }
}
/* zona dati*/
.data-container {
  width: 70%;
  margin: 0 auto;
  padding-top: 30px;
  display: flex;
  max-height: 617px;

  .rate-container {
    margin: 80px auto;
    border-top: 6px solid #7ABC64;
    border-radius: 20px;
    padding: 50px;
    background-color: white;
    box-shadow: 0px 15px 8px rgba(0, 0, 0, 0.1);

    div {
      width: 220px;
      text-align: center;
      border-radius: 50%;
      border: 10px solid #7ABC64;
      height: 220px;
      font-size: 3rem;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #929AA3;
    }
    h4{
      text-align: center;
      padding-top: 20px;
      color: #929AA3;
    }
    .radius-0 {
      border-color:#bec5cc;
      .green-ball{
        position: absolute;
        width: 18px;
        height: 10px;
        border-radius: 40%;
        top: 816px;
        border: none;
        background-color: #7ABC64;
      }
      }
      .hidden{
        position: absolute;
        .grey-ball{
        position: absolute;
      width: 220px;
      height: 220px;
      overflow: hidden;
      border-radius: 50%;
      border: 10px solid #bec5cc;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #929AA3;
      z-index: 2;
      clip-path: polygon(0 0, 60% 0, 0 20%);; 
      }
    }
  
  }
}
/*istruttori */
.instructor-container{
  text-align: center;
  width: 100%;
  margin: 100px auto;
  h3{
    font-size: 3rem;
  }
  .instructor-info{
    display: flex;
    align-items: center;
    p{
      width: 40%;
      font-size: 1.4rem;
      line-height: 30px;
      text-align: left;
      margin-left: 320px;
      margin-right: 150px;
      color: #929AA3;
    }

    button{
      height: 50px;
        padding: 0px 80px;
        background-color: #7ABC64;
        border-radius: 20px;
        color: white;
        border: 5px solid transparent;
        font-weight: bolder;
      }
      button:hover{
        background-color: white;
        color:#7ABC64 ;
        padding: 0px 80px;
        border: 5px solid #7ABC64;
        cursor: pointer;
  }
 
  }
  .info-instructor-container {
    width: 25%;
    margin: 80px auto;
    border-top: 6px solid #7ABC64;
    border-radius: 20px;
    padding: 20px 25px 30px 25px ;
    background-color: white;
    box-shadow: 0px 15px 8px rgba(0, 0, 0, 0.1);
    z-index: 1;

    div {
      text-align: center;
      height: 250px;
      font-size: 3rem;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #929AA3;
      justify-content: center;
      img{
        width: 80%;
      }
    }
      h5{
          margin: 0;
          font-size: 2rem;
        }
      i{
        padding: 0 10px 20px 10px;
        color: #929AA3;
    }
    p{
      color: #929AA3;
    }
  }
  .bigger{
    width: 28%;
   height: 430px;
  }
}
}
</style>