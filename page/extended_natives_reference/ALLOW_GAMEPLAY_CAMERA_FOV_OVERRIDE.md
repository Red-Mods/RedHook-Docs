# ALLOW_GAMEPLAY_CAMERA_FOV_OVERRIDE `0x5E632574`

Allow the gameplay camera FOV to be overridden, bcs the game by default is resetting the value every frame.

> [!TIP]
> This function doesn't need to be ran every frame, just set it to **true**, when you need to override the FOV, and restore it to **false** when no longer needed.

```cpp
void ALLOW_GAMEPLAY_CAMERA_FOV_OVERRIDE(bool _Toggle);
```

#### Example

```cpp
REDHOOK::ALLOW_GAMEPLAY_CAMERA_FOV_OVERRIDE(true);

Camera gameplayCamera = CAM::GET_GAME_CAMERA();

CAMERA::SET_CAMERA_FOV(gameplayCamera, 100.0f); // Set the Gameplay FOV to 100.0
```