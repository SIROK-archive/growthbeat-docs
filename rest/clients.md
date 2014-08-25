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

```

```

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

```

```

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

```

```

```
