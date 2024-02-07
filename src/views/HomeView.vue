<script setup>
import {ref, onMounted} from 'vue'

const dialog=ref(true)
const nahh=ref(false)
const first=ref(false)
const second=ref(false)
const third=ref(false)
const fourth=ref(false)
const fifth=ref(false)

function yass(){
  fifth.value=true
  first.value=false
  second.value=false
  third.value=false
  fourth.value=false
}

</script>

<template>

<v-container fluid class="bg-grey-darken-4 " v-if="!dialog" >

<v-card height="500" class=" bg-grey-darken-4 overflow-auto">

  <v-row  class="mt-2" v-if="!fifth">

    <v-card 
          class="mx-auto"
          width="344"
          color="indigo"
          variant="outlined"
        >
          <v-card-item>
            <div>
              <div class="text-overline mb-1">
               
              </div>
              <div class="text-h6 mb-1">
                Hello Love
              </div>
              <div class="text-caption">AAIYE APKA INTZAR THA!!!</div>
            </div>
          </v-card-item>

          <v-card-actions>
            <v-btn @click="first=true" variant="outlined">
              next
            </v-btn>
          </v-card-actions>
        </v-card>



 






  </v-row>

<v-row v-if="first" >

<v-card
      class="ma-5"
      width="344"
      color="indigo"
      variant="outlined"
    >
      <v-card-item>
        <div>
          <div class="text-overline mb-1">
           
          </div>
          
          <div class="text-caption">
 My bro...You are beautiful like Rohit's Pull Shot.</div>
 <div class="text-caption">
 You are beautifull like Messi's Freekick .</div>
 <div class="text-caption">
 You are beautiful like Kholi's Cover Drive.</div>


        </div>
      </v-card-item>

      <v-card-actions>
        <v-btn @click="second=true" variant="outlined">
          next
        </v-btn>
      </v-card-actions>
    </v-card>



</v-row>
<v-row v-if="second" >

<v-card
      class="ma-5"
      width="344"
      color="indigo"
      variant="outlined"
    >
      <v-card-item>
        <div>
          <div class="text-overline mb-1">
           
          </div>
          
          <div class="text-caption">
  You are the best thing that has ever happened to me in my life.</div>
  <div>
    <div class="text-caption">
 Aapse 2 baat kya kar lu aisa lagne lagta hai h ke mere se khush insan duniya ma koi nahi hain or na he kabhi hoga</div>

  </div>
        </div>
      </v-card-item>

      <v-card-actions>
        <v-btn @click="third=true" variant="outlined">
          next
        </v-btn>
      </v-card-actions>
    </v-card>



</v-row>

<v-row v-if="third" >

<v-card
      class="ma-5"
      width="344"
      color="indigo"
      variant="outlined"
    >
      <v-card-item>
        <div>
          <div class="text-overline mb-1">
           
          </div>
          
          <div class="text-caption">
  I loveeeeeeeeeeeeeeeee YOUUUUUUUUUUUUUU</div>
  <div>
    <div class="text-caption">
next daba saali</div>

  </div>
        </div>
      </v-card-item>

      <v-card-actions>
        <v-btn @click="fourth=true" variant="outlined">
          next
        </v-btn>
      </v-card-actions>
    </v-card>



</v-row>

<v-row v-if="fourth" >

<v-card
      class="ma-5"
      width="344"
      color="indigo"
      variant="outlined"
    >
      <v-card-item>
        <div>
          <div class="text-overline mb-1">
           
          </div>
          
          <div class="text-caption">
 But as a friend so will you be my friend forever</div>
  <div>

  </div>
        </div>
      </v-card-item>

      <v-card-actions>
        <v-btn @click="yass()" variant="outlined">
       dil se haan
        </v-btn>
        <v-btn @click="yass()" variant="outlined">
         dil se nahhh
        </v-btn>
      </v-card-actions>
    </v-card>



</v-row>
<v-row v-if="fifth" >

<v-card
      class="ma-5"
      width="344"
      color="indigo"
      variant="outlined"
    >
      <v-card-item>
        <div>
          <div class="text-overline mb-1">
          Your Reply:
          </div>
          
          <div class="text-caption">
 YASS I LOVE U TOOOOOO AND I WILL MARRY YOU..........(SCAMMMED )</div>
 <div class="text-caption">
 And ofcourse i hate u too GM DIDI</div>
  <div>
  
  
 

  </div>
        </div>
      </v-card-item>

    
    </v-card>



</v-row>



 

  

</v-card>


</v-container>

<v-dialog v-model="dialog" width="auto">

<v-card width="250" height="150">
  <v-card-text>
    <v-row  v-if="!nahh">
   kya app wahi hai jiski mai talash kar raha hu ?Urf mere sapne ki raani?

  </v-row>
  <v-row v-if="nahh">
   Saali chup chap se haan pr click kijiye
    
  </v-row>
    <v-row class="mt-5">
      <v-col cols="6" >
        <v-btn class="text-none" color="green" variant="tonal" rounded="lg" @click="dialog=false">
          Ji Haan

        </v-btn>
       </v-col>
        <v-col cols="6">
        <v-btn class="text-none" color="red" variant="tonal" rounded="lg" @click="nahh=true">
          Ji Nahh

        </v-btn>
        </v-col>
    </v-row>
  </v-card-text>



</v-card>

</v-dialog>



</template>
