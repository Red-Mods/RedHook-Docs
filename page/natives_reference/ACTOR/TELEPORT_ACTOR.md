# TELEPORT_ACTOR `0x2D54B916`

Teleport an actor at a specfic position.

```cpp
void TELEPORT_ACTOR(Actor _Actor, const Vector3* _Position, bool _UnkFlag0, bool _UnkFlag1, bool _UnkFlag2);
```

```cpp
// Teleport the local player to Blackwater
Actor localPlayerActor = ACTOR::GET_PLAYER_ACTOR(-1);

Vector3 position = Vector3(711.18f, 78.31f, 1252.763f);

ACTOR::TELEPORT_ACTOR_WITH_HEADING(localPlayerActor, &position, false, false, false);
```