---
title: Flyhack
layout: default
---
# How it works - Flyhack
**Flyhack** is a hack that allows you to fly in the server.

**Flyhack** works by using the `G.CONFIG` variable in Craftnite. `G.CONFIG` includes all the config, like the player movement, etc. The specific variable, `G.CONFIG.a143` includes the thing that lets **Flyhack** work. It includes movement "speed" information. If this variable is changed to something over 1, it will let you fly. The code changes this value to `75` *only* when the keyboard is used. Sort of like this:
```javascript
document.addEventListener("keydown", (e) => {
    G.CONFIG.a143 = 75;
});
```
There would be extra code to get it to work only when **Flyhack** is enabled.