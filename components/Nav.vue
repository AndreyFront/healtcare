<template>
    <nav class="nav">
        <ul class="nav__list list-reset">
            <li 
                class="nav__li"
                v-for="link in links"
                :key="link?.id"
            >
                <nuxt-link class="nav__link link-reset" :to="link?.href">{{ link?.name }}</nuxt-link>
            </li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: 'Nav',
    props: {
        links: {
            type: Array,
            required: true
        }
    }
}
</script>