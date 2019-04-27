<template>
    <header class="header">
        <nav class="top-nav">
            <nuxt-link to="/"><icon-what-dinner/></nuxt-link>
            <nuxt-link to="/feature-request">Feature request</nuxt-link>
        </nav>
    </header>
</template>

<script>

import iconWhatDinner from '@/components/icons/iconWhatDinner.vue'

export default {
    components: {
        iconWhatDinner
    }
}
</script>

<style lang="scss" scoped>
.header {
    background-color: #fff;
    width: 100%;
    position: absolute;
    top: 0;
    left: 0;
    display: flex;
    justify-content: center;
    padding: 1em;
}

.logo {
    fill: $primary;
    height: 40px;
}

.top-nav {
    width: 100%;
    max-width: 700px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>
