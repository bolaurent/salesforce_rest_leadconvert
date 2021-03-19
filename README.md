Provides a REST endpoint that exposes the Lead Conversion feature of Apex.

## URI ##
<baseurl>/services/apexrest/leadconvert/<leadid>
  
## Format ##
JSON

## HTTP Method ##
POST


## request body ##
If request body is omitted, convertedStatus is set to 'Opportunity' and all other fields to null

Maximal request body content is json as follows. All name/value pairs (except convertedStatus) are optional. The meanings of all these parameters are documented in Apex Developer Guide, see class Database.LeadConvert

```
{
"accountId":null,
"accountRecord":null,
"bypassAccountDedupeCheck":null,
"bypassContactDedupeCheck":null,
"contactId":null,
"contactRecord":null,
"convertedStatus":null,
"doNotCreateOpportunity":false,
"leadId":null,
"opportunityId":null,
"opportunityName":null,
"opportunityRecord":null,
"overwriteLeadSource":false,
"ownerId":null,
"relatedPersonAccountId":null,
"relatedPersonAccountRecord":null,
"sendNotificationEmail":false
}
```

## Response Body ##

The Response body contains a Database.LeadConvertResult, also documented in Apex Developer Guide.

  
