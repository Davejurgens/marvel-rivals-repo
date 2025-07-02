# Get a Strategist superhero by name

![alt text](<../media/Strategist 2.png>)

Lists all the Strategist Marvel Rivals superhero characters by name.

## Method

`GET`

## Endpoints
•	**List all Strategists**: `{base_url}/strategists` <br>
•	**Get a Strategist superhero by name**: `{base_url}/strategists/{superhero_name}` 

## Base URL parameters
•	**Optional**: The title of a specific Strategist to list.

## Headers

`Content-Type: application/json`

## Request body

None required

### cURL example
Returns the Strategist with the name `Cloak and Dagger`.

```
curl -X GET http://localhost:3000/strategist/Cloak and Dagger
```

## Return body
Returns all Strategists or the specific Strategist superhero requested. The following example shows the result of 
requesting the Strategist with the title `Cloak and Dagger`:

```json
],
"strategists": [
{
"superhero_name": "Cloak and Dagger",
"healing_type": "Hit Scan (with Auto Aim), Area of Effect",
"damage_type": "Hit Scan (with Auto Aim), Projectile",
"difficulty": "3",
"id": 1
},
```

## Post return status

| Status value | Return status | Description |
| ------------ | ------------- | ------------------------------------------------------------ |
| 200          | OK       | Request successful. The server has responded as required |
| 400          | Bad Request   | The server couldn't understand the request |
| 404 | Not Found | Requested resource could not be found |

