<script>
    export let bg = "";
    export let my = "my-0"
    export let p=""
    export let height=''
  </script>
  
  <section class="container-fluid jumbotron rounded-0  {bg} {my} {p} {height}">
    <slot />
  </section>