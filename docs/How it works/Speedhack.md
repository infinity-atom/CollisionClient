---
title: Speedhack
layout: default
parent: How it works
---
# How it works - Speedhack
**Speedhack** is a hack that allows you to run fast.

**Speedhack** works by changing `G.CONFIG.a143` to `75`, like in [Flyhack]. Unlike [Flyhack], it only changes to `75` if the user is pressing W,S,A,D and not Space. The code looks like this:
```javascript
document.addEventListener("keydown", (e) => {
    const keys = ["KeyW","KeyS","KeyA","KeyD"];
    if(keys.includes(e.keyCode)) {
        G.CONFIG.a143 = 75;
    }
});
```
There would be extra code to get it to work only when **Speedhack** is enabled.

[Flyhack]: Flyhack.md