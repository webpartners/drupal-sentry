
Sentry
======

Logs Drupal errors and exceptions to [Sentry](https://github.com/getsentry) via the
[Raven-PHP](https://github.com/getsentry/raven-php) library.


Installation
------------

Enable the `sentry` module and add your Sentry DSN to the site's `settings.php`
file.

    $conf['sentry_dsn'] = '{{ DSN }}';

Customization
------------

If you want to subclass Raven_Client you can do it in your own module and set:
    $conf['sentry_class'] = 'MyOwnRavenSubClass';
