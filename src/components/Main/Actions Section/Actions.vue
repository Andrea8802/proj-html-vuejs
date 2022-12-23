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

            // Ciclo per azzerare tutti gli elementi active
            this.category.forEach(element => element.active ? element.active = false : "");

            // Assegnazione elemento active
            item.active = true;
        }
    }

}
</script>

<template>

    <!-- Testo blu -->
    <div class="blue-text">
        WE DO MORE FOR EVERYONE
    </div>

    <!-- Title -->
    <div class="title">
        Actions &

        <!-- Title con bg colorato -->
        <div class="bg-title">
            Project
        </div>
    </div>

    <ul>
        <!-- Lista per switchare le categorie -->
        <li v-for="(item, index) in category" :info="item" :key="index" :class="item.active ? 'item-selected' : ''"
            @click="itemClicked(item)">
            {{ item.name }}
        </li>
    </ul>

    <!-- Lista card -->
    <div class="card-list">
        <ActionCards />
    </div>

</template>

<style lang="scss" scoped>
@use '../../../styles/partials/variables' as *;
@use '../../../styles/partials/mixins' as *;

.blue-text {
    font-size: 12px;
}

.title {
    color: white;
    margin: 30px 0;
    font-size: 45px;
}

.bg-title {
    background-color: $dark-bg-title;
    color: white;
    font-size: 45px;
    padding: 3px 10px
}

ul {
    @include d-flex(space-evenly, center);
    gap: 10px;
}

.item-selected {
    background-color: $dark-bg-title;
}

li {
    list-style: none;
    color: white;
    font-size: 15px;
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
