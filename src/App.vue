<template>
  <div id="app">
    <!-- nav -->
    <b-navbar toggleable="lg" type="dark" >
    <b-navbar-brand href="#"> <img src="./assets/images/logo.png"/></b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    <b-collapse id="nav-collapse" is-nav>
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-item class="defult-color" href="/">home</b-nav-item>
        <b-nav-item class="defult-color" href="/about">about</b-nav-item>
        <b-nav-item class="defult-color" href="/services">services</b-nav-item>
        <b-nav-item class="defult-color" href="/">web</b-nav-item>
        <b-nav-item class="defult-color" href="/">elements</b-nav-item>
        <b-nav-item class="defult-color" href="/contact">contact</b-nav-item>
        <b-nav-item class="defult-color" href="/">
          <b-icon icon="search"></b-icon>
        </b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
      
    <router-view/>
      <!-- footer -->
  <footer>
    <div class="upper-footer">
      <b-container>
        <b-row align-h="center">
          <b-col cols="9">
            <b-form>
              <b-form-input placeholder="Enter your email"></b-form-input>
              <button>Subscribe now</button>
            </b-form>
            <h1> <span>2020</span>Free Multipurpose Responsive  Landing Page </h1>
            <div>
              <b-list-group horizontal>
                <b-list-group-item><b-icon icon="facebook" ></b-icon></b-list-group-item>
                <b-list-group-item><b-icon icon="twitter"></b-icon></b-list-group-item>
                <b-list-group-item><b-icon icon="linkedin"></b-icon></b-list-group-item>
                <b-list-group-item><b-icon icon="instagram"></b-icon></b-list-group-item>
                <b-list-group-item><b-icon icon="youtube"></b-icon></b-list-group-item>
              </b-list-group>
            </div>
          </b-col>
        </b-row>
      </b-container>  
    </div> 
    <div class="last-footer">
      <p>2020 All Rights Reserved Design by </p>
    </div>
  </footer>

  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  
}
.defult-color a{
  color: black !important;
  font-size: 18px;
  text-transform: uppercase;
  font-style: italic;
  &:hover{
    color:#9a26e2!important;
  }
}
 //footer
 footer{
  .upper-footer{
    background-image: linear-gradient(to right, #942dd4 , #5b1abc);
    margin-top: 40px;
    margin-bottom: 15px;
    padding-bottom: 40px;
    form{
      position: relative;
      margin-top: 20%;
      input{
        background: none !important;
        padding: 6%;
        border: 0px !important;
        border-bottom: 1px solid white !important;
        border-radius: 0px !important;
        &::placeholder{
          color: white !important;
          font-size: 15px;
        }
        &:focus{
          box-shadow: none;
        }
        }
        button{
          position: absolute !important;
          right: 0 !important;
          padding: 15px 20px !important;
          bottom: 5px !important;
          border-radius: 30px !important;
          background: none !important;
          border: 1px solid white !important;
          color: white !important;
          font-size: 14px !important;
          text-transform: uppercase !important;

        }
      }
      h1{
        color: white;
        text-transform: uppercase;
        font-size: 27px;
        span{
          display: block;
          padding: 6px;
          font-size: 3rem;
        }
      }
      .list-group{
        margin-left: 25%;
        .list-group-item{
          background-color: transparent !important;
          border: none !important;
          .b-icon {
        
              color: white;
              font-size: 30px;
            
          }
        }
      }
    }
  }
  @media screen and (max-width: 900px) {
    footer{
      .upper-footer{
      .list-group{
        margin-left:0%;
        .list-group-item{
          .b-icon {
            font-size: 15px;
          }
        }
      }
    }
    }

  }

 
</style>
