# Users API

##  User

|Key|Value|
|---|---|
|mail||
|thumbnail||
|name|Name for the user|
|company||
|phone||
|account||
|created|Time the consumption permission|

## Get user

### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/users|

### Parameters

|Key|Value|Default|
|---|---|---|
|accountId|Account ID||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|Resource:Growthbeat:Account:{accountId}|Action:Growthbeat:GetUser|

### Example

```

```

```

```

## Create user

### Request

|Key|Value|
|---|---|
|Method|POST|
|URL|https://api.growthbeat.com/1/users|

### Parameters

|Key|Value|Default|
|---|---|---|
|mail|||
|password|||
|name||(Empty string)|
|company||(Empty string)|
|phone||(Empty string)|
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

