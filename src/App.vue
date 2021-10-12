<template>

<audio src="@/components/sound.mp3" autoplay loop></audio>

 <div class="container">
   <img src="@/components/titulo.png" >
  <FilterByStatus />
    <FilterByName />
    <ListCharacters />
  </div>
</template>

<script>
import ListCharacters from '@/components/ListCharacters'
import FilterByStatus from '@/components/FilterByStatus'
import FilterByName from '@/components/FilterByName'
export default {
  name: 'App',
  components: {
    ListCharacters,
    FilterByStatus,
    FilterByName
  }
}
</script>

<style lang="scss">
:root {
  --background-body: #304D74;
  --background-card: #8DC660;
  --text-white: #fff;
  --text-gray: black;
  --text-orange: #1B7800;
}
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  background-color: var(--background-body);
  color: var(--text-white);
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
h1 {
  margin-bottom: 3rem;
  text-align: center;
  font-size: 80px;
}
.container {
  width: 980px;
  max-width: 90%;
  margin: 5rem auto;
}
img {
  width: 100%;
}
</style>