<template>
  <div class="about-me">
    <Headerarrow/>
        <section id="sectionabout-me">
        <h2 id="prez-about">A propos de moi :</h2>
        <article id="prez-me">
            <p>Je suis Antoine Baptista, futur développeur web “junior”.</p>
            <p>Après plus de quarante années de travail en tant que salarié, j’ai décidé de faire une formation de développeur web et web mobile pour devenir freelance.</p>
            <p>Il me plait à penser que c’est un joli pied de nez au destin. Les diplômes ne sont-ils pas normalement obtenus en début de carrière ? Monsieur Cyclopède et sa minute nécessaire aurait dit :<br/>
                “- Etonnant, non ?”</p>
            <p>De surcroit, je souhaite pouvoir donner un peu de mon temps à des personnes qui ne seraient pas à l’aise avec l’informatique ni avec le web.</p>
            <p>Je me suis lancé, vous êtes les premiers visiteurs à parcourir mon travail.</p>
            <p>Merci pour vos commentaires.</p>
        </article>
        <div id="video">
            <h2 id="babou">Babou à la plage :</h2>
            <div class="iframe_container">
                <!-- <iframe width="416" height="234" src="https://www.youtube.com/embed/-eP0a5Ih67E" title="Babou à la plage" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->
                <iframe src="https://www.youtube.com/embed/-eP0a5Ih67E" title="Babou à la plage" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
        </div>
        <Networks/>
    </section>
    
    <main id="about-meindex">
        <img src="../assets/triangle.png" alt="Triangle" width="90" height="90">
    </main>
    
    <Footer/>
  </div>
</template>



<script>

// @ is an alias to /src
import Headerarrow from '@/components/Headerarrow.vue'
import Networks from '@/components/Networks.vue'
import Footer from '@/components/Footer.vue'
document.title="Fanzine de Breizh | About me";

export default {
  name: 'About-me',
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
  overflow: hidden;
  /* on affecte à l'élément 'Body' une image de fond */
  background-image: url('/img/sable.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  }

</style>

