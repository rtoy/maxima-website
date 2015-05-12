Maxima Website
==============

This is the GIT repository for the Website of project Maxima
<http://maxima.sourceforge.net>

Mirroring
---------

You are welcome to keep a mirror of Maxima's Website in you own site or
to use it as a template for your own Website. To do that, you just have
to retrieve this repository somewhere in your own site. It will work
without any additional configuration or external files.

A copy of this repository will even work locally in your computer, even
if you don't have a Web server installed. This could be a handy way of
keeping a local copy of all the information in the Website. All you need
is a Web browser with Javascript enabled. Simply point your browser
to file:///dir/index.html, where dir is the name of the directory where
you retrieved this repository.

Contributing
------------

You can help us by correcting any typos you find, translating pages to
other languages or adding new pages. Just copy the page you are going to
modify or translate to your disk, edit it and send the result to
villate@fe.up.pt.

If you are a member of the project, you can also commit your changes
directly into the Git repository. If you are not a member but would
like to have write privileges to help improve the site, ask villate@fe.up.pt
or other project administrators to give you access.

After committing any modifications to this repository, the Sourceforge Web
server pages must be refreshed manually by running "git pull" in the
directory /home/project-web/maxima/htdocs. If you are not a member of
the project, the project administrators will do that once they become aware
that the repository changed or you can ask them to do that in the project
mailing list.

If you are a member of the project and you use Linux, you can automate the
process of refreshing the pages by creating a file "update_maximaweb"
with the following content:

    #!/bin/sh
    USER=sourceforge_name
    ssh $USER,maxima@shell.sourceforge.net create
    ssh $USER,maxima@shell.sourceforge.net "cd /home/project-web/maxima/htdocs; git pull"
    ssh $USER,maxima@shell.sourceforge.net shutdown

Where sourceforge_name should be replaced with your username in
Sourceforge. Make that file executable and put it somewhere in your
executable commands path. Then run that command every time you would
like to update the Website with the current GIT repository.
