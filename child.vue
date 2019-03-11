<template>
<div>
    <button @click="ChildEvent">{{name}}</button>
</div>
    
    
</template>

<script>
export default {
    
    data() {
        return {
            btninfo: '点击我',
        }
    },
    props: {
        name: String
    },
    mounted() {

    },
    methods: {
        ChildEvent() {
            this.$emit('events',{a:1,b:2},'haha')
        }
    }
    

}
</script>
