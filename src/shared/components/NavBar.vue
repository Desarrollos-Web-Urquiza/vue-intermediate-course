<script setup lang="ts">

// const props = defineProps({
//   title:  {
//     type: String,
//     required: true,
//   }
// });

// const props = defineProps<{ title?: string}>();

// Con interfaces/clases
interface Props {
 title: string;
}

const props = defineProps<Props>();


</script>

<template>
  <nav>  
    <img src="@/assets/logo.svg" alt="Vue logo" height="25" width="25">
    <span>{{ props.title || 'no title' }}</span>

    <RouterLink to="/" >Inicio</RouterLink>
    <RouterLink to="/about" >Sobre</RouterLink>
  </nav>
</template>


<style scoped>

nav{
    width: 100%;
    font-size: 12px;
    text-align: center;
    margin-top: 10px;
    text-align: center;
    width: 100%;
}

img {
    margin-right: 5px;
}

span {
    margin-right: 10px;
}

a {
    margin-right: 5px;
}

</style>
