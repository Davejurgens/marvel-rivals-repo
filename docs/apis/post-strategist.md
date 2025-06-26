## Add a new Strategist superhero

![alt text](<../media/Strategist 3.png>)

Creates a new Strategist superhero entry in the Marvel Rivals Ranking database.

## Method: 
`POST`

## URL
`{base_url}/strategists`

## Base URL parameters
**Optional**: You should include all properties: superhero_name,healing_type, difficulty, and id.

## Headers
`Content-Type: application/json`

## Request body
A JSON object containing the properties of the superhero to be added.

### cURL example
How to create a new superhero named Cloak and Dagger".

```
curl -X POST \
-H "Content-Type: application/json" \
-d '"strategists": [
    {
      "superhero_name": "Cloak and Dagger",
      "healing_type": "Hit Scan (with Auto Aim), Area of Effect",
      "damage_type": "Hit Scan (with Auto Aim), Projectile",
      "difficulty": "3",
      "id": 1
    },\
http://localhost:3000/strategists
```

## Response
Returns the information from the request body.

```
"strategists": [
    {
      "superhero_name": "Cloak and Dagger",
      "healing_type": "Hit Scan (with Auto Aim), Area of Effect",
      "damage_type": "Hit Scan (with Auto Aim), Projectile",
      "difficulty": "3",
      "id": 1
    },
```

## Return status

| Status value | Return status | Description |
| --- | --- | --- |
| 201 | Created | A new resource was created successfully |
