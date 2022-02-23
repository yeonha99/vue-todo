<template>
    <div>
        <input type="text" v-model="newTodoItme">
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
            localStorage.setItem(this.newTodoItme, this.newTodoItme);
            console.log(this.newTodoItme)
        }
    }
}
</script>

<style>

</style>