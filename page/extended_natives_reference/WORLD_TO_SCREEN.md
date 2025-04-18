# WORLD_TO_SCREEN `0xBAA72911`

Convert world position to 2D screen position.

> [!WARNING]
> **`_X`** **& `_Y`** are in 0.0 to 1.0 based coordinates.
> That mean 0.0, 0.0 represent the top left corner of your screen, and 1.0, 1.0 the bottom right.

```cpp
bool WORLD_TO_SCREEN(Vector3* _WorldPosition, float* _X, float* _Y);
```

#### Example

```cpp
Actor localPlayerActor = ACTOR::GET_PLAYER_ACTOR(-1);

Vector3 playerPosition = ACTOR::GET_POSITION(localPlayerActor);

float x, y;
if (REDHOOK::WORLD_TO_SCREEN(&playerPosition, &x, &y))
{
    Print(Log_Info, "%f %f", x, y); // Output the screen coordinates.
}
```