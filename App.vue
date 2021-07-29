<template lang="html">

    <h4> 404 NOT FOUND </h4>

    <img class="bounce" src="./assets/Scarecrow.png" alt="Scarecrow">

    <div class="badNews">

      <h1> I have bad news for you </h1>

      <div class="page">
        <p>
          The page you are looking
          for might be removed or
          is temporarily unavailable
        </p>
      </div>

      <button type="button" name="button"> BACK TO HOMEPAGE </button>

    </div>
    <Footer />
</template>

<script>
import Footer from './components/Footer.vue';
export default {
  components: {
    Footer
  }
}
</script>

<style lang="css" scoped >

  @import url('https://fonts.googleapis.com/css2?family=Space+Mono&display=swap');

  h4 {
    margin: 0 1rem 9rem 0;
    font-family: 'Space Mono', monospace;
  }

  h1 {
    font-size: 4rem;
    color: #333333;
  }

  p {
    font-size: 1rem;
    color: #4f4e4e;
    margin-bottom: 3.5rem;
  }

  img {
    max-width: 22rem ;
    margin-left: 5rem;
  }

  .badNews {
    position: relative;
    bottom: 20rem; left: 40%;
    width: 55%;
    font-family: 'Space Mono', monospace;
  }

  .page {
    width: 50%
  }

  button {
    background-color: #333333;
    color: white;
    padding: 1.3rem;
    cursor: pointer;
    border: none;
  }

  button:hover {
    background-color: #5A5A5A
  }

  @media only screen and (max-width: 40rem) {
    img { margin-left: 0.5rem }
    .badNews {
      bottom: 0%; left: 0%;
      width: 100%;
      padding: 1rem;
    }
    h1 { font-size: 2.3rem }
    .page { width: 100%; font-size: 1.2rem }
    p { font-size: 1.2rem }
    button { margin-bottom: 3.5rem }
    span { margin-left: 10%}
}

</style>
