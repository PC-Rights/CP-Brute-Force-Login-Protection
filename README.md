# CP Brute Force Login Protection

This is a fork of [Brute Force Login Protection](https://github.com/jpkleemans/Brute-Force-Login-Protection/releases) tailored for ClassicPress v1.1.0 and above.

Protects your ClassicPress website against brute force login attacks using .htaccess

## Description
A Brute Force Attack aims at being the simplest kind of method to gain access to a site: it tries usernames and passwords, over and over again, until it gets in.
CP Brute Force Login Protection is a lightweight plugin that protects your website against brute force login attacks using .htaccess.

After a specified limit of login attempts within a specified time, the IP address of the hacker will be blocked.

### Features

* Limit the number of allowed login attempts using normal login form
* Limit the number of allowed login attempts using Auth Cookies
* Manually block/unblock IP addresses
* Manually whitelist trusted IP addresses
* Delay execution after a failed login attempt (to slow down brute force attack)
* Option to inform user about remaining attempts on login page
* Option to email administrator when an IP has been blocked
* Custom message to show to blocked users

## Installation
1. Download the plugin zip file from https://github.com/PC-Rights/CP-Brute-Force-Login-Protection/releases/latest
2. Upload the zip file through your admin panel>plugins>add new.
3. Activate the plugin through the ClassicPress admin panel.
4. Customize the settings via the Security page.
5. Done!

## Frequently Asked Questions
### My own IP is blocked, what do I do?
If you have FTP access to your website edit the .htaccess file and remove the line: 'deny from x.x.x.x', where x.x.x.x is your own IP address.
If you don't have FTP access, the only way to unblock your IP is to log in your ClassicPress admin panel from another IP address and unblock it via the plugin settings page.

### I get an error: .htaccess file not readable/writeable
CP Brute Force Login Protection will only work if your .htaccess file is writeable by ClassicPress. If you get this error, make sure that your .htaccess file has read and write permissions.

## Contribute
If you'd like to make a contribution to the CP-Brute Force Login Protection plugin, you can submit a pull request to our [GitHub Repository](https://github.com/PC-Rights/CP-Brute-Force-Login-Protection/).

## Changelog

### 2.0.1
* Remove from Settings tab and assume Security page exists

### 2.0.0
* Fork from 1.5.3 and add code for ClassicPress Security Page

### 1.5.2
* Bugfix

### 1.5.1
* Security fix

### 1.5
* Improved stability

### 1.4.1
* Option to email administrator when an IP has been blocked
* Button to whitelist your current IP
* Bugfixes and improvements

### 1.4
* Ability to whitelist trusted IPs
* Ability to create custom message to show to blocked users
* Delay execution after a failed login attempt (to slow down brute force attack)
* Performance improvements

### 1.3
* Protection against brute force attacks using Auth Cookies

### 1.2
* Option to inform user about remaining attempts on login page
* Ability to reset options
* Status panel on the settings page

### 1.1
* Added Dutch translation

### 1.0
* Initial version
