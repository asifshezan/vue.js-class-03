    <template>
    <div>
        <h1>Child Component</h1>
        <!-- <h2>{{ name }}</h2> -->
        <table border="1">
            <tr>
                <th>Name</th>
                <th>Email</th>
            </tr>
            <tr v-for="user in users" :key="user.name">
                <td>{{ user.name }}</td>
                <td>{{ user.email }}</td>
            </tr>
        </table>
    </div>
</template>
<script>
export default {
    name: 'AsifChild',
    props:['users']

};
</script>