<template>
    <div class="wrapper">
        <app-header ref="header"/>
        <main class="main">
            <nuxt/>
        </main>
    </div>
</template>

<script>

import appHeader from '@/components/app/appHeader.vue'

export default {
    components: {
        appHeader
    }
}
</script>

<style>
.wrapper {
    height: 100vh;
    display: flex;
    flex-direction: column;
}

.main {
    padding: 1em;
    background: url('/images/home-background-brooke-lark.jpg') no-repeat left center /cover;
    flex: 1;
}

.container {
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    backdrop-filter: blur(2px);
    background: rgba(255, 255, 255, 0.9);
    padding: 1em;
}
</style>
