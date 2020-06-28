<template>
  <Layout>
    <About />
    <Videos />
  </Layout>
</template>

<script>
import About from '../components/About';
import Videos from '../components/Videos';
export default {
  components: {
    About,
    Videos,
  },
  metaInfo: {
    title: 'Home',
  },
};
</script>
