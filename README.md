Codepad
=======

A simple interface to http://codepad.org. There are many like it. This
one is mine. I was tempted to use https://github.com/daltonmatos/codepad/
but I didn't like how it was a "proper" python app. I just wanted
something smaller and in a single file.

Usage
-----

Input can be read from stdin

    $ codepad < file.txt

or a pipe

    $ cat file.txt | codepad

or a file.

    $ codepad file

If you want your post to be public, use the "-p" flag.

    $ codepad not_so_secret.txt

If you want to change the language from the default of "Plain Text",
use the "-l" flag. (See the source for language options.)

    $ codepad -l cool_file.py

If you want codepad.org to run your file, add the "-r" flag

    $ codepad -r -l c runme.c


Install
-------

Requires `perl`, `LWP`, and `HTTP::Request::Common`. If you don't
already have them, install them via your OS's package manager...

    $ sudo apt-get install perl libwww-perl libhttp-message-perl

or via cpan

    $ sudo cpan LWP
    $ sudo cpan HTTP::Request::Common

Then copy `codepad` to someplace in your path

    $ cp codepad ~/bin/
    $ chmod a+x ~/bin/codepad

License
-------

Too trivial. Public domain.
