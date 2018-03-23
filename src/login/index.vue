<template >
    <div class="login">
        <input type="text" v-model="user">
        <input type="text" v-model="password">
        <button>登录</button>
    </div>
</template>
<script>
    export default{
        data(){
            return {
                user:'',
                password:'',
            }
        },
        mounted:function(){
            alert()
        },
        methods:{

        }
    }
</script>
<style lang="less">
    .login{
        width: 200px;
        height: 200px;
        input{
            width: 120px;
            margin: auto;
            margin-top: 20px;
        }
        button{
            width: 100px;
            height: 30px;
            margin: auto;
            margin-top: 20px;
        }
    }
</style>
