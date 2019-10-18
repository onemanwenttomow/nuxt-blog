<template >
    <div class="posts-page">
        <PostList :posts="loadedPosts"/>
    </div>
</template>

<script>

import PostList from '@/components/Posts/PostList'

export default {
  components: {
      PostList
  },
  data() {
      return {
          loadedPosts: [
              {
                  id: '1',
                  title: 'First Post',
                  previewText: 'Some preview text',
                  thumbnail: "https://picsum.photos/id/715/300/200"
              },
              {
                  id: '2',
                  title: 'Second Post',
                  previewText: 'Some preview text',
                  thumbnail: "https://picsum.photos/id/715/300/200"
              }
          ]
      }
  },
  mounted: function() {
      console.log("mounted!!");
  }
}
</script>

<style lang="css" scoped>
    .posts-page {
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>
