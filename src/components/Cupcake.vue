<template>
    <div class="cupcake">
        <h2>{{ cupcake.title }}</h2>
        <p>{{ cupcake.desc }}</p>
        <ul class="list">
            <li v-for="(name, i) in cupcake.stuff" :key="i">{{ name }};</li>
        </ul>
        <button>Veja Mais</button>
    </div>
</template>

<script>
export default {
    name: "cupcake",
    props: [
        'cupcake'
    ]
};
</script>

<style scoped lang="scss">
.cupcake {
    color: red;
}
</style>

