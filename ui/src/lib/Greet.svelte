<script>
    import { invoke } from '@tauri-apps/api/tauri'

    let name = ''
    let greetMsg = ''
  
    async function greet() {
      greetMsg = await invoke('greet', { name })
    }
</script>
  <div>
    <p>Page content</p>
    <input id="greet-input" placeholder="Enter a name..." bind:value="{name}" />
    <button class="btn"on:click="{greet}">Greet</button>
    <p>{greetMsg}</p>
</div>