<script setup>
//Vue Material Kit 2 components
import MaterialInput from "@/components/MaterialInput.vue";
import MaterialTextArea from "@/components/MaterialTextArea.vue";
import MaterialButton from "@/components/MaterialButton.vue";
import MaterialSwitch from "@/components/MaterialSwitch.vue";
</script>
<template>
  <section>
    <div class="container py-4">
      <div class="row">
        <div class="col-lg-7 mx-auto d-flex justify-content-center flex-column">
          <h3 class= "text-center">Contacto</h3>
          <br>
        <form>  
          <label>Nombre(s)</label>
              <input/>
        </form> 
        <br>
        <form>  
          <label>Apellido(s)</label>
              <input/>
        </form> 
        <br>
        <form>  
          <label> Email</label>
              <input type= "email"/>
        </form> 
        <br>
        <label> Asunto</label>
        <textarea></textarea>
        
                </div>
              </div>
            </div>
      
  </section>
</template>

