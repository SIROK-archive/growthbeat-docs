# Connections API

## Connection

|Key|Value|
|---|---|
|id|Connection ID|
|account|Account for the connection|
|service|Service for the connection|
|childAccount|Child account for the connection|
|created|Time the connection created|

## List connection


### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/connections|

### Parameters

|Key|Value|Default|
|---|---|---|
|childAccountId|Child account ID||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{childAccountId}|Action:Growthbeat:ListConnection|


### Example

```
curl -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/connections?childAccountId=xoCKaD10WHqoRLNw&credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
{
	"id":"SRyYEWOnJJ5os3AY",
	"created":"2014-06-26T06:44:55+0000",
	"application":null,
	"service":{
		"icon":"http://dev-growthbeat.s3-ap-northeast-1.amazonaws.com/services/wTvYPtGWuyKKMvyy/icon.png",
		"banner":"http://dev-growthbeat.s3-ap-northeast-1.amazonaws.com/services/wTvYPtGWuyKKMvyy/banner.png",
		"logo":"http://dev-growthbeat.s3-ap-northeast-1.amazonaws.com/services/wTvYPtGWuyKKMvyy/logo.png",
		"name":"Growthbeat",
		"id":"wTvYPtGWuyKKMvyy",
		"namespace":"Growthbeat",
		"url":"http://growthbeat.local:8085/",
		"domain":"growthbeat.local",
		"created":"2014-06-01T02:32:50+0000",
		"account":null
	},
	"account":{
		"name":"SIROK",
		"id":"6qt4K7DNIzKFEtRF",
		"created":"2014-06-26T06:44:55+0000"
	},
	"childAccount":{
		"name":"Subaccount for Growthbeat",
		"id":"xoCKaD10WHqoRLNw",
		"created":"2014-06-26T06:44:55+0000"
	}
}
```
