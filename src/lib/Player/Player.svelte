<script lang="ts">
  let { src } = $props<{ src: string }>();

  let player = $state<HTMLVideoElement | null>(null);

  $inspect(player);
</script>

<video bind:this={player} controls {src}> </video>
