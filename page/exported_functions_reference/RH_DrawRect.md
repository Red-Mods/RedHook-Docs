# RH_DrawRect

Draw a rectangle with color.

> [!WARNING]
> **`_X`, `_Y`, `_Width`** & **`_Height`** are all in 0.0 to 1.0 based coordinates.
> That mean 0.0, 0.0 represent the top left corner of your screen, and 1.0, 1.0 the bottom right.

```cpp
void RH_DrawRect(float _X, float _Y, float _Width, float _Height, int _R, int _G, int _B, int _A);
```