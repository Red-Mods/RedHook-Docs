# RH_DrawText

Draw a text with a specific text, color, font id, font scale.

> [!WARNING]
> **`_X`** **& `_Y`** are in 0.0 to 1.0 based coordinates.
> That mean 0.0, 0.0 represent the top left corner of your screen, and 1.0, 1.0 the bottom right.

> [!CAUTION]
> **\_Text** is what we call an "unsafe" variable bcs <mark style="color:yellow;">**DrawText**</mark> get called from a different thread, that mean if you pass a <mark style="color:blue">**std::string**</mark> using <mark style="color:yellow;">**.c\_str()**</mark> the temporary value will not be retained. I suggest doing a wrapper using <mark style="color:yellow">**strdup**</mark> so you get a safe copy of your ptr (See example below)

```cpp
void RH_DrawText(const char* _Text, float _X, float _Y, int _FontId, float _FontScale, int _R, int _G, int _B, int _A, TextAlignment _TextAlignment);
```

```cpp
// Safe wrapper so we don't lose the temporary conversion using .c_str()
void DrawText(const std::string& _Text, float _X, float _Y, int _FontId, float _FontScale, int _R, int _G, int _B, int _A, TextAlignment _TextAlignment)
{
	const char* safeCStr = _strdup(_Text.c_str());

	return RH_DrawText(safeCStr, _X, _Y, _FontId, _FontScale, _R, _G, _B, _A, _TextAlignment);
}
```