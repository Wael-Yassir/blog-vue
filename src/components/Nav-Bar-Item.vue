<template>
    <div style='margin-bottom: 45px;'>
        <b-navbar type="dark" variant="success">
            <b-icon :flip-h="false" icon="vector-pen"/>
            <b-navbar-brand href="#">|BLOGGER</b-navbar-brand>
            <div id="nav">
                <router-link to="/">Home</router-link> |
                <router-link to="/about">About</router-link>
            </div>
        </b-navbar>
    </div>
</template>

<script>
export default {
  name: 'Nav-Bar-Item'
}
</script>

<style>
    a.navbar-brand {
        margin-left: 10px;
        font-family: 'Zen Kurenaido', sans-serif;
        letter-spacing: 10px;
        font-weight: 500;
    }

    svg.bi-vector-pen {
        margin-left: 10px;
        color: white;
    }

    #nav a {
        color: white;
        text-decoration: none;
        font-family: 'Zen Kurenaido', sans-serif;
        letter-spacing: 3px;
        font-weight: 500;
        font-size: 20px;
        margin: 0 5px;
    }

    #nav {
        color: white;
        margin-left: auto;
        margin-right: 5px;
    }
</style>
