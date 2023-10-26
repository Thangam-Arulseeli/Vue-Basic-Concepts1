<template>
<!-- <div class="container mt-3 border"> 
      <MC2 ComValue1="G2 - Covai" ComValue2='CG-VAK, Coimbatore'></MC2> 
</div>

  <div class="container mt-3 border">
     <h3 class="text-center text-primary"> Hello Welcome to my Vue JS </h3>
     <h4 class="text-center text-warning"> Vue JS Training </h4> 
</div> -->

 <!-- <div class="container mt-3 border">
     <MC1> </MC1>
</div>   -->

<div class="container mt-3 border">
     <MC1 /> 
</div> 

<div class="container mt-3 border"> 
      <MC2 ComValue1="Common Values Pass Here" ComValue2='CG-VAK, Coimbatore'></MC2> 
</div>

 
<div class="container mt-3 border">
  <MethodsVsComputed /> 
</div> 

<div class="container mt-3 border">
  <MethodsVsComputed1></MethodsVsComputed1>
</div>


 <component is="M-C2" ComValue1='qqqqqqqqq' ComValue2='wwwwwwww'> </component> 
 
  <!-- <keep-alive>  -->
  <!-- <component v-bind:is="comp"> </component> -->
<!-- </keep-alive>   -->

<div>
<component :is="MC1" />
<component :is="someCondition ? Foo : Bar" />
</div>

      <div> 
          <h3> defineProps Example </h3>
           <ParentComp />
      </div>

<!-- <h5> My first VUE Component</h5>
        <hr  />
        {{title}} <br />
        Count value is : <strong> {{count}} </strong>
        <hr /> 

        <div class="text-secondary text-center">
            <p>My name is <u><b> {{firstName}}  {{lastName}} </b> </u> </p>
        </div>

        <div class="text-worning text-center">
          <h5> {{a}} * {{b}} = {{multiply() }}</h5>
            <br />
              Value  {{ a * 100 }}
            <br />
             Condition :   {{ status ? 'YES' : 'NO' }}
            <br />
            {{ title.split(' ').reverse().join(' ') }}
            <br />
         </div> -->

         
</template> 

 <script setup> 
 
//  import HelloWorld from './components/HelloWorld.vue'
//  import TheWelcome from './components/TheWelcome.vue'

 import MC1 from './components/MyComponent1.vue'
 import MC2 from './components/MyComponent2.vue' 
  
 import MethodsVsComputed from './components/MethodsVsComputed.vue';  
 import MethodsVsComputed1 from './components/MethodsVsComputed1.vue';

 import ParentComp from './components/ParentComp.vue';

 
components: { ParentComp }
 
 //export default{
  //  components: {
  //      'M-C1': MC1
  //       , 'M-C2': MC2
  //     //MC1
  //     , MC2
  //     , MethodsVsComputed
  //     , MethodsVsComputed1
  //  }   ,
  //     data (){
  //       return { comp:'M-C1'}
  //     }
//}  




// export default {
//         data() {
//           return {  count: 100,
//                     a: 10,
//                     b: 20,
//                     title : 'JS file with HTML file in VUE example',
//                     status : true,
                    
//                     firstName : "Arulseeli",
//                     lastName : "Churchill"
//             }
//         },
//         methods: 
//         {
//          multiply()
//         {
//           var c= this.a * this.b
//           console.log(this.a + ' * ' + this.b + ' = ' + c )
//           alert ('Hai!!!! ' + this.firstName + " " + this.lastName)
//           return c
//         }
//         }
//       }

 </script> 











//  <!--  @close="toggleContainer"  
//     v-if="showContainer"
//     -->

// <!-- <header>
//     <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

//     <div class="wrapper">
//       <HelloWorld msg="You did it!" />
//     </div>
//   </header>

//   <main>
//     <TheWelcome />
//   </main> -->
  







// <!-- <style>
// @import './assets/base.css';

// #app {
//   max-width: 1280px;
//   margin: 0 auto;
//   padding: 2rem;

//   font-weight: normal;
// }

// header {
//   line-height: 1.5;
// }

// .logo {
//   display: block;
//   margin: 0 auto 2rem;
// }

// a,
// .green {
//   text-decoration: none;
//   color: hsla(160, 100%, 37%, 1);
//   transition: 0.4s;
// }

// @media (hover: hover) {
//   a:hover {
//     background-color: hsla(160, 100%, 37%, 0.2);
//   }
// }

// @media (min-width: 1024px) {
//   body {
//     display: flex;
//     place-items: center;
//   }

//   #app {
//     display: grid;
//     grid-template-columns: 1fr 1fr;
//     padding: 0 2rem;
//   }

//   header {
//     display: flex;
//     place-items: center;
//     padding-right: calc(var(--section-gap) / 2);
//   }

//   header .wrapper {
//     display: flex;
//     place-items: flex-start;
//     flex-wrap: wrap;
//   }

//   .logo {
//     margin: 0 2rem 0 0;
//   }
// }
// </style> -->
