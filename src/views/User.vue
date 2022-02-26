<template>
    <div>
        <UserList :users="[...users]" />
    </div>
</template>

<script>
import UserList from '../components/UserList.vue';
export default {
    components: { UserList },
    data() {
        return {
            users: [],
            userActivated: {},
        };
    },
    mounted() {
        const users = [
            { id: 10, name: 'Tiago' },
            { id: 20, name: 'Marcos' },
        ];

        this.users = users;
    },
};
</script>

<style></style>
