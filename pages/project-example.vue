<template>
    <div class="container">
    <section>
      <div class='main-content-project'>
        <img src='~/assets/images/illu-refuge-project.png'>
        <h1>
            Refuge du GOUTER
        </h1>
      </div>
    </section>
        <section class="information first">
      <p class="first-text">Déconstruction et désamiantage de l'ancien refuge.
    Création d'un volume recueil dans l'ancienne annexe du refuge.
    Construction d'un bâtiment positif, vivant en autonomie complète à 4 000m d'altitude.
    140 couchages - Bâtiment HQE.</p>
    </section>
    <section class="project">
        <h2>Informations</h2>
        <div class='project-wrapper'>
            <div>
                <h3>Maitre d’ouvrage</h3>
                <p>CLUB ALPIN Français<br>
                Fédération française des clubs alpins et de montagne<br>
                24 avenue de Laumière 75019 PARIS<br>
                M. Pietu - Tél : 01.53.72.87.00</p>
            </div>
            <div>
                <h3>Details</h3>
                <p>
                    Missions DENIZOU :<br>
                    Économiste, Mission de base + EXE <br>
                    Dates : <br>
                    2010 - 2013 <br>
                    Surfaces : <br>
                    700 m² <br>
                    Montants des travaux : <br>
                    5 000 000 € H.T. <br>
                </p>
            </div>
            <div>
                <h3>Composition de l’équipe</h3>
                <p>Architecte : Groupe H, DécaLaage Architecture<br>
                    BET Fluides : STREM <br>
                    Simulations thermiques : Albédo Énergie <br>
                    BET Structure fondations : Betech <br>
                    Ingénieur bois : Charpente Concept </p>
            </div>
        </div>
    </section>
    </div>
</template>

<style lang="scss" scoped>
    section{
        min-height: 100vh;
        width: 100vw;
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;

        &.information{
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
        }
    }
    .main-content-project{
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

</style>

<style lang="scss" scoped>
 section.project{
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
      grid-template-columns: 1fr 1fr;
      grid-column-gap: 32px;
      grid-row-gap: 64px;
      div{
          h3{
              color: white;
              font-size: 48px;
              margin-bottom: 16px;
              font-family: Arial, Helvetica, sans-serif;
          }
          p{
              color:white;
              font-size: 24px;
              font-family: Arial, Helvetica, sans-serif;
          }
      }
  }
 }
</style>