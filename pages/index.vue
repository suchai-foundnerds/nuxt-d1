<script setup lang="ts">
const people = [{
  id: 1,
  name: 'Lindsay Walton',
  title: 'Front-end Developer',
  email: 'lindsay.walton@example.com',
  role: 'Member'
}, {
  id: 2,
  name: 'Courtney Henry',
  title: 'Designer',
  email: 'courtney.henry@example.com',
  role: 'Admin'
}, {
  id: 3,
  name: 'Tom Cook',
  title: 'Director of Product',
  email: 'tom.cook@example.com',
  role: 'Member'
}, {
  id: 4,
  name: 'Whitney Francis',
  title: 'Copywriter',
  email: 'whitney.francis@example.com',
  role: 'Admin'
}, {
  id: 5,
  name: 'Leonard Krasner',
  title: 'Senior Designer',
  email: 'leonard.krasner@example.com',
  role: 'Owner'
}, {
  id: 6,
  name: 'Floyd Miles',
  title: 'Principal Designer',
  email: 'floyd.miles@example.com',
  role: 'Member'
}]
</script>

<template>
  <main class="p-24">
    <UCard>
      <template #header>
        <div class="flex gap-x-2 items-center text-xl">
          <UIcon class="text-blue-600" name="i-mdi-account" />
          <span class="text-slate-800 font-bold">Users</span>
        </div>
      </template>

      <UTable :rows="people" />

      <template #footer>
        <div class="text-sm text-slate- text-right">Total 2,410 users</div>
      </template>
    </UCard>
  </main>
</template>

