<script setup lang="ts">
import { ref } from "vue";
  const query = ref('' as string)
  const songs = [{
    id:1, artist: 'Great Artis', name: 'Great Song'
  },{
    id:2, artist: 'Greater Artis', name: 'Greater Song'
  },{
    id:3, artist: 'Much Great Artis', name: 'Much Great Song'
  }]

  const getMusic = (): void => {
    console.log(typeof query.value);
    
  }
</script>

<template>
  <div class="about">
    <h1>Tunes</h1>

    <form @submit.prevent="getMusic()">
      <input type="text" v-model="query">
    </form>

    <ul>
      <li v-for="song in songs" :key="song.id">
        {{ song }}
      </li>
    </ul>
  </div>
</template>

<style>

</style>
