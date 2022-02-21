<template>
    <div id="titlecomments">
        <div id="nbrfeedback">
            {{ comments.length }}
        </div>  
        <h2 id="prez-comment">Commentaires:</h2>
    </div>
    <article id="feedback">
        <ul>
            <li v-for="comment in comments" :key="comment">
                <p>{{ comment.visitor }}</p>{{ comment.feedback }}<br />{{ comment.date }}
            </li>
        </ul>
    </article>
</template>



<script>
    import axios from 'axios'

    export default{
        name: 'comments',
        data(){
        return {
            comments: [],
            errors:[]
        }  
        },
        created() {
        axios.get('http://localhost:8080/comments.json')
        .then(response => (this.comments = response.data.comments))
        } 
    }

</script>



<style>

#titlecomments{
    margin-top: -860px;
    display: flex;
    flex-direction: row;
    align-items: center;
    width: 100%;
}

#nbrfeedback {
    /* on donne un positionnement à tous les 'h2' */
    /* height: calc(100%-90px); */
    margin-top: 20px;
    margin-left: 20px;
    max-height: 1.6em;
    font-family: 'Source Serif Pro', serif;
    font-size: 24px;
    text-shadow: 1px 3px 1px rgb(61,166,193);
    color: rgb(13,40,89);
}

#feedback ul {
    list-style-type: none;
    padding-left: 0;
}

#feedback li{
    margin-top: 20px;
    margin-left: 10px;
    width: calc(100vw - 30px);
    font-family: 'Trebuchet MS','Lucida Grande','Lucida Sans Unicode','Lucida Sans',Tahoma,sans-serif;
    font-size: 14px;
    background-color: rgba(255, 255, 255, 0.63);
}

#feedback ul li p{
    font-weight: bold;
    color: rgb(13,40,89);
    text-shadow: 1px 3px 1px rgba(255, 255, 255, 0.63);
}


</style>