# using-signal

From [Using Signals](https://docs.godotengine.org/en/stable/getting_started/step_by_step/signals.html)

## Modifications

- Kept on using the player sprite from first-gdscript

## Key class and methods

- [`set_process`](https://docs.godotengine.org/en/stable/classes/class_node.html#class-node-method-set-process)
- `_on_button_pressed()`: built-in signal from Class Button that sends signal when the button is pressed
- `_on_timer_timeout()`: called directly from the script instead of connecting the signal in the Signals panel. Triggers visibility change when the timer wait time has been reached. Autostart toggled.
