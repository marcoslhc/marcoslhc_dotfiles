Lista de cosas que instalo siempre
==============

Utilities & Package Managers
--------------------------
* [Homebrew][]:	


	`ruby -e "$(curl -fsSkL raw.github.com/mxcl/homebrew/go)"`
	brew update
	brew upgrade

* [wget][]:		`brew install wget --enable-iri`
* [git][]:


	brew install git 
	git config --global user.name "Your Name Here"
	# Sets the default name for git to use when you commit

	git config --global user.email "your_email@youremail.com"
	# Sets the default email for git to use when you commit



[Homebrew]: http://mxcl.github.com/homebrew/
[wget]: 	http://www.gnu.org/software/wget/

Python
------
* [Virtual Environment][]:			`pip install virtualenv`
* [Django][]:						`pip install django`
* [Python Imaging Library (PIL)][]:	`pip install pil`
* [pyMongo][]:						`pip install pymongo`
* [mongoengine]():					`pip install mongoengine`

[Virtual Environment]: http://http://pypi.python.org/pypi/virtualenv
[Django]: http://djangoproject.com
[Python Imaging Library (PIL)]: http://www.pythonware.com/products/pil/
[pyMongo]: http://www.mongodb.org/display/DOCS/Python+Language+Center

Node
----

* [mongodb Node Driver][]:	`npm install -g mongodb`
* [mongodb ORM][]:			`npm install -g mongoose`
* [Less CSS Compiler][]:	`npm install -g less`
* [Swig Template Engine][]:	`npm install -g swig`
* [Express Framework][]:	`npm install -g express`

[mongodb Node Driver]:	http://www.mongodb.org/display/DOCS/node.JS
[mongodb ORM]:			http://mongoosejs.com/
[Less CSS Compiler]:	http://lessjs.org/
[Swig Template Engine]:	http://paularmstrong.github.com/swig/
[Express Framework]:	http://expressjs.com

Databases
---------
* [mysql][]:	`brew mysql
* [mongodb][]:	`brew mongodb`

[mysql]:	http://mysql.com
[mongodb]:	http:/mongodb.org

Editors, IDEs, etc.
------------------
* [Textmate][]:


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
	
[Textmate]:	https://github.com/textmate/textmate