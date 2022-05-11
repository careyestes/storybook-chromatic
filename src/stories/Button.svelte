<script>
  import './button.css';
  import { createEventDispatcher } from 'svelte';

  export let type = 'Primary';
  export let size = 'medium';
  export let disabled = false;
  export let label = '';
  
  let mode;

  switch (type) {
    case 'Primary':
      mode = 'storybook-button--primary';
      break;
    case 'Secondary':
      mode = 'storybook-button--secondary';
      break;
    case 'Destructive':
      mode = 'storybook-button--destructive';
      break;
    default:
      mode = 'storybook-button--primary';
  }



  const dispatch = createEventDispatcher();

  /**
   * Optional click handler
   */
  function onClick(event) {
    dispatch('click', event);
  }
</script>

<button
  type="button"
  class={['storybook-button', `storybook-button--${size}`, mode].join(' ')}
  disabled={disabled}
  on:click={onClick}>
  {label}
</button>
