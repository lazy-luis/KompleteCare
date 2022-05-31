<template>
    <section>
        <div>
            <label> CT Scan </label>
            <select>
                <option> *Specify </option>
            </select>
        </div>
        <div>
            <label> MRI </label>
            <select>
                <option> *Specify </option>
            </select>
        </div>
    </section>
</template>

<script>
export default {
    name: "FormSelects"
}
</script>

<style scoped>
    *{
        color: #9FA2B4;
    }

    section{
        display: flex;
        flex-direction: row;
        flex-wrap: nowrap;
        align-items: center;
        justify-content: space-around;
        padding: 20px 0;
        width: 80%;
        margin: 5px auto;
    }

    div{
        width: 45%;
    }

    label{
        font-size: .9rem;
        font-weight: 600;
        display: block;
    }

    select{
        width: 90%;
        margin: 10px 0;
        padding: 12px;
        background: transparent;
        border: 1px solid #C4C4C4;
        border-radius: 5px;
    }

    @media (max-width: 600px) {
        section{
            width: 90%;
        }

        div{
            width: 50%;
        }
    }

    
</style>