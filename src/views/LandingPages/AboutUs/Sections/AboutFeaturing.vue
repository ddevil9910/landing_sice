<script setup>
// example component
import DefaultCounterCard from "../../../../examples/cards/counterCards/DefaultCounterCard.vue";
import computer from "@/assets/img/computadora.png";
import team from "@/assets/img/equipo.png";
import statistics from "@/assets/img/estadistica.png";


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
          <div class="row">
            <div class="col-12">
            </div>
          </div>
          <div class="row">
            <div class="col-md-10">
            <img :src="computer" alt="computadora.png" style="width:100%; height:auto;">
             Nuestro equipo tiene un alto nivel de capacitación en
             las nuevas tecnologías lo que hace que los procesos sean mas rápidos, 
             eficaces y seguros para tí y tu empresa.
            </div>
          </div>
        </div>
        <div class="col-md-3"><br>
             <img :src="statistics" alt="estadistica.png" style="max-width:100%; height:auto;">
                Todos nuestros servicios buscan darte la mejor
              atención para que tengas el resultado que tanto 
              deseas y hagas crecer tu negocio tanto como quieras.
        </div>

        <div class="col-md-3"><br>
             <img :src="team" alt="equipo.png" style="max-width:100%; height:auto;">
             Nuestros servicios son totalmente realizados por 
            un equipo de profesionales con una basta 
            experiencia en el campo laboral para ofrecerte
             un equipo confiable.  
        </div>
      </div>
    </div>

  </section>
</template>
