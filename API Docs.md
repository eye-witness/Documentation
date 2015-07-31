# Server API

## Pull Appeals for Information for selected blocks

### Sample HTTP Request

IP: 104.236.110.36

```JSON
POST /index.php/api/appeals/
Accept: application/json
Content-Type: application/json
Content-Length: 60

{
	"blocks": [
		{"latitude":105,"longitude":5},
	],
	"time": 1438082766,
	"lastFetched": 1438082200
}
```

### Sample JSON Response

```JSON
[
  {
	"caseID": 1,
	"time" : 4789735435,
	"latitude": "56.4354534543",
	"longitude": "56.458908453",
	"radius": 5,
	"police_force_id": 1,
	"description" : {
		"location": "Near motorway",
		"crimeType": "Stolen socks",
		"text": "",
	},
	"block_id": "105,-4",
	"created" : 543784590,
	"contact": {
		"phoneNumber": "101",
		"policeForce": "Hampshire Constabulary",
	}
  }
]
```
