<script>
import { store } from '../store.js';

export default {
  data() {
    return {
      store,

      testimonials :[
        {
          "name":'Sophia Jones' ,
          "image":'../assets/img/courses-instructor-200x200.jpg',
        },

        {
          "name":'grant' ,
          "image":'../assets/img/testimonial-grant.png' ,
        },
   
        {
          "name": 'harold',
          "image": '../assets/img/testimonial-harold.png',
        },
     
        {
          "name": 'kate',
          "image": '../assets/img/testimonial-kate.png',
        },
       {
          "name": 'kelly',
          "image": '../assets/img/testimonial-kelly.png',
        },
      ],
      selectedTestimonial: null,
    selectedTestimonialIndex: null,
    };
    
  },
  methods: {
  changeTestimonial(index) {
    this.selectedTestimonial = this.testimonials[index];
    this.selectedTestimonialIndex = index;
  },
},

};
</script>

<template>
 <div class="third-container">
    <div class="testimonials-background-container">
      <div class="testimonials-container">
        <h3>Tesrimonials</h3>
        <p>Here's what our happy drivers had to say about our services:</p>
        <img v-if="selectedTestimonial" :src="selectedTestimonial.image" :alt="selectedTestimonial.name">
        <p>Avada Driving School really helped build my confidence behind the wheel and driving in general, and they got me a first time pass! <br>
        Highly recommended.</p>
        <h5 v-if="selectedTestimonial">{{ selectedTestimonial.name }}</h5>
        <div class="button-carousel">
          <button v-for="(testimonial, index) in testimonials" :key="index" @click="changeTestimonial(index)"></button>
        
        </div>
      </div>
    </div>
    <!-- latest news -->
    <div class="background-news">
      <div class="container-news">
        <h2>Latest News</h2>
        <div class="news">
          <div class="single-news">
            <img src="../assets/img/blog-choosecar-700x441.jpg" alt="">
            <h5 class="green-text">What Car to Start with?</h5>
            <h6>february 7th, 2019 | <span class="green-text">0 comments</span></h6>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
          </div>
          <div class="single-news">
            <img src="../assets/img/blogpost-10and2-700x441.jpg" alt="">
            <h5 class="green-text">Avada Driving School Expanding</h5>
            <h6>february 7th, 2019 | <span class="green-text">0 comments</span></h6>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
          </div>
        </div>
        <button>
          MORE FROM THE BLOG
        </button>
        <img class="triangles" src="../assets/img/latestnews-bottom-800x70.png" alt="">
      </div>
    </div>
    <!--  newsletter -->
    <div class="newsletter-background">
      <div class="newsletter">
        <h2>Sing up to our Newsletter</h2>
        <form action="">
          <input type="email" id="email" name="email"  required>
          <button type="submit" >SUBSCRIBE</button>
      </form>
      <p>(we do not share data whit anybody, and only use it for intended purpuse)</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.third-container{
  width: 100%;
  margin: 0 auto;
  z-index: 0;
  .testimonials-background-container{
    background-image: url(../assets/img/testimonial-background.jpg);
    .testimonials-container{
    padding-top: 80px;
    width: 60%;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    h3{
      font-size: 2.7rem;
      margin-bottom: 0;
    }
    p{
      color: #929AA3;
    }
    img{
      border-radius: 50%;
      height: 200px;
      width: 200px;
      margin-bottom: 30px;
    }
    h5{
      color: #929AA3;
      font-size: 1.2rem;
      font-weight: bold
    }
    
    .button-carousel {
    display: flex;
    
    button {
      margin: 0 10px 30px 10px;
      border-radius: 50%;
      height: 15px;
      width: 12px;
      background-color: transparent;
      border: 2px solid #929AA3;
      margin-bottom: 200px;
      
      &:hover {
        background-color: black;
        cursor: pointer;
      }
      
      &:active,
      &:focus {
        background-color: black;
      }
    }
  }
    }
  }
  /*news */
  .background-news{
    width: 100%;
    background-image: url(../assets/img/latestnews-background.jpg);
    height: 900px;
    background-position: center;
    .container-news{
      width: 60%;
      margin: 0 auto;
      background-color: white;
      position: relative;
      top: -30px;
      border-top: 5px solid #81A2B3;
      border-radius: 10px 10px 0 0;
      text-align: center;
      color: #929AA3;
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
      h2{
        color: black;
        font-size: 2rem;
        padding-top: 30px;
        padding-bottom: 20px;
      }
      .green-text{
        color: #7ABC64;
      }
      .green-text:hover{
        cursor: pointer;
      }
      h5{
        font-size: 1.4rem;
        margin: 10px 0 -10px 0;
      }
      h5:hover{
        cursor: pointer;
        text-decoration: underline;
      }
      .news{
        display: flex;
        justify-content: center;
        margin-bottom: 30px;
        .single-news{
          width: 40%;
          margin: 0 10px;
          img{
            width: 100%;
          }
        }
      }
      .triangles{
        width: 100%;
        position: relative;
        top: 102px;
      }
    }
  }
  /*newsletter */
  .newsletter-background{
    background-image: url(../assets/img/newsletter_background.jpg);
    width: 100%;
    background-size: cover;
    .newsletter{
      width: 70%;
      text-align: center;
      color:#929AA3 ;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      align-items: center;
      h2{
        font-size: 2.4rem;
        color: black;
        margin: 70px 0 50px 0;
      }
      input{
        width: 550px;
        display: block;
        margin: 0 auto 40px auto;
        padding: 10px 20px;
        border: 1px solid #929AA3;
      }
      button{
      height: 50px;
        padding: 0px 240px;
        background-color: #7ABC64;
        border-radius: 20px;
        color: white;
        border: 5px solid transparent;
        font-weight: bolder;
        margin-bottom: 30px;
      }
      button:hover{
        background-color: white;
        color:#7ABC64 ;
        padding: 0px 240px;
        border: 5px solid #7ABC64;
        cursor: pointer;
  }
  p{
    margin-bottom: 80px;
  }
    }
  }
}
</style>