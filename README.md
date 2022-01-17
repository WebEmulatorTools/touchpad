# Touchpad

A gamepad overlay compatible with touch devices that emulates a real controller by hijacking the gamepad API.

# Usage

```
  <div id="gamepad"></div>
  <script>
    gamePadType = 'simple'; // (Optional)
  </script>
  <script src="touchpad.js"></script>
```

Available gamepad types: 
* default- Leave `gamePadType` unset to render an snes style gamepad on page.
* simple- Two button gamepad similar to nes.
* modern- Full dual analog style controller.

### Loading in dynamically

```
if (myCondition) {
  var touchDiv = document.createElement('div');
  touchDiv.setAttribute('id', 'gamepad');
  document.body.appendChild(touchDiv);
  var touchscript = document.createElement('script');
  touchscript.src = 'touchpad.js';
  document.head.append(touchscript);
}
```
