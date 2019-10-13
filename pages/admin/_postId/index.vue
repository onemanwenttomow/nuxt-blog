<template lang="html">
    <div class="admin-post-page">
        <section class="update-form">
            <AdminPostForm :post="loadedPost"/>
        </section>
    </div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm';
export default {
    layout: 'admin',
    components: {
        AdminPostForm
    },
    data() {
        return {
            loadedPost: {
                author: "Pete",
                title: "My amazing post",
                content: "Great content!!",
                thumbnailLink: 'https://picsum.photos/id/715/300/200'
            }
        }
    }
}
</script>

<style lang="css" scoped>
    .update-form {
        width: 90%;
        margin: 20px auto;
    }

    @media (min-width: 768px) {
        .update-form {
            width: 500px;
        }
    }
</style>
