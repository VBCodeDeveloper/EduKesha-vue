<script setup>
// // eslint-disable-next-line
import Swiper from "swiper";
import { Pagination, Navigation } from "swiper/modules";
import { onMounted } from "vue";
// import 'swiper/swiper-bundle.min.css';

onMounted(() => {
  const swiper = new Swiper(".swiper", {
    modules: [Pagination, Navigation],
    // Optional parameters
    direction: "horizontal",
    loop: true,
    spaceBetween: 30,
    // If we need pagination
    pagination: {
      el: ".swiper-pagination",
    },
  });
});
</script>
<template>
  <div class="opportunities">
    <div class="container">
      <h2>Возможности</h2>
      <div class="row">
        <div class="col-12 col-md-6 col-lg-3">
          <div class="opportunities__card chet">
            <div class="opportunities__card-img-wrap">
              <img src="/public/opportunities_chat.svg" alt="" />
            </div>
            <div class="opportunities__card-name">
              <h3>Общение с классом</h3>
            </div>
            <div class="opportunities__card-description">
              <p>
                Видеосвязь <br />
                Чат с классом
              </p>
            </div>
          </div>
        </div>
        <div class="col-12 col-md-6 col-lg-3">
          <div class="opportunities__card nechet">
            <div class="opportunities__card-img-wrap">
              <img src="/public/opportunities_screen.svg" alt="" />
            </div>
            <div class="opportunities__card-name">
              <h3>Проведение занятий</h3>
            </div>
            <div class="opportunities__card-description">
              <p>
                Презентация файлов <br />
                Демонстрация экрана
              </p>
            </div>
          </div>
        </div>
        <div class="col-12 col-md-6 col-lg-3">
          <div class="opportunities__card chet">
            <div class="opportunities__card-img-wrap">
              <img src="/public/opportunities_check.svg" alt="" />
            </div>
            <div class="opportunities__card-name">
              <h3>Посещаемость</h3>
            </div>
            <div class="opportunities__card-description">
              <p>
                Автоматическое <br />
                отслеживание <br />
                присутствующих
              </p>
            </div>
          </div>
        </div>
        <div class="col-12 col-md-6 col-lg-3">
          <div class="opportunities__card nechet">
            <div class="opportunities__card-img-wrap">
              <img src="/public/opportunities_time.svg" alt="" />
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
      <!-- Slider main container -->
      <div class="swiper">
        <!-- Additional required wrapper -->
        <div class="swiper-wrapper">
          <!-- Slides -->
          <div class="swiper-slide">
            <div class="opportunities__card chet">
              <div class="opportunities__card-img-wrap">
                <img src="/public/opportunities_chat.svg" alt="" />
              </div>
              <div class="opportunities__card-name">
                <h3>Общение с классом</h3>
              </div>
              <div class="opportunities__card-description">
                <p>
                  Видеосвязь <br />
                  Чат с классом
                </p>
              </div>
            </div>
          </div>
          <div class="swiper-slide">
            <div class="opportunities__card nechet">
              <div class="opportunities__card-img-wrap">
                <img src="/public/opportunities_screen.svg" alt="" />
              </div>
              <div class="opportunities__card-name">
                <h3>Проведение занятий</h3>
              </div>
              <div class="opportunities__card-description">
                <p>
                  Презентация файлов <br />
                  Демонстрация экрана
                </p>
              </div>
            </div>
          </div>
          <div class="swiper-slide">
            <div class="opportunities__card chet">
              <div class="opportunities__card-img-wrap">
                <img src="/public/opportunities_check.svg" alt="" />
              </div>
              <div class="opportunities__card-name">
                <h3>Посещаемость</h3>
              </div>
              <div class="opportunities__card-description">
                <p>
                  Автоматическое <br />
                  отслеживание <br />
                  присутствующих
                </p>
              </div>
            </div>
          </div>
          <div class="swiper-slide">
            <div class="opportunities__card nechet">
              <div class="opportunities__card-img-wrap">
                <img src="/public/opportunities_time.svg" alt="" />
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
        <br>
        <br>
        <!-- If we need pagination -->
        <div class="swiper-pagination"></div>

      </div>
    </div>
  </div>
</template>

<style scoped></style>
