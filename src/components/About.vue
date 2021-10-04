<template>
<div>
<section class="location-section">
    <h1>Sobre mim</h1>
    <p>Eu sou cidadão do ponto mais oriental das américas! João Pessoa, Paraíba.</p>
</section>
<section class="questions-section">
    <h2>Experiência profissional:</h2>
    <p>Possuo experiência fullstack, no qual ja trabalhei com intergração de sistemas com PHP, 
    Postgres e os mais diversos frameworks front-end.Atualmente trabalho apenas como desenvolvedor front-end, com as principais stacks do mercado javascript</p>
    <h2>Meus hobbies?</h2>
    <p>Estudar sobre front-end, viajar de moto e conhecer novos lugares!</p>
    <h2>Minha forma de trabalho atual</h2>
    <p>Hoje construo aplicações front-end preferênciamente com reactjs e vuejs em meus freelas.</p>
</section>
</div>
</template>

<script>
export default {
    name:'Sobre'
}
</script>

<style>
  body {
    /* Typography Declarations */
    color: #222222;
    font-size: 1em;
    font-family: "Open Sans", "Helvetica Neue", sans-serif;
}

.content-footer,
.masthead-heading,
.masthead-intro {
  text-align: center;
}

.masthead {
  padding: 6em 0;
  background-image: url('https://i.imgur.com/yGmrlyg.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  border-top: solid 1em #FFCF33;
}

.masthead-intro {
    /* Layout Declarations */
    margin-bottom: 0.1em;
    /* Typography Declarations */
    font-family: "Gentium Book Basic", Georgia, serif;
    font-size: 2em;
}

.masthead-heading {
    /* Layout Declarations */
    color: #F1C863;
    margin-top: -0.2em;
    /* Typography Declarations */
    font-family: "Open Sans", "Helvetica Neue", sans-serif;
    font-weight: bold;
    font-size: 6em;
    letter-spacing: -0.02em;
    text-transform: uppercase;
}

.introduction-section,
.location-section,
.questions-section {
    max-width: 38em;
    margin-left: auto;
    margin-right: auto;
    margin-top: 2em;
}

.introduction-section > p,
.location-section > p,
.questions-section,
.content-footer > p {
    /* Typography Declarations */
    font-weight: 300;
    letter-spacing: 0.05em;
}

.questions-section > h2 {
    font-family: "Gentium Book Basic", Georgia, serif;
    font-size: 1.2em;
    font-weight: bold;
    /* Layout */
    margin: 2em 0 1em 0;
}

section > h1 {
    margin-top: 2em;
}

.content-footer,
.masthead-heading,
.masthead-intro {
  text-align: center;
}

.masthead {
  padding: 6em 0;
  background-image: url('https://i.imgur.com/yGmrlyg.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  border-top: solid 1em #FFCF33;
}

.masthead-intro {
  margin-bottom: 0.1em;
  font-family: "Gentium Book Basic", Georgia, serif;
    font-size: 2em;
}

.masthead-heading {
  margin-top: -0.2em;
  font-family: "Open Sans", "Helvetica Neue", sans-serif;
  font-weight: bold;
  font-size: 6em;
  letter-spacing: -0.02em;
  text-transform: uppercase;
}
.introduction > p,
.location > p,
.content-footer > p {
    /* Typography Declarations */
    font-weight: 300;
    letter-spacing: 0.05em;
}
h2 {
    /* Typography Declarations */
    font-family: "Gentium Book Basic", Georgia, serif;
    font-size: 1.2em;
    font-weight: bold;
}

.introduction-section,
.location-section,
.questions-section {
    max-width: 38em;
    margin-left: auto;
    margin-right: auto;
    margin-top: 2em;
}
.content-footer {
  margin: 50px 0;
  padding: 20px 0;
  text-align: center;
  background-color: #73A8C2;
  text-decoration: none;
}
.social > li {
  display: inline-block;
  margin: 0 5px;
}
.content-footer > p {
  color: #F7EDE1;
}
a {
    font-weight: bold;
    text-decoration: none;
    color: #F1C863;
}
  
@media only screen and (max-width: 500px) {
    .masthead {
        padding: 3em 0;
    }
    .masthead-heading {
        font-size: 3em;
    }
    .content-footer {
        padding: 2em 2.5em;
  }
}
</style>