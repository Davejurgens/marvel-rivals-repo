# Get all Marvel Rivals video game characters ranking by title

![alt text](/docs/media/Cover.png)

Lists information about duelists, strategists, or vanguard in Marvel Rivals by character name.

## Method

`GET`

## Endpoints
•	**List all duelist characters**: `{base_url}/duelists` <br>
•	**Get a strategist character by name**: `{base_url}/strategist/{superhero_name}` 
•	**Get a duelist character by name**: `{base_url}/duelist/{superhero_name}` 

## Base URL parameters
•	**Optional**: The superhero name of a specific duelist character.

## Headers

`Content-Type: application/json`

## Request body

None required

### cURL example
Returns the strategist `superhero_name` with the title "Cloak and Dagger".

```
curl -X GET http://localhost:3000/strategists/Cloak and Dagger
```

## Return body
Returns all Marvel Rivals duelists, strategists, or vanguard by character name requested. The following example shows the result of requesting the duelist charcter with the title "Cloak and Dagger":

```json
{
  "superhero_name": "Cloak and Dagger",
  "healing_type": "Hit Scan (with Auto Aim), Area of Effect",
  "damage_type": "Hit Scan (with Auto Aim), Projectile",
  "difficulty": "3",
  "id": 1
}
```

## Return status

| Status value | Return status | Description |
| ------------ | ------------- | ------------------------------------------------------------ |
| 200          | OK       | Request successful. The server has responded as required |
| 400          | Bad Request   | The server couldn't understand the request |
| 404 | Not Found | Requested resource could not be found |

This documentation provides details on how to fetch all Marvel Rivals duelists, strategists, or vanguard by character name, using a cURL example.
