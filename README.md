# Omnistack10 back-end

## These are some basic information for requesting this api.

### Methods
`GET`|`POST`

### Valids resources
`/devs`|`/search`

## Sample call
### This request: *GET http://localhost:port/api/devs*

Results for this request:
`[
  {
    "techs": [
      "Java",
      "Angular"
    ],
    "_id": "6019e11737e569405f197b58",
    "github_username": "José",
    "name": "José",
    "avatar_url": "https://avatars.githubusercontent.com/u/id?v=4",
    "bio": null,
    "location": {
      "coordinates": [
        latitude_code,
        longitude_code
      ],
      "_id": "6019e11737e569405f197b59",
      "type": "Point"
    },
    "__v": 0
  },
  {
    "techs": [
      "Node",
      "React"
    ],
    "_id": "6019e272c38e4b41ba958bb6",
    "github_username": "diego",
    "name": "Diego",
    "avatar_url": "https://avatars.githubusercontent.com/u/id?v=4",
    "bio": "description",
    "location": {
      "coordinates": [
        latitude_code,
        longitude_code
      ],
      "_id": "6019e272c38e4b41ba958bb7",
      "type": "Point"
    },
    "__v": 0
  }
  ]`

### This request: *POST https://localhost:port/api/devs*
With this JSON body: 
`{
  "github_username": "tiago",
	"techs": "Python",
	"latitude": latitude_code,
	"longitude": longitude_code
}`

Results for this request:
`{
  "techs": [
    "Python"
  ],
  "_id": "602bf52f5d23a77af137a316",
  "github_username": "tiago",
  "name": "Tiago",
  "avatar_url": "https://avatars.githubusercontent.com/u/id?v=4",
  "bio": null,
  "location": {
    "coordinates": [
      latitude_code,
      longitude_code
    ],
    "_id": "602bf52f5d23a77af137a317",
    "type": "Point"
  },
  "__v": 0
}`
