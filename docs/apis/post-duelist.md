## Add a new Duelist supehero

![alt text](<../media/Duelist 3.png>)

Creates a new Duelist superhero entry in the Marvel Rivals Ranking database.

## Method: 
`POST`

## URL
`{base_url}/duelists`

## Base URL parameters
**Optional**: You should include all properties: `superhero_name`, `damage_type`, `difficulty`, and `id`.

## Headers
`Content-Type: application/json`

## Request body
A JSON object containing the properties of the superhero to be added.

### cURL example
How to create a new superhero named Scarlet Witch".

```
curl -X POST \
-H "Content-Type: application/json" \
-d '],
  "duelists": [
    {
      "superhero_name": "Scarlet Witch",
      "damage_type": "Projectile, Area of Effect",
      "difficulty": "3",
      "id": 1' \
http://localhost:3000/duelists
```

## Response
Returns the information from the request body.

```
],
  "duelists": [
    {
      "superhero_name": "Scarlet Witch",
      "damage_type": "Projectile, Area of Effect",
      "difficulty": "3",
      "id": 1
```

## Return status

| Status value | Return status | Description |
| --- | --- | --- |
| 201 | Created | A new resource was created successfully |
