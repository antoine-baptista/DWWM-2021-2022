<template>
  <div class="home">
    <Header/>
    <main id="homeindex">
        <p class="balades">BALADES EN CORNOUAILLE</p>
        <img src="../assets/triangle.png" alt="Triangle" width="90" height="90">
    <Navigation/>
    </main>
    <!-- <Networks/> -->
    <Footer/>
    
  </div>
</template>



<script>

// @ is an alias to /src
import Header from '@/components/Header.vue'
import Navigation from '@/components/Navigation.vue'
// import Networks from '@/components/Networks.vue'
import Footer from '@/components/Footer.vue'

document.title="Fanzine de Breizh | Accueil";

export default {
  name: 'Home',
  components: {
    Header,
    Navigation,
    // Networks,
    Footer
  },
}


</script>



<style>

/* on enlève les marges de la page Home */
Body{
  margin: 0;
  padding: 0;
  /* on affecte à l'élément 'Body' une image de fond */
  background-image: url('/img/loc-amand.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  }

.balades{
    /* fixe le paragraphe <p> en lui donnant
    le style recherché */
    font-family: 'Bebas Neue', cursive;
    font-size: 45px;
    text-shadow: 1px 3px 1px rgb(13,40,89);
    color: rgb(61,166,193);
    text-align: center;
    width: 100%;
    }

/* Média queries pour la nav -- l'élargissement des boutons ne fonctionne pas ailleurs !! */
/* ███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████
   premier point de rupture
   Sur uniquement les écrans, quand la largeur de la fenêtre fait au minimum 700px et au maximum 913px */
@media screen and (min-width: 700px) and (max-width: 913px)
{
    #move-buttons a {
        width: 150px;
    }
    #bouton-admin a {
        width: 150px;
    }
    .balades{
    /* fixe le paragraphe en lui donnant
    le style recherché */
    font-family: 'Bebas Neue', cursive;
    font-size: 45px;
    text-shadow: 1px 3px 1px rgb(13,40,89);
    color: rgb(61,166,193);
    text-align: center;
    width: 100%;
    }
}

/* ███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████
   second point de rupture
   Sur uniquement les écrans, quand la largeur de la fenêtre fait au minimum 914px et au maximum 1249px */
@media screen and (min-width: 914px) and (max-width: 1249px)
{
    #move-buttons a {
        width: 150px;
    }
    #bouton-admin a {
        width: 150px;
    }
    .balades{
    /* fixe le paragraphe en lui donnant
    le style recherché */
    font-family: 'Bebas Neue', cursive;
    font-size: 64px;
    text-shadow: 1px 3px 1px rgb(13,40,89);
    color: rgb(61,166,193);
    text-align: center;
    width: 100%;
    }
}

/* ███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████
   troisième point de rupture
   Sur uniquement les écrans, quand la largeur de la fenêtre fait au minimum 1250px */
@media screen and (min-width: 1250px)
{
    #move-buttons a {
        width: 200px;
        margin: 15px 50px 15px 15px;
    }
    #bouton-admin a {
        width: 200px;
        margin-top: 129px;
        padding-right: 15px;
    }
    .balades{
    /* fixe le paragraphe en lui donnant
    le style recherché */
    font-family: 'Bebas Neue', cursive;
    font-size: 80px;
    text-shadow: 1px 3px 1px rgb(13,40,89);
    color: rgb(61,166,193);
    text-align: center;
    width: calc( 100vw - 300px);
    }
}

</style>
