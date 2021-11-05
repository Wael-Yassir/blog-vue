<template>
    <div>
        <b-navbar type="dark" variant="success">
            <b-icon flip-h="false" icon="vector-pen"/>
            <b-navbar-brand href="#">|BLOGGER</b-navbar-brand>
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
</style>
