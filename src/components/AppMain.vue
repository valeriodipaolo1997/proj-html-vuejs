<script>
import AppConsulting from './AppConsulting.vue'
import AppStrategy from './AppStrategy.vue';

export default {
    name: 'AppMain',

    data() {
        return {


        }
    },
    components: {
        AppConsulting,
        AppStrategy
    }
}

</script>

<template>
    <main>
        <AppConsulting />
        <AppStrategy />
    </main>
</template>

<style lang="scss" scoped>


</style>
