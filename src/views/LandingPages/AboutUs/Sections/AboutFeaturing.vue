<script setup>
// example component
import DefaultCounterCard from "../../../../examples/cards/counterCards/DefaultCounterCard.vue";
import computer from "@/assets/img/computadora.png";
</script>
<template>
  <section class="pt-4 pb-6" id="count-stats">
    <div class="container">
      <div class="row mb-7">
        <div class="col-lg-2 col-md-4 col-6 mb-4">
          <img
            class="w-100 opacity-7"
            src="@/assets/img/logos/gray-logos/logo-coinbase.svg"
            alt="logo"
          />
        </div>
        <div class="col-lg-2 col-md-4 col-6 mb-4">
          <img
            class="w-100 opacity-7"
            src="@/assets/img/logos/gray-logos/logo-nasa.svg"
            alt="logo"
          />
        </div>
        <div class="col-lg-2 col-md-4 col-6 mb-4">
          <img
            class="w-100 opacity-7"
            src="@/assets/img/logos/gray-logos/logo-netflix.svg"
            alt="logo"
          />
        </div>
        <div class="col-lg-2 col-md-4 col-6 mb-4">
          <img
            class="w-100 opacity-7"
            src="@/assets/img/logos/gray-logos/logo-pinterest.svg"
            alt="logo"
          />
        </div>
        <div class="col-lg-2 col-md-4 col-6 mb-4">
          <img
            class="w-100 opacity-7"
            src="@/assets/img/logos/gray-logos/logo-spotify.svg"
            alt="logo"
          />
        </div>
        <div class="col-lg-2 col-md-4 col-6 mb-4">
          <img
            class="w-100 opacity-7"
            src="@/assets/img/logos/gray-logos/logo-vodafone.svg"
            alt="logo"
          />
        </div>
      </div>
      <div class="row justify-content-center text-center">
        <div class="col-md-3">
          <DefaultCounterCard
           
            description="Nuestro equipo tiene un alto nivel de capacitación en
             las nuevas tecnologías lo que hace que los procesos sean mas rápidos, 
             eficaces y seguros para ti y tu empresa."
            :image="5234"
            :duration="3000"
          />
        </div>
        <div class="col-md-3">
          <DefaultCounterCard
           
            description="Todos nuestros servicios buscan darte la mejor
             atención para que tengas el resultado que tanto 
             deseas y hagas crecer tu negocio tanto como quieras."
            :count="3400"
            suffix="+"
            :duration="3000"
          />
        </div>
        <div class="col-md-3">
          <DefaultCounterCard
           
            description="Nuestros servicios son totalmente realizados por 
            un equipo de profesionales con una basta 
            experiencia en el campo laboral para ofrecerte
             un equipo confiable."
            :count="24"
            suffix="/7"
            :duration="4000"
          />
        </div>
      </div>
    </div>
  </section>
</template>
