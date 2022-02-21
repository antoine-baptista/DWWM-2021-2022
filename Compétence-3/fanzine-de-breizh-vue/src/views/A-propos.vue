<template>
  <div class="a-propos">
    <Headerarrow/>
    <h2 id="prez-blog">A propos de ce blog:</h2>
    <article  id="prez-texte">
        <p>J’ai créé ce blog dans le cadre de ma formation de développeur Web et Web Mobile. Au sein de l’AFPA, huit mois durant, j’ai appris les langages qui me permettent de concevoir des sites Web.</p>
        <p>Amoureux de la Bretagne au plus profond de moi, il me tenait à coeur de vous présenter les balades que régulièrement je fais dans ces merveilleux paysages. La contemplation des horizons lorsque la lumière naissante embrase la végétation, lorsque le soleil s’échappe flamboyant à la nuit tombée, les embruns et l’iode, le sourire des gens, sont des choses qui me font me sentir moi, là à cet endroit.</p>
        <p>J’essaierai tout au long de ce voyage de vous faire partager le bonheur que j’ai à marcher et à flâner en Cornouaille et en Bretagne. D’être présent avec les gens qui y habitent et qui font que ce pays est unique.</p>
        <p>Très bonne balade.</p>
        <p>Bevet Breizh !</p>
    </article>
    <main id="a-proposindex">
        <img src="../assets/triangle.png" alt="Triangle" width="90" height="90">
    </main>
    <Commentaires/>
    <Networks/>
    <Footer/>
  </div>
</template>



<script>

// @ is an alias to /src
import Headerarrow from '@/components/Headerarrow.vue'
import Networks from '@/components/Networks.vue'
import Footer from '@/components/Footer.vue'
import Commentaires from '../components/Commentaires.vue'
document.title="Fanzine de Breizh | A propos"

export default {
  name: 'A-propos',
  components: {
    Headerarrow,
    Networks,
    Footer,
    Commentaires
}

// data(){
//         return {
//             comments:[],
//             errors: []
//         }
//   },
//   // Fetches Details when the component is created.
//   created() {
//     axios.get(`http://localhost:8080/commentaires.json`)
//     .then(response => {
//       // JSON responses are automatically parsed.
//       this.comments = response.data.comments
//     })
//     .catch(e => {
//       this.errors.push(e)
//     })
//   }  
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
  overflow-y: visible;
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

