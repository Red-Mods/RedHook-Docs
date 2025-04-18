# TELEPORT_ACTOR_WITH_HEADING `0xE4DE507C`

Teleport an actor at a specfic position & heading.

```cpp
void TELEPORT_ACTOR_WITH_HEADING(Actor _Actor, Vector2 _PositionXY, float _PositionZ, float _Heading, bool _UnkFlag0, bool _UnkFlag1, bool _UnkFlag2);
```

> [!WARNING]
> This example below use 'PACK_VECTOR3' macro featured in [RedHookSDK](https://github.com/K3rhos/RedHookSDK/blob/main/Headers/Structs.h#L239).

```cpp
// Teleport the local player to Blackwater with a 90° heading
Actor localPlayerActor = ACTOR::GET_PLAYER_ACTOR(-1);

Vector3 position = Vector3(711.18f, 78.31f, 1252.763f);
float heading = 90.0f;

ACTOR::TELEPORT_ACTOR_WITH_HEADING(localPlayerActor, PACK_VECTOR3(position), heading, false, false, false);
```