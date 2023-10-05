<script>
import AppConsulting from './AppConsulting.vue'
import AppStrategy from './AppStrategy.vue'
import AppHelp from './AppHelp.vue'
import AppNews from './AppNews.vue'
import AppJumbotron from './AppJumbotron.vue';

export default {
    name: 'AppMain',

    data() {
        return {


        }
    },
    components: {
        AppConsulting,
        AppStrategy,
        AppHelp,
        AppNews,
        AppJumbotron
    }
}

</script>

<template>
    <main>
        <AppConsulting />
        <AppStrategy />
        <AppHelp />
        <AppNews />
        <AppJumbotron />
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
main {
    background-color: $bc_dark;
}

</style>
