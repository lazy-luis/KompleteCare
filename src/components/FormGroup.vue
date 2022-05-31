<template>
    <h6> {{formTitle}} </h6>
    <div>
        <p :key="item" v-for="item in formItems">
        <input type="checkbox" /> <span>{{item}}</span>
        </p>
    </div>
</template>

<script>
export default {
    name: "FormGroup",
    props: {
        formTitle: String,
        formItems: Array
    }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Manrope:wght@500;600;700&display=swap');
*{
    font-family: 'Manrope', sans-serif;
}
h6{
    font-size: 1.1rem;
    font-weight: 700;
    color: #382F90;
    width: 80%;
    margin: 5px auto;
}
div{
    width: 80%;
    margin: 5px auto;
    display: flex;
    align-items: center;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: flex-start;
    border-bottom: 1px solid #E0E0E0;
    padding-bottom: 18px;
    margin-bottom: 18px;
}
p{
    width: 25%;
    display: flex;
    align-items: center;
    font-size: .8rem;
    font-weight: 600;
    letter-spacing: 1px;
    margin: 10px 0;
    text-transform: capitalize;
}
input{
    display: inline-block;
    margin: 0px 8px;
}
  @media (max-width: 600px) {
    p {
        width: 50%;
    }
  }
</style>