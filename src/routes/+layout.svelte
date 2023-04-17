<script lang="ts">
    import Header from "../components/header.svelte";
    import Footer from "../components/footer.svelte";    
    import "../app.css";
</script>
  
    
      <Header/>      
      <main>
        <slot/>
      </main>
      <Footer/>
      
    