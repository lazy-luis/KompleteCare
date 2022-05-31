<template>
    <div>
        <a href="#" class="active">
            <img src="../assets/dashboard.svg" />
            <span> Dasboard </span>
        </a>
        <a href="#">
            <img src="../assets/profile.svg" />
            <span> Profile </span>
        </a>
        <a href="#">
            <img src="../assets/services.svg" />
            <span> Services </span>
            <img src="../assets/arrow_down.svg" />
        </a>
        <a href="#">
            <img src="../assets/medical.svg" />
            <span> Medical Records </span>
        </a>
        <a href="#">
            <img src="../assets/wallet.svg" />
            <span> Care Wallet </span>
        </a>
        <a href="#">
            <img src="../assets/messages.svg" />
            <span> Messages </span>
        </a>
        <a href="#">
            <img src="../assets/resources.svg" />
            <span> Resources </span>
        </a>
        <div class="accountDetails">
            <a href="#">
                <img src="../assets/settings.svg" />
                <span> Account Settings </span>
            </a>
            <a href="#">
                <img src="../assets/support.svg" />
                <span> Contact Support </span>
            </a>
            <a href="#">
                <img src="../assets/logout.svg" />
                <span> Logout </span>
            </a>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SideBar'
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Lexend+Deca&display=swap');

*{
    font-family: 'Lexend Deca', sans-serif;
}
div {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    flex-wrap: nowrap;
    margin-top:10vh;
    box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.12);
    height: 90vh;
}

.accountDetails{
    border-top: 1px solid #DFE0EB;
    margin-top: 12px;
    padding-top: 12px;
    box-shadow: unset;
    height: auto;
    width: 100%;
}

a{
    display:block;
    padding: 12px 0;
    margin: 2px 0;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    align-items: center;
    justify-content: space-around;
    width: 100%;
    font-size: .9rem;
    font-weight: 400;
    color: #A0A0A0;
}

a img{
    width: 12px;
    aspect-ratio: 1/1;
    display: inline-block;
    margin: 5px 12px;
}

a span{
    width: 80%;
}

a.active {
    background: #2A36A4;
    color: #ffffff;
}
</style>