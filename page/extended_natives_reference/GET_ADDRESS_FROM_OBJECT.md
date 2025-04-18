# GET_ADDRESS_FROM_OBJECT `0xFDCAED7C`

Get address from object id. (Works with actors/props, ...)

```cpp
uintptr_t GET_ADDRESS_FROM_OBJECT(Object _Object);
```

```cpp
Actor localPlayerActor = ACTOR::GET_PLAYER_ACTOR(-1);

uintptr_t addr = REDHOOK::GET_ADDRESS_FROM_OBJECT(localPlayerActor);

if (addr)
{
    BYTE entityType = *reinterpret_cast<BYTE*>(addr + 0x2C);
    
    Print(Log_Info, "%d", entityType);
}
```