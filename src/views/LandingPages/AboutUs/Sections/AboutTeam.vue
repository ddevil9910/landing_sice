<script setup>
// example component
import HorizontalTeamCard from "@/examples/cards/teamCards/HorizontalTeamCard.vue";

// images
import Julissa from "@/assets/img/Jgonzalez.png";
import Omar from "@/assets/img/Omorales.png";
</script>

<template>
  <section class="pb-5 position-relative bg-gradient-dark mx-n3">
    <div class="container">
      <div class="row">
        <div class="col-md-8 text-start mb-5 mt-5">
          <h3 class="text-white z-index-1 position-relative">
            Equipo de profesionales
          </h3>
          <p class="text-white opacity-8 mb-0">
            There’s nothing I really wanted to do in life that I wasn’t able to
            get good at. That’s my skill.
          </p>
        </div>
      </div>
      <div class="row">
        <div class="col-12 col-md-6">
          <HorizontalTeamCard
            class="mt-4"
            :image="Julissa"
            :profile="{ name: 'Julissa González', link: 'javascript:;' }"
            :position="{ label: 'CO-FOUNDER', color: 'succes' }"
            description="Contadora Pública egresada de la Escuela Superior de Comercio y 
            Administración (I.P.N.), con 10 años de experiencia en materia fiscal y
             contable."
       
          />

        </div>
      </div>
      <div class="row mt-4">
        <div class="col-12 col-md-6">
          <HorizontalTeamCard
            class="mt-4 z-index-2"
            :image="Omar"
            :profile="{ name: 'Omar Morales', link: 'javascript:;' }"
            :position="{ label: 'CO-FOUNDER', color: 'succes' }"
            description="Contador Público egresado de la Escuela Superior de Comercio y
             Administración (I.P.N.), con más de 15 años de experiencia en materia fiscal  
             contable y catedrático del Instituto Universitario Anáhuac."
          />
       
        </div>
      </div>
    </div>
  </section>
</template>
