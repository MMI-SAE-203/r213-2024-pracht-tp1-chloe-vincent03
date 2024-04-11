<script setup lang="ts">
//

import { ref } from 'vue';

const sectionOpen = ref(1)
//*log('sectionOpen:', sectionOpen.value)*//


</script>

<template>
  <h1>Accordeon</h1>
  <section>
  <button class="text-xl" @pointerdown="sectionOpen = 1">bouton 1</button>
    <p v-show="sectionOpen === 1">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aperiam, placeat fuga accusamus eveniet enim, aliquid in eos, ipsa blanditiis rerum explicabo. Aliquid aut eaque delectus veniam eius necessitatibus magni nobis.</p>
  </section>
  <section>
    <button class="text-xl" @pointerdown="sectionOpen = 2">bouton 2</button>
    <p v-show="sectionOpen === 2">Rerum eveniet iusto rem mollitia alias saepe corrupti sapiente similique officia voluptates delectus dicta amet voluptatum, ea dolor. Quibusdam molestias velit quas repudiandae expedita adipisci cumque quam totam cum maiores.</p>
  </section>
  <section>
    <button class="text-xl" @pointerdown="sectionOpen = 3">bouton 3</button>
    <p v-show="sectionOpen === 3">Voluptatibus tempore nisi animi vel distinctio, quam, laudantium nostrum laboriosam, maiores temporibus corporis omnis? Commodi inventore vel voluptate, recusandae ipsam quos minus cupiditate ut atque, nisi, fuga quia tenetur reiciendis!</p>
  </section>
</template>
