<template>
  <div class="about">
    <div id="nav">
      <router-link to="/">INICIO</router-link>|
      <router-link to="/about">QUIÉNES SOMOS</router-link>|
      <div class="animated infinite heartBeat delay-5s slower">
        <router-link to="/projects">NUESTROS PROYECTOS</router-link>
      </div>
    </div>
    <br class="none" />
    <br class="none" />
    <Row type="flex" justify="center">
      <Col :lg="10"> </Col>
    </Row>
    <br />
    <br />
    <Row type="flex" justify="center">
      <Col class="m-auto align-center" :lg="4">
        <img class="br-50 maxw-100 mob-height" src="../assets/image.jpeg" />
        <p class="namePartner">Andrea Monroy</p>

        <br />
        <Button>
          <a
            target="_blank"
            href="https://drive.google.com/file/d/1MtMNy8qtaFXgiDxNZKapQPZEDajI4dmM/view?usp=sharing"
            >VER CV</a
          >
        </Button>
      </Col>
      <Col :lg="7" class="align-center">
        <p class="font-16">
          <br class="none" />
          <br />
          <strong>Queremos</strong> aportar a nuestra comunidad. <br /><strong
            >Buscamos</strong
          >
          proyectos interesantes y creativos. <br />
          <strong>Nuestro objetivo:</strong>
          desarrollarlos, generar impacto y hacerlos inclusivos.
          <br /><br /><strong>Nos encantaría</strong> hacer realidad tu idea.<br />
          <strong>Trabajemos juntxs.</strong>
        </p>
      </Col>
      <Col class="m-auto align-center pt-2em" :lg="4">
        <img class="br-50 maxw-100 mob-height" src="../assets/image-fio.jpeg" />
        <p class="namePartner">Fiorella Sánchez</p>

        <br />
        <Button>
          <a
            target="_blank"
            href="https://drive.google.com/file/d/1pd2US_sTYSAeNMjTaWWTJo_rLJPegeer/view?usp=sharing"
            >VER CV</a
          >
        </Button>
      </Col>
    </Row>
    <br />
    <br />
    <Row type="flex" justify="space-around">
      <Col :lg="20">
        <h1 class="font-22">
          <vue-typer
            :text="[
              'CREEMOS',
              'DESARROLLEMOS',
              'DISEÑEMOS',
              'IDEEMOS',
              'TRABAJEMOS POR'
            ]"
            :repeat="Infinity"
            :shuffle="false"
            initial-action="typing"
            :pre-type-delay="70"
            :type-delay="70"
            :pre-erase-delay="200"
            :erase-delay="500"
            erase-style="select-all"
            :erase-on-complete="false"
            caret-animation="blink"
          ></vue-typer>
        </h1>
      </Col>
    </Row>
    <br />
    <br />
    <Row class="align-center" type="flex" justify="space-around">
      <Col :lg="8">
        <h2>SOLUCIONES DIGITALES</h2>
        <br />
        <img class="maxw-100" src="../assets/solution.jpg" />
        <br />
        <p class="font-22">
          Queremos mejorar servicios tradicionales implementando soluciones
          digitales innovadoras.
        </p>
      </Col>
      <Col :lg="8">
        <h2>IMPACTO SOCIAL</h2>
        <br />
        <img class="maxw-100" src="../assets/social.png" />
        <br />
        <br />
        <p class="font-22">
          Queremos diseñar de una forma inclusiva y accesible, creando un mundo
          digital para tod@s
        </p>
      </Col>
    </Row>
    <br />
    <br />
  </div>
</template>
<script>
import { VueTyper } from "vue-typer";
export default {
  components: {
    // ES6; property shorthand + Vue should automatically dasherize the key for us
    VueTyper
  }
};
</script>

<style>
.namePartner {
  font-size: 25px;
}
</style>
