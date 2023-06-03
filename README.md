# wgpu-conway-game-of-life
Conway game of life in WebGPU. Very notes heavy, non clean version for my own learning.

## Personal Notes
- `<script type='modules'>` allows for top-level `await`. Works only at the top level of modules and only works with `type='modules`
- Cool benefits
- Dynamic dependency pathing: use runtime values in order to determine dependencies so you can have development/production splits, internationalization. Example ```const strings = await import(\`/i18n/${navigator.language}\`);```
- Resource initialization `const connection = await dbConnector();` 
- WebGPU allows for canvas configuration to be seperate from device creation. This allows for any number of canvases to render on a single device. Allows for multi-pane 3D editors much easier to develop 