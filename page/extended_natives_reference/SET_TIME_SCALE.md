# SET_TIME_SCALE `0xA7F84694`

Override the current game time scale.

> [!NOTE]
> Doesn't apply when using deadeye, there is already a game native for that.

```cpp
void SET_TIME_SCALE(float _TimeScale);
```

#### Example

```cpp
// Game frozen
REDHOOK::SET_TIME_SCALE(0.0f);

// Slow motion (x0.5)
REDHOOK::SET_TIME_SCALE(0.5f);

// Game execution is 2 times faster (speedhack)
REDHOOK::SET_TIME_SCALE(2.0f);
```