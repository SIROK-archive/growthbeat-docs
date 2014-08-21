# Accounts API

## Account

|Key|Value|
|---|---|
|id|Account ID|
|name|Name for the account|
|created|Time the account created|

## Get account

Get account of the accountId.

### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/accounts/{accountId}|

### Parameters

|Key|Value|Default|
|---|---|---|
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{accountId}|Action:Growthbeat:GetAccount|

### Example

```
curl -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/accounts/akfbW0ewZ4IAGLtZ?credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
{
	"name":"Subaccount for Growthbeat",
	"id":"akfbW0ewZ4IAGLtZ",
	"created":"2014-06-26T06:44:56+0000"
}
```

## Create account

Create a new account. The created account gives permission of all actions to the account of credential.

### Request

|Key|Value|
|---|---|
|Method|POST|
|URL|https://api.growthbeat.com/1/accounts|
|Content-Type|application/x-www-form-urlencoded|

### Parameters

The name is used to display on dashboard.

|Key|Value|Default|
|---|---|---|
|name|Name for the account|(Empty string)|
|credentialId|Credential ID for authentication||

### Required permission

The accountId of resource is for the account of credential.

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{accountId}|Action:Growthbeat:CreateAccount|

### Example

```
curl -X POST -H 'Accept: application/json' -H 'Content-Type: application/x-www-form-urlencoded' 'https://api.growthbeat.com/1/accounts' -d 'name=Account for production' -d 'credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
{
	"name":"Account for production",
	"id":"Wcgc1MjCoj4eHhnh",
	"created":"2014-08-21T15:26:31+0000"
}
```
