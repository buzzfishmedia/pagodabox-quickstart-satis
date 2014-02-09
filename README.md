Satis Pagoda Box - Quickstart
=============================

Quickly launch a [Satis](http://getcomposer.org/doc/articles/handling-private-packages-with-satis.md) Repository Generator to Pagoda Box.

Usage
-----

To get working simply create a `config.json` in the root of the project.

###Example:

```
{
  "name": "acme",
  "homepage": "http://example.com",
  "repositories": [
    {
        "type": "package",
        "package": {
            "name": "wordpress/wordpress",
            "type": "wordpress-core",
            "version": "3.8.1",
            "dist": {
              "url": "http://wordpress.org/wordpress-3.8.1.zip",
              "type": "zip"
            }
        }
    }
  ],
  "require-all": true
}
```

Read the more detailed instructions in the 
[documentation](http://getcomposer.org/doc/articles/handling-private-packages-with-satis.md).

*Currently only public repositories are usable, the build and cron job are set to `--skip-errors` to avoid having build/deploy/update issues.


Requirements
------------

PHP 5.3+



License
-------

Satis is licensed under the MIT License - see the LICENSE file for details
