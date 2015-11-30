# JenkinsApp
A Mac OS X app wrapper for Jenkins.

# Design
The app is intended to be used in a way that makes Jenkins highly portable on Mac OS X. All data is contained in the app file/folder structure which helps avoid dealing with admin privileges and start/stop service scripts that you normally have to deal with using the [traditional Jenkins installer](http://mirrors.jenkins-ci.org/osx/).

# Future Changes
The wrapper should be able to handle common admin tasks like updating to the current jenkins.war with a bleeding edge vs LTS toggle, restarting the app or deleting the JENKINS_HOME folder in order to reinitilize the application if so desired.

I also want to parameterize the app in a way that lets the end user easily modify specific Jenkins/Java startup switches in order to help ease the process of correcting scaling issues like raising JVM permgen/memory, enabling/disabling hudson DIY chunking, changing ports, etc.
