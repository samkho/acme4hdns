# ACME client for Hetzner DNS users
* An ACME v2 client that uses dns challenge, for Hetzner DNS users.
* Forked from [kaienkira/acme-v2-client](https://github.com/kaienkira/acme-v2-client), and modified to use dns challenge instead of http directory challenge.
* Single php file for easy modification.  Some extra convenience scripts provided.
* Note that [Hetzner DNS](https://www.hetzner.com/dns-console) is *free* even for non-Hetzner customers.
* This project is not affiliated with Hetzner.  I just needed something for my own use.

## Main code
* **acme4dns.php**

## Input arguments to acme4hdns.php
* domain name
* Hetzner Auth API Token

## Input Files (hardcoded names)
* account.key
* domain.csr

## Output File (hardcoded name)
* domain.crt

## Other File (hardcoded name)
* domain.key

## Files to install on your server
* **domain.crt**
* **domain.key**

## Convenience scripts
First, chmod +x \*.sh

Scripts are not necessary but may be helpful:
* clean.sh - removes files from previous run
* **optrun.sh** - "optional runner script" that creates input files, runs main php code, and uploads files to server.
You'll need to set some variables in this file.

## See also
* README.md at [kaienkira/acme-v2-client](https://github.com/kaienkira/acme-v2-client)
* [Hetzner DNS Public API](https://dns.hetzner.com/api-docs/)
* [diafygi/gethttpsforfree](https://github.com/diafygi/gethttpsforfree) is a great way to learn how ACME protocol works.
* [samkho/when2renew](https://github.com/samkho/when2renew) (shameless plug)

## Thanks
[kaienkira](https://github.com/kaienkira), tialaramex@reddit
