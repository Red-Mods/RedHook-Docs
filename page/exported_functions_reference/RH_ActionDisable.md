# RH_ActionDisable

Disable a game action by passing an ActionName and a state (disabled/enabled).

> [!CAUTION]
> Pretty sure I'm gonna delete this function in the future, bcs I'm now using the in-house **"natives invoker"** R* is using to register their script functions.
> So I'm probably gonna replace this exported function and add it to my custom natives db.
> 
> So please don't use this function to much in your code, or make a wrapper, so you can just replace the function later easily.

```cpp
void RH_ActionDisable(const char* _ActionName, bool _Disabled);
```