<!-- DO NOT EDIT THIS FILE! -->
<!-- Instead edit contrib/raygun.php -->
<!-- Then run bin/docgen -->

# raygun

[Source](/contrib/raygun.php)


## Installing

Add to your _deploy.php_

```php
require 'contrib/raygun.php';
```

## Configuration

- `raygun_api_key` – the API key of your Raygun application
- `raygun_version` – the version of your application that this deployment is releasing
- `raygun_owner_name` – the name of the person creating this deployment
- `raygun_email` – the email of the person creating this deployment
- `raygun_comment` – the deployment notes
- `raygun_scm_identifier` – the commit that this deployment was built off
- `raygun_scm_type` - the source control system you use

## Usage

To notify Raygun of a successful deployment, you can use the 'raygun:notify' task after a deployment.

```php
after('deploy', 'raygun:notify');
```


* Tasks
  * [`raygun:notify`](#raygunnotify) — Notifying Raygun of deployment


## Tasks
### raygun:notify
[Source](https://github.com/deployphp/deployer/search?q=%22raygun%3Anotify%22+in%3Afile+language%3Aphp+path%3Acontrib+filename%3Araygun.php)



