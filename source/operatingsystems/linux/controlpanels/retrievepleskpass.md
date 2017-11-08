# Recovering The Plesk Password

If the Plesk password is ever forgotten, you can always find out the current Plesk password using one of the following methods.

## Plesk 10 and earlier

In these versions, the password is stored in plaintext in the following location:

``#
  /etc/psa/.psa.shadow
``

## Plesk 11 and later

In these versions, the psa.shadow file still exists, but it now contains a hash of the password.

To see the pasword in plaintext, use the following command:

``#
  /usr/local/psa/bin/admin --show-password
``

```eval_rst
  .. meta::
     :title: Retrieving your Plesk password on Linux | UKFast Documentation
     :description: A guide to retrieving your Plesk password on Linux servers
     :keywords: ukfast, plesk, password, get, retrieve, cloud, server, shadow
