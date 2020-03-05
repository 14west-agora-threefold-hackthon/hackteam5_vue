<template>
  <div id="content">
    <articleContent />
  </div>
</template>

<script>
export default {
  name: 'Content',
  components: {
    ArticleContent: () => import('@/components/content/Article')
  }
}
</script>
