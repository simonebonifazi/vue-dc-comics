<template>
    <div class="footer-top">
        <div class="container d-flex">
            <ul>

            </ul>
            <figure>
                <img id="big-logo" src="../assets/img/dc-logo-bg.png" alt="logo-big">
            </figure>
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterTop"
}
</script>

<style scoped>
.footer-top {
    background-image: url(../assets/img/footer-bg.jpg);

    height: 320px;
}

.container {
    height: 100%;

    justify-content: space-between;
}

#big-logo {
    height: 80%;
}
</style>