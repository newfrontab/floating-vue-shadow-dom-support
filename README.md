### Forked version of https://github.com/Akryum/floating-vue/releases/tag/v2.0.2

### Changes
- Add support for running v-tooltip in shadow dom
- New option (rootNode) where you assign the root of the shadow dom

This addresses a bug where tooltips doesn't close when existing in shadow dom. This was caused by "lib/tooltip.js > _scheduleHide" where it searched the light dom for an open tooltip which it couldn't find.
