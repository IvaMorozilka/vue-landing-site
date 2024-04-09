<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import JSConfetti  from 'js-confetti';

const jsConfetti = new JSConfetti();


</script>

<template>
  <header>
    <!-- <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div> -->

    <div>
      <h1>Здесь будет разрабатываться сайт</h1>
    </div>
  </header>

  <main>
    <!-- <TheWelcome /> -->
    <h2>Идет настройка проекта... Скоро появится хеадер :)</h2>
    <img id = 'zdun' @click = "jsConfetti.addConfetti({emojis: ['😎','👀','🧐']})" src="https://resizer.mail.ru/p/8e2e46c4-7137-5f91-8a6a-7bf4e963c943/AQACB_rBp9_0xvGVY942sS8CqVucCdtu8YKpYJacXOxNAs-gEpeDt2EturYJt-hSXunjquPgOmmBEuTD5ohw9vxeLUw.jpg">
  </main>
</template>

<style scoped>
#zdun {
  cursor: pointer;
}
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
