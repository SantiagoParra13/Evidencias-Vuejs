<template>
    <div class="LandingProyecto">
      <NavBar></NavBar>

      

       <!--Slider-->
       <div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
          <div class="carousel-item active" data-bs-interval="3000" >
            <img src="../assets/BIenestar.png" class="d-block w-100" alt="slide1" width="1536px" hight="761">
          </div>
          <div class="carousel-item" data-bs-interval="2000" >
            <img src="../assets/BIenestar.png" class="d-block w-100" alt="slide2" width="1536px" hight="761">
          </div>
          <div class="carousel-item"  data-bs-interval="2000" >
            <img src="../assets/BIenestar.png" class="d-block w-100" alt="slide3" width="1536px" hight="761">
          </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Anterior</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Siguiente</span>
        </button>
      </div>

      <!--Acerca de Nosotros-->
      <div class="container " id="Nosotros">
        <div class="fs-1 text-center pt-5 fw-lighter  fw-bold ">Acerca de Nosotros</div>
        <div class="row pt-5">
          <div class="col">
            <img src="../assets/bienestar_SENA_600.jpg" width="99%">
          </div>
          <div class="col pt-2">
            <div class="fw-bolder fs-2">MISION</div>
            <br>
             Promover las condiciones de bienestar durante el desarrollo de la FPI de los aprendices del SENA, mediante la formulación y seguimiento a la ejecución del PNIBA y la implementación y seguimiento al programa de atención al egresado
          </div>


          <div class="row">
            <div class="col pt-5">
              <div class="fw-bolder fs-2 ">VISION</div>
            <br>
            <div class="text-">Lograr que aprendices y egresados sean referentes de consulta permanente para la toma de decisiones estrategicas de la entidad, de tal forma que se garantice participación e inclusión diferencial.
            </div>
              </div>
           <div class="col p-3">
            <img src="../assets/bienestar_SENA_600.jpg" width="99%"  >
           </div>
            </div>

        </div>
      </div>

 <CalendarioActividades></CalendarioActividades>

 <br><br>
       <div class="container" id="Charla">
        <div class="row pt-5">
          <div class="fs-1 text-center">
            Agenda Una Charla Con Nuestros Profesionales
          </div>
          <div class="col-sm-4 pt-4">
            
            <div class="card" style="width: 18rem;">
              <img src="../assets/perfil-1024x754.jpg" class="card-img-top " alt="...">
              <div class="card-body">
                <h5 class="card-title">Profesional </h5>
                <p class="card-text">Un texto de ejemplo rápido para colocal cerca del título de la tarjeta y componer la mayor parte del contenido de la tarjeta.</p>
                <ModalSolicitarCharla></ModalSolicitarCharla>
              </div>
            </div>


          </div>
          <div class="col-sm-4 pt-4">
            <div class="card" style="width: 18rem;">
              <img src="../assets/perfil-1024x754.jpg" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card-title">Profesional</h5>
                <p class="card-text">Un texto de ejemplo rápido para colocal cerca del título de la tarjeta y componer la mayor parte del contenido de la tarjeta.</p>
                <ModalSolicitarCharla></ModalSolicitarCharla>
              </div>
            </div>
          </div>

          <div class="col-4 pt-4">
            <div class="card" style="width: 18rem;">
              <img src="../assets/perfil-1024x754.jpg" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card-title">Profesional</h5>
                <p class="card-text">Un texto de ejemplo rápido para colocal cerca del título de la tarjeta y componer la mayor parte del contenido de la tarjeta.</p>
              <ModalSolicitarCharla></ModalSolicitarCharla>
              </div>
            </div>
          </div>
        </div>
       </div>

   
   <FooterdelLanding></FooterdelLanding>
   
</div>
</template>

<script>
// @ is an alias to /src

import NavBar from '@/components/NavBar.vue'
import CalendarioActividades from '@/components/CalendarioActividades.vue'
import ModalSolicitarCharla from '@/components/ModalSolicitarCharla.vue'
import FooterdelLanding from '@/components/FooterdelLanding.vue'

export default {
  name: 'LandingProyecto',
  components: {
    NavBar,
    CalendarioActividades,
    ModalSolicitarCharla,
    FooterdelLanding

  }
}
</script>