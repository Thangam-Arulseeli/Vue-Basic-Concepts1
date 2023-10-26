<template>
   <div>
          <h3>  My name is  {{firstname}} {{lastname}}  </h3>
            <h4> My age is {{age}} </h4>
            <h4> {{result}} </h4>
            <h5 class="text-danger"> {{ComValue1}} </h5>
            <h5> {{ComValue2}} </h5>
            <!-- <slot> </slot> -->
             <!-- <button @click="toggleShow"> Open Container </button> -->
     </div>
 </template>   


<script>
export default
    { props: ['ComValue1', 'ComValue2'],
    data(){
        return{ 
            
               firstname : 'Arulseeli',
               lastname : 'Churchill',
               age : 20,
               result : 'true'
              // showContainer : false
               }
    }
    }

    </script>