<script setup>
//    const props = defineProps([
//         'label',
//         'color'
//    ])


//if you want to provide some default value then you have to follow the below orientation of defining props
    const props = defineProps({
        label:{
            type: String,
            default: 'Button'
        },
        color:{
            type:String,
            default:'cyan'
        }
    })

   function getColor(){
        return `bg-${props.color}-500 hover:bg-${props.color}-700`
   }
</script>


<template>
    <button :class="getColor()" class="text-white font-bold py-2 px-4 rounded">
        {{ label }}
    </button>
</template>


<style scoped>
</style>