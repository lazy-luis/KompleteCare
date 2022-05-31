<template>
    <MainHeader />
    <h6> Update Patient Medical Record </h6>
    <p> Click the tabs to view and edit patient medical details </p>
    <MainForm />
</template>

<script>
import MainHeader from './MainHeader.vue';
import MainForm from './MainForm.vue';
export default {
    name: "MainBody",
    components: { MainHeader, MainForm }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Manrope:wght@500;700&display=swap');
    *{
        font-family: 'Manrope', sans-serif;
    }
    h6{
        font-size: 2rem;
        width: 80%;
        margin: 8px auto;
        font-weight: 700;
        color: #382F90;
    }
    p{
        font-size: 1rem;
        width: 80%;
        margin: 8px auto;
        font-weight: 500;
        color: #9FA2B4;
    }
</style>