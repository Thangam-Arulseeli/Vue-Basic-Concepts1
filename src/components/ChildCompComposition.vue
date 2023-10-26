<template>
    <div>
        <h2>
            Child Component
        </h2>
     <strong> Person Details in Child </strong>
     <p> Person Name : {{ personName }}</p>
     <p> Person Age : {{ personAge }}</p> 
     </div>
</template>
 
   <!--  <script setup>    props using script setup tag  (defineProps) - Composition API  
    const props =defineProps(['personName','personAge'])

    console.log(`Age of ` + props.personName +  ` is  ` + props.personAge)
  </script>   -->


 <script>  /*  props using script tag with setup()  (props) - Composition API */
 export default{
 props: ['personName','personAge'],
  setup(props){   // setup() receives props as the first argument
     console.log(`Age of ` + props.personName +  ` is  ` + props.personAge)
  }
}  
</script>