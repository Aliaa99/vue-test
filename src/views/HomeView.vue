<template>
  <div>
    <div class="home">
      <div class="web-element">
        <h1>Web eLements Templates</h1>
        <h3>Free Multipurpose Responsive Landing Page</h3>
        <button type="button" class="btn btn-secondary">Read more</button>
      </div>
    </div>
  <!-- about component -->
    <div >
      <about />
    </div>
<!-- services component-->
    <div>
       <services />
    </div>
<!-- contact component-->
    <div>
       <contact />
    </div>
    <!-- clients -->
    <div>
        <clients />
    </div>
  </div>
  
</template>


<style lang="scss">
  .home{
    background-image: url(../assets/images/banner-bg.png);
    position: relative;
    z-index: -1;
    &::after{
      content: url("../assets/images/bg-main.png");
      bottom: -15%;
      position: absolute;
      left: 0;
      right: 0;
    };
    .web-element{
      padding : 10%;
      color:white;
      h3{
        padding: 20px;
      }
      button{
        background-color: white;
        color:#9a26e2;
      }
    }
  };
  @media screen and (max-width: 900px) {
  .home {
    &::after{
      bottom: -20%;    
    }
   }
  }

</style>

<script>
import About from '@/components/About.vue'
import Services from '@/components/Services.vue'
import Contact from '@/components/Contact.vue'
import Clients from '@/components/Clients.vue'
export default {
  name: 'HomeView',
  components:{
    About,
    Services,
    Contact,
    Clients
  }
}
</script>
