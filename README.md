###INTRODUCTION

Lightqvod is a small bash script that helps users download and manage qvod resources from web.
It makes you a wiarzd with qvod movies.

###WINE

Qvod is not officially supported on linux systems. 
Wine allows you to run many Windows programs (including the qvod movie downloader) on linux. Please follow the instructions on http://www.winehq.org/download/ to download and install wine.

###BROWSER EXTENSION

In order to capture qvod url on internet, you need add an extension to your browser. Two versions of extensions for firefox and chromium can be found in the *lightqvod/plugins* directory.
- For firefox users, simply drag the .xpi file onto the browser to install.
- For chromium users, click on the 'customize' icon on the upper-right, then choose 'tools->extensions->Load unpacked extension', select the whole directory 'qvodurlfinder_chromium' and click 'open'.

###HOW TO USE

First, go inside the *lightqvod* directory,
```bash
./install
```
This will initialize lightqvod for the current user. Then use command *lq* everywhere to launch lightqvod. If you want to uninstall lightqvod, add an '-u' option after this command.

To start, use the following command to let lightqvod listen to the port:
```bash
lq -l
```
Then after you open a webpage containing a qvod resource or player window, press 'ctrl+e' in firefox or 'ctrl+q' in chromium. If capture succeeds, a qvod URL will be sent to lightqvod. For other uses, please see *help*.

###LICENSE

This software is under MIT license.
