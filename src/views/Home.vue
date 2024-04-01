<template>
  <v-container class="custom-background">
      <v-row align="center" justify="center" >
          <v-col cols="12" sm="10">
            <v-card class="elevation-6 mt-10"  >
             <v-window v-model="step">
                <v-window-item :value="1">
                  <v-row>
                    <v-col cols="12" md="6">
                      <v-card-text class="mt-12">
                        <h1
                          class="text-center"
                        >Login in to Your Account</h1>
                        
                        <h6
                          class="text-center  grey--text "
                        > <br></h6>
                        <v-row align="center" justify="center">
                          <v-col cols="12" sm="8">
                           
                          <v-text-field
                            label="Email"
                            outlined
                            dense
                            color="blue"
                            autocomplete="false"
                           class="mt-16"
                          />
                          <v-text-field
                            label="Password"
                            outlined
                            dense
                            color="blue"
                          autocomplete="false"
                           type="password"
                          
                          />
                            <v-row>
                              <v-col cols="12" sm="7">
                                <v-checkbox
                       
                        label="Remember Me"
                        class="mt-n1"
                        color="blue"
                      > </v-checkbox>
                              </v-col>
                              <v-col cols="12" sm="5">
                                <span class="caption blue--text">Forgot password</span>
                              </v-col>
                            </v-row>
                          <v-btn color="blue" dark block tile>Log in</v-btn>
                     
                         <h5
                          class="text-center  grey--text mt-4 mb-3"
                        >Or Log in using</h5>
                         <div class="d-flex  justify-space-between align-center mx-10 mb-16">
                        
                        
                        
                         </div>
                          </v-col>
                        </v-row>  
                      </v-card-text>
                    </v-col>
                    <v-col cols="12" md="6" class="blue rounded-bl-xl" >
                    <div style="  text-align: center; padding: 70px 0; ">
                      <!-- <v-img src="../assets/Images/Image1.jpg"  alt="Your Image" class="centered-image"></v-img> -->
                      <v-container class="d-flex justify-center align-start">
    <img src="../assets/Images/Image3.jpg" alt="Your Image" class="centered-image">
  </v-container>
                      <v-card-text class="white--text" >
                        <h3 class="text-center ">Don't Have an Account Yet?</h3>
                        <h6
                          class="text-center"
                        ><br> </h6>
                      </v-card-text>
                      <div class="text-center">
                        <v-btn tile outlined dark @click="step++">SIGN UP</v-btn>
                      </div>
                      </div>
                    </v-col>
                  </v-row>
                </v-window-item>
                <v-window-item :value="2">
                  <v-row >
                    <v-col cols="12" md="6" class="blue rounded-br-xl">
                     <div style="  text-align: center; padding: 70px 0;">
                      <v-container class="d-flex justify-center align-start">
    <img src="../assets/Images/Image5.jpg" alt="Your Image" class="second-image">
  </v-container>
                      <v-card-text class="white--text" >
                        <h3 class="text-center ">Alredy Signed up?</h3>
                        <h6
                          class="text-center"
                        ><br> </h6>
                      </v-card-text>
                      <div class="text-center">
                        <v-btn tile outlined dark @click="step--">Log in</v-btn>
                      </div>
                      </div>
                    </v-col>

                    <v-col cols="12" md="6">
                      <v-card-text class="mt-12">
                        <h2
                          class="text-center"
                        >Sign Up for an Account</h2>
                        <h6
                          class="text-center  grey--text "
                        ></h6>
                        <v-row align="center" justify="center">
                          <v-col cols="12" sm="8">
                           <v-row>
                           <v-col cols="12" sm="6">
                            <v-text-field
                            label="First Name"
                            outlined
                            dense
                            color="blue"
                            autocomplete="false"
                           class="mt-4"
                          />
                           </v-col>
                           <v-col cols="12" sm="6">
                            <v-text-field
                            label="Last Name"
                            outlined
                            dense
                            color="blue"
                            autocomplete="false"
                           class="mt-4"
                          />
                           </v-col>
                           </v-row>
                           <v-text-field
                            label="Employee Id"
                            outlined
                            dense
                            color="blue"
                            autocomplete="false"
                          />
                          <v-text-field
                            label="Email"
                            outlined
                            dense
                            color="blue"
                            autocomplete="false"
                          />
                          <v-text-field
                            label="Password"
                            outlined
                            dense
                            color="blue"
                          autocomplete="false"
                           type="password"
                          
                          />
                          <v-text-field
                            label="Confirm Password"
                            outlined
                            dense
                            color="blue"
                          autocomplete="false"
                           type="password"
                          
                          />
                            <v-row>
                              <v-col cols="12" sm="7">
                                <v-checkbox
                       
                        label="I Accept"
                        class="mt-n1"
                        color="blue"
                      > </v-checkbox>
                              </v-col>
                              <v-col cols="12" sm="5">
                                <span class="caption blue--text ml-n4">Terms &Conditions</span>
                              </v-col>
                            </v-row>
                          <v-btn color="blue" dark block tile>Sign up</v-btn>
                     
                         <h5
                          class="text-center  grey--text mt-4 mb-3"
                        >Or Sign up using</h5>
                         <div class="d-flex  justify-space-between align-center mx-10 mb-11">
                        
                        
                         </div>
                          </v-col>
                        </v-row>  
                      </v-card-text>
                    </v-col>
                  </v-row>
                </v-window-item>
              </v-window>
            </v-card>
          </v-col>
      </v-row>
  </v-container>
</template>

<script>
  

  export default {
   data: () => ({
    step: 1
  }),
  props: {
    source: String
  } 

    
  }
</script>
<style scoped>

.centered-image {
  max-width: 80%; /* Adjust the maximum width of the image as needed */
   max-height: 80%; /* Adjust the maximum height of the image as needed */
   border-radius: 20px;

 } 

 .second-image {
  max-width: 90%; /* Adjust the maximum width of the image as needed */
   max-height: 90%; /* Adjust the maximum height of the image as needed */
   border-radius: 20px;

 } 

.custom-background {
  background-color: #e193c8; /* Change this to your desired background color */
}


.v-application .rounded-bl-xl {
    border-bottom-left-radius: 300px !important;
}
.v-application .rounded-br-xl {
    border-bottom-right-radius: 300px !important;
}
</style>
