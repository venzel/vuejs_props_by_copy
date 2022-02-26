<template>
    <div class="users">
        <ul>
            <li v-for="user in users" :key="user.id">{{ user.name }}</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'UserList',
    props: {
        users: {
            type: Array,
            default: [],
        },
    },
};
</script>

<style></style>
