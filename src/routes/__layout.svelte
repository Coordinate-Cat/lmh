<script>
  import "../assets/styles/global.css";
  import Header from "$lib/components/Header.svelte";
  import Container from "$lib/components/Container.svelte";
  import Content from "$lib/components/Content.svelte";
  // @ts-ignore
  import Background from "$lib/components/Background.svelte";
  // import Footer from "$lib/components/Footer.svelte";
</script>

<Background />
<Container>
  <Header />
  <Content>
    <slot />
  </Content>
  <!-- <Footer /> -->
</Container>
