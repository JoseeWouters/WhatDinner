<template>
    <header class="header">
        <nav class="top-nav">
            <nuxt-link to="/"><icon-what-dinner/></nuxt-link>
            <div class="nav-items">
                <nuxt-link to="/feature-request" class="nav-item">Feature request</nuxt-link>
                <nuxt-link to="/privacy-policy" class="nav-item">Privacy policy</nuxt-link>
            </div>
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
    background-color: $primary;
    color: $support;
    width: 100%;
    display: flex;
    justify-content: center;
    padding: 1em;
}

.logo {
    height: 40px;
    fill: $support;
}

.top-nav {
    width: 100%;
    max-width: 700px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav-item:not(:last-child) {
    margin-right: 1em;
}
</style>
