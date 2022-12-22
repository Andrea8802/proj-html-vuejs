<script>
import ActionCards from './ActionCards.vue';
export default {
    name: "Actions",
    components: {
        ActionCards
    },

    data() {
        return {
            category: [
                {
                    name: "ALL",
                    active: true
                },

                {
                    name: "INSTITUTIONAL",
                    active: false
                },

                {
                    name: "SOCIAL",
                    active: false
                },

                {
                    name: "EVENTS",
                    active: false
                },

                {
                    name: "INNOVATION",
                    active: false
                },

                {
                    name: "ENVIROMENT",
                    active: false
                },

                {
                    name: "TECHNOLOGY",
                    active: false
                }
            ]
        }
    },
    methods: {
        itemClicked(item) {
            this.category.forEach(element => element.active ? element.active = false : "")
            item.active = true;
        }
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
        <li v-for="(item, index) in category" :info="item" :key="index" :class="item.active ? 'item-selected' : ''"
            @click="itemClicked(item)">
            {{ item.name }}
        </li>
    </ul>

    <div class="card-list">
        <ActionCards />
    </div>

</template>

<style lang="scss" scoped>
@use '../../../styles/partials/variables' as *;
@use '../../../styles/partials/mixins' as *;

.title {
    font-weight: bold;
    font-size: 40px;
    color: white;
    margin: 30px 0;
}

.bg-title {
    background-color: $dark-bg-title;
    color: white;
}

ul {
    @include d-flex(space-evenly, center);
    gap: 10px;
}

.item-selected {
    background-color: $dark-bg-title;
    text-decoration: underline;
}

li {
    list-style: none;
    color: white;
    font-size: 16px;
    padding: 5px 10px;
    cursor: pointer;

    &:hover {

        background-color: $dark-bg-title;
    }
}

.card-list {
    margin-top: 30px;
    @include d-flex(center, center);
    flex-wrap: wrap;
    gap: 50px;
    width: 80%;
}
</style>
