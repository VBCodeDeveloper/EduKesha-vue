<script>
    export default { 
      data() { 
        return { 
              isActive: false 
            }; 
        }, 
        methods: { 
            toggleClass() { 
                this.isActive = !this.isActive; 
            } 
        } 
    } 
        
</script>

<template>
    <header class="header" id="header">
        <nav class="navigation">
            <div class="container">
                <div class="navigation__wrap">
                    <img src="/logo.svg" alt="">
                    
                    <div class="navigation__links" :class="{ active: isActive }">
                        <ul class="navigation__links_list" :class="{ active: isActive }" id="menu">
                            <li class="navigation__links_list-item">
                                <a href="#" class="navigation__links_list-link">Возможности</a>
                            </li>
                            <li class="navigation__links_list-item">
                                <a href="#" class="navigation__links_list-link">Как это работает?</a>
                            </li>
                        </ul>
                        <div class="navigation__links_list__reference" :class="{ active: isActive }">
                            <p>г Сургут, ул Базовая, д. 34, офис 10
                                <br> ОГРН 1238600001200 
                                <br> ИНН 8602309464
                            </p>
                            <p>ООО Дотсолюшн © 2023</p>
                        </div>
                    </div>
                    <div class="burger" :class="{ active: isActive }" @click="toggleClass">
                            <span class="bar"></span>
                            <span class="bar"></span>   
                            <span class="bar"></span>
                    </div>
                </div>
            </div>
        </nav>
        <div class="navigation__links__popup-dark" :class="{ active: isActive }" id="popup"></div>
    </header>
</template>

<style scoped>

</style>
