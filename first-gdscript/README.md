# first-gdscript
Combined [Creating your first script](https://docs.godotengine.org/en/stable/getting_started/step_by_step/scripting_first_script.html) and [Listening to User Input](https://docs.godotengine.org/en/stable/getting_started/step_by_step/scripting_player_input.html).

## Modifications

- Changed played sprite.
- Instead of rotate with the left and right arrow keys and move forward by pressing `Up`, the player is able to move up, down, left and right with the respective arrow key or with `w` `s` `a` `d`. The player can also rotate clock- or anticlockwise with `e` or `q`

## Key methods

- `_process(delta)` see [Node._process()](https://docs.godotengine.org/en/stable/classes/class_node.html#class-node-method-process). More on [Idle and Physics Processing](https://docs.godotengine.org/en/stable/tutorials/scripting/idle_and_physics_processing.html).

- `Input` singleton see [`InputEventAction`](https://docs.godotengine.org/en/stable/classes/class_inputeventaction.html#class-inputeventaction) and [`InputMap`](https://docs.godotengine.org/en/stable/classes/class_inputmap.html#class-inputmap). The input map in this project is defined in the project settings instead of being hard coded.
