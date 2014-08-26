# Consumptions API

## Consumption

|Key|Value|
|---|---|
|count||
|account|Account for the consumption|
|action|action for the consumption|
|created|Time the consumption created|

## Create consumption


### Request

|Key|Value|
|---|---|
|Method|POST|
|URL|https://api.growthbeat.com/1/consumptions|

### Parameters

|Key|Value|Default|
|---|---|---|
|accountId|Account ID||
|actionId|Action ID||
|count|||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Service:{serviceId}|Action:Growthbeat:CreateConsumption|


### Example

```
curl -X POST -H 'Accept: application/json' -H 'Content-Type: application/x-www-form-urlencoded' 'https://api.growthbeat.com/1/consumptions' -d 'accountId=akfbW0ewZ4IAGLtZ' -d 'actionId=Action:Growthbeat:GetAccount' -d 'count=1' -d 'credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
{
	"created":"2014-08-26T10:03:37+0000",
	"count":1,
	"account":{
		"name":"Subaccount for Growthbeat",
		"id":"akfbW0ewZ4IAGLtZ",
		"created":"2014-06-26T06:44:56+0000"
	},
	"action":{
		"name":"GetAccount",
		"id":"Action:Growthbeat:GetAccount",
		"created":"2014-05-29T04:39:40+0000"
	}
}
```
