<script setup>
const card = [ 
    {
     img: {
        src: "/schadule.png", 
        alt: "Составьте расписание"
     }, 
     link: { 
        href: "#", 
        title: "Составьте расписание"
     }, 
     description: "Выберите время, предмет и класс. Ученики получат уведомление о предстоящем уроке."   
    }, 

    {
     img: {
        src: "/schadule_docs.png", 
        alt: "Подготовьте материал"
     }, 
     link: { 
        href: "#", 
        title: "Подготовьте материал"
     }, 
     description: "Загружайте необходимые материалы к уроку."   
    }, 

    {
     img: {
        src: "/schadule_work.png", 
        alt: "Начните урок с учениками"
     }, 
     link: { 
        href: "#", 
        title: "Начните урок с учениками"
     }, 
     description: "Задавайте вопросы и вызывайте «к доске» детей с поднятой рукой."   
    }, 

]

</script>

<template>
    <div class="schaduleWork">
        <div class="container">
             <h2>Как это работает?</h2>
             <div class="row">
                    <div class="col-sm-6 col-lg-4"
                        v-for="(item, index) in card"
                        :key="index">
                        <div class="schaduleWork-card">
                            <img :src="item.img.src" :alt="item.img.alt">
                            <div class="schaduleWork-card-text">
                                <a :href="item.link.href">{{item.link.title}}</a>
                                <p>{{item.description}}</p>
                            </div>
                        </div>
                    </div>  
                </div>
        </div>
    </div>
</template>

<style scoped>

</style>
