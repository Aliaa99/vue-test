<template>
    <div class="clients">
      <b-container>
        <b-row align-h="center">
            <b-col cols="8">
                <h1>what is say clients</h1>
                <p class="first-p">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore 
                , sed do eiusmod tempor incididunt ut labore 
                </p>
                <div>
                    <h4>Consectetur adipiscing </h4>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
                        sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                         Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris 
                         nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in 
                    </p>
                    <img src="../assets/images/icon-4.png" alt="">
                </div>
            </b-col>
        </b-row>
    </b-container>
    </div> 
  </template>
  
  <script>
  export default {
    name: 'Clients',
    props: {
  
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">
    .clients{
        h1{
           text-transform: uppercase;
           font-weight: bold;
        }
        .first-p{
            margin-bottom: 15%;
        }
        h4{
            margin-bottom: 10px;
        }
    }
  </style>
  