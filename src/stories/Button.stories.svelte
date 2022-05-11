<script>
  import { Meta, Template, Story } from "@storybook/addon-svelte-csf";
  import { withDesign } from 'storybook-addon-designs';
  import Button from "./Button.svelte";
</script>

<!-- More on default export: https://storybook.js.org/docs/react/writing-stories/introduction#default-export -->
<!-- More on argTypes: https://storybook.js.org/docs/svelte/api/argtypes -->
<Meta
  title="Example/Button" 
  decorators={[withDesign]}
  component={Button}
  argTypes={{
    label: { control: "text" },
    onClick: { action: "onClick" },
    type: { 
      control: { type: 'select' },
      options: ['Primary', 'Secondary', 'Destructive'], 
    },
    size: {
      control: { type: 'select' },
      options: ['small', 'medium', 'large'],
    },
    disabled: {
      control: { type: "boolean" },
    }
  }}
/>

<!-- More on component templates: https://storybook.js.org/docs/svelte/writing-stories/introduction#using-args -->
<Template let:args>
  <Button {...args} on:click={args.onClick} />
</Template>

<!-- More on args: https://storybook.js.org/docs/svelte/writing-stories/args -->
<Story
  name="Primary"
  parameters={{
    design: {
      type: 'figma',
      url: 'https://www.figma.com/file/zRTmnRLepOqUdFdtZyh97t/Components?node-id=9%3A12510'
    }
  }}
  args={{
    type: 'Primary',
    label: "Button",
  }}
/>
