<template>
<div>
    <h2>Parent Component</h2>
    <p> Parent Data : Person Name : {{ pName }} , Age : {{ pAge }} </p>
    <p v-if="viewChild"> 
    <Child :personName="pName" v-bind:personAge="pAge" />
    </p>
    <button @click="viewChild=!viewChild"> Show Child </button>
</div>
</template>
<script>
import ChildCompComposition from './ChildCompComposition.vue';
export default{
    data(){
        return {
            pName: 'Victor',
            pAge: 34,
            viewChild: false
        }
    },
    components: {
        Child: ChildCompComposition
    }
}
</script>