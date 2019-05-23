# ![LOGO](logo.png) Google Sheets **flow**ground Connector

## Description

A generated **flow**ground connector for the Google Sheets API (version v4).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/sheets/v4/swagger.json<br/>
Generated at: 2019-05-23T12:13:40+03:00

## API Description

Reads and writes Google Sheets.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Creates a spreadsheet, returning the newly created spreadsheet.

*Tags:* `spreadsheets`

#### Input Parameters
* `$.xgafv` - _optional_ - V1 error format.
    Possible values: 1, 2.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Returns the spreadsheet at the given ID.<br/>
> The caller must specify the spreadsheet ID.<br/>
> <br/>
> By default, data within grids will not be returned.<br/>
> You can include grid data one of two ways:<br/>
> <br/>
> * Specify a field mask listing your desired fields using the `fields` URL<br/>
> parameter in HTTP<br/>
> <br/>
> * Set the includeGridData<br/>
> URL parameter to true.  If a field mask is set, the `includeGridData`<br/>
> parameter is ignored<br/>
> <br/>
> For large spreadsheets, it is recommended to retrieve only the specific<br/>
> fields of the spreadsheet that you want.<br/>
> <br/>
> To retrieve only subsets of the spreadsheet, use the<br/>
> ranges URL parameter.<br/>
> Multiple ranges can be specified.  Limiting the range will<br/>
> return only the portions of the spreadsheet that intersect the requested<br/>
> ranges. Ranges are specified using A1 notation.

*Tags:* `spreadsheets`

#### Input Parameters
* `includeGridData` - _optional_ - True if grid data should be returned.
This parameter is ignored if a field mask was set in the request.
* `ranges` - _optional_ - The ranges to retrieve from the spreadsheet.
* `spreadsheetId` - _required_ - The spreadsheet to request.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Returns the developer metadata with the specified ID.<br/>
> The caller must specify the spreadsheet ID and the developer metadata's<br/>
> unique metadataId.

*Tags:* `spreadsheets`

#### Input Parameters
* `metadataId` - _required_ - The ID of the developer metadata to retrieve.
* `spreadsheetId` - _required_ - The ID of the spreadsheet to retrieve metadata from.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Returns all developer metadata matching the specified DataFilter.<br/>
> If the provided DataFilter represents a DeveloperMetadataLookup object,<br/>
> this will return all DeveloperMetadata entries selected by it. If the<br/>
> DataFilter represents a location in a spreadsheet, this will return all<br/>
> developer metadata associated with locations intersecting that region.

*Tags:* `spreadsheets`

#### Input Parameters
* `spreadsheetId` - _required_ - The ID of the spreadsheet to retrieve metadata from.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Copies a single sheet from a spreadsheet to another spreadsheet.<br/>
> Returns the properties of the newly created sheet.

*Tags:* `spreadsheets`

#### Input Parameters
* `sheetId` - _required_ - The ID of the sheet to copy.
* `spreadsheetId` - _required_ - The ID of the spreadsheet containing the sheet to copy.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Returns a range of values from a spreadsheet.<br/>
> The caller must specify the spreadsheet ID and a range.

*Tags:* `spreadsheets`

#### Input Parameters
* `dateTimeRenderOption` - _optional_ - How dates, times, and durations should be represented in the output.
This is ignored if value_render_option is
FORMATTED_VALUE.
The default dateTime render option is [DateTimeRenderOption.SERIAL_NUMBER].
    Possible values: SERIAL_NUMBER, FORMATTED_STRING.
* `majorDimension` - _optional_ - The major dimension that results should use.

For example, if the spreadsheet data is: `A1=1,B1=2,A2=3,B2=4`,
then requesting `range=A1:B2,majorDimension=ROWS` will return
`[[1,2],[3,4]]`,
whereas requesting `range=A1:B2,majorDimension=COLUMNS` will return
`[[1,3],[2,4]]`.
    Possible values: DIMENSION_UNSPECIFIED, ROWS, COLUMNS.
* `range` - _required_ - The A1 notation of the values to retrieve.
* `spreadsheetId` - _required_ - The ID of the spreadsheet to retrieve data from.
* `valueRenderOption` - _optional_ - How values should be represented in the output.
The default render option is ValueRenderOption.FORMATTED_VALUE.
    Possible values: FORMATTED_VALUE, UNFORMATTED_VALUE, FORMULA.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Sets values in a range of a spreadsheet.<br/>
> The caller must specify the spreadsheet ID, range, and<br/>
> a valueInputOption.

*Tags:* `spreadsheets`

#### Input Parameters
* `includeValuesInResponse` - _optional_ - Determines if the update response should include the values
of the cells that were updated. By default, responses
do not include the updated values.
If the range to write was larger than than the range actually written,
the response will include all values in the requested range (excluding
trailing empty rows and columns).
* `range` - _required_ - The A1 notation of the values to update.
* `responseDateTimeRenderOption` - _optional_ - Determines how dates, times, and durations in the response should be
rendered. This is ignored if response_value_render_option is
FORMATTED_VALUE.
The default dateTime render option is
DateTimeRenderOption.SERIAL_NUMBER.
    Possible values: SERIAL_NUMBER, FORMATTED_STRING.
* `responseValueRenderOption` - _optional_ - Determines how values in the response should be rendered.
The default render option is ValueRenderOption.FORMATTED_VALUE.
    Possible values: FORMATTED_VALUE, UNFORMATTED_VALUE, FORMULA.
* `spreadsheetId` - _required_ - The ID of the spreadsheet to update.
* `valueInputOption` - _optional_ - How the input data should be interpreted.
    Possible values: INPUT_VALUE_OPTION_UNSPECIFIED, RAW, USER_ENTERED.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Appends values to a spreadsheet. The input range is used to search for<br/>
> existing data and find a "table" within that range. Values will be<br/>
> appended to the next row of the table, starting with the first column of<br/>
> the table. See the<br/>
> [guide](/sheets/api/guides/values#appending_values)<br/>
> and<br/>
> [sample code](/sheets/api/samples/writing#append_values)<br/>
> for specific details of how tables are detected and data is appended.<br/>
> <br/>
> The caller must specify the spreadsheet ID, range, and<br/>
> a valueInputOption.  The `valueInputOption` only<br/>
> controls how the input data will be added to the sheet (column-wise or<br/>
> row-wise), it does not influence what cell the data starts being written<br/>
> to.

*Tags:* `spreadsheets`

#### Input Parameters
* `includeValuesInResponse` - _optional_ - Determines if the update response should include the values
of the cells that were appended. By default, responses
do not include the updated values.
* `insertDataOption` - _optional_ - How the input data should be inserted.
    Possible values: OVERWRITE, INSERT_ROWS.
* `range` - _required_ - The A1 notation of a range to search for a logical table of data.
Values will be appended after the last row of the table.
* `responseDateTimeRenderOption` - _optional_ - Determines how dates, times, and durations in the response should be
rendered. This is ignored if response_value_render_option is
FORMATTED_VALUE.
The default dateTime render option is [DateTimeRenderOption.SERIAL_NUMBER].
    Possible values: SERIAL_NUMBER, FORMATTED_STRING.
* `responseValueRenderOption` - _optional_ - Determines how values in the response should be rendered.
The default render option is ValueRenderOption.FORMATTED_VALUE.
    Possible values: FORMATTED_VALUE, UNFORMATTED_VALUE, FORMULA.
* `spreadsheetId` - _required_ - The ID of the spreadsheet to update.
* `valueInputOption` - _optional_ - How the input data should be interpreted.
    Possible values: INPUT_VALUE_OPTION_UNSPECIFIED, RAW, USER_ENTERED.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Clears values from a spreadsheet.<br/>
> The caller must specify the spreadsheet ID and range.<br/>
> Only values are cleared -- all other properties of the cell (such as<br/>
> formatting, data validation, etc..) are kept.

*Tags:* `spreadsheets`

#### Input Parameters
* `range` - _required_ - The A1 notation of the values to clear.
* `spreadsheetId` - _required_ - The ID of the spreadsheet to update.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Clears one or more ranges of values from a spreadsheet.<br/>
> The caller must specify the spreadsheet ID and one or more ranges.<br/>
> Only values are cleared -- all other properties of the cell (such as<br/>
> formatting, data validation, etc..) are kept.

*Tags:* `spreadsheets`

#### Input Parameters
* `spreadsheetId` - _required_ - The ID of the spreadsheet to update.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Clears one or more ranges of values from a spreadsheet.<br/>
> The caller must specify the spreadsheet ID and one or more<br/>
> DataFilters. Ranges matching any of the specified data<br/>
> filters will be cleared.  Only values are cleared -- all other properties<br/>
> of the cell (such as formatting, data validation, etc..) are kept.

*Tags:* `spreadsheets`

#### Input Parameters
* `spreadsheetId` - _required_ - The ID of the spreadsheet to update.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Returns one or more ranges of values from a spreadsheet.<br/>
> The caller must specify the spreadsheet ID and one or more ranges.

*Tags:* `spreadsheets`

#### Input Parameters
* `dateTimeRenderOption` - _optional_ - How dates, times, and durations should be represented in the output.
This is ignored if value_render_option is
FORMATTED_VALUE.
The default dateTime render option is [DateTimeRenderOption.SERIAL_NUMBER].
    Possible values: SERIAL_NUMBER, FORMATTED_STRING.
* `majorDimension` - _optional_ - The major dimension that results should use.

For example, if the spreadsheet data is: `A1=1,B1=2,A2=3,B2=4`,
then requesting `range=A1:B2,majorDimension=ROWS` will return
`[[1,2],[3,4]]`,
whereas requesting `range=A1:B2,majorDimension=COLUMNS` will return
`[[1,3],[2,4]]`.
    Possible values: DIMENSION_UNSPECIFIED, ROWS, COLUMNS.
* `ranges` - _optional_ - The A1 notation of the values to retrieve.
* `spreadsheetId` - _required_ - The ID of the spreadsheet to retrieve data from.
* `valueRenderOption` - _optional_ - How values should be represented in the output.
The default render option is ValueRenderOption.FORMATTED_VALUE.
    Possible values: FORMATTED_VALUE, UNFORMATTED_VALUE, FORMULA.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Returns one or more ranges of values that match the specified data filters.<br/>
> The caller must specify the spreadsheet ID and one or more<br/>
> DataFilters.  Ranges that match any of the data filters in<br/>
> the request will be returned.

*Tags:* `spreadsheets`

#### Input Parameters
* `spreadsheetId` - _required_ - The ID of the spreadsheet to retrieve data from.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Sets values in one or more ranges of a spreadsheet.<br/>
> The caller must specify the spreadsheet ID,<br/>
> a valueInputOption, and one or more<br/>
> ValueRanges.

*Tags:* `spreadsheets`

#### Input Parameters
* `spreadsheetId` - _required_ - The ID of the spreadsheet to update.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Sets values in one or more ranges of a spreadsheet.<br/>
> The caller must specify the spreadsheet ID,<br/>
> a valueInputOption, and one or more<br/>
> DataFilterValueRanges.

*Tags:* `spreadsheets`

#### Input Parameters
* `spreadsheetId` - _required_ - The ID of the spreadsheet to update.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Applies one or more updates to the spreadsheet.<br/>
> <br/>
> Each request is validated before<br/>
> being applied. If any request is not valid then the entire request will<br/>
> fail and nothing will be applied.<br/>
> <br/>
> Some requests have replies to<br/>
> give you some information about how<br/>
> they are applied. The replies will mirror the requests.  For example,<br/>
> if you applied 4 updates and the 3rd one had a reply, then the<br/>
> response will have 2 empty replies, the actual reply, and another empty<br/>
> reply, in that order.<br/>
> <br/>
> Due to the collaborative nature of spreadsheets, it is not guaranteed that<br/>
> the spreadsheet will reflect exactly your changes after this completes,<br/>
> however it is guaranteed that the updates in the request will be<br/>
> applied together atomically. Your changes may be altered with respect to<br/>
> collaborator changes. If there are no collaborators, the spreadsheet<br/>
> should reflect your changes.

*Tags:* `spreadsheets`

#### Input Parameters
* `spreadsheetId` - _required_ - The spreadsheet to apply the updates to.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Returns the spreadsheet at the given ID.<br/>
> The caller must specify the spreadsheet ID.<br/>
> <br/>
> This method differs from GetSpreadsheet in that it allows selecting<br/>
> which subsets of spreadsheet data to return by specifying a<br/>
> dataFilters parameter.<br/>
> Multiple DataFilters can be specified.  Specifying one or<br/>
> more data filters will return the portions of the spreadsheet that<br/>
> intersect ranges matched by any of the filters.<br/>
> <br/>
> By default, data within grids will not be returned.<br/>
> You can include grid data one of two ways:<br/>
> <br/>
> * Specify a field mask listing your desired fields using the `fields` URL<br/>
> parameter in HTTP<br/>
> <br/>
> * Set the includeGridData<br/>
> parameter to true.  If a field mask is set, the `includeGridData`<br/>
> parameter is ignored<br/>
> <br/>
> For large spreadsheets, it is recommended to retrieve only the specific<br/>
> fields of the spreadsheet that you want.

*Tags:* `spreadsheets`

#### Input Parameters
* `spreadsheetId` - _required_ - The spreadsheet to request.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

## License

**flow**ground :- Telekom iPaaS / googleapis-com-sheets-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
