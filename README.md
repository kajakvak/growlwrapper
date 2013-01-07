Wrapper script for Growl. Used to send notifications to the user when a process has finished. Specifically used for Maven builds, but can also be used for other programs as well.

This instruction works for Windows with Cygwin.


Usage
=====

**Maven wrapper**

Use mvn as usual. This will trigger the mvn-wrapperscript which will trigger the maven executable.

    mvn clean install

This will publish an event to Growl when maven has finished executing.

**Generic wrapper**
        
    n echo foo

This will publish an event to Growl when the program following 'n' has finished executing.

Setting up
==========


1. Download Growl for windows: http://www.growlforwindows.com/gfw/
1. Download growlnotify for windows: http://www.growlforwindows.com/gfw/help/growlnotify.aspx
1. Unzip and put growlnotify.exe in ~/bin
1. Clone repository

        git clone https://github.com/mortenberg80/growlwrapper.git

1. Copy wrapper scripts from this repo and put them in ~/bin
1. Ensure that ~/bin is on your PATH. Add the following to your .bashrc or .bash_profile

        if [ -d "${HOME}/bin" ] ; then
          PATH="${HOME}/bin:${PATH}"
        fi

1. Create environment variable MVN\_HOME and point it to your maven directory
        
        export MVN_HOME=/opt/maven-2.2.1
1. Ensure that Growl is running.