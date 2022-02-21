<template>
    <nav id="move-buttons">
        <router-link to="/rechercher">RECHERCHER</router-link>
        <router-link to="/a-propos">A PROPOS</router-link>
        <router-link to="/about-me">ABOUT ME</router-link>
        <router-link to="/contact">CONTACT</router-link>
        <router-link to="/copyright">COPYRIGHT</router-link>
        <div id="bouton-admin"><router-link to="/connexion">CONNEXION</router-link></div>
    </nav>
</template>

<script>
export default {
  name: 'Navigation',
  props: {

  }
}
</script>

<style>

    #move-buttons {
    /* les boutons de navigation sont cachés
    et on leur donne une largeur de 0%
    pas vu ... pas pris */
    visibility: hidden;
    width: 0%;
    display: flex;
    flex-direction: column;
    text-align: center;
    }

/* ███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████
   premier point de rupture
   Sur uniquement les écrans, quand la largeur de la fenêtre fait au minimum 700px et au maximum 913px */
@media screen and (min-width: 700px) and (max-width: 913px)
{
    #move-buttons {
    /* les boutons de navigation ne sont plus sont cachés */
    visibility: visible;
    width: 200px;
    height: 100%;
    margin-top: 172px;
    padding-right: 10px;
    text-align: center;
    }

    #move-buttons a {
    background: rgb(61,166,193);
    background-image: -webkit-linear-gradient(top, rgb(61,166,193), rgb(61,166,193));
    background-image: -moz-linear-gradient(top, rgb(61,166,193), rgb(61,166,193));
    background-image: -ms-linear-gradient(top, rgb(61,166,193), rgb(61,166,193));
    background-image: -o-linear-gradient(top, rgb(61,166,193), rgb(61,166,193));
    /* background-image: -webkit-gradient(to bottom, rgb(61,166,193), rgb(61,166,193)); */
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
    width: 150px;
    color: rgb(255,255,255);
    text-decoration: none;
    font-family: 'Trebuchet MS','Lucida Grande','Lucida Sans Unicode','Lucida Sans',Tahoma,sans-serif;;
    font-weight: bold;
    font-size: 16px;
    font-weight: 600;
    padding: 10px;
    margin: 15px 50px 15px 15px;
    -webkit-box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    -moz-box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    text-shadow: 1px 1px 20px rgb(0,0,0);
    border: solid rgb(61,166,193) 1px;
    text-decoration: none;
    display: inline-block;
    cursor: pointer;
    text-align: center;
    }
     
    #move-buttons a:hover {
    border: solid rgb(61,166,193) 1px;
    background: rgb(186,199,0);
    background-image: -webkit-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -moz-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -ms-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -o-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    /* background-image: -webkit-gradient(to bottom, rgb(186,199,0), rgb(186,199,0)); */
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
    text-decoration: none;
    }

    #bouton-admin a {
    background: rgb(186,199,0);
    background-image: -webkit-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -moz-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -ms-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -o-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    /* background-image: -webkit-gradient(to bottom, rgb(186,199,0), rgb(186,199,0)); */
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
    color: rgb(255,255,255);
    font-family: 'Trebuchet MS','Lucida Grande','Lucida Sans Unicode','Lucida Sans',Tahoma,sans-serif;;
    font-size: 16px;
    font-weight: 600;
    padding: 10px;
    margin-top: 129px;
    -webkit-box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    -moz-box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    text-shadow: 1px 1px 20px rgb(0,0,0);
    border: solid rgb(61,166,193) 1px;
    text-decoration: none;
    display: inline-block;
    cursor: pointer;
    text-align: center;
    }
     
    #bouton-admin a:hover {
    border: solid rgb(186,199,0) 1px;
    background: rgb(213,0,80);
    background-image: -webkit-linear-gradient(top, rgb(213,0,80), rgb(213,0,80));
    background-image: -moz-linear-gradient(top, rgb(213,0,80), rgb(213,0,80));
    background-image: -ms-linear-gradient(top, rgb(213,0,80), rgb(213,0,80));
    background-image: -o-linear-gradient(top, rgb(213,0,80), rgb(213,0,80));
    /* background-image: -webkit-gradient(to bottom, rgb(213,0,80), rgb(213,0,80)); */
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
    text-decoration: none;
    }
}

/* ███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████
   second point de rupture
   Sur uniquement les écrans, quand la largeur de la fenêtre fait au minimum 914px et au maximum 1249px */
@media screen and (min-width: 914px) and (max-width: 1249px)
{
    #move-buttons {
    /* les boutons de navigation ne sont plus sont cachés */
    visibility: visible;
    width: 200px;
    height: 100%;
    margin-top: 172px;
    padding-right: 20px;
    text-align: center;
    }

    #move-buttons a {
    background: rgb(61,166,193);
    background-image: -webkit-linear-gradient(top, rgb(61,166,193), rgb(61,166,193));
    background-image: -moz-linear-gradient(top, rgb(61,166,193), rgb(61,166,193));
    background-image: -ms-linear-gradient(top, rgb(61,166,193), rgb(61,166,193));
    background-image: -o-linear-gradient(top, rgb(61,166,193), rgb(61,166,193));
    /* background-image: -webkit-gradient(to bottom, rgb(61,166,193), rgb(61,166,193)); */
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
    width: 150px;
    color: rgb(255,255,255);
    text-decoration: none;
    font-family: 'Trebuchet MS','Lucida Grande','Lucida Sans Unicode','Lucida Sans',Tahoma,sans-serif;;
    font-weight: bold;
    font-size: 16px;
    font-weight: 600;
    padding: 10px;
    margin: 15px 15px 15px 15px;
    -webkit-box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    -moz-box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    text-shadow: 1px 1px 20px rgb(0,0,0);
    border: solid rgb(61,166,193) 1px;
    text-decoration: none;
    display: inline-block;
    cursor: pointer;
    text-align: center;
    }
     
    #move-buttons a:hover {
    border: solid rgb(61,166,193) 1px;
    background: rgb(186,199,0);
    background-image: -webkit-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -moz-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -ms-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -o-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    /* background-image: -webkit-gradient(to bottom, rgb(186,199,0), rgb(186,199,0)); */
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
    text-decoration: none;
    }
    
    #bouton-admin a{
    background: rgb(186,199,0);
    background-image: -webkit-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -moz-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -ms-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -o-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    /* background-image: -webkit-gradient(to bottom, rgb(186,199,0), rgb(186,199,0)); */
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
    color: rgb(255,255,255);
    font-family: 'Trebuchet MS','Lucida Grande','Lucida Sans Unicode','Lucida Sans',Tahoma,sans-serif;;
    font-size: 16px;
    font-weight: 600;
    padding: 10px;
    margin-top: 129px;
    -webkit-box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    -moz-box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    text-shadow: 1px 1px 20px rgb(0,0,0);
    border: solid rgb(61,166,193) 1px;
    text-decoration: none;
    display: inline-block;
    cursor: pointer;
    text-align: center;
    }
     
    #bouton-admin a:hover {
    border: solid rgb(186,199,0) 1px;
    background: rgb(213,0,80);
    background-image: -webkit-linear-gradient(top, rgb(213,0,80), rgb(213,0,80));
    background-image: -moz-linear-gradient(top, rgb(213,0,80), rgb(213,0,80));
    background-image: -ms-linear-gradient(top, rgb(213,0,80), rgb(213,0,80));
    background-image: -o-linear-gradient(top, rgb(213,0,80), rgb(213,0,80));
    /* background-image: -webkit-gradient(to bottom, rgb(213,0,80), rgb(213,0,80)); */
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
    text-decoration: none;
    }
}

/* ███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████
   troisième point de rupture
   Sur uniquement les écrans, quand la largeur de la fenêtre fait au minimum 1250px */
@media screen and (min-width: 1250px)
{
   
#move-buttons {
    /* les boutons de navigation ne sont plus sont cachés */
    visibility: visible;
    width: 200px;
    height: 100%;
    margin-top: 137px;
    margin-left: 20px;
    text-align: center;
    }

    #move-buttons a {
    background: rgb(61,166,193);
    background-image: -webkit-linear-gradient(top, rgb(61,166,193), rgb(61,166,193));
    background-image: -moz-linear-gradient(top, rgb(61,166,193), rgb(61,166,193));
    background-image: -ms-linear-gradient(top, rgb(61,166,193), rgb(61,166,193));
    background-image: -o-linear-gradient(top, rgb(61,166,193), rgb(61,166,193));
    /* background-image: -webkit-gradient(to bottom, rgb(61,166,193), rgb(61,166,193)); */
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
    /* width: 150px; */
    color: rgb(255,255,255);
    text-decoration: none;
    font-family: 'Trebuchet MS','Lucida Grande','Lucida Sans Unicode','Lucida Sans',Tahoma,sans-serif;;
    font-weight: bold;
    font-size: 16px;
    font-weight: 600;
    padding: 10px;
    margin: 15px 15px 15px 15px;
    -webkit-box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    -moz-box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    text-shadow: 1px 1px 20px rgb(0,0,0);
    border: solid rgb(61,166,193) 1px;
    text-decoration: none;
    display: inline-block;
    cursor: pointer;
    text-align: center;
    }

    #move-buttons a:hover {
    border: solid rgb(61,166,193) 1px;
    background: rgb(186,199,0);
    background-image: -webkit-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -moz-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -ms-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -o-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    /* background-image: -webkit-gradient(to bottom, rgb(186,199,0), rgb(186,199,0)); */
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
    text-decoration: none;
    }
    
    #bouton-admin a{
    background: rgb(186,199,0);
    background-image: -webkit-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -moz-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -ms-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    background-image: -o-linear-gradient(top, rgb(186,199,0), rgb(186,199,0));
    /* background-image: -webkit-gradient(to bottom, rgb(186,199,0), rgb(186,199,0)); */
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
    color: rgb(255,255,255);
    font-family: 'Trebuchet MS','Lucida Grande','Lucida Sans Unicode','Lucida Sans',Tahoma,sans-serif;;
    font-size: 16px;
    font-weight: 600;
    padding: 10px;
    margin-top: 129px;
    -webkit-box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    -moz-box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    box-shadow: 1px 1px 20px 0 rgb(0,0,0);
    text-shadow: 1px 1px 20px rgb(0,0,0);
    border: solid rgb(61,166,193) 1px;
    text-decoration: none;
    display: inline-block;
    cursor: pointer;
    text-align: center;
    }
     
    #bouton-admin a:hover{
    border: solid rgb(186,199,0) 1px;
    background: rgb(213,0,80);
    background-image: -webkit-linear-gradient(top, rgb(213,0,80), rgb(213,0,80));
    background-image: -moz-linear-gradient(top, rgb(213,0,80), rgb(213,0,80));
    background-image: -ms-linear-gradient(top, rgb(213,0,80), rgb(213,0,80));
    background-image: -o-linear-gradient(top, rgb(213,0,80), rgb(213,0,80));
    /* background-image: -webkit-gradient(to bottom, rgb(213,0,80), rgb(213,0,80)); */
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
    text-decoration: none;
    }
    
}

</style>