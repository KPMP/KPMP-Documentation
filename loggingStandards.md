## Logging Standards for KPMP apps

In order to make log mining easier, we want to ensure that all of our applications capture the following pieces of information:
- userId (this can be the email address, or Shibboleth eppn)
- uri (at the Controller level, this is the endpoint the user requested, for anything deeper in the service layer, this would be the className.methodName)
- logging message

The format of the log message must look like this:

    USERID: <userid> | URI: <uri> | MSG: <message>

For the Data Lake Uploader, packageId is also included and tagged with "PKGID".

The data elements do not need to be in a particular order, but they must be tagged in the same way in order to allow us to easily parse the logs.
