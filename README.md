# Learning Vue Fundamentals

### Install

`npm init vite`
then
`npm install`

### Run

`npm run dev`

## Lessons

- HelloWorld:
  - defineProps
  - pass props from parent to children
- MyForm:
  - Add ref to input
  - Display ref value
  - (v-on)@click to call functions
  - (v-bind):disabled="" to bind an attribute to an expression
  - life cycle hook: onMounted
- CaptionContent:
  - Use slot to pass in component from parent
  - Name slot to use multiple
  - use source to pass value to parent
- TypingForm:
  - WatchEffect to rerender DOM when condition changes
  - v-if for condition rendering component
  - onInvalidate argument
  - stop watcher
- VueEmit + CustomInput
  - Emit: Send custom events from child component to parent, optionally with a payload

# Vue 3 + Vite

This template should help get you started developing with Vue 3 in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

## Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).
