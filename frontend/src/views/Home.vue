<template>
    <div class="home">
        <!-- <img alt="Vue logo" src="../assets/logo.png">
        <HelloWorld msg="Welcome to Your Vue.js App"/> -->
        <h1>Health Tasker</h1>
        <p>A website that helps you organize and track your daily tasks developing healthy habits</p>
        <div class="entry">
            <button class="entry__login">Login</button>
            <button class="entry__signup">Create Account</button>
        </div>
    </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';
import Login from '@/components/LoginModal.vue';

export default {
    name: 'Home',
    components: {
        HelloWorld,
        Login
    }
}
</script>

<style scoped lang="scss">
    .home{
        width: 100%;
        height: 100%;
        background-color: bisque;
        position: relative;
        z-index: 0;
    }

    p{
        width: 60%;
        margin: auto;
        font-size: 1.4rem;
        padding-top: 20px;
    }

    h1{
        font-family: Arial, Helvetica, sans-serif;
        font-size: 4rem;
        text-align: center;
        padding-top: 10%;
    }

    .entry{
        display: flex;
        flex-direction: row;
        width: 40%;
        margin: auto;
        justify-content: space-between;
        align-items: stretch;
        margin-top: 100px;
        height: 50px;

        & > button{
            width: 40%;
            border: none;
            border-radius: 10px;
            
            font-size: 1.4rem;
            transition: all .2s;
            &:hover{
                cursor: pointer;
                transform: scale(1.1);

            }

        }

        &__login{
            background-color: #42b983;
            color: white;
            &:hover{
                background-color: #329669;
            }
        }

        &__signup{
            background-color: white;
            color: #2c3e50;
            &:hover{
                background-color: #d3d3d3;
            }
        }
    }
</style>