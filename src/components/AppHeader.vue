<script>
export default {
    name: "AppHeader",
    data() {
        return {
            menu: [
                {
                    title: "Characters",
                    url: "/characters",
                    active: false
                },
                {
                    title: "Comics",
                    url: "/comics",
                    active: true
                },
                {
                    title: "Movies",
                    url: "/movies",
                    active: false
                },
                {
                    title: "TV",
                    url: "/tv",
                    active: false
                },
                {
                    title: "Games",
                    url: "/games",
                    active: false
                }
            ]
        }
    }
}
</script>


<template>
    <header>
        <div class="container flex-row justify-between">
            <div class="logo">
                <a href="">
                    <img src="../assets/img/dc-logo.png" alt="">
                </a>
            </div>
            <div class="menu">
                <nav>
                    <ul>
                        <li v-for="(link, index) in menu" :key="index">
                            <a :class="{ `active`: link.active }" :href="link.url">
                                {{ link.title }}
                            </a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
</template>

<style>
header{
    width: 80%;
    height: 200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    border: 1px solid;
    align-items: center;
}

ul{
    display: flex;
}

li{
    list-style-type: none;
    margin: .4rem;
}
</style>
