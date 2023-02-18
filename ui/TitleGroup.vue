<template>
    <div class="title-group">
        <h2 class="title title--h2 title-reset">{{ title }}</h2>
        <span class="title-group__desc" v-if="desc">{{ desc }}</span>
    </div>
</template>

<script>
export default {
    name: 'TitleGroup',
    props: {
        title: {
            type: String
        },
        desc: {
            type: String
        }
    }
}
</script>