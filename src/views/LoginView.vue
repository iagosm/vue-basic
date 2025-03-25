<script setup> // Composition Api
  import {ref, reactive, onMounted} from 'vue';

  // const email = ref('');
  // const password = ref('');

  const user = reactive({
    email: '',
    password: ''
  })

  const login = () =>{
    console.log(user)
  }

  function remove(user) {
    const index = names.findIndex(name => name.firstName === user.firstName);
    names.splice(index, 1)
  }

  const names = reactive([]);

  onMounted(() => {
	  names.push(
      {
        firstName: 'Iago',
        age:25
      },
      {
        firstName: 'Joao',
        age:78
      },
      {
        firstName: 'Maia',
        age:15
      },
    );
  })
</script>
<template>
  {{ email }}
  {{ password }}

  <template v-if="names.length > 0">
    <ul>
      <li v-for="name in names">{{ name.firstName }} - <button v-on:click="remove(name)">remove</button></li>
    </ul>
  </template>
  <template v-else>Nenhum user encontrado</template>

  <template v-if="user.email.length <= 0">Email vazio</template>
  <template v-else>Email: {{user.email}}</template>

  <form action="" v-on:submit.prevent="login">
    <input type="text" placeholder="Email" v-model="user.email">
    <input type="text" placeholder="Password" v-model="user.password">
    <button type="submit">Login</button>
  </form>

</template>
<style></style>