<script>
export default {
    props: ['src', 'alt', 'title', 'description', 'links']
}
</script>

<template>
    <div class="card card-hover" style="width: 18rem">
        <!-- <img src="..." class="card-img-top" alt="..." /> -->
        <div class="card-body">
            <h5 class="card-title">{{title}}</h5>
            <p class="card-text">{{description}}</p>
        </div>
        <div class="card-footer">
            <a :href="link" v-for="(link, index) in links"
            :key="index"
            >click here to open</a>
        </div>
    </div>
</template>

<style scoped>
    .card-hover{
        margin-bottom: 30px;
        transition: all 0.5s;
    }
    .card-hover:hover{
        transform: translateY(-10px);
        background-color: rgb(150, 211, 206);
    }
    </style>