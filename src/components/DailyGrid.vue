<script setup>
// IMPORTS
import { ref } from 'vue'

// PROPS

// STORES

// DATA & REFS
const pickems = ref([
  [
    {
      team_name: 'Jazz',
      team_logo: 'https://content.sportslogos.net/logos/6/234/full/utah_jazz_logo_primary_19973688.png'
    },
    {
      team_name: 'Kings',
      team_logo: 'https://content.sportslogos.net/logos/6/234/full/utah_jazz_logo_primary_19973688.png'
    },
  ],
  [
    {
      team_name: 'Jazz',
      team_logo: 'https://content.sportslogos.net/logos/6/234/full/utah_jazz_logo_primary_19973688.png'
    },
    {
      team_name: 'Kings',
      team_logo: 'https://content.sportslogos.net/logos/6/234/full/utah_jazz_logo_primary_19973688.png'
    },
  ],
  [
    {
      team_name: 'Jazz',
      team_logo: 'https://content.sportslogos.net/logos/6/234/full/utah_jazz_logo_primary_19973688.png'
    },
    {
      team_name: 'Kings',
      team_logo: 'https://content.sportslogos.net/logos/6/234/full/utah_jazz_logo_primary_19973688.png'
    },
  ],
  [
    {
      team_name: 'Jazz',
      team_logo: 'https://content.sportslogos.net/logos/6/234/full/utah_jazz_logo_primary_19973688.png'
    },
    {
      team_name: 'Kings',
      team_logo: 'https://content.sportslogos.net/logos/6/234/full/utah_jazz_logo_primary_19973688.png'
    },
  ],
])
// COMPUTED

// EMITS

// LIFECYCLE EVENTS

// METHODS
</script>

<template>
  <div class="grid grid-cols-2 w-auto max-w-screen-lg gap-12">
    <div v-for="(pickem, index) in pickems" :key="index" class="h-64 border shadow divide-y">
      <div v-for="pick in pickem" :key=pick.team_name class="h-1/2 flex justify-center items-center cursor-pointer hover:bg-gray-100">
        <div class="w-32 h-32 flex items-center">
          <img
            class="object-cover"
            :src="pick.team_logo"
            alt=""
          >
        </div>
        <p class="text-2xl font-semibold">{{ pick.team_name }}</p>
      </div>
    </div>
  </div>
</template>