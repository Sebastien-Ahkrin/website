<template>
    <div>
        <router-link to="/"><navigation-logo></navigation-logo></router-link>
        <router-link to="/articles">Articles</router-link>
    </div>
</template>

<script>
import NavigationLogo from './NavigationLogo.vue';

export default {
    name: 'navigation-left',
    components: {
        NavigationLogo,
    }
};
</script>

<style scoped>
a, a:visited {
    color: #d1d1d1;
    text-decoration: none;
    transition: text-shadow 100ms, color 100ms;
}

a:hover {
    color: #ffffff;
    text-shadow: 0 0 5px rgba(255, 255, 255, 0.5);
}

a {
    display: inline-block;

    padding-left: 20px;
    padding-right: 20px;

    font-size: 18px;
    font-weight: bold;

    height: 70px;
    vertical-align: top;
    line-height: 60px;
}

svg.navigation-logo {
    padding-right: 20px;
}

div {
    margin: 0;
    padding: 0;
    padding-top: 5px;
    height: 60px;
    width: auto;
}
</style>
