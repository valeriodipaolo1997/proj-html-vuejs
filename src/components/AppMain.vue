<script>
import AppConsulting from './AppConsulting.vue'
import AppStrategy from './AppStrategy.vue'
import AppHelp from './AppHelp.vue';

export default {
    name: 'AppMain',

    data() {
        return {


        }
    },
    components: {
        AppConsulting,
        AppStrategy,
        AppHelp
    }
}

</script>

<template>
    <main>
        <AppConsulting />
        <AppStrategy />
        <AppHelp />
    </main>
</template>

<style lang="scss" scoped>


</style>
