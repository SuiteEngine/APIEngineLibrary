## Version 1.15
### Improvements
- Added support for GraphQL payload builder.
- Masked values are now stored in isolated storage, rather than in the API parameter record.
- Streamlined the OAuth 2.0 authentication process.
- Added support for OAuth 2.0 Authorization Code, Client Credentials, Password Credentials, and Refresh Token grant types.
- Introduced a new interface for automation processing.
- Added a new action on the API Setup page to register API Engine–related tables in the Retention Policy list.

### New Events
- OnRequestProcessingOnBuildRequestOnBeforeAttachAuthorizationToWebRequest
- OnAfterExecuteAPIMessageOnProcessAPIAutomation

<br><br>

## Version 1.14
### Fixed
- The “Access Token Expiry Threshold” defined in the Credential record did not automatically generate a new token upon expiry.
- The default Execute API Message did not run the NEXT API Function, even when it was defined.

### Improvements
- Updated the minimum supported BC application version to 24.
- Masked values are now stored in isolated storage, rather than in the API parameter record.
- Enhanced tooltips for actions and fields to provide more descriptive information.

<br><br>

## Version 1.13
### Fixed
- API calls failed when a masked value was used in the request header.
- The API call progress dialog box displayed a blank function name.
- Sensitive information in isolated storage remained linked to an old record after renaming the API Set code.
- The ISO8601Date2DT value processing function threw an error when handling a datetime in the format YYYY-MM-DDThh:mm:ss.
- The API Mapping page could not be opened from the API Function page if no existing mapping was present.
- An incorrect LookupPageID reference was used in the API application table and API Function.
- Automation Tasks failed to run when the Last Run Timestamp field was blank.

### Improvements
- Marked the Last Run Timestamp field in Automation Task as mandatory.
- Added API Engine tables to the data retention policy list.
- Set the Masked property to true on all sensitive fields in the API Credential.
- Added all action buttons to the API Function Card (previously, they were only available on the list page).
- Added the option to specify a prefix for the SOAP payload builder.
- Grouped API Function list actions under Request and Response categories for clarity.
- Introduced an action to duplicate existing automations.
- Moved masked value mappings to isolated storage (previously stored in API parameter records).
- Added a new value processing function, ZeroToBlank, which converts a 0 (zero) to an empty string.
