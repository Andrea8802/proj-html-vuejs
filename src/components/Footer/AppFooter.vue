<script>
import TopFooter from './TopFooter.vue';
export default {
    name: "AppFooter",
    components: {
        TopFooter
    }
}
</script>

<template>

    <footer>
        <TopFooter />
    </footer>

</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;
</style>
