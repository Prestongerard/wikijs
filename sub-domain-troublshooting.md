<!-- TITLE: Sub Domain Troublshooting -->
<!-- SUBTITLE: A quick summary of Sub Domain Troublshooting -->

# Apache - sub domain broke

steps I have taken so far:

Add a new A record (lwst), point it to the same IP address as my site
Duplicate mysite.com.conf, change all instances of mysite.com.conf to the staging URL lwst.mysite.com.conf
Created /var/www/html/lwst.mysite.com/
Copied all files from /var/www/html/mysite.com to /var/www/html/lwst.mysite.conf
Used Certbot to add https certificate for lwst.mysite.com
Enabled my new site [sudo a2ensite lwst.mysite.com.conf]
Restarted Apache[service apache2 reload]

Look into lwst.mysite.com.conf and make sure DocumentRoot is properly configured (/var/www/html/lwst.mysite.com/).

MAke sure you set the permissions right for lwst.mysite.com.conf file and /var/www/html/lwst.mysite.com/ folder.

Try to add the virtual host directly to the apache httpd.conf
Try without the SSL Certificate see if it works(you can get time out errors if you didn t properly installed your SSL Certificate).

ref: https://www.linode.com/community/questions/17221/setting-up-a-staging-sub-domain-what-have-i-done-wrong