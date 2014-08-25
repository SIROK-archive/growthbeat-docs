# Applications API

## Application

|Key|Value|
|---|---|
|id|Application ID|
|name|Name for the account|
|created|Time the account created|

## Get application


### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/applications/{applicationId}|

### Parameters

|Key|Value|Default|
|---|---|---|
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Application:{applicationId}|Action:Growthbeat:GetApplication|


### Example

```

```

```

```

## List application

### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/applications|

### Parameters

|Key|Value|Default|
|---|---|---|
|accountId|account ID||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{accountId}|Action:Growthbeat:ListApplication|


### Example
```

```

```

```



## Create application

### Request

|Key|Value|
|---|---|
|Method|POST|
|URL|https://api.growthbeat.com/1/applications|

### Parameters

|Key|Value|Default|
|---|---|---|
|name|Name for the account||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Application|Action:Growthbeat:CreateApplication|


### Example
```

```

```

```

## Update application

### Request

|Key|Value|
|---|---|
|Method|PUT|
|URL|https://api.growthbeat.com/1/applications/{applicationId}|

### Parameters

|Key|Value|Default|
|---|---|---|
|name|Name for the account||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Application:{applicationId}|Action:Growthbeat:UpdateApplication|


### Example
```

```

```

```
