<template>
    <div class="login-page">
        <h3>INSTA<span>CLONE</span></h3>
        <div class="form-group">
            <input type="text" v-model="email" placeholder="Email">
            <input type="password" v-model="password" placeholder="Password">
            <button class="login-btn">Log in</button>
        </div>
    </div>

</template>

<script>
export default {
    name: 'login',
    data () {
        return {
            email: '',
            password: ''
        }
    }
}
</script>
<style lang="scss" scoped>
.login-page {
    padding: 25px;
}
h3 {
    color: #000;
    font-size: 28px;
    text-align: center;
    font-weight: 900;
    span {
        font-weight: 300;
    }
}

.form-group {
    display: flex;
    justify-content: center;
    flex-flow: column;
    input {
        width: 100%;
        height: 30px;
        border: 1px, solid, #DDD;
        margin-bottom: 15px;
        text-indent: 5px;
        background: #EEE;
        outline: none;

        &:focus {
            border: 1px, solid, #AAA;
        }
    }
    button {
        width: 100%;
        height: 30px;
        background: rgb(30, 88, 245);
        color: white;
        appearance: none;
        border: none;
        outline: none;
        border-radius: 4px;

        font-size: 15px;
        font-weight: 100;
    }
}
</style>