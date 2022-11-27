<template>
    <div>
        <h2>Asset-{{ id }}</h2>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore aspernatur omnis, illo exercitationem delectus corrupti quas voluptatem molestiae minus nemo fugiat repellat tempore atque libero voluptates? Quod expedita facere dolores?</p>
    </div>
  </template>
  
  <script setup>
    const { id } = useRoute().params
  </script>