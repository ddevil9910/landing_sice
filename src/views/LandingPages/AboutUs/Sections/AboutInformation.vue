<script setup>
// example components
import ideas from "@/assets/img/ideas.jpg";
import office from "@/assets/img/oficina.jpg";

function randomStyle(i) {
  // Genera estilos aleatorios para cada partícula
  const size = Math.random() * 6 + 4;             // tamaño entre 4px y 10px
  const left = Math.random() * 100;               // posición horizontal %
  const duration = 10 + Math.random() * 10;       // duración entre 10s y 20s
  const delay = Math.random() * -20;              // inicio adelantado negativo
  const opacity = Math.random() * 0.5 + 0.3;
  return {
    width: `${size}px`,
    height: `${size}px`,
    left: `${left}%`,
    animationDuration: `${duration}s`,
    animationDelay: `${delay}s`,
    background: 'radial-gradient(circle, rgba(106, 147, 185, 1) 0%, rgba(0,123,255,0) 60%)',
    opacity,
  };
}


</script>
<template>
  <section class="py-7">
    <div class="container">
      <div class="row align-items-center">
         <div class="particle-layer">
          <span
            v-for="i in 30"
            :key="i"
            class="particle"
            :style="randomStyle(i)"
            ></span>
          </div>
        <div class="col-12">
          <div class="row justify-content-start">
            <div class="row elevated-card full-width">
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
                <img :src="ideas" class="ideas-image">
              </div>
              <div class="col-12 col-md-6 mt-6">
                <img :src="office" class="ideas-image">
              </div>
              <div class="col-12 col-md-6 mt-6">
                <h1 class="blue-sice" >VALORES</h1>
                <p> <span class="has-inline-color"><b><span style="font-size: 20px; font-family: 'Arial',sans-serif; color: #cf2e2e; text-transform: uppercase;">S</span></b></span><span class="has-inline-color"><b><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #0693e3;">eguridad</span></b></span><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #748182;">. Brindar a nuestros clientes las mejores estrategias de crecimiento empresarial respaldándonos en la ética profesional con la que cuenta cada integrante de SICE.</span></p>
                <p> <span class="has-inline-color"><b><span style="font-size: 20px; font-family: 'Arial',sans-serif; color: #cf2e2e; text-transform: uppercase;">I</span></b></span><span class="has-inline-color"><b><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #0693e3;">ntegridad</span></b></span><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #748182;">. Poner al servicio de nuestros clientes personal ético, profesional y responsable, que brinde apropiadamente nuestra amplia gama de servicios y asesorías.</span></p>             
                <p> <span class="has-inline-color"><b><span style="font-size: 20px; font-family: 'Arial',sans-serif; color: #0693e3;">C</span></b></span><span class="has-inline-color"><b><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #cf2e2e;">alidad</span></b></span><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #748182;">. Presentar proyectos organizados, dirigidos y éticos que ayuden a nuestros clientes a tener un desarrollo empresarial exitoso.</span></p>
                <p> <span class="has-inline-color"><b><span style="font-size: 20px; font-family: 'Arial',sans-serif; color: #0693e3;">E</span></b></span><span class="has-inline-color"><b><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #cf2e2e;">strategia</span></b></span><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #748182;">. Sugerir los procedimientos y mecanismos más adecuados que lleven al cumplimiento de las metas de nuestros clientes, sin poner en riesgo su seguridad administrativa o financiera y a su vez cumpliendo con los objetivos trazados que sean redituables y confortables para nuestros clientes.</span></p>
             </div> 
            </div>
            <!-- <div class="row elevated-card space-sup">
              <div class="col-12 col-md-6">
                <img :src="office" class="ideas-image">
              </div>
              <div class="col-12 col-md-6">
                <h1 class="blue-sice" >VALORES</h1>
                <p> <span class="has-inline-color"><b><span style="font-size: 20px; font-family: 'Arial',sans-serif; color: #cf2e2e; text-transform: uppercase;">S</span></b></span><span class="has-inline-color"><b><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #0693e3;">eguridad</span></b></span><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #748182;">. Brindar a nuestros clientes las mejores estrategias de crecimiento empresarial respaldándonos en la ética profesional con la que cuenta cada integrante de SICE.</span></p>
                <p> <span class="has-inline-color"><b><span style="font-size: 20px; font-family: 'Arial',sans-serif; color: #cf2e2e; text-transform: uppercase;">I</span></b></span><span class="has-inline-color"><b><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #0693e3;">ntegridad</span></b></span><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #748182;">. Poner al servicio de nuestros clientes personal ético, profesional y responsable, que brinde apropiadamente nuestra amplia gama de servicios y asesorías.</span></p>             
                <p> <span class="has-inline-color"><b><span style="font-size: 20px; font-family: 'Arial',sans-serif; color: #0693e3;">C</span></b></span><span class="has-inline-color"><b><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #cf2e2e;">alidad</span></b></span><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #748182;">. Presentar proyectos organizados, dirigidos y éticos que ayuden a nuestros clientes a tener un desarrollo empresarial exitoso.</span></p>
                <p> <span class="has-inline-color"><b><span style="font-size: 20px; font-family: 'Arial',sans-serif; color: #0693e3;">E</span></b></span><span class="has-inline-color"><b><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #cf2e2e;">strategia</span></b></span><span style="font-size: 11.5pt; font-family: 'Arial',sans-serif; color: #748182;">. Sugerir los procedimientos y mecanismos más adecuados que lleven al cumplimiento de las metas de nuestros clientes, sin poner en riesgo su seguridad administrativa o financiera y a su vez cumpliendo con los objetivos trazados que sean redituables y confortables para nuestros clientes.</span></p>
             </div> 
            </div> -->
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.full-width{
  width: 100%;
}
.ideas-image{
  max-width: 100%;
}
.red-sice {
  color: #cc1d1d;
}
.blue-sice{
  color:#3576de
}
.elevated-card{
  border-radius: 12px;
  padding: 24px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.262);
}
.space-sup{
  margin-top: 20px;
}

/*estilos delas particulas*/ 

.row-with-particles {
  position: relative;
  overflow: hidden;
  min-height: 200px;
  background: #021027; /* color de fondo de la fila */
}
.particle-layer {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 0;
}
.particle {
  position: absolute;
  border-radius: 50%;
  animation-name: move, fade;
  animation-timing-function: linear;
  animation-iteration-count: infinite;
}
@keyframes move {
  from { transform: translateY(100vh); }
  to   { transform: translateY(-10vh); }
}
@keyframes fade {
  0%   { opacity: 1; }
  50%  { opacity: 0.7; }
  100% { opacity: 1; }
}
.contenido {
  position: relative;
  z-index: 1;
  padding: 1rem;
  color: white;
}
</style>
