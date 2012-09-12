Opauth-Do
=============
[Opauth][1] strategy for Do authentication.

Opauth is a multi-provider authentication framework for PHP.

Getting started
----------------
1. Install Opauth-Do:
   ```bash
   cd path_to_opauth/Strategy
   git clone git://github.com/arbales/opauth-do.git Do
   ```

2. Request Do API credentials by e-mailing operations@do.com.
   - Enter URL as your application URL (this can be outside of Opauth)
   - Callback URL: enter `http://path_to_opauth/do/oauth2callback`
   
3. Configure Opauth-Do strategy with `client_id` and `client_secret`.

4. Direct user to `http://path_to_opauth/do` to authenticate


Strategy configuration
----------------------

Required parameters:

```php
<?php
'Do' => array(
	'client_id' => 'YOUR CLIENT ID',
	'client_secret' => 'YOUR CLIENT SECRET'
)
```

Optional parameters:
`scope`, `state`

License
---------
Opauth-Do is MIT Licensed  
Copyright © 2012 Austin Bales (http://austinbales.com)
Copyright © 2012 Do.com, Inc. (https://do.com)

Based on opauth-github by U-Zyn Chua (http://uzyn.com)

