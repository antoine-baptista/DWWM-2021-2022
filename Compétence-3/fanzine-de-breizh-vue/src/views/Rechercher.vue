<template>
  <div class="rechercher">
    <Headerarrow/>
    <!-- <h2 id="titre-search">Rechercher:</h2>
      <article  id="info-search">
          <p>Vous souhaitez rechercher une balade que j’ai faite ?</p>
          <p>Rien de plus simple, tapez tout ou partie du nom de la ville et cliquez sur ‘Lancer la recherche’.</p>
          <p>Ci-contre s’afficheront les balades effectuées où figure le nom de la ville.</p>
          <p>N’hésitez pas à me suivre sur ma chaine Youtube ainsi que sur Twitter.</p>
          <p>Merci.</p>
      </article> -->
    <main id="rechercherindex">
        <p class="information">🚧 Cette page est en cours de création.</p>   
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
document.title="Fanzine de Breizh | Rechercher";

export default {
  name: 'Rechercher',
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

.information{
    /* fixe le paragraphe <p> en lui donnant
    le style recherché */
    font-family: 'Source Serif Pro', serif;
    font-size: 22px;
    font-weight: bold;
    color: rgb(13,40,89);
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
    
.information{
    /* fixe le paragraphe <p> en lui donnant
    le style recherché */
    font-family: 'Source Serif Pro', serif;
    font-size: 30px;
    font-weight: bold;
    color: rgb(13,40,89);
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

.information{
    /* fixe le paragraphe <p> en lui donnant
    le style recherché */
    font-family: 'Source Serif Pro', serif;
    font-size: 35px;
    font-weight: bold;
    color: rgb(13,40,89);
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
    
.information{
    /* fixe le paragraphe <p> en lui donnant
    le style recherché */
    font-family: 'Source Serif Pro', serif;
    font-size: 35px;
    font-weight: bold;
    color: rgb(13,40,89);
    text-shadow: 1px 3px 1px rgb(61,166,193);
    margin: auto;
    text-align: center;
    width: 100vw;
    }
}
</style>

