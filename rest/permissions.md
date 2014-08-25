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
