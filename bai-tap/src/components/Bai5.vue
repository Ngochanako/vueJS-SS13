<template>
    <div>
      <v-alert
        style="width: 300px;color: brown;"
        v-model="alert"
        close-label="Close Alert"
        title="Xác nhận"
        variant="tonal"
        closable
      >
        Bạn có muốn xóa không?
        <template #close>
        <v-icon @click.stop="alert = false" class="custom-close-icon">mdi-close</v-icon>
      </template>
      </v-alert>
  
      <div v-if="!alert">
        <v-btn style="color: red;" @click="alert = true">
          Reset
        </v-btn>
      </div>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  const alert = ref(true)
  </script>
<style>
.custom-close-icon {
  color: white; /* Màu icon */
  font-size: 24px; /* Kích thước icon */
  cursor: pointer; /* Con trỏ khi hover */
  transition: color 0.3s; /* Hiệu ứng chuyển màu */
}

.custom-close-icon:hover {
  color: red; /* Màu khi hover */
} 
</style>
  