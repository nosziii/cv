<template>
  <div>
    <Header/>
    <Body/>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import Body from '@/components/Body.vue'
import Footer from '@/components/Footer.vue'
import Test from 'raw-loader'
// import dsd from './assets/test.txt'

export default {
  name: 'Wiki',
  components: {
    Header,
    Body,
    Footer
  },
  methods: {

  },
  created() {
    // console.log("==== dsd", dsd)
    console.log("==== Test", Test('./assets/test.txt'))
  }
}
</script>
