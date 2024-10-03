<template>
    <div>
    <v-table density="compact">
      <thead>
        <tr>
          <th class="text-left">
            Name
          </th>
          <th class="text-left">
            Project Name
          </th>
          <th>Post</th>
          <th>Status</th>
          <th>Bugets</th>
        </tr>
      </thead>
      <tbody>
        <tr
          v-for="item in desserts"
          :key="item.name"
        >
          <td>{{ item.name }}</td>
          <td>{{ item.nameProject }}</td>
          <td>{{ item.post }}</td>
          <td><v-chip
          border="success sm opacity-100"
          color="green"
          size="small"
          variant="text"
        >
        {{ item.status }}
        </v-chip>
        </td>
          <td>{{ item.budgets }}</td>
        </tr>
      </tbody>
      <div style=" display: flex; gap: 20px; justify-content: flex-end;align-items: center;">        
        <div>
            <div>Item per page</div>
            <v-select
               density="compact"
              style="width: 80px"
              :items="['5','10']"
              label="5"
            />
        </div>
        <div>1-5 of 10</div>
        <v-pagination :length="4"></v-pagination>
      </div>
    </v-table>
    </div>
  </template>
  
  <script setup>
    import { ref } from 'vue'
  
    const desserts = ref([
      {
        name: 'Frozen Yogurt',
        nameProject: 'ABC',
        post: '2022-01-15',
        status: 'Pending',
        budgets: '$500',
      },
      {
        name: 'Ice cream sandwich',
        nameProject: 'ABC',
        post: '2022-01-15',
        status: 'Pending',
        budgets: '$500',
      },
      {
        name: 'Eclair',
        nameProject: 'ABC',
        post: '2022-01-15',
        status: 'Pending',
        budgets: '$500',
      }
    ])
  </script>

<style>
</style>