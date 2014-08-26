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

```

```

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

```

```

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

```

```

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
