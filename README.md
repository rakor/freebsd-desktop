# freebsd-desktop
Script to setup a FreeBSD machine for desktopuse


This script is meant to be run once after a fresh installation of
FreeBSD. It will do an update of the system, install a lot of packages
and setup some stuff you could like to have on a desktop machine such as
languagesettings, tmp-cleanup, anacron, powerd, ntp etc.

At the moment the script will install a desktop based on KDE

You should have at least 8GB free space to install all the packages.

## Using this script
After having done a freh installation of FreeBSD (I'd recommend not to add a user during installation, but after this script has done its work) log in as root and download the script like this:
<pre><code>fetch --no-verify-peer https://raw.githubusercontent.com/rakor/freebsd-desktop/master/freebsd-desktop</code></pre>

The default behaviour is to install a german KDE. If you'd like to have an other language open the script and edit the variables at the top to meet your joice.

Then let the script do its job
<pre><code>sh ./freebsd-desktop</code></pre>

If the script has done its job and everything went well reboot into your new desktop
<pre><code>reboot</code></pre>
