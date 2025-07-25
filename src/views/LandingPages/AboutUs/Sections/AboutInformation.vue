<script setup>
// example components
import DefaultInfoCard from "../../../../examples/cards/infoCards/DefaultInfoCard.vue";
import CenteredBlogCard from "../../../../examples/cards/blogCards/CenteredBlogCard.vue";
import rocket from "@/assets/img/cohete.png";
</script>
<template>
  <section class="py-7">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-12">
          <div class="row justify-content-start">
            <div class="row full-width">
              <div class="col-12 col-md-6">
                <h1 class="red-sice" >SOMOS</h1>
                <br>
                <h4 class="red-sice">Misi&oacute;n</h4>
                <p>Ofrecer servicios de alta calidad, que garanticen a nuestros clientes 
                  seguridad jurídica, financiera y administrativa; y así poder contribuir a su desarrollo empresarial.
                </p>
                <br>
                <h4 class="red-sice">Visi&oacute;n</h4>
                <p>Ser una empresa prestigiada y reconocida en el ámbito financiero, administrativo y fiscal, que ayude 
                  al crecimiento y desarrollo de los proyectos de cada uno de nuestros clientes a través de asesorías personalizadas
                   impartidas por nuestros especialistas en cada área.</p>
              </div>
              <div class="col-12 col-md-6">
                <img :src="rocket" class="rocket-image">
              </div>
            </div>
            <hr style="border:1px solid grey; width: 100%">
            <div class="row">
              <div class="col-12 col-md-6">
                <img src="" alt="">
              </div>
              <div class="col-12 col-md-6">
                <h1 class="blue-sice" >VALORES</h1>
              </div> 
            </div>


            <!-- <DefaultInfoCard
              color="Info"
              title="SOMOS"
              description="We get insulted by others, lose trust for those We get back
                  freezes"
            />
            <DefaultInfoCard
              color="Info"
              title="Misión"
              description="Ofrecer servicios de alta calidad, que garanticen a nuestros clientes seguridad jurídica, financiera y administrativa; y así poder contribuir a su desarrollo empresarial."
            />
            <DefaultInfoCard
              color="Info"
              title="Visión"
              description="Ser una empresa prestigiada y reconocida en el ámbito financiero, administrativo y fiscal, que ayude al crecimiento y desarrollo de los proyectos de cada uno de nuestros clientes a través de asesorías personalizadas impartidas por nuestros especialistas en cada área."
            /> -->
          </div>
        </div>
        <!-- <div class="col-lg-4 ms-auto mt-lg-0 mt-6"> -->
          <!-- <CenteredBlogCard
            image="file:///C:/Users/Sherlyn/Downloads/mundo%2002.svg"
            title="Get insights on Search"
            description="Website visitors today demand a frictionless user expericence — especially when using search. Because of the hight standards."
          /> -->
        <!-- </div> -->
      </div>
    </div>
  </section>
</template>

<style scoped>
.full-width{
  width: 100%;
}
.rocket-image{
  max-width: 100%;
}
.red-sice {
  color: #cc1d1d;
}
.blue-sice{
  color:#3576de
}
</style>
