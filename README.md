# CiviCRM with WordPress on Pantheon

While [excellent guides](https://civicrm.stackexchange.com/a/4493/12) for using CiviCRM on Pantheon with Drupal 7 exist, there appears to be no documentation on running CiviCRM with WordPress on Pantheon.

Ultimately, the main difference is just in the `civicrm.settings.php` file - all the other existing documentation is sufficient.  This repo contains a `civicrm.settings.php` file suitable for use with WordPress on Pantheon.

### Usage
Assuming you've migrated CiviCRM from an existing install, download the `civicrm.settings.php` from this repo.  Open it, look for the string `%%YOUR_SITE_KEY_HERE%`, and put in your own site key.  If you don't have a site key, and string of random letters and numbers will suffice.

Once you've changed the site key, enter your Pantheon dev site, switch to "SFTP mode", and upload this file to the `/files/civicrm` folder.

Finally, create a folder `/files/tmp/civicrm` which will be used for compiled templates.
