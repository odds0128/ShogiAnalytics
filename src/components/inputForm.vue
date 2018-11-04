<template>
    <div>
        <input style="width:200px" type="text"  v-model="username" placeholder="ユーザー名を入力してください">
        <button v-on:click="sendUsername()">送信</button>
        <p>{{username}}</p>
    </div>
</template>

<script>
export default{
    name: "inputForm",
    data: function(){
        return {
            username: ''
        }
    },
    methods: {
        sendUsername: function(event){
            console.log(this.username)
        }
    }
}
</script>
