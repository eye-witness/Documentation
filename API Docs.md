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
	"created" : 543784590,
	"block": {"latitude" : 56.5, "longitude": 56.5},
	"caseID": 1,
	"time" : 4789735435,
	"radius": 5,
	"location" : {"latitude": "56.4354534543", "longitude": "56.458908453"},
	"description" : {
		"location": "Near motorway",
		"crimeType": "Stolen socks",
		"text": "",
	},
	"contact": {
		"phoneNumber": "",
		"policeForce": "",
	}
  },
  {
    "created" : 543784590,
	"block": {"latitude" : 56.5, "longitude": 56.5},
	"caseID": 2,
	"time" : 4789735435,
	"radius": 5,
	"location" : {"latitude": "56.4354534543", "longitude": "56.458908453"},
	"description" : {
		"location": "Near motorway",
		"crimeType": "Stolen socks",
		"text": "",
	},
	"contact": {
		"phoneNumber": "",
		"policeForce": "",
	}
  },
  {
    "created" : 543784590,
	"block": {"latitude" : 56.5, "long": 56.5},
	"crimeID": 2,
	"time" : 4789735435,
	"radius": 5,
	"location" : {"latitude": "56.4354534543", "longitude": "56.458908453"},
	"description" : {
		"location": "Near motorway",
		"crimeType": "Stolen socks",
		"text": "",
	},
	"contact": {
		"phoneNumber": "",
		"policeForce": "",
	}
    }
]
```
