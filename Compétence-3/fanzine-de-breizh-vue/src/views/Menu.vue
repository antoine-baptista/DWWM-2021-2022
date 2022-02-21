<template>
  <div class="menu">
    <Headerarrow/>
    <main id="menuindex">
        <h2 class="blog">Blog :</h2>
        <img src="../assets/triangle.png" alt="Triangle" width="90" height="90">
    </main>
    <Navigationmobile/>
    <Networks/>
    <Footer/>
  </div>
</template>



<script>

// @ is an alias to /src
import Headerarrow from '@/components/Headerarrow.vue'
import Navigationmobile from '@/components/Navigationmobile.vue'
import Networks from '@/components/Networks.vue'
import Footer from '@/components/Footer.vue'
document.title="Fanzine de Breizh | Menu";

export default {
  name: 'Menu',
  components: {
    Headerarrow,
    Navigationmobile,
    Networks,
    Footer
    
  }
}

</script>


<style>

Body{
  /* on affecte à l'élément 'Body' une image de fond */
  background-image: url('/img/sable.jpg');
  background-attachment: fixed;
  background-position-y: bottom;
  background-size: cover;
  background-repeat: no-repeat;
  overflow: hidden;
  }



</style>

