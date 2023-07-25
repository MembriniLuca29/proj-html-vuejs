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
<div class="container">
  <div>
    <h2>Get Behind The Wheel</h2>
    <h4>e culum molestias, accusamus laudantium dolorem quod! Delectus repellat dolore temporibus laboriosam?</h4>
    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et cupiditate dignissimos corporis assumenda, nihil consequuntur ut porro. Adipisci aliquam vero assumenda inventore quaerat reiciendis earum aliquid dolor. Obcaecati, quibusdam voluptatibus.
    Nihil quibusdam, blanditiis odit qui minus tenetur nemo debitis, earum incidunt dolor enim rerum, temporibus iste ipsum! Eveniet, corporis. Temporibus quis esse sit cupiditate sequi officia perferendis officiis repudiandae minima.
    </p>
  </div>
  <div class="firstform">
    <h3 class="text-green">First Lesson Free!</h3>
    <p>When you make a block booking whit us your first  lesson is included free.</p>
    <form action="">
      <input type="text" placeholder="Your name*" class="input-icon" required>
      <input type="email" id="email" name="email" placeholder="Email*" required>
      <input type="tel" id="phone" name="phone" pattern="[0-9]{10}" required placeholder="Telephone">
      <input type="text" placeholder="Location" required>
      <button type="submit"> REQUEST A CALLBACK</button>
    </form>
  </div>
</div>
</template>

<style lang="scss" scoped>
.container{
  width: 80%;
  margin: 0 auto;
  display: flex;
  background-color:#F6F6F6 ;
  div{
    margin: 30px 20px;
    width: calc((100% / 2) - 80px);
    text-align: left;
    line-height: 30px;
    h2{
      font-size: 2.3rem;
    }
    h4{
      font-size: 1.6rem;
      color: rgb(168, 165, 165);
      line-height: 40px;
      font-weight: lighter;
    }
    p{
      color: rgb(168, 165, 165);
    }
    h3{
      color: #7ABC64;
      font-size: 2rem;
    }
    form{
      display: flex;
      flex-direction: column;
      align-items: center;
      input{
        margin: 20px 0;
        padding: 20px 10px;
        width: 80%;
       border: 2px solid rgb(221, 217, 217);
      }
      input::placeholder{
        color: rgb(168, 165, 165);
      }
      .input-icon{
        background-image: url(../assets/img/image.png);
        background-repeat: no-repeat;
        background-position: calc(95%) ;
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
  }
  .firstform{
    background-color: white;
    border-radius: 10px;
    position:relative;
    top: -80px;
    text-align: center;
    p{
      font-size: 1.2rem;
      max-width: 80%;
      margin: 0 auto;
    }
  }
}

</style>