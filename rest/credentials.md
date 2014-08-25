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

```

```

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

```

```

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

```

```

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

```

```

```
