<template>
    <div class="contact">
        <b-container>
          <b-row>
            <b-col md="6">
                <h1>Requeste a call back</h1>
                <b-form >
                    <b-form-group>
                        <b-form-input
                        id="input-1"
                        type="text"
                        placeholder="Name"
                        required
                        ></b-form-input>
                    </b-form-group>
                    <b-form-group>
                        <b-form-input
                        id="input-2"
                        type="email"
                        placeholder="Email"
                        required
                        ></b-form-input>
                    </b-form-group>
                    <b-form-group>
                        <b-form-input
                        id="input-3"
                        type="number"
                        placeholder="Phone"
                        required
                        ></b-form-input>
                    </b-form-group>
                    <b-form-group>
                        <b-form-select v-model="selected" :options="options" class="form-control"></b-form-select>
                    </b-form-group>
                    <b-form-group>
                        <b-form-textarea
                        id="textarea-Large"
                        size="lg"
                        placeholder="Message"
                    ></b-form-textarea>
                </b-form-group>
                <b-button>
                  Send
                </b-button>
                </b-form>
            </b-col>
            <b-col>
                <img src="../assets/images/contact-bg.png" alt="">
            </b-col>
          </b-row>
        </b-container>
    </div> 
  </template>
  
  <script>
  export default {
    name: 'Contact',
    props: {
  
    },
    
    data() {
      return {
        selected: null,
        options: [
          { value: null, text: 'Select element' },
          { value: 'a', text: 'one' },
          { value: 'b', text: 'two' },
          { value: 'c', text: 'three' },
        
        
        ]
      
    }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">
   .custom-select{
    background: #fff !important;
    color: #495057;
    background-color: #fff;
    background-clip: padding-box;
    border: 1px solid #ced4da;
    border-radius: 0.25rem;
    transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
   }
   .contact{
        margin: 7% 1%;
    h1{
        text-transform: uppercase;
        font-size: 35px;
        font-weight: bold;
    };
    img{
        width: 100%;
    }
    form{
        background-color: #4323b1;
        padding: 7%;
        width: 80%;
        margin: auto;
        input{
            height: calc(1.5em + 0.75rem + 10px);
            margin-bottom: 10px;
            border-radius: 0px !important;
        }
        button{
            background-color: #8929cf;
            color: white;
            text-transform: uppercase;
            padding: 15px 35px;
            margin: 30px 0px 5px;
            &:hover{
                color: black;
                background-color: white;
            }
        }
    }
   }
  </style>
  