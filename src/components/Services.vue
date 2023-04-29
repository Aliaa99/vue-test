<template>
    <div class="services">
      <b-container class="bv-example-row">
        <h1>services</h1>
        <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore 
        </p>
        <div class="services-detailes">
            <b-row>
                <b-col>
                    <img src="../assets/images/icon-1.png" />
                    <h5>website element</h5>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore </p>
                </b-col>
                <b-col>
                    <img src="../assets/images/icon-2.png" />
                    <h5>applicatinos element</h5>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore </p>
                </b-col>
                <b-col>
                    <img src="../assets/images/icon-3.png" />
                    <h5>design element</h5>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore </p>
                </b-col>
            </b-row>
        </div>
      </b-container>
    </div> 
  </template>
  
  <script>
  export default {
    name: 'services',
    props: {
  
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">
    .services{
        background-color: #fcf8fe !important;
        h1{
            margin: 0px;
            padding: 5% 0% 0% 0%;
            text-transform: uppercase;
        }
        .services-detailes{
            margin-top: 10%;
            padding-bottom: 10%;
            h5{
                text-transform: uppercase;
                margin: 30px 0px;
                // font-size: 100%;
                font-weight: 500;
            }
            p{
              margin: 5px;
            }
        }

    }
  </style>
  