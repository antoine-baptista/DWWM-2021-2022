<template>
  <div class="connexion">
    <Headerarrow/>
    <main id="connexionindex">
        <p class="information-admin">🚧 Cette page est en cours de création.</p>
        <img src="../assets/triangle.png" alt="Triangle" width="90" height="90">
    </main>
    <Networks/>
    <Footer/>
  </div>
</template>



<script>

// @ is an alias to /src
import Headerarrow from '@/components/Headerarrow.vue'
import Networks from '@/components/Networks.vue'
import Footer from '@/components/Footer.vue'
document.title="Fanzine de Breizh | Menu admin";

export default {
  name: 'Connexion',
  components: {
    Headerarrow,
    Networks,
    Footer
    
  }
}

</script>


<style>
/* on enlève les marges de la page A-propos */
Body{
  margin: 0;
  padding: 0;
  /* on affecte à l'élément 'Body' une image de fond */
  background-image: url('/img/sable.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  }

.information-admin{
    /* fixe le paragraphe <p> en lui donnant
    le style recherché */
    font-family: 'Source Serif Pro', serif;
    font-size: 22px;
    font-weight: bold;
    color: rgb(213,0,80);
    text-shadow: 1px 3px 1px rgb(61,166,193);
    margin: auto;
    text-align: center;
    width: 100vw;
    }


/* Média queries pour la nav -- l'élargissement des boutons ne fonctionne pas ailleurs !! */
/* ███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████
   premier point de rupture
   Sur uniquement les écrans, quand la largeur de la fenêtre fait au minimum 700px et au maximum 913px */
@media screen and (min-width: 700px) and (max-width: 913px)
{
    
.information-admin{
    /* fixe le paragraphe <p> en lui donnant
    le style recherché */
    font-family: 'Source Serif Pro', serif;
    font-size: 30px;
    font-weight: bold;
    color: rgb(213,0,80);
    text-shadow: 1px 3px 1px rgb(61,166,193);
    margin: auto;
    text-align: center;
    width: 100vw;
    }
}

/* ███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████
   second point de rupture
   Sur uniquement les écrans, quand la largeur de la fenêtre fait au minimum 914px et au maximum 1249px */
@media screen and (min-width: 914px) and (max-width: 1249px)
{

.information-admin{
    /* fixe le paragraphe <p> en lui donnant
    le style recherché */
    font-family: 'Source Serif Pro', serif;
    font-size: 35px;
    font-weight: bold;
    color: rgbrgb(213,0,80);
    text-shadow: 1px 3px 1px rgb(61,166,193);
    margin: auto;
    text-align: center;
    width: 100vw;
    }
}

/* ███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████
   troisième point de rupture
   Sur uniquement les écrans, quand la largeur de la fenêtre fait au minimum 1250px */
@media screen and (min-width: 1250px)
{
    
.information-admin{
    /* fixe le paragraphe <p> en lui donnant
    le style recherché */
    font-family: 'Source Serif Pro', serif;
    font-size: 35px;
    font-weight: bold;
    color: rgb(213,0,80);
    text-shadow: 1px 3px 1px rgb(61,166,193);
    margin: auto;
    text-align: center;
    width: 100vw;
    }
}

</style>

