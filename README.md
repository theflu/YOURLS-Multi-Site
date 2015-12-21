# YOURLS Multi-Site Instance

Run multiple YOURLS sites from the same YOURLS instance.

Instructions:

1. Create a DB for each domain you want to run YOURLS on with this naming convention `yourls_example.com`
2. Create MySQL user named `yourls`
3. Give that user full access to all DBs with the `yourls` prefix
4. Add `config.php` to the `user` directory in YOURLS
5. Add your domains to the `$allowed_hosts` array on line 13 Ex. `$allowed_hosts = array('example.com', 'test.com');`
6. Add MySQL username on line 27
7. Add MySQL password on line 30
8. Add MySQL host on line 37
9. Add your secret hash to line 70 ( you can get a has at http://yourls.org/cookie )
10. Edit the login info on line 76
11. Visit each site and install YOURLS
12. Enjoy