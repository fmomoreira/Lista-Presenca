<script>
 import Tasks from "./Tasks/Task.svelte"; // permite incluir um componente
 const projectName = "Visita LosHope";
 const src = "https://s2.glbimg.com/9TytIChyyDB4gRdgiq6fyl7sP5k=/0x0:1152x864/1000x0/smart/filters:strip_icc()/i.s3.glbimg.com/v1/AUTH_59edd422c0c84a879bd37670ae4f538a/internal_photos/bs/2019/3/x/oMAiA9R6Awm8zOOikAOw/navio-logos-hope-2-.jpeg";

</script>

<section class="section">
 <div class="container">
   <figure class="image is-200x200">
     <img id="imagembarco"{src} alt="Svelte3" />
   </figure>
   <h1 class="title">{projectName}</h1>
   <p class="subtitle">
     Total de Pessoas:
     <strong id="resultadofinal"></strong>
   </p>
 </div>
 <Tasks /> <!-- aqui o componente é incluido -->
</section>