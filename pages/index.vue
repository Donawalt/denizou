<template>
  <div class="container">
    <section>
      <div class='main-content-home'>
        <img src='~/assets/images/main-home-image.png'>
        <h1>
          Assistants aux maitres d’ouvrages & économistes de la construction
        </h1>
      </div>
    </section>
    <section class="information first">
      <p class="first-text">Le Cabinet a été créé en 1971. Monsieur Stéphane NARDY en assure la Direction depuis le 1er octobre 2014. Monsieur Paul GIRIN était le Directeur de 1989 à septembre 2014. Nous intervenons pour des Maîtres d’Ouvrages Publics ou Privés soit en tant que conseil (AMO), soit en tant que partenaire économiste au sein d’équipes de conception.
DENIZOU est adhérent à l’Union nationale des Économistes de la construction (UNTEC) depuis plus de trente ans.</p>
    </section>
  <section class='projects'>
      <h2>Nos Projets</h2>
      <div class="project-wrapper grid-2">
        <nuxt-link class="project item" to="">
          <div><img src='~/assets/images/illu-refuge.png'></div>
          <p>Saint-gervais</p>
          <h3>Refuge du GOUTER</h3>
        </nuxt-link>
        <nuxt-link class="project item" to="">
          <div><img src='~/assets/images/illu-belle.png'></div>
          <p>Grenoble</p>
          <h3>La Belle Électrique</h3>
        </nuxt-link>
      </div>
      <div class="project-wrapper grid-3">
         <nuxt-link class="project item" to="">
          <div><img src='~/assets/images/illu-fourviere.png'></div>
          <p>Lyon</p>
          <h3>Basilique de Fourvière</h3>
        </nuxt-link>
        <nuxt-link class="project item" to="">
          <div><img src='~/assets/images/illu-grangette.png'></div>
          <p>Thonons-les-bains</p>
          <h3>La GRANGETTE</h3>
        </nuxt-link>
        <nuxt-link class="project item" to="">
          <div><img src='~/assets/images/illu-ho.png'></div>
          <p>Lyon</p>
          <h3>Hôpital Édouard‑Herriot</h3>
        </nuxt-link>
      </div>
      <button><nuxt-link to="/projets">En voir plus</nuxt-link></button>
    </section>
    <section class="information">
      <div class="info-component">
        <h2>Organisations</h2>
        <p>Notre Cabinet est composé de 11 Économistes de la Construction de niveau BTS et DUT et de 3 secrétaires techniques et 2 comptables. Chaque opération est pilotée par un Chef de Projet, celui-ci est secondé par deux, voir trois, techniciens dans les phases d’études PRO/DCE. Le Chef de Projet est l’interlocuteur privilégié des autres partenaires de l’équipe de conception.</p>
      </div> 
      <img class='info-img rellax' src='~/assets/images/illu-orga.png' data-rellax-speed="-1">
    </section>
    <section class="information reverse">
      <img class='info-img rellax' src='~/assets/images/illu-mission.png' data-rellax-speed="1">
      <div class="info-component">
        <h2>Missions</h2>
        <p>A.M.O. : Assistance à Maitrise d’Ouvrage (Description et références)<br>
          Économiste de la construction.<br>
          <br>
          <br>
          Étude de faisabilité, définition de budget en Phase Programmation.<br>
          Économie des projets.<br>
          <br>
          <br>
          Expertise économique de projets en Phase concours ou Avant Projet.<br>
          <br>
          Création de bordereaux de prix pour les Maîtres d’Ouvrages institutionnels.
        </p>
      </div>
    </section>
    <section class="information">
      <div class="info-component">
        <h2>Activités</h2>
        <p>Nous intervenons sur tous types de bâtiments neufs ou réhabilités :<br>
        - Logements (références)<br>
        - Refuges de haute montagne (références)<br>
        - Monuments historiques (références)<br>
        - Équipements culturels, publiques et sportifs (références)<br>
        - Établissements de Santé (références)<br>
        - Établissements scolaire et bureau (références)<br>
      <br>
      <br>
        Nous sommes habitués à travailler au sein d’équipe de conception pluridisciplinaire dans le respect de chacun des intervenants. Nous intégrons sur tous nos projets, les notions de Qualité Environnementale des Bâtiments en veillant au respect des enveloppes budgétaires allouées.</p>
      </div>
      <img class='info-img rellax' src='~/assets/images/illu-act.png' data-rellax-speed="-1">
    </section>
    <section class="information reverse">
      <img class='info-img rellax' src='~/assets/images/illu-bim.png' data-rellax-speed="1">
      <div class="info-component">
        <h2>BIM</h2>
        <p>Depuis 2017 nous intégrons le BIM au travers des maquettes IFC pour nos quantitatifs. Dans cet esprit nous développons une synergie autour du BIM et ces applications avec deux autres bureaux d'étude - DPI Structure et STREM (BE fluides) - au travers de la société OCABIM.</p>
      </div>
    </section>
    <section class="information">
      <div class="info-component">
        <h2>Logiciels</h2>
        <p>IAO :<br>
          Devis , Gestion des Appels d'Offres.<br>
          ATTIC+ : Descriptifs, Quantitatifs en IFC (par maquette BIM)<br>
          AUTOCAD</p>
      </div>
      <img class='info-img rellax' src='~/assets/images/illu-software.png' data-rellax-speed="-1">
    </section>
  </div>
</template>

<script>
import anime from 'animejs'
import Rellax from 'rellax'
export default {
  mounted:()=>{
    var rellax = new Rellax('.rellax', {
    center:true
  });

    let tl = anime.timeline({
      duration: 2000
    })

    tl.add({
      targets: '.container', 
      opacity: [0, 1]
    }).add({
      targets: '.main-content-home img',
      easing: "easeInOutQuad",
      translateY: ["-50%", 0],
      opacity: [0, 1],
    }, "-=500").add({
      targets: '.main-content-home h1',
      easing: "easeInOutQuad",
      translateY: ["25%", 0],
      opacity: [0,1],
      duration: 800
    }, "-=1500")
  }
}
</script>

<style lang="scss" scoped>
.container{
  section{
    min-height: 100vh;
    width: 100vw;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    .main-content-home{
      margin-left: 11.25%;
      margin-right: 11.25%;
      width: 77.5vw;
      display: grid;
      grid-template-columns: 1fr 1fr 1fr 1fr;
      grid-template-rows: 1fr;
      img{
        display: flex;
        z-index: 1;
        grid-column: 1/3;
        grid-row: 1/1;
      }
      h1{
        display: flex;
        z-index: 10;
        grid-column: 2/5;
        grid-row: 1/1;
        color: #FFAFAF;
        justify-content: center;
        align-items: center;
        font-size: 90px;
        font-family: Arial, Helvetica, sans-serif;
      }
    }
    &.information {
      overflow: hidden;
      min-height: 50vh;
      justify-content: center;
      align-items: center;
      background-color: #046BD9;
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      grid-gap: 16px;
      padding-left: 11.25vw;
      padding-right: 11.25vw;
      width: auto;
      &.first{
        display: flex;
        p{
          margin-top: 64px;
          text-align: center;
          font-size: 24px;
          color: #FFAFAF;
          font-weight: lighter;
          font-family: Arial, Helvetica, sans-serif;
          width: 850px;
          line-height: 153%;
          margin-bottom: 64px;
          grid-column: 1/4;
        }
      }
      &.reverse{
        background-color: #232424;
        margin-bottom: 64px;
        margin-top: 64px;
        img{
          grid-column: 1/2;
        }
        .info-component{
          grid-column: 2/4;
          h2{
            color: #FFAFAF;
          }
          p{
            color: white;
          }
        }
      }
      .info-component{
        h2 {
          font-size: 72px;
          color: white;
          font-family: Arial, Helvetica, sans-serif;
          margin-bottom: 16px;
        }
        p{
          font-size: 24px;
          color: #FFAFAF;
          font-weight: lighter;
          font-family: Arial, Helvetica, sans-serif;
          line-height: 153%;
        }
        grid-column: 1/3;
      }
      img{
        width: 100%;
      }
    }
  }
}
</style>

<style lang="scss" scoped>
section.projects{
  display: block;
  padding-left: 11.25vw;
  padding-right: 11.25vw;
  width: auto;
  h2{
    font-size: 72px;
    color: #FFAFAF;
    font-family: Arial, Helvetica, sans-serif;
  }
  .project-wrapper{
    display: grid;
    margin-bottom: 64px;
    &.grid-2{
      grid-template-columns: 1fr 1fr;
      grid-column-gap: 32px;
    }
    &.grid-3{
      grid-template-columns: 1fr 1fr 1fr;
      grid-column-gap: 32px;
    }
    .project.item{
      color: white;
      text-decoration: none;
      &:hover{
        p{
          color:#FFAFAF;
          transition: 300ms;
        }
        h3 {
          color:#046BD9;
          transition: 300ms;
        }
        div{
          &:before,&:after{
            opacity: 0;
            transition: 300ms;
          }
        }
      }
      div{
          position: relative;
          padding: 0px;
         &:before {
          background-color:#FFAFAF;
          content: "";
          display: block;
          width: 100%;
          height: 100%;
          mix-blend-mode: darken;
          position: absolute;
          top: 0;
          left: 0;
        }

        &:after {
          background-color:#046BD9;
          content: "";
          display: block;
          width: 100%;
          height: 100%;
          mix-blend-mode: lighten;
          position: absolute;
          top: 0;
          left: 0;
        }
      }
      img{
        width: 100%;
        margin-bottom: 8px;
        margin: 0px;
      }
      p{
        font-size: 16;
        font-weight: bold;
        margin-bottom: 16px;
        font-family: Arial, Helvetica, sans-serif;
      }
      h3{
        font-size: 48px;
        font-family: sans-serif;
        margin: 0px;
      }
    }
  }

  button{
    width: 200px;
    height: 48px;
    border: none;
    border-radius:5px;
    margin: auto;
    background-color: #046BD9;
    margin-bottom: 64px;
    margin-left: 50%;
    transform: translate(-50%);
    &:hover{
      background-color: #FFAFAF;
      transition: 400ms;
      a{
        color:#046BD9;
        transition: 400ms;
      }
    }
    a{
      text-decoration: none;
      color: white;
      margin: auto;
    }
  }
}
</style>