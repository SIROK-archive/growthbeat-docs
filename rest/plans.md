# Plans API

##  Plan

|Key|Value|
|---|---|
|id|Plan ID|
|name|Name for the plan|
|capacity||
|price||
|grade||
|opened||
|created|Time the consumption permission|

## Get plan

### Request

|Key|Value|
|---|---|
|Method|GET|
|URL|https://api.growthbeat.com/1/plans|

### Parameters

|Key|Value|Default|
|---|---|---|
|accountId|Account ID||
|credentialId|Credential ID for authentication||

### Required permission

|Resource|Action|
|---|---|
|||

### Example

```
curl -X GET -H 'Accept: application/json' 'https://api.growthbeat.com/1/plans?accountId=L6rmAwrpJvMjowGu&credentialId=nMdZa0PfT1rmxHEh4MTnpfG6ncxtiTgY'
```

```
{
	"name":"Enterprise 1T",
	"id":"swEwwZYLiqlXY1Z4",
	"created":"2014-07-15T05:43:35+0000",
	"price":0,
	"grade":"large",
	"opened":false,
	"capacity":10000000000000
}
```
