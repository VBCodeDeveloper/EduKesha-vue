<script>
// import {Pagination} from '../../node_modules/swiper';

// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from '../../node_modules/swiper/vue';

// Import Swiper styles
import '../../node_modules/swiper/swiper-bundle.min.css';

// Import Swiper styles
export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const onSwiper = (swiper) => {
      console.log(swiper);
    };
    const onSlideChange = () => {
      console.log('slide change');
    };
    return {
      onSwiper,
      onSlideChange,
    //   modules: [Pagination],
    };
  },
};
</script>

<template>
    <div class="opportunities">
        <div class="container">
            <h2>Возможности</h2>
            <div class="row">
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="opportunities__card chet">
                    <div class="opportunities__card-img-wrap">
                        <img src="/public/opportunities_chat.svg" alt="">
                    </div>
                    <div class="opportunities__card-name">
                        <h3>Общение с классом</h3>
                    </div>
                    <div class="opportunities__card-description">
                        <p>Видеосвязь <br>
                        Чат с классом</p>
                    </div>
                </div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="opportunities__card nechet">
                        <div class="opportunities__card-img-wrap">
                            <img src="/public/opportunities_screen.svg" alt="">
                        </div>
                        <div class="opportunities__card-name">
                            <h3>Проведение занятий</h3>
                        </div>
                        <div class="opportunities__card-description">
                            <p>Презентация файлов <br>
                            Демонстрация экрана</p>
                        </div>
                    </div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="opportunities__card chet">
                        <div class="opportunities__card-img-wrap">
                            <img src="/public/opportunities_check.svg" alt="">
                        </div>
                        <div class="opportunities__card-name">
                            <h3>Посещаемость</h3>
                        </div>
                        <div class="opportunities__card-description">
                            <p>Автоматическое <br> отслеживание <br> присутствующих</p>
                        </div>
                    </div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="opportunities__card nechet">
                        <div class="opportunities__card-img-wrap">
                            <img src="/public/opportunities_time.svg" alt="">
                        </div>
                        <div class="opportunities__card-name">
                            <h3>История занятий</h3>
                        </div>
                        <div class="opportunities__card-description">
                            <p>Материалы урока</p>
                        </div>
                    </div>
                </div>
            </div>

            <swiper
                :modules="modules"
                :slides-per-view="1"
                :space-between="50"
                :pagination="{ clickable: true }"
                @swiper="onSwiper"
                @slideChange="onSlideChange"
                class="swiper"
            >
                <swiper-slide>
                <div class="opportunities__card chet">
                <div class="opportunities__card-img-wrap">
                    <img src="/public/opportunities_chat.svg" alt="">
                </div>
                <div class="opportunities__card-name">
                    <h3>Общение с классом</h3>
                </div>
                <div class="opportunities__card-description">
                    <p>Видеосвязь <br>
                    Чат с классом</p>
                </div>
            </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="opportunities__card nechet">
                        <div class="opportunities__card-img-wrap">
                            <img src="/public/opportunities_screen.svg" alt="">
                        </div>
                        <div class="opportunities__card-name">
                            <h3>Проведение занятий</h3>
                        </div>
                        <div class="opportunities__card-description">
                            <p>Презентация файлов <br>
                            Демонстрация экрана</p>
                        </div>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="opportunities__card chet">
                        <div class="opportunities__card-img-wrap">
                            <img src="/public/opportunities_check.svg" alt="">
                        </div>
                        <div class="opportunities__card-name">
                            <h3>Посещаемость</h3>
                        </div>
                        <div class="opportunities__card-description">
                            <p>Автоматическое <br> отслеживание <br> присутствующих</p>
                        </div>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="opportunities__card nechet">
                        <div class="opportunities__card-img-wrap">
                            <img src="/public/opportunities_time.svg" alt="">
                        </div>
                        <div class="opportunities__card-name">
                            <h3>История занятий</h3>
                        </div>
                        <div class="opportunities__card-description">
                            <p>Материалы урока</p>
                        </div>
                    </div>
                </swiper-slide>
                <div class="swiper-pagination"></div>
            </swiper>
        </div>
    </div>
</template>

<style scoped>
</style>
