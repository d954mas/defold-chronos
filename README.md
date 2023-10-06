`# Chronos for Defold

High resolution monotonic timers for Lua.
https://github.com/ldrumm/chronos

## Installation
__1)__ Add defold-chronos in your own project as a Defold library dependency. Open your game.project file and in the dependencies field under project add:
https://github.com/d954mas/defold-chronos/archive/refs/tags/1.0.0.zip

## Example
```lua
function update(self, dt)
	if chronos then
		local time = chronos.nanotime()
		local a = 1
		for i=1,10000 do
			a = a + 1
		end
		print("seconds:" .. chronos.nanotime() - time)
	end
end
```

## Api

### chronos.nanotime()

**RETURN**
* (number) - seconds with nanosecond precision

`