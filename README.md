### Configuration Steps

1.  Import the collection and environment file into your Postman environment.
2.  Assign the imported environment as the active environment.
3.  Edit the `api_host` environment variable to set the region code to the region where the Organization containing the Information Intelligence plan is hosted. By default the region is 'us'. [Click here](https://developer.opentext.com/cloud-platform/documentation/authentication#region) for more information on regions.
4.  Set the `app_confclient_id` and `app_confclient_secret` variables for the application through which you will be accessing Information Intelligence. See [Getting Started](https://developer.opentext.com/services/products/information-intelligence/tutorials/getting-started-information-intelligence/2) instructions.
5.  Set the `tenant_id` for the tenant through which you will be accessing Information Intelligence. See [Getting Started](https://developer.opentext.com/services/products/information-intelligence/tutorials/getting-started-information-intelligence/2) instructions.
6.  Save your changes to the environment.
7.  Extract the ZIP of test input files into the working directory for Postman, `C:\users\<user>\Postman\files`. If you do not put them here you will need to reconfigure the file input on every request in the collection.

### Executing the Postman collection

1.  Get an access token by executing the **Get Tenant Access Token** request. This will populate the `tmp_tenant_access_token` variable in the environment which is configured as the bearer token for every request in the collection using the **inherit from parent** authorization configuration.
2.  From this point on you can execute individual requests or batches of requests using the folders. Test scripts are configured on every request.
