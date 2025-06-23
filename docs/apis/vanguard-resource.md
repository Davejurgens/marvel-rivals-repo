---
layout: page
---

# `vanguard` resource

![alt text](../docs/media/Vanguard.png)

Base endpoint:

```shell

{server_url}/vanguard
```

Contains information about the build of Vanguard superhero characters in the Marvel Rivals video game. A Vanguard 
is a tank based superhero, focused on absorbing damage and protecting their teammates. A Vanguard resource 
provides details about the name of a Vanguard superhero, tank type, damange type, difficulty level, and ID.

## Resource properties

Sample `vanguard` resource

```js

],
  "vanguards": [
    {
      "superhero_name": "Emma Frost",
      "tank_type": "Shield",
      "damage_type": "Melee, Projectile",
      "difficulty": "2",
      "id": 1
    },
```

| Property name    | Type     | Description                                                                                 |
|------------------|----------|---------------------------------------------------------------------------------------------|
| `superhero_name` | string   | The name of the duelist superhero character (e.g., "Cloak and Dagger")                      |
| `healing_type`   | string   | The characteristics and type of healing the superhero does (e.g., "Auto Aim, Area of Effect") |
| `damage_type`    | string   | The type of damage the superhero does (e.g., "Auto Aim, Projectile")                        |
| `difficulty`     | integer  | The ranking level of difficulty (e.g., "3")                                                 |
| `id`             | integer  | The ID (e.g., "1")                                                                          |


This resource can be used to rank the spec of the best character to play in Marvel Rivals, including adding, updating, and 
retrieving detailed 
information about each superhero in the game.


