<template>
    <form>
        <h1>Log In</h1>
        <div>
            <label for="email">Email</label>
            <input type="text" name="email" required>
            <div style="height: 10px"></div>
            <label for="email">Password</label>
            <input type="password" name="password" required>
            <button>Log In</button>
        </div>
    </form>
</template>

<script>

export default {
    name: 'LoginModal',
}
</script>

<style scoped lang="scss">
    form{
        border-radius: 10px;
        background-color: white;
        width: clamp(300px, 25%, 30%);
        height: 60%;
        position: absolute;
        z-index: 10;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }

    div{
        width: 80%;
        margin: auto;
        display: flex;
        flex-direction: column;
        align-items: stretch;

        & > label{
            text-align: left;
        }

        & > input{
            padding: 10px 15px;
            border-radius: 10px;
            border: solid 1px #bfbfbf;
            font-size: 1rem;
            outline: none;

            &:focus{
                // outline: solid #42b983;
                border: solid 1px #42b983;
            }

        }

        & > button{
            margin-top: 25px;
            background-color: #42b983;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 1.4rem;
            border-radius: 10px;

            &:hover{
                cursor: pointer;
                background-color: #329669;
            }
        }
    }

    h1{
        padding-top: 20px;
        text-align: center;

    }
</style>
