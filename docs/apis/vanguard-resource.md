---
layout: page
---

# `vanguard` resource

![alt text](<../media/Vanguard 3.png>)

Base endpoint:

```shell

{server_url}/vanguard
```

Contains information about the build of the Vanguard superhero character in the Marvel Rivals video game. A Vanguard 
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

| Property name    | Type     | Description                                                       |
|------------------|----------|-------------------------------------------------------------------|
| `superhero_name` | string   | The name of the superhero character (e.g., "Emma Frost")          |
| `tank_type`      | string   | The type of tanking the superhero does (e.g., "Shield")           |
| `damage_type`    | string   | The type of damage the superhero does (e.g., "Melee, Projectile") |
| `difficulty`     | integer  | The ranking level of difficulty (e.g., "2")                       |
| `id`             | integer  | The ID (e.g., "1")                                                |


This resource can be used to rank the spec of the best character to play in Marvel Rivals, including adding, updating, and 
retrieving detailed 
information about each superhero in the game.


