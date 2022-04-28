    <template>
    <div>
        <button v-on:click="updateTitle">Update parent title</button>
    </div>
</template>
<script>
export default {
    name: 'AsifChild',
    methods:{
        updateTitle(){
            this.$emit('changeTitle', "parent updated");
        }
    }
};
</script>
