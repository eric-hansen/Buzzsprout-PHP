# Buzzsprout-PHP
Buzzsprout API consumer written for PHP.

## Why?
There is none, and it seemed like a fun little project to work on.

## Installation
`composer require eric-hansen/buzzsprout-php`

## Dependencies
Right now there are none.  The API is not that difficult to work with, is minimal enough to not require a lot of behind-the scenes logic, and minimalism is a fun approach to programming. :)

## Requirements
Get your Buzzsprout API token from the Buzzsprout Admin panel.  Set that as an env var named `BUZZSPROUT_PHP_TOKEN` and run this script.  If the env var isn't detected or is empty, the service will error out.

## Error Handling
Each response will be returned in a `Response` object (from `Response/Response.php`) containing the response code and body as either a class or nothing.  The clas will have the appropriate data.  Beyond that it is up to the consuming client to handle the response from there.

## Available Endpoints
Look at the `Response/Types` directory for an idea of what endpoints are officially supported.  Unfortunately there does not seem to be any sort of sandbox environment so none of the CUD of the CRUD are tested via PHPUnit.  This may change in the future as we can create episodes, for example, that are private.  But that is not optimal.  Mocking may be considered as well.
