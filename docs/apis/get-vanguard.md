# Get  Vanguard characters by name

![alt text](<../media/Vanguard.png>)

Lists all the Vanguard Marvel Rivals characters by name.

## Method

`GET`

## Endpoints
•	**List all Vanguards**: `{base_url}/vanguards` <br>
•	**Get a Vanguard by name**: `{base_url}/vanguards/{superhero_name}` 

## Base URL parameters
•	**Optional**: The title of a specific Vanguard to list.

## Headers

`Content-Type: application/json`

## Request body

None required

### cURL example
Returns the Duelist with the name "Emma Frost".

```
curl -X GET http://localhost:3000/vanguards/Emma Frost
```

## Return body
Returns all Vanguards or the specific Vanguard superhero requested. The following example shows the result of 
requesting the Vanguard with the name "Emma Frost":

```json
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

## Post return status

| Status value | Return status | Description |
| ------------ | ------------- | ------------------------------------------------------------ |
| 200          | OK       | Request successful. The server has responded as required |
| 400          | Bad Request   | The server couldn't understand the request |
| 404 | Not Found | Requested resource could not be found |

