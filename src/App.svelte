<script lang="ts">
  import BottomNav from './lib/components/BottomNav.svelte'
  import Router from './lib/routes/index.svelte'
</script>

<main>
  <Router />
</main>

<div class="sm:hidden">
  <BottomNav />
</div>
