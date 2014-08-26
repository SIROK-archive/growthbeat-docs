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
curl -i -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/users?accountId=L6rmAwrpJvMjowGu&credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
HTTP/1.1 200 OK
Server: Apache-Coyote/1.1
Content-Length: 0
Date: Tue, 26 Aug 2014 15:43:07 GMT
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
curl -X POST -H 'Accept: application/json' 'https://api.growthbeat.com/1/users' -d 'mail=hogehoge@co.jp' -d 'password=hogehoge' -d 'name=foo' -d 'company=bar' -d 'phone=0120-123-456' -d 'credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
{
	"created":"2014-08-26T15:52:17+0000",
	"subscription":true,
	"mail":"hogehoge@co.jp",
	"company":"bar",
	"phone":"0120-123-456",
	"thumbnail":"http://www.gravatar.com/avatar/3c69f10a57b6634a8d6edcb36d7ba521.jpg?d=identicon",
	"account":{
		"name":"foo",
		"id":"4J84zhZGEkOQjCKf",
		"created":"2014-08-26T15:52:17+0000"
	}
}
```

