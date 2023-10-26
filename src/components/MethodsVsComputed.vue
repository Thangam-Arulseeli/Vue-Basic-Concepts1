<template>
<div>
  <button @click="counterMethod++">Method Button</button>   
  <p>{{ counterMethod }}</p> <br/>
    {{ printTextMethod() }}
  
  <button @click="counterComputed++">Computed Button</button>
  <p>{{ counterComputed }}</p> <br/>
     {{ printTextComputed }}
</div>
</template>

<script>
export default{
data: function() {
  return {
    counterComputed: 0,
    counterMethod: 0
  };
},

methods: {
  printTextMethod: function() {
    console.log("Counter printed from method:", this.counterMethod);
  }
},

computed: {
  printTextComputed: function() { 
    console.log("counter printed from computed:",     
    this.counterComputed);
  }
}

}
</script>