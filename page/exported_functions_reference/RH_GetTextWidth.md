# RH_GetTextWidth

Return the width of a text by passing font id and font scale.

> [!WARNING]
> Return value is in 0.0 to 1.0 based coordinates.\
> That mean 0.0 represent no size and 1.0 is taking the whole screen width.

```cpp
float RH_GetTextWidth(const char* _Text, int _FontId, float _FontScale);
```