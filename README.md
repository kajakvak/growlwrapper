Wrapper script for growl.



Instructions
============


1. Download Growl for windows: http://www.growlforwindows.com/gfw/
1. Download growlnotify for windows: http://www.growlforwindows.com/gfw/help/growlnotify.aspx
1. Unzip and put growlnotify.exe in ~/bin
1. Clone repository: git clone https://github.com/mortenberg80/growlwrapper.git
1. Create symlink for mvn wrapper script: ln -s growlnotify/mvn ~/bin/mvn
1. Create symlink for generic wrapper script: ln - growlnotify/n ~/bin/n
1. Ensuer that ~/bin is on your PATH. Add the following to your .bashrc

        if [ -d "${HOME}/bin" ] ; then
          PATH="${HOME}/bin:${PATH}"
        fi



