<template>
  <div class="main" style="flex-direction: {{ direction }}">
    <div class="description">
      <h1>{{ title }}</h1>
      <span>{{ lead }}</span>
      <p>
        {{ paragraph }}
        Olá! Sou um profissional de tecnologia apaixonado, formado em Técnico em Informática e atualmente cursando Bacharelado em Ciência da Computação. Tenho experiência em manutenção de computadores, automação de processos e infraestrutura de rede. Além disso, possuo conhecimentos em VueJS, CodeIgniter, PHP e administração de redes Linux. Vamos colaborar?

      </p>
    </div>
    <div class="imageDiv">
      <img :src="imageUrl" :alt="imageAlt" :title="imageTitle" :longdesc="imageLongDesc"/>
    </div>
  </div>
</template>

<script defer>
export default {
    name: 'CardComponent',
    props: {
        direction     : String,
        title         : String,
        lead          : String,
        paragraph     : String,
        imageUrl      : String,
        imageAlt      : String,
        imageTitle    : String,  
        imageLongDesc : String
    }
};
</script>

<style scoped>

div.main{
    display: flex;
    flex-direction: row;
    flex-wrap: no-wrap;
    justify-content: center;
    align-items: center;
}

h1 {
  font-family: Ubuntu;
}

div.description{
    width: 50%;
    padding: 100px;
}

div.description > p{
    text-align: justify;
    font-family: monospace;
    font-size: 1.5rem;
}

div.imageDiv{  
    width: 50%;
}

div.imageDiv > img {
    width: 450px;
    height: 450px;
}

</style>