# Contributing

It is normal compiled CSS to generate complex conflicts to be resolved, perhaps best would be to avoid compiling, but for now, be free to compile it and keep your development branch always up to date.

## Guidelines

Follow the setting to compile SASS using Terminal for the Minimal style example:

```
sass --watch minimal/_main.scss:minimal.css --style expanded --precision 3 --no-cache --sourcemap=none
```  

#### About the CSS Property Ordering  

The goal is avoid conflicts and confusion while reading the code, for this reason, try to keep this property ordering that follows:

```
selector {
  color: rgba(20,23,26,0.9);    // main color
  ...
  font-size: 14px;              // Font size
  ...
  font-weight: bold;            // Followed by others font properties.
  font-style: italic;
  ...
  line-height: 1.5em;           // leading
  ...
  letter-spacing: 1px;          // Letter or Word spaces
  ...
  text-transform: uppercase;    // Texts customizations
  ...
  margin: 0 0 30px 6px;         // Margin and Padding
  padding: 15px 0 30px 6px;
  ...
  width: 100%;                  // Width and height
  height: 190px;
  ...
  border: 1px solid red;        // Borders and box
  border-bottom: none;
  border-collapse: collapse;
  box-shadow: none;
  ...
  display: none;                // Display
  ...
  background: #fff;             // Background
  ...
  position: relative;           // Position and specs
  left: 10px;
  z-index: 100;
}
```
