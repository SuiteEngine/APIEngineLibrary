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
