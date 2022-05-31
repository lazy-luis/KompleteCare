<template>
    <div>
        <a href="#"> Take a tour </a>
        <img src="../assets/message.svg" />
        <img src="../assets/bell.svg" />
        <img src="../assets/user.svg" />
    </div>
</template>

<script>
export default {
    name: 'MainHeader'
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Manrope:wght@600&display=swap');
    div {
        width: 95%;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        padding: 40px 0;
    }

    a{
        color: #382F9099;
        display: inline-block;
        margin: 5px 20px;
        font-family: 'Manrope', sans-serif;
        font-weight: 600;
    }

    img{
        display: inline-block;
        margin: 0 12px;
    }
</style>