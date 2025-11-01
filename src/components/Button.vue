<script setup lang="ts">
const props = defineProps<{
    promoText: string;
    btncolor: string;
}>();
const shopNow = () => {
    alert("Let's shop: "+props.promoText);
}

</script>


<template>
    

    <button class="text-white py-1 px-3 font-semibold rounded-sm"  v-on:click="shopNow()" :style="{backgroundColor: props.btncolor}">Shop Now →</button>
</template>