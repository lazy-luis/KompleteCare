<template>
    <div>
        <FormGroup formTitle="X-Ray" :formItems="formList" />
        <FormGroup formTitle="Ultrasound Scan" :formItems="formList" />
        <FormSelects />
        <button> Save and Send </button>
    </div>
</template>

<script>
import FormGroup from './FormGroup.vue';
import FormSelects from './FormSelects.vue';
import axios from "axios";
export default {
    name: "MainForm",
    components: { FormGroup, FormSelects },
    data(){
        this.formList = ["chest", "elbow", "wrist", "head", "toe", "foot", "Thoraco Lumbar Vertebrae"]
    },
    async created() {
        const loginData = {
            email: "tester@kompletecare.com",
            password: "password"
        }
        await axios.get("https://testdrive.kompletecare.com/api/investigations", 
        {headers: { 
            'Accept': 'application/json',
            'Authorization': 'Bearer 5|xK9ypbpdQU2qEBa7AuRO016OuyJtYwFlBcSAFVLJ'
        }}).then((data)=>console.log(data))
    }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Manrope:wght@500;600;700&display=swap');
    div{
        background: #ffffff;
        width: 80%;
        margin: 40px auto;
        padding: 40px 0;
        border-radius: 5px;
    }
    button{
        padding: 15px;
        margin-left: 75%;
        align-self: flex-end;
        text-align: center;
        background: #382F90;
        color: #ffffff;
        border-radius: 7px;
        font-weight: 700;
        font-size: .9rem;
        font-family: 'Manrope', sans-serif;
    }
  @media (max-width: 600px) {
    div{
        background: #ffffff;
        width: 95%;
    }
    button{
        margin-left: 60%;
    }
  }
</style>