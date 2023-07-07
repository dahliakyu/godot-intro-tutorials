# dodge-the-creep

From [Your first 2D game](https://docs.godotengine.org/en/stable/getting_started/first_2d_game/index.html)

## Project Structure

- Main Scene
  - Child Scenes
	- Player (instantiated directly from the 'Scene' panel)
	- HUD (Heads up display, also instantiated directly from the 'Scene' panel)
	- Mob (instantiated as [PackedScene](https://docs.godotengine.org/en/stable/classes/class_packedscene.html) in main.gd, allows choosing different scenes as the "Mob Scene" in the Inspector panel under "Script Variables")
  - Other Child Nodes
	- ColorRect: Provide a background colour for the game
	- Timers
	  - MobTimer: 0.5s, time taken for new mob to spawn
	  - ScoreTimer: 1s, +1 score for every second survived
	  - StartTimer: 2s, one shot, delayed start for the game
	- StartPosition ([Marker2D](https://docs.godotengine.org/en/stable/classes/class_marker2d.html))
	- MobPath ([Path2D](https://docs.godotengine.org/en/stable/classes/class_path2d.html))
	  - MobSpawnLocation ([PathFollow2D](https://docs.godotengine.org/en/stable/classes/class_pathfollow2d.html#class-pathfollow2d))
	- Music and DeathSound ([AudioStreamPlayer2D](https://docs.godotengine.org/en/4.0/classes/class_audiostreamplayer2d.html))

- Player Scene 
  - Grouped Child Nodes
	- [AnimatedSprite2D](https://docs.godotengine.org/en/stable/tutorials/2d/2d_sprite_animation.html):
	  - up: 5fps
	  - walk: 5fps
	- [CollisionShape2D](https://docs.godotengine.org/en/stable/classes/class_collisionshape2d.html)
  - Script (player.gd)
	- Player Input:
	  - up, down, left, right
