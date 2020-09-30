# Tooltip

Pure css hover-activated tool-tip configured with custom HTML attributes.<br>**Implementation**: [View article on Medium](https://medium.freecodecamp.org/a-step-by-step-guide-to-making-pure-css-tooltips-3d5a3e237346)

<p align="center"><img width="400px" src="https://i.ibb.co/hm5nc0J/tooltips.png"></p>

## Features

- Two new HTML attributes that define a tool-tip and its position:

  - `tooltip` - The text content of the tool-tip pseudo-element
  - `tooltip-position` - The position of the tooltip (relative to current element)

  **Examples**:

  ```html
  <button tooltip="Button 1" tooltip-position="top">Button</button>
  <button tooltip="Button 2" tooltip-position="right">Button</button>
  <button tooltip="Button 3" tooltip-position="bottom">Button</button>
  <button tooltip="Button 4" tooltip-position="left">Button</button>
  ```

- An SCSS map for some basic tool-tip styling customization:

  ```scss
  $tooltip: (
      padding: 4px 2px,
      min-width: 80px,
      font-size: 12px,
      border-width: 4px 6px 0 6px,
      border-style: solid,
      border-color: rgba(0,0,0,0.7) transparent transparent transparent,
      border-radius: 3px,
      background-color: rgba(0,0,0,0.7),
      color: white,
  );
  ```

  **Note**: New CSS attributes for the tool-tip cannot be added to this map.
