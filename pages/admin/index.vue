<template lang="html">
    <div class="admin-page">
        <section class="new-post">
            <button>Create Post</button>
        </section>
        <section class="exisiting-posts">
            <h1>Existing Posts</h1>
            <PostList />
        </section>
    </div>
</template>

<script>
import PostList from '@/components/Posts/PostList'

export default {
}
</script>

<style lang="css" scoped>
.admin-page {
  padding: 20px;
}

.new-post {
  text-align: center;
  border-bottom: 2px solid #ccc;
  padding-bottom: 10px;
}

.existing-posts h1 {
  text-align: center;
}
</style>
