<template>
    <!-- Conociendo el v-model -->
    <form>
        <input v-model="inputText" type="text" />
        <input v-model="inputCheckBox" type="checkbox" /> Acepto terminos y condiciones
        <select v-model="inputSelect">
            <option value="es">Spain</option>
            <option value="en">UK</option>
            <option value="fr">France</option>
        </select>
    </form>
    <h3>Input text: {{ inputText }}</h3>
    <h3>Input check: {{ inputCheckBox }}</h3>
</template>

<script lang="ts" setup>
    import { Ref, ref } from 'vue'

    let inputText:Ref<string> = ref('')
    let inputCheckBox:Ref<boolean> = ref(false)
    let inputSelect = ref('en')
</script>

<style scoped>
</style>
