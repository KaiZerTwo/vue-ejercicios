<script setup>
import { ref } from 'vue';

// ref de un objeto. También se puede con reactive.
let Nombre = ref('Fran');
let Apellido = ref('Quezada');
</script>

<template>
    <hr class="mb-5">

    <h2 class="mt-5">Datos personales</h2>
    <div class="card col-4 p-3">
        <div class="mb-3">
            <label class="form-label" for="nombre">Nombre</label>
            <input class="form-control" id="nombre" type="text" v-model="Nombre"/>
        </div>
        <div class="mb-3">
            <label class="form-label" for="tamanyo">Apellido</label>
            <input class="form-control" id="tamanyo" type="text" v-model="Apellido"/>
        </div>
        <div class="container pt-3">
            <p class="alert alert-success">Tu nombre es : {{Nombre}} {{Apellido}}</p>
        </div>
    </div>
</template>

<style scoped>
</style>
