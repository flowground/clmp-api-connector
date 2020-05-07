# ![LOGO](logo.png) CLMP API **flow**ground Connector

## Description

A generated **flow**ground connector for the CLMP API API (version 1.0.0).

Generated from: https://localhost/pub_api<br/>
Generated at: 2020-05-07T16:09:14+00:00

## API Description

API for getting report data out of Customer Lifetime Magagement Platform (CLMP). You need a API key for these endpoints. You can create a personal token in your CLMP profile.<br/>

## Authorization

Supported authorization schemes:
- Bearer Token

## Actions

### Returns information about the current user.
> Takes the api token from the header and returns a json object which includes user data<br/>

### Returns a list of fields for the report

#### Input Parameters
* `id` - _required_ - Report ID<br/>

### Returns the result of a report
> Returns all rows of the report as json objects<br/>

#### Input Parameters
* `id` - _required_ - Report ID<br/>
* `segment` - _optional_ - Segmentation - one of Day, Week, Month, Year, null. Specifies how the data should be aggregated<br/>
* `start` - _optional_ - The start date from where data should be received. Default: Today minus 1 week. Format: YYYY-MM-DD<br/>
* `end` - _optional_ - The end date to where data should be received. Default: Today. Format: YYYY-MM-DD<br/>
* `fields` - _optional_ - Comma separated list of fields to be shown. Default would be only Date. Get the list of fields by requesting /reports/{id}/fields. The field names must be the same as defined in the report column name.<br/>

## License

**flow**ground :- Telekom iPaaS / clmp-api-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
