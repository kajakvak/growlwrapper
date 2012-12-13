Wrapper script for growl.



Instructions
============

# Download Growl for windows: http://www.growlforwindows.com/gfw/
# Download growlnotify for windows: http://www.growlforwindows.com/gfw/help/growlnotify.aspx
# Unzip and put growlnotify.exe in ~/bin
# Clone repository: git clone <repo>
# Create symlink for mvn wrapper script: ln -s growlnotify/mvn ~/bin/mvn
# Create symlink for generic wrapper script: ln - growlnotify/n ~/bin/n

# Ensuer that ~/bin is on your PATH.

    if [ -d "${HOME}/bin" ] ; then
      PATH="${HOME}/bin:${PATH}"
    fi



