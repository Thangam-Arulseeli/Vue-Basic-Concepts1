<template>
  <p class="display">Computed reversed message: "{{ reversedMessage }}"</p>
  <b> Array values-For loop: </b> <ul class="display" v-for="name in names"><li>{{name}} </li> </ul>
 <b> Start with H - Computed(for): </b> <p class="display" v-for="stname in startsWithH">{{stname}} </p>
 <b> End with ni - Computed(for): </b> <p class="display" v-for="name in endWithNi">{{name}} </p>
 <p class="display"> Listing Start value using Method : "{{ startsWithChar('H') }}"</p>
</template>

<script>
export default{
    data: function(){
        return {
            message : 'GOD BLESS YOU ALL',
            names: ["Harishmitha", "Yamini", "Harry", "Ranita",'Harini','Yashika']
        }
    },

   methods: {
    startsWithChar(whichChar){
        return this.names.filter(n => n.startsWith(whichChar))
    }
   },

   computed: {
        // a computed getter
        reversedMessage: function () {
        // `this` points to the vm instance
        return this.message.split('').reverse().join('')
     },
     startsWithH(){
        return this.names.filter(n => n.startsWith("H"))
    },
    endWithNi(){
        return this.names.filter(n => n.endsWith("ni"))
    }
   } 
}
</script>

<style>
   .display{
    font-style: italic;
    font-size: larger;
    color: crimson;
    background-color: cornsilk;
   }
</style>