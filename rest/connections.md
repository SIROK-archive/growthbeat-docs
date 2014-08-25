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

```

```

```
