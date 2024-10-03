<template>
    <div>
        <h4>Bài 2</h4>
        <v-text-field 
        :rules="rules"
        hide-details="auto" 
        label="Input">
        </v-text-field>
    </div>
</template>

<script setup>
const rules = [
  v => !!v || 'Input is required',
  v => v.length >= 5 || 'Min 5 characters',
]
</script>

<style>

</style>