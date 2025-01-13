### HTHAXZ
HTHAXZ is a malicious .htaccess file that I created which tests for dozens of .htaccess related security issues or misconfigurations 

### How to use:
Generally this would be used in conjunction with an arbitrary file upload or arbitrary file overwrite vulnerability. Simply download the .htaccess file found within this repository and whenever you see an upload form on your target site, try uploading it. Similarly, if you find a vulnerability that allows you to overwrite the contents of a file, then overwrite their current .htaccess file with the one found in this repo.

### Additional notes:
- Some of the attack vectors (primarily "destructive" attacks such as different forms of DoS) have been commented out so that sny pentesters or bug bounty hunters using this file don't crash the webserver. If yoy want to test for these attacks, then simply uncomment them.
- Similarly, the methods of spawning webshells have also been commented out. Depending on your target environment, uncomment the lines to spawn a shell for the relevant server-side scripting language that is in use on your target.
