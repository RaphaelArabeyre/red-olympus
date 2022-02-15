<script setup lang="ts">

import Header from "@/components/Header.vue";
import ROButton from "@/components/ROButton.vue";
import TitleSection from "@/components/TitleSection.vue";</script>

<template>

  <body>
  <Header/>

  <div id="top">

    <img id="top-bg" src="./assets/img/top-bg.png">

    <div id="top-text-section">

      <div id="top-left">
        <div id="title">
          <h1 id="top-title">VOYAGE</h1>
          <h2>Mars à porée de main</h2>
        </div>

        <p id="top-text">Red Olympus se porte garant de votre<br/>
          confort et vous invite à embarquer,<br/>
          destination : Mars.</p>

        <ROButton id="top-button" primary='true' text='Je Découvre'/>
      </div>

      <img id="top-" src="">

    </div>

    <div id="top-card-section">

      <img id="top-card-img" src="./assets/img/top-dome.png">

      <div id="top-card-text-section">
        <h3>VOYAGE GREEN sur MARS</h3>
        <p>Découvrez Red Olympus, la première entreprise à vous offrir des<br>
          solutions de voyage sur les colonies martiennes. Filiale du groupe<br>
          spatial Space X, notre expertise technologique et notre<br>
          connaissance de l'environnement vous permettront de vivre un<br>
          voyage serein et épanouissant à travers nos trois offres de voyages.</p>
      </div>

    </div>
  </div>

  <div id="detail-section">

    <div id="row-detail">
      <div id="pointer">

        <div id="pointer-icon" class="icon-pack">
          <img src="./assets/img/icon-pointer.png" alt="pointer">
        </div>

        <h2>Pointer</h2>

        <p>Nous localiser et estimer son temps<br> de trajet.</p>
      </div>

      <div id="transport">

        <h2>Transport</h2>

        <p>Nos moyens de transports vous<br> garantiront un confort optimal !</p>

        <div id="rocket-icon" class="icon-pack">
          <img src="./assets/img/icon-rocket.png" alt="pointer">
        </div>


      </div>

      <div id="map">
        <div id="map-icon" class="icon-pack">
          <img src="./assets/img/icon-map.png" alt="pointer">
        </div>

        <h2>Carte</h2>

        <p>Découvrez nos différents cites et<br>
          leurs particularités grâce à cette<br>
          carte holographique qui vous<br>
          transportera en un instant sur le site<br>
          tant convoité !</p>
      </div>

    </div>

  </div>

  <div id="video-section">

    <TitleSection title="Red Olympus en image" :primary="true"/>


    <div id="video"></div> <!-- TODO : Insert video here -->

  </div>

  <div id="pack-section">


    <TitleSection title="Nos Packs" :primary="false"/>


    <img id="pack-img" src="./assets/img/packs.png">


    <div id="pack-detail">

      <div id="discover" class="pack">
        <h3>Pack découverte</h3>
        <p>Profitez du confort de nos
          hébergements sans aucune autre
          contrainte que votre volonté. Vous
          pourrez vous balder librement
          dans la colonie de Curiosity en
          profitant des magnifiques paysages.</p>

        <div class="see-more">
          <h4>Voir</h4>
          <hr>
        </div>
      </div>

      <div id="culture" class="pack">
        <h3>Pack culturel</h3>
        <p>Pour les amoureux de la culture martienne, ce pack
          de voyage vous offrira voyage, hébergement, mais
          aussi une multitude d'activités comme des visites
          guidées de lieux historiques préservés (astérisque
          avec « véhiculés à énergie verte »), des visites de
          musées et des city tours.</p>

        <div class="see-more">
          <h4>Voir</h4>
          <hr>
        </div>
      </div>

      <div id="olympus" class="pack">
        <h3>Pack Olympus</h3>

        <p>Destiné aux sportifs, aux passionnés de
          défis, ce pack de voyage vous mènera la vie
          dure en vous proposant des activités
          sportives comme des randonnées et de
          'escalade sur le mont Olympus,...</p>

        <div class="see-more">
          <h4>Voir</h4>
          <hr>
        </div>

      </div>

    </div>


  </div>

  <div id="hotel">

    <TitleSection id="hotel-title" title="Hôtels" :primary="true"/>

    <div id="row-card-hotel">

      <div id="nihi-sumba">

        <img class="hotel-img" src="./assets/img/nihi-sumba.png">

        <div class="text-hotel-card">
          <h2>Nihi sumba</h2>
          <p>Un maximum de confort dans votre
            cité spatiale.Idéale pour les familles
            souhaitant tout avoir à disposition !</p>
        </div>


        <div class="money-card-hotel">
          <img src="./assets/img/unicash.png">
          <p>67</p>
        </div>

        <ROButton class="reserve-button" :primary="false" text="RESRVER"/>

      </div>

      <div id="the-gratte-terre">

        <img class="hotel-img" src="./assets/img/top-dome.png">
        <div class="text-hotel-card">
          <h2>THE GRATTE TERRE
          </h2>
          <p> Creusée dans le sol, cette tour de 65
            niveaux, enfouis sous la place
            Mercure, près des espaces rando
            est idéal pour les sportifs</p>
        </div>


        <div class="money-card-hotel">

          <img src="./assets/img/unicash.png">
          <p>53</p>
        </div>

        <ROButton class="reserve-button" :primary="false" text="RESRVER"/>

      </div>

      <div id="Zarafa-camp">

        <img class="hotel-img" src="./assets/img/Zarafa-camp.png">
        <div class="text-hotel-card">
          <h2>ZARAFA CAMP
          </h2>
          <p>Comme un poison dans l'eau nos
            logements 'exception vous
            offrirons un service haut de
            gamme!</p>
        </div>


        <div class="money-card-hotel">

          <img src="./assets/img/unicash.png">
          <p>67</p>
        </div>

        <ROButton class="reserve-button" :primary="false" text="RESRVER"/>
      </div>

    </div>


  </div>

  <div id="space"></div>

  </body>
</template>

<style lang="scss">
@import "assets/scss/app";

.marge {

}

body {

  margin: 0 auto;

  #top {
    display: flex;
    height: 110vh;
    width: 100%;
    flex-direction: column;

    justify-content: space-between;


    #top-bg {
      margin-top: -100px;
      position: absolute;
      width: 100vw;
      z-index: -1;
    }

    #top-text-section {
      display: flex;
      flex-direction: column;
      align-self: center;

      width: 60%;

      #title {
        margin-top: 60px;

        h1 {
          margin-top: auto;
          margin-bottom: 0;
          font-size: 70px;
          font-weight: 400;
        }

        h2 {
          margin-top: -3px;
          margin-bottom: 0;
          text-transform: uppercase;

        }
      }

      #top-text {
        margin-top: 50px;
        font-size: 17px;
        margin-bottom: 40px;
      }


    }

    #top-card-section {
      width: 60%;

      background: $color-white;
      display: flex;
      align-self: center;

      height: 300px;

      margin-bottom: 30px;

      #top-card-img {
        padding: 5px;
      }

      #top-card-text-section {
        width: 100%;

        display: flex;
        flex-direction: column;

        justify-content: center;
        align-items: center;


        h3 {
          color: $color-secondary;
          margin-top: 50px;
          font-size: 24px;
          letter-spacing: 3px;
        }

        p {
          flex: 3;
          font-size: 12px;
          text-align: center;
        }

      }


    }

  }

  #detail-section {
    background: $color-white;
    display: flex;
    flex-direction: column;
    width: 100%;


    #row-detail {
      margin-top: 60px;
      align-self: center;
      display: flex;
      justify-self: center;
      width: 60%;

      justify-content: space-between;

      * {
        display: flex;
        flex-direction: column;

        h2 {
          align-items: center;
          text-transform: uppercase;
          letter-spacing: 2px;
          color: $color-primary;
        }

        p {
          text-align: center;
          font-size: 11px;
          color: $color-gray;
        }

        .icon-pack {
          margin-top: 30px;

          align-items: center;
          display: flex;
          justify-content: center;
          align-content: center;

          img {
            height: 100px;
            width: 100px;
          }
        }

        #rocket-icon {
          img {
            padding: 20px;
            height: 45px;
            width: 45px;
          }
        }

      }
    }
  }

  #video-section {
    margin-top: 100px;
    display: flex;
    flex-direction: column;
    align-items: center;

    justify-content: center;


    #video {
      margin-top: 40px;
      height: 500px;
      width: 70vw;
      background: #f2f2f2;

    }

  }


  #pack-section {
    margin-top: 200px;
    display: flex;
    flex-direction: column;
    width: 100%;


    #pack-img {
      margin-top: -2px;
    }

    #pack-detail {
      background: $color-white;
      align-self: center;
      height: 400px;

      display: flex;
      width: 60%;

      justify-content: space-between;

      div.pack {
        margin-top: 20px;
        height: 250px;
        width: 235px;
        display: flex;
        flex-direction: column;


        h3 {
          font-size: 17px;
          font-weight: 400;
          letter-spacing: 2px;
        }

        p {
          color: $color-gray;
          font-size: 12px;
        }

        .see-more {
          margin-top: auto;
          margin-bottom: 0;
          align-items: center;

          h4 {
            color: $color-secondary;
            text-align: center;
            margin-top: auto;
            margin-bottom: 0;
            text-transform: uppercase;
            font-size: 10px;
            font-weight: 400;
            letter-spacing: 2px;
          }

          hr {
            border: 0;
            margin-top: 5px;
            position: relative;
            height: 1.5px;
            width: 45px;
            background: $color-secondary;
          }
        }


      }

      #discover {
        align-items: flex-start;
        text-align: start;
      }

      #culture {
        width: 280px;
        align-items: center;
        text-align: center;
      }

      #olympus {
        align-items: flex-end;
        text-align: end;
      }


    }

  }

  #hotel {
    display: flex;
    flex-direction: column;
    background: $color-light-gray;
    height: 650px;


    #hotel-title {
      padding-top: 50px;
    }


    #row-card-hotel {
      margin-top: 50px;

      align-self: center;
      width: 60vw;
      display: flex;
      justify-content: space-between;
      align-items: center;

      div {

        background: $color-white;
        height: 100px;
        width: 280px;


        .hotel-img {
          object-fit: cover;
          height: 175px;
          width: 100%;
        }

        .text-hotel-card {

          display: flex;
          flex-direction: column;

          justify-content: center;
          align-items: center;

          h2 {
            font-size: 20px;
            font-weight: 400;
            text-transform: uppercase;
            color: $color-secondary;
            margin-top: 20px;
            margin-bottom: 0;
            letter-spacing: 1px;
          }

          p {
            color: $color-gray;
            text-align: center;
            font-size: 12px;
          }

        }

        .money-card-hotel {
          display: flex;
          align-items: center;
          justify-content: center;

          img {
            margin-bottom: 5px;
            height: 44px;
          }

          p {
            color: $color-primary;
            font-size: 20px;
            font-weight: 400;
            margin-left: 5px;
          }

          &:before, &:after {
            margin-left: 20px;
            margin-right: 20px;
            content: ' ';
            height: 1px;
            width: 100px;
            background: $color-gray;
          }




        }

        .reserve-button{
          margin-right: auto;
          margin-left: auto;
           height: 40px;
           width: 120px;
         }

      }

    }


  }


  #space {
    background: #a5a5a5;
    height: 1000px;
  }
}

</style>
