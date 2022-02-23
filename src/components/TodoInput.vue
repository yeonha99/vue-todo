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
            if(this.newTodoItme!=""){
                var value = this.newTodoItme&&this.newTodoItme.trim()
                //텍스트의 앞뒤 공백 문자열 제거
                localStorage.setItem(value, value);
                console.log(value)
                this.clearInput()
            }

        }
        ,
        clearInput(){
            this.newTodoItme='';
        }
    }
}
</script>

<style>

</style>