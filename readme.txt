
######## ORIGINAL README FOLLOWS ###########

This plugin was developed for the use with a status.net-installation and a accessable yourls-shortener-installation.
See: * http://status.net
     * http://yourls.org

== Installation ==

1. Upload the YourlsPlugin.php in the plugin-folder of your status.net-installation.

2. Modify the following lines by replacing "your-yourls-installati.on" with URL of your YOURLS-installation and replace "your-secret-yourls-signature" with the signature of your YOURLS-installation, which you can found in the tools-section in your admin-backend.

// YOURLS-Shortener-For-Status.net Plugin
addPlugin('Yourls', array('shortenerName'=>'YOURLS','freeService'=>false,'serviceUrl'=>'http://your-yourls-installati.on/yourls-api.php?signature=your-secret-yourls-signature&action=shorturl&url=%1$s&format=json'));

3. Copy the lines in the config.php of your status.net-installation.

4. Log in your status-net-Server, go to "Account/Other", choose "YOURLS" as your favourite shortener and have fun shortening. Status.net by now olny will shorten links if the status-notice including the url is greater than the allowed amount of chars to be sended (usually 140 chars).

Tested with status.net 0.9.1/0.9.2 and yourls 1.4.3, as can be seen at http://s.wuerzblog.de

######### ADDENDUM FROM TONY BALDWIN ###########

This plugin was two years old, and built to work with old Laconica code.
Changing one line made it work again.
(just the location of urlshortenerplugin.php had changed).

As of 2012.03.16 Also tested with current Status.Net code
version 1.0.1, up to date, and pulled TODAY (2012.03.16) from gitorious,
and Yourls v.1.5

tony 
http://tonybaldwin.me
