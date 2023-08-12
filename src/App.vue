<script setup lang="ts">
import Web3 from 'web3'
const web3 = new Web3(Web3.givenProvider || 'wss://mainnet.infura.io/ws/v3/6c5e1d3ae0f5407d88652c5e82fd72de')

const account = web3.eth.accounts.create('123456')
console.log(account.address)
</script>

<template>
  <div>
    <h1>{{ account.address }}</h1>
  </div>

</template>

<style scoped>


</style>
