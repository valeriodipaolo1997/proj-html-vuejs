<script>
import AppConsulting from './AppConsulting.vue'
import AppStrategy from './AppStrategy.vue'
import AppHelp from './AppHelp.vue'
import AppNews from './AppNews.vue';

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
        AppNews
    }
}

</script>

<template>
    <main>
        <AppConsulting />
        <AppStrategy />
        <AppHelp />
        <AppNews />
    </main>
</template>

<style lang="scss" scoped>


</style>
