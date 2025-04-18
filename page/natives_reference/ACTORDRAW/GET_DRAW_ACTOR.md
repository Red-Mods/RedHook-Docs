# GET_DRAW_ACTOR `0x085A9CA6`

Get if an actor is visible or not

```cpp
bool GET_DRAW_ACTOR(Actor _Actor);
```

```cpp
// Get the visible state of the local player
Actor localPlayerActor = ACTOR::GET_PLAYER_ACTOR(-1);

bool isVisible = ACTOR::GET_DRAW_ACTOR(localPlayerActor);

Print(Log_Info, "IsVisible: %d", isVisible); // Print in console
```