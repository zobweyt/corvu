<div align="center">
  <a href="https://corvu.dev">
    <img src="https://corvu.dev/readme/corvu.png" width=1000 alt="corvu banner" />
  </a>
</div>
<br />
<div align="center">

![NPM Downloads](https://img.shields.io/endpoint?color=a888f1&label=downloads&url=https://combined-npm-downloads.deno.dev/@corvu/accordion,@corvu/calendar,@corvu/dialog,@corvu/disclosure,@corvu/drawer,@corvu/otp-field,@corvu/popover,@corvu/resizable,@corvu/tooltip)
[![License](https://img.shields.io/github/license/corvudev/corvu?color=a888f1)](https://github.com/corvudev/corvu/blob/main/LICENSE)

**[Documentation](https://corvu.dev/) • [Discussion](https://github.com/corvudev/corvu/discussions) • [Discord](https://discord.com/invite/solidjs)**
</div>

## About
This is the [UnoCSS](https://unocss.dev/) preset for [corvu](https://corvu.dev/). It adds variants to style primitives based on their state:

```tsx
<Dialog.Content
  class="corvu-open:animate-in corvu-closed:animate-out"
>
  ...
</Dialog.Content>
```

## Getting started
Install the plugin with the package manager of your choice:

```bash
npm install @corvu/unocss
```

Then add the preset to your `uno.config.tsx` file:

```ts
import { defineConfig } from 'unocss'
import presetCorvu from '@corvu/unocss'

export default defineConfig({
  // ...
  presets: [
    // Use it with the default prefix 'corvu'
    presetCorvu(),
    // or with a custom prefix
    presetCorvu({ prefix: 'ui' }),
    // ...
  ],
})
```
