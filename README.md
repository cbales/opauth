Opauth-microsoft-v2-auth
=================================
Opauth is a multi-provider authentication framework for PHP, inspired by [OmniAuth for Ruby](https://github.com/intridea/omniauth).

The microsoft-v2-auth strategy extends opauth to allow users to authenticate against MSA and AAD logins using oauth2 for use with Microsoft Graph and other applications.


Getting Started
---------------
1. Install opauth-microsoft-v2-auth:

```cd path_to_opauth/Strategy
git clone git://github.com/cbales/opauth-microsoft-v2-auth.git Microsoft-V2-Auth```

2. Register an app on the [Microsoft Application Registration Portal](https://apps.dev.microsoft.com)
3. Configure the strategy with the app-id, app-secret, and optional scope (see the [Permission Scopes](https://graph.microsoft.io/en-us/docs/authorization/permission_scopes) document for all available scopes)
4. Direct the user to ```http://yourhost.com/microsoft_v2_auth``` to authenticate

Strategy Configuration
---------------------
Required parameters:
```
<?php
'Microsoft-V2-Auth' => array(
    'api_key' => 'YOUR API KEY',
    'secret_key' => 'YOUR API SECRET'
)
```

Optional parameter:
``` 'scope' => 'YOUR CUSTOM SCOPE HERE' ```

License
--------------
Copyright (c) Microsoft Corporation. All Rights Reserved. Licensed under the MIT license.
