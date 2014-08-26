# Permissions API

##  Permission

|Key|Value|
|---|---|
|account|Account for the permission|
|targetAccount||
|resource||
|action||
|created|Time the consumption permission|

## List permission

### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/permissions|

### Parameters

|Key|Value|Default|
|---|---|---|
|accountId|Account ID||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{accountId}|Action:Growthbeat:ListPermission|

### Example

```
curl -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/permissions?accountId=L6rmAwrpJvMjowGu&credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
[
	{
		"created":"2014-05-27T13:36:25+0000",
		"account":{
			"name":"Root Account",
			"id":"L6rmAwrpJvMjowGu",
			"created":"2014-05-27T06:15:19+0000"
		},
		"targetAccount":{
			"name":"Growthbeat Master Account",
			"id":"qRkucFch8owN2PWs",
			"created":"2014-06-01T02:23:46+0000"
		},
		"resource":{
			"name":"Resource",
			"id":"Resource",
			"created":"2014-06-01T01:22:29+0000"
		},
		
	　（中略）
	　
	}
]
```


## List permission

### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/permissions|

### Parameters

|Key|Value|Default|
|---|---|---|
|targetAccountId|Target account ID||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{targetAccountId}|Action:Growthbeat:ListPermission|

### Example

```
curl -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/permissions?targetAccountId=L6rmAwrpJvMjowGu&credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
[
	{
		"created":"2014-05-27T13:36:25+0000",
		"account":null,
		"targetAccount":{
			"name":"Root Account",
			"id":"L6rmAwrpJvMjowGu",
			"created":"2014-05-27T06:15:19+0000"
		},
		"resource":{
			"name":"Resource",
			"id":"Resource",
			"created":"2014-06-01T01:22:29+0000"
		},
		
	　（中略）

	}
]
```

## List permission

### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/permissions|

### Parameters

|Key|Value|Default|
|---|---|---|
|accountId|Account ID|
|targetAccountId|Target account ID||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{accountId}|Action:Growthbeat:ListPermission|

### Example

```
curl -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/permissions?accountId=DFhnn09qoQQiG1YX&targetAccountId=qRkucFch8owN2PWs&credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
[
	{
		"created":"2014-05-27T13:36:25+0000",
		"account":{
			"name":"Default Permission Account",
			"id":"DFhnn09qoQQiG1YX",
			"created":"2014-06-01T02:23:46+0000"
		},
		"targetAccount":{
			"name":"Growthbeat Master Account",
			"id":"qRkucFch8owN2PWs",
			"created":"2014-06-01T02:23:46+0000"
		},
		"resource":{
			"name":"Resource",
			"id":"Resource",
			"created":"2014-06-01T01:22:29+0000"
		},
		"action":{
			"name":"Action",
			"id":"Action",
			"created":"2014-06-01T01:15:44+0000"
		}
	}
]
```

## Create permission

### Request

|Key|Value|
|---|---|
|Method|POST|
|URL|https://api.growthbeat.com/1/permissions|

### Parameters

|Key|Value|Default|
|---|---|---|
|accountId|Account ID||
|targetAccountId|Target account ID||
|resourceId|||
|actionId|||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{accountId}|Action:Growthbeat:CreatePermission|

### Example

```
curl -X POST -H 'Accept: application/json' -H 'Content-Type: application/x-www-form-urlencoded' 'https://api.growthbeat.com/1/permissions' -d 'accountId=L6rmAwrpJvMjowGu' -d 'targetAccountId=qRkucFch8owN2PWs' -d 'resourceId=Resource:Growthbeat:Account:L6rmAwrpJvMjowGu' -d 'actionId=Action:Growthbeat:GetAccount' -d 'credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
{
	"created":"2014-08-26T14:12:25+0000",
	"account":{
		"name":"Root Account",
		"id":"L6rmAwrpJvMjowGu",
		"created":"2014-05-27T06:15:19+0000"
	},
	"targetAccount":{
		"name":"Growthbeat Master Account",
		"id":"qRkucFch8owN2PWs",
		"created":"2014-06-01T02:23:46+0000"
	},
	"resource":{
		"name":"L6rmAwrpJvMjowGu",
		"id":"Resource:Growthbeat:Account:L6rmAwrpJvMjowGu",
		"created":"2014-05-29T04:39:40+0000"
	},
	"action":{
		"name":"GetAccount",
		"id":"Action:Growthbeat:GetAccount",
		"created":"2014-05-29T04:39:40+0000"
	}
}
```

## Delete permission

### Request

|Key|Value|
|---|---|
|Method|DELETE|
|URL|https://api.growthbeat.com/1/permissions|

### Parameters

|Key|Value|Default|
|---|---|---|
|accountId|Account ID||
|targetAccountId|Target account ID||
|resourceId|||
|actionId|||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{accountId}|Action:Growthbeat:DeletePermission|

### Example

```

```

```

```

## Authenticate

### Request

|Key|Value|
|---|---|
|Method|POST|
|URL|https://api.growthbeat.com/1/authorize|

### Parameters

|Key|Value|Default|
|---|---|---|
|resourceId|||
|actionId|||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|||

### Example

```

```

```

```
