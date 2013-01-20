Lista de cosas que instalo siempre
==============

Utilities & Package Managers
--------------------------


### [Homebrew][]: ###

Install from source, then update, then upgrade (Sanity check)

        ruby -e "$(curl -fsSkL raw.github.com/mxcl/homebrew/go)
        brew update
        brew upgrade

[Homebrew]:         http://mxcl.github.com/homebrew/



### GNU Tools ###

* [GNU coreutils][]

        brew install coreutils
        export $PATH=$(brew --prefix coreutils)/libexec/gnubin:$PATH


* [findutils][]:    `brew install findutils`
* [bash][]:         `brew install bash`
* [wget][]:         `brew install wget --enable-iri`
* [ack][]:          `brew install ack`
* [rename][]: `brew install rename`
* [tree][]:   `brew install tree`

[GNU coreutils]:    http://www.gnu.org/software/coreutils/
[findutils]:        http://www.gnu.org/software/findutils/
[bash]:             http://www.gnu.org/software/bash/
[wget]:             http://www.gnu.org/software/wget/
[ack]:              http://betterthangrep.com/
[rename]:           http://plasmasturm.org/code/rename/
[tree]:             http://mama.indstate.edu/users/ice/tree/



### OSX specific tools ###

        brew tap homebrew/dupes
        brew install homebrew/dupes/grep



### [git][]: ###

Install from formula, basic config

        brew install git 
        git config --global user.name "Your Name Here"
        # Sets the default name for git to use when you commit

        git config --global user.email "your_email@youremail.com"
        # Sets the default email for git to use when you commit

Check the [github help][] to finish setup


[git]:              http://git-scm.org/
[github help]:      https://help.github.com/articles/set-up-git



Python
------
* [Virtual Environment][]:          `pip install virtualenv`
* [Django][]:                       `pip install django`
* [Python Imaging Library (PIL)][]: `pip install pil`
* [pyMongo][]:                      `pip install pymongo`
* [mongoengine]():                  `pip install mongoengine`

[Virtual Environment]:          http://http://pypi.python.org/pypi/virtualenv
[Django]:                       http://djangoproject.com
[Python Imaging Library (PIL)]: http://www.pythonware.com/products/pil/
[pyMongo]:                      http://www.mongodb.org/display/DOCS/Python+Language+Center


Node
----

* [mongodb Node Driver][]:  `npm install -g mongodb`
* [mongodb ORM][]:          `npm install -g mongoose`
* [connect][]:              `npm install -g connect`
* [epub][]:                 `npm install -g epub`
* [expresso][]:             `npm install -g expresso`
* [jshint][]:               `npm install -g jshint`
* [node-inspector][]:       `npm install -g node-inspector`
* [phantom][]:              `npm install -g phantom`
* [recess][]:               `npm install -g recess`
* [uglify-js][]:            `npm install -g uglify-js`
* [Less CSS Compiler][]:    `npm install -g less`
* [Swig Template Engine][]: `npm install -g swig`
* [Express Framework][]:    `npm install -g express`

[mongodb Node Driver]:  http://www.mongodb.org/display/DOCS/node.JS
[mongodb ORM]:          http://mongoosejs.com/
[connect]:              http://www.senchalabs.org/connect/       
[epub]:                 https://github.com/andris9/epub
[expresso]:             http://visionmedia.github.com/expresso/
[jshint]:               https://github.com/jshint/jshint
[node-inspector]:       https://github.com/dannycoates/node-inspector
[phantom]:              http://phantomjs.org/
[recess]:               https://github.com/twitter/recess
[uglify-js]:            https://github.com/mishoo/UglifyJS
[Less CSS Compiler]:    http://lessjs.org/
[Swig Template Engine]: http://paularmstrong.github.com/swig/
[Express Framework]:    http://expressjs.com


Databases
---------
* [mysql][]:    `brew mysql`
* [mongodb][]:  `brew mongodb`

[mysql]:    http://mysql.com
[mongodb]:  http:/mongodb.org


Editors, IDEs, Browsers.
------------------
* [Textmate][] (ver el [README.md][textmate_readme]):

Prerequisites:

    brew install ragel boost multimarkdown hg ninja

Clone and Build

    git clone https://github.com/textmate/textmate.git  
    cd textmate
    git submodule update --init
    ./configure && ninja


`io` Library:

    ninja io                 # Build the io library and run tests.
    ninja io/coerce          # Build the io library and skip tests.
    ninja io/clean           # Remove the build folder for the io library.
    ninja io/headers         # Copy exported headers to $builddir/include.

`mate` application (Muy importante recordar este!!)

    ninja mate               # Build the mate executable.
    ninja mate/run           # Build and run the mate executable.
    ninja mate/clean         # Remove the build folder for the mate executable.

Texmate Bundle Application:

    ninja TextMate           # Build and sign TextMate.app.
    ninja TextMate/run       # Build, sign, and run TextMate.app.
    ninja TextMate/clean     # Remove the build folder for TextMate.app.
    ninja TextMate/dsym      # Create a tarball with extracted dSYM files.
    ninja TextMate/tbz       # Create a tarball of TextMate.app. Also produce the dsym tarball.
    ninja TextMate/deploy    # Push a nightly build. Fails without proper credentials :)

Clean

    ninja -t clean

* [multimarkdown][]:    `brew install multimarkdown`
* [lynx][]:             `brew install lynx`
* [webkit2png][]:       `brew install webkit2png`


[multimarkdown]:    https://github.com/fletcher/peg-multimarkdown
[Textmate]:         https://github.com/textmate/textmate
[textmate_readme]:  https://github.com/textmate/textmate/blob/master/README.md
[lynx]:             http://lynx.isc.org/
[webkit2png]:       http://www.paulhammond.org/webkit2png/


Libraries, Sources, Boilerplates, Repos, Etc.
----------------------------------------------
* [html5boilerplate][]: `git clone https://github.com/h5bp/html5-boilerplate.git`
* [h5bp Node Build][]:  `curl https://raw.github.com/gist/2359881/install.sh | sh`

[html5boilerplate]: http://html5boilerplate.com/
[h5bp Node Build]:  https://github.com/h5bp/node-build-script