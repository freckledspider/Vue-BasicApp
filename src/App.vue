<template>
<section>
    <h2>My Friends</h2>
    <ul>
        <friend-contact></friend-contact>
        <friend-contact></friend-contact>
    </ul>
</section>
</template>

<script>
export default {
    data() {
        return {
            friends: [
                {
                    id: 'manuel',
                    name: "Manuel Lorenz",
                    phone: '123 456 7890',
                    email: 'manuel@localhost.com'
                },
                {
                    id: 'julie',
                    name: "Julie Jones",
                    phone: '098 765 4321',
                    email: 'julie@localhost.com'
                }
            ]
        }
    }
};
</script>