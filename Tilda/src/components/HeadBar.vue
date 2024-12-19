<template>
    <div class="header-container">
        <h1>Tilda publishing</h1>
        <nav>
            <router-link to="/">
                <p class="nav-link">Главная</p>
            </router-link>
            <router-link to="/pricing">
                <p class="nav-link">Тарифы</p>
            </router-link>
            <router-link to="/report">
                <p class="nav-link">Сообщить о нарушении</p>
            </router-link>
        </nav>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.header-container {
    height: 50px;
    display: flex;
    width: 1200px;
    margin: 0 auto;
    margin-bottom: 105px;
    align-items: center;
    justify-content: space-between;
}

h1 {
    font-size: 16px;
    font-weight: 700;
}

nav {
    display: flex;
    align-items: center;
    height: 100%;
    font-size: 12px;
}

.nav-link{
    text-transform: uppercase;
    margin-left: 18px;
    font-weight: 300;
}
</style>