<template>
  <div id="home">
    <articles />

    <about />
  </div>
</template>

<script>
export default {
  name: 'Home',

  components: {
    About: () => import('@/components/content/Article'),
    Articles: () => import('@/components/home/Articles')
  }
}
</script>
