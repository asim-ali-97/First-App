<template>
    <button @click="$emit('click')" class="btn">{{ title }}</button>
</template>

<script>
    export default{
        name: "CustomPrimaryBtn",
        props: {
            title: {
                type: String,
                default: ""
            }
        }
    }
</script>

<style>
.btn{
    color: white;
    width: 250px;
    border-radius: 20px;
    background-color: #00DC82;
}
</style>