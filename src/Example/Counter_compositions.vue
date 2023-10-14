<script setup lang="ts">
import { onMounted, ref } from 'vue'

const count = ref(0);

function aumentar() {
    count.value +=1;
}
onMounted(()=>{
    console.log('el valor inicial del contador es '+ count.value);
});
</script>

<template>
    <p>hola yo soy la version composition API</p>
    <h1>contador:{{ count }}</h1>
    <button @click="aumentar">
        Incrementar contador
    </button>
</template>