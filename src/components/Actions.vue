<script>
import ActionCards from './ActionCards.vue';
export default {
    name: "Actions",
    components: {
        ActionCards
    }

}
</script>

<template>
    <div class="blue-text">
        WE DO MORE FOR EVERYONE
    </div>

    <div class="title">
        Actions &
        <div class="bg-title">
            Project
        </div>
    </div>

    <ul>
        <li>
            B
        </li>

        <li>
            B
        </li>

        <li>
            B
        </li>

        <li>
            B
        </li>

        <li>
            B
        </li>

        <li>
            B
        </li>
    </ul>

    <div class="card-list">
        <ActionCards />
    </div>

</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.title {
    font-weight: bold;
    font-size: 40px;
    color: white;
    margin: 30px 0;
}

.bg-title {
    background-color: #0e272d;
    color: white;
}

ul {
    @include d-flex(space-evenly, center);
    gap: 50px;
}

li {
    list-style: none;
    color: white;
}

.card-list {
    margin-top: 30px;
    @include d-flex(center, center);
    flex-wrap: wrap;
    gap: 50px;
    width: 80%;
}
</style>
