# WORLD_GET_ALL_ACTORS `0xD892AD02`

Get all actors spawned in the world.

> [!NOTE]
> Max world actors at once cannot exceed **70**.

```cpp
int WORLD_GET_ALL_ACTORS(Actor* _Array);
```

#### Example

```cpp
// A cool wrapper !
static const std::vector<Actor> GetWorldAllActors()
{
	std::vector<Actor> result = {};

	Actor actors[70];
	int actorsCount = REDHOOK::WORLD_GET_ALL_ACTORS(actors);

	for (int i = 0; i < actorsCount; i++)
	{
		Actor actor = actors[i];

		if (!ENTITY::IS_ACTOR_VALID(actor))
			continue;

		result.push_back(actor);
	}

	return result;
}
```