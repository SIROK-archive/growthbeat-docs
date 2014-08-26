# Credentials API

## Credential

|Key|Value|
|---|---|
|id|Credential ID|
|account|Account for the credential|
|created|Time the consumption created|

## Get credential

### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/credentials/{credentialId}|

### Parameters

|Key|Value|Default|
|---|---|---|
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{accountId}|Action:Growthbeat:GetCredential|


### Example

```
curl -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/credentials/nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY?credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
{
	"id":"nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY",
	"created":"2014-05-27T06:17:05+0000",
	"account":{
		"name":"Root Account",
		"id":"L6rmAwrpJvMjowGu",
		"created":"2014-05-27T06:15:19+0000"
	}
}
```

## List credential

### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/credentials|

### Parameters

|Key|Value|Default|
|---|---|---|
|accountId|Account ID||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{accountId}|Action:Growthbeat:ListCredential|

### Example

```
curl -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/credentials?accountId='L6rmAwrpJvMjowGu'&credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
[
	{
		"id":"nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY",
		"created":"2014-05-27T06:17:05+0000",
		"account":{
			"name":"Root Account",
			"id":"L6rmAwrpJvMjowGu",
			"created":"2014-05-27T06:15:19+0000"
		}
	}
]
```

## Create credential

### Request

|Key|Value|
|---|---|
|Method|POST|
|URL|https://api.growthbeat.com/1/credentials|

### Parameters

|Key|Value|Default|
|---|---|---|
|accountId|Account ID||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{accountId}|Action:Growthbeat:CreateCredential|

### Example

```
curl -X POST -H 'Accept: application/json' -H 'Content-Type: application/x-www-form-urlencoded' 'https://api.growthbeat.com/1/credentials' -d 'accountId=L6rmAwrpJvMjowGu' -d 'credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'```

```
{
	"id":"qrsshfX9sItzaSQJ7T0js9sUYQkkKexJ",
	"created":"2014-08-26T12:32:13+0000",
	"account":{
		"name":"Root Account",
		"id":"L6rmAwrpJvMjowGu",
		"created":"2014-05-27T06:15:19+0000"
	}
}
```

## Get credential

### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/credentials|

### Parameters

|Key|Value|Default|
|---|---|---|
|sessionId|Session ID||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Service:{serviceId}|Action:Growthbeat:GetCredential|

### Example

```
curl -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/credentials?sessionId=30630PW1HIIy8pcdkPzuJzAxDzbxG4rv&credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
[
	{
		"id":"3wr8sYcxZweD5ohp6vzfRiQKQilxhlhH",
		"created":"2014-06-26T06:44:55+0000",
		"account":{
			"name":"Subaccount for Growthbeat",
			"id":"xoCKaD10WHqoRLNw",
			"created":"2014-06-26T06:44:55+0000"
		}
	}
]
```
