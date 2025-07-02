# Get a Duelist superhero by name

![alt text](<../media/Duelist 2.png>)

Lists all the Duelist Marvel Rivals supehero characters by name.

## Method

`GET`

## Endpoints
•	**List all Duelist characters**: `{base_url}/duelists` <br>
•	**Get a Duelist supehero character by name**: `{base_url}/duelists/{superhero_name}`  

## Base URL parameters
•	**Optional**: The superhero name of a specific Duelist character.

## Headers

`Content-Type: application/json`

## Request body

None required

### cURL example
Returns the Duelist `superhero_name` with the title `Cloak and Dagger`.

```
curl -X GET http://localhost:3000/duelists/Cloak and Dagger
```

## Return body
Returns all Marvel Rivals Duelists by supehero name requested. The following example shows the result of requesting the 
Duelist character with the superhero name `Cloak and Dagger`:

```json
],
"duelists": [
{
"superhero_name": "Scarlet Witch",
"damage_type": "Projectile, Area of Effect",
"difficulty": "3",
"id": 1
},
```

## Return status

| Status value | Return status | Description |
| ------------ | ------------- | ------------------------------------------------------------ |
| 200          | OK       | Request successful. The server has responded as required |
| 400          | Bad Request   | The server couldn't understand the request |
| 404 | Not Found | Requested resource could not be found |

This resource can be used to rank the spec of the best superhero character to play in Marvel Rivals, including adding, updating, and
retrieving detailed
information about each superhero in the game.
