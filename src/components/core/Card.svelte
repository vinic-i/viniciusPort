<script>
  export let className = "p-4";
  export let shadow = false;
  export let animation = "";
  export let delay = "";
  export let duration = "";
</script>

<style>
  .box-shadow {
    -webkit-box-shadow: -9px 11px 22px 0px rgba(0, 0, 0, 0.16);
    -moz-box-shadow: -9px 11px 22px 0px rgba(0, 0, 0, 0.16);
    box-shadow: -9px 11px 22px 0px rgba(0, 0, 0, 0.16);
  }
  .custom-card {
    /* border-radius: 1rem !important; */
    -webkit-transform: translateZ(0);
    transform: translateZ(0);
    transition-duration: 0.5s;
  }
</style>

<div
  data-aos={animation}
  data-aos-delay={delay}
  data-aos-duratio={duration}
  class="card py-4 h-100 custom-card {shadow ? 'shadow' : ''} ">
  <div class="card-body text-center {className}">
    <slot />
  </div>
</div>
