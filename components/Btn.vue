<template>
    <button 
        v-bind:style="{
            background: '#AA0001'
        }"
        v-if="!is_link" class="v-Btn btn btn-danger" :type="type">{{ label }}</button>
    <a 
        v-bind:style="{
            background: '#AA0001',
            color: 'white'
        }"
        v-else :href="href" class="v-Btn btn btn-danger">{{ label }}</a>
</template>

<script>
    export default {
        props: [
            'label',
            'is_link', 'type', 'href'
        ]
    }
</script>

<style scoped>
    .v-Btn {
        padding-left: 28px!important;
        padding-right: 28px!important;
        border-radius: 12.5px!important;
    }
</style>