# Clients API

## Client

|Key|Value|
|---|---|
|id|Client ID|
|application|Application for the client|
|created|Time the client created|


## Get client


### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/clients/{clientId}|

### Parameters

|Key|Value|Default|
|---|---|---|
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Application:{applicationId}|Action:Growthbeat:GetClient|


### Example

```
curl -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/clients/5FCgfMiXq8r2goLj?credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
{
	"id":"5FCgfMiXq8r2goLj",
	"created":"2014-06-26T06:46:16+0000",
	"application":{
		"name":"My365",
		"id":"dy6VlRMnN3juhW9L",
		"created":"2014-06-26T06:46:02+0000"
	}
}
```

## List client

### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/clients|

### Parameters

|Key|Value|Default|
|---|---|---|
|applicationId|Application ID||
|clientId|Client ID||
|order||ascending|
|limit||100|
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Application:{applicationId}|Action:Growthbeat:ListClient|


### Example

```
curl -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/clients?applicationId=dy6VlRMnN3juhW9L&clientId=5FCgfMiXq2goLj&order=ascending&limit=100&credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
[
	{"id":"5FCgfMiXq8r2goLj","created":"2014-06-26T06:46:16+0000","application":{"name":"My365","id":"dy6VlRMnN3juhW9L","created":"2014-06-26T06:46:02+0000"}},
	{"id":"a0sSoL0ZWfucxHma","created":"2014-06-26T06:46:17+0000","application":{"name":"My365","id":"dy6VlRMnN3juhW9L","created":"2014-06-26T06:46:02+0000"}}
	
]
```

## Create client

### Request

|Key|Value|
|---|---|
|Method|POST|
|URL|https://api.growthbeat.com/1/clients|

### Parameters

|Key|Value|Default|
|---|---|---|
|applicationId|Application ID||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Application:{applicationId}|Action:Growthbeat:CreateClient|


### Example

```
curl -X POST -H 'Accept: application/json' -H 'Content-Type: application/x-www-form-urlencoded' 'https://api.growthbeat.com/1/clients' -d 'applicationId=LBYtXQ26k6pHRZZB' -d 'credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
{
	"id":"sp0vUsS9vxAehlHc",
	"created":"2014-08-26T07:34:38+0000",
	"application":{
		"name":"Account for production",
		"id":"LBYtXQ26k6pHRZZB",
		"created":"2014-06-26T06:44:55+0000"
	}
}
```
