<template>
    <li>
        <h2>{{ friends.name }}</h2>
        <button @click="toggleDetails">Show Details</button>
        <ul v-if="detailsAreVisible">
            <li><strong>Phone:</strong> {{ friends.phone }}</li>
            <li><strong>Email:</strong> {{ friends.email }}</li>
        </ul>
    </li>
</template>

<script>
export default {
    data() {
        return {
            detailsAreVisible: false,
            friends: {
                    id: 'manuel',
                    name: "Manuel Lorenz",
                    phone: '123 456 7890',
                    email: 'manuel@localhost.com'
                },
        }
    },
    methods: {
        toggleDetails() {
            this.detailsAreVisible = !this.detailsAreVisible
        }
    }
};
</script>