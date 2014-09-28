# Sessions API

## Session

|Key|Value|
|---|---|
|id|Account ID|
|created|Time the session created|
|account|Account|
|service|Service|

## Get session

Get session of the sessionId.

### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/sessions/{sessionId}|

### Parameters

|Key|Value|Default|
|---|---|---|
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{accountId}|Action:Growthbeat:GetSession|

### Example

```
curl -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/sessions/8pE0v2AngPUibjlf5Nw3OHdHkFc7DJGt?credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
{
	"id":"8pE0v2AngPUibjlf5Nw3OHdHkFc7DJGt",
	"created":"2014-09-28T22:05:48+0000",
	"account":{
		"id":"6qt4K7DNIzKFEtRF",
		"created":"2014-06-26T06:44:55+0000",
		"name":"SIROK"
	},
	"service":{
		"icon":null,
		"banner":null,
		"logo":null,
		"namespace":"Growthbeat",
		"domain":"growthbeat.local",
		"id":"wTvYPtGWuyKKMvyy",
		"created":"2014-06-01T02:32:50+0000",
		"name":"Growthbeat",
		"url":"http://growthbeat.local:8085/",
		"account":null
	}
}
```
