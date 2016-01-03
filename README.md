# freebsd-desktop
Script to setup a FreeBSD machine for desktopuse

This script is meant to be run once after a fresh installation of
FreeBSD. It will do an update of the system, install a lot of packages
and setup some stuff you could like to have on a desktop machine such as
languagesettings, tmp-cleanup, anacron, powerd, ntp etc.

At the moment the script will install a desktop based on KDE, Lumina-DE or Awesome (you have the choice).

You should have at least 8GB free space to install a KDE desktop.

To get all benefits out of this script you should _not_ add a user during installation, but after having this script added some config-files to the homedir-skeleton. If you have added users nevertheless, the script will ask you to remove them in order to re-add them afterwards.


## Using this script
After having done a freh installation of FreeBSD (I'd recommend not to add a user during installation, but after this script has done its work) log in as root and download the script like this:
<pre><code>fetch --no-verify-peer https://raw.githubusercontent.com/rakor/freebsd-desktop/master/freebsd-desktop</code></pre>

The default behaviour is to install a german KDE with additional software (office, browser, etc.). If you'd like to have an other language or a smaller Awesome or Lumina-desktop instead open the script and edit the variables at the top to meet your choice.

Next, let the script do its job
<pre><code>sh ./freebsd-desktop</code></pre>

At the end the script gives you the possibility to add an initial user. If you need any additional users, this is the right time for it:
<pre><code>adduser</code></pre>

If the script has done its job and everything went well reboot into your new desktop
<pre><code>reboot</code></pre>
