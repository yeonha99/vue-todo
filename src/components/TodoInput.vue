<template>
    <div>
        <input type="text" v-model="newTodoItmes">
        <button v-on:click="addTodo">추가</button>
        
    </div>
</template>

<script>
export default {
    data(){
        return{
            newTodoItme:' '
        }
    },
    methods: {
        addTodo(){
            console.log(this.newTodoItmes);
        }
    },
}
</script>

<style>

</style>