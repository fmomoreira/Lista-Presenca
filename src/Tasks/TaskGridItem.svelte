<script>
 // props recebem valores do componente superior
 export let id; 
 export let description;
 // permite utilizar o dispatch
 import { createEventDispatcher } from "svelte";
 const dispatch = createEventDispatcher();
</script>
<tr>
 <td>{description}</td>
 <!-- event dispatch: enviando eventos com dados para o componente superior -->
 <td on:click={() => dispatch('edit', { id: id, description: description })}>
   <i class="fas fa-edit" />
 </td>
 <td on:click={() => dispatch('delete', { id: id })}>
   <i class="fas fa-trash" />
 </td>
</tr>
