<script>
    // const burger = document.getElementById('#burger'); 

    // burger.addEventListener("click", ()=>{
    //     console.log("ok");
    // })
</script>

<template>
    <header class="header">
        <nav class="navigation">
            <div class="container">
                <div class="navigation__wrap">
                    <img src="/logo.svg" alt="">
                    <div class="burger" id="burger">
                            <span class="bar"></span>
                            <span class="bar"></span>
                            <span class="bar"></span>
                    </div>
                    <div class="navigation__links">
                        <ul class="navigation__links_list" id="menu">
                            <li class="navigation__links_list-item">
                                <a href="#" class="navigation__links_list-link">Возможности</a>
                            </li>
                            <li class="navigation__links_list-item">
                                <a href="#" class="navigation__links_list-link">Как это работает?</a>
                            </li>
                        </ul>
                        <div class="navigation__links_list__reference">
                            <p>г Сургут, ул Базовая, д. 34, офис 10
                                <br> ОГРН 1238600001200 
                                <br> ИНН 8602309464
                            </p>
                            <p>ООО Дотсолюшн © 2023</p>
                        </div>
                        
                    </div>
                </div>
            </div>
        </nav>
        <div class="navigation__links__popup-dark" id="popup"></div>
    </header>
</template>

<style scoped>

</style>
