<template>
  <main class="column items-center justify-center">
    <h1>Faça seu Login</h1>

    <form action="">
      <div class="q-pa-md formContainer">
        <div class="pDiv">
          <p>Que bom ter você denovo!</p>
        </div>
        <q-form @submit="onSubmit" @reset="onReset" class="q-gutter-md">
          <div>
            <AccountsInputComponent lable="Username" type="text" />
            <AccountsInputComponent lable="Senha" type="password" />

            <ButtonComponent text="Entrar" to="/" />
          </div>
        </q-form>
      </div>
    </form>
  </main>
</template>

<script>
import AccountsInputComponent from 'src/components/AccountsInputComponent.vue'
import ButtonComponent from 'src/components/ButtonComponent.vue'

export default {
  name: 'LoginPage',
  components: {
    AccountsInputComponent,
    ButtonComponent,
  },
}
</script>

<style scoped>
main {
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.formContainer {
  text-align: center;
  width: 512px;
  padding: 40px 24px;
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.03);
}

h1 {
  font-size: 36px;
  color: #4f4f4f;
  font-weight: 600;
  margin-bottom: 24px;
}

.pDiv {
  margin-bottom: 32px;
}

p {
  color: #98a2b3;
  font-size: 16px;
  font-weight: 500;
  line-height: 25px;
}
</style>
