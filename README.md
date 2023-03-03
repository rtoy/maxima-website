Maxima Website
==============

This is the GIT repository for the Website of project Maxima
<https://maxima.sourceforge.io>

Mirroring
---------

You are welcome to keep a mirror of Maxima's Website in you own site or
to use it as a template for your own Website. To do that, you just have
to retrieve this repository somewhere in your own site. It will work
without any additional configuration or external files.

A copy of this repository will even work locally in your computer, even
if you don't have a Web server installed. This could be a handy way of
keeping a local copy of all the information in the Website. All you need
is a Web browser. Simply point your browser
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

After committing any modifications to the repository, the Sourceforge
Web server pages must be refreshed manually by copying any new files
and updating changed files in the Web server. If you are not a member
of the project, the project administrators will do that once they
become aware that the repository has changed or you can request a Web
server update in the mailing list.

Obsolete
--------

There is now, in hooks/post-receive-user, a few lines that
automatically update the website. The following is retained for
information only.


If you are a member of the project and you use Linux, you can update the
pages in the Web server using rsync. First move to the directory where you
have your copy of the Web repository, make sure you don't have any additional
files or changes that have not been committed, and then issue the following
command:

    rsync -avz --delete * username@web.sf.net:/home/project-web/maxima/htdocs

Where username should be replaced with the username you use in
Sourceforge. In addition to rsync, you can also use sftp or scp to copy files
to the web.sf.net; if you use one of those programs instead, make sure you
send any new files, update the files that have changed and delete the ones
that have been removed from the repository.
