<template>
  <div class="about">
    <b-container>
      <h1>about web elements</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore 
        <span><img src="../assets/images/about-bg.png"/></span>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore 
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore 
      </p>
      <button type="button" class="btn">Read more</button>
  </b-container>
  </div> 
</template>

<script>
export default {
  name: 'About',
  props: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.about{
  margin: 8% 5%;
  h1{
    text-transform: uppercase;
  }
  span{
    display: block;
    img{
      width:75%;
      height: 100%;
    }
   }
  button{
    background-color: #9a26e2;
    color: white;
    padding: 10px 20px;
    margin: 10px;
    border-radius: 4px;
    &:hover{
      background-color: black;
    }

  }
}
</style>
