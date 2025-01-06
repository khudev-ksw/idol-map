<script>
    import { Node, Svelvet, Minimap, Controls } from 'svelvet';

    const nodes = ['Node 1', 'Node 2', 'Node 3', 'Node 4'];
  </script>
  
  <Svelvet id="my-canvas" width="{500}" height="{500}" TD controls>
    <Node />
    <Node id="alpha" bgColor="red" label="Default Node" />
    
    {#each nodes as node}
        <Node bgColor="blue" textColor="white" label={node} />
    {/each }

    <Node />
  </Svelvet>
  

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>