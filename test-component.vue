<template>
<div>
    <h1>哈哈哈哈哈哈哈</h1>
    <p>{{message}}</p>
    <child name="我是子组件" @events="FatherEvent"></child>
</div>
    
    
</template>

<script>
import child from './child.vue'
export default {
    
    data() {
        return {
            message: 1,
        }
    },
    mounted() {
        // alert(12321)
    },

    methods: {
        FatherEvent(e,one) {
            // alert('father');
            /* eslint-disable */
            console.log(e, one);
        }
    },

    components: {
        child: child
    }
}
</script>

<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
</style>
