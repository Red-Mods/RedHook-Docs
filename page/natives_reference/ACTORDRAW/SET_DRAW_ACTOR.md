# SET_DRAW_ACTOR `0xE6644CE5`

Set if an actor is visible or not

```cpp
void SET_DRAW_ACTOR(Actor _Actor, bool _Draw);
```

```cpp
// Set the currently riden mount by the local player invisible
Actor localPlayerActor = ACTOR::GET_PLAYER_ACTOR(-1);

if (RIDING::IS_ACTOR_RIDING(localPlayerActor))
{
    Actor mount = RIDING::GET_MOUNT(localPlayerActor);

    ACTOR::SET_DRAW_ACTOR(mount, false);
}
```