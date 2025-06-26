## Add a new Vanguard superhero

![alt text](<../media/Vanguard 2.png>)

Creates a new Vanguard superhero entry in the Marvel Rivals Ranking database.

## Method: 
`POST`

## URL
`{base_url}/vanguards`

## Base URL parameters
**Optional**: You should include all properties: superhero_name,tank_type,damage_type, difficulty, and id.

## Headers
`Content-Type: application/json`

## Request body
A JSON object containing the properties of the superhero to be added.

### cURL example
How to create a new superhero named Emma Frost".

```
curl -X POST \
-H "Content-Type: application/json" \
-d '],
  "vanguards": [
    {
      "superhero_name": "Emma Frost",
      "tank_type": "Shield",
      "damage_type": "Melee, Projectile",
      "difficulty": "2",
      "id": 1
    },\
http://localhost:3000/vanguards
```

## Response
Returns the information from the request body.

```
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

## Return status

| Status value | Return status | Description |
| --- | --- | --- |
| 201 | Created | A new resource was created successfully |
