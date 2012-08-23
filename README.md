# The GENI Developer Docs (Source Code)

This is the source tree for the documentation for the GENI platform &minus; a platform sponsored by the National Science Foudnation and in partnership with Mozilla Ignite. These docs can be viewed in HTML and PDF form at: [Read The Docs](http://geni-app-developer-documentation.readthedocs.org/en/latest/index.html).

## Building Locally

These docs were written in ReStructured Text, and can be built with [Sphinx](http://sphinx.pocoo.org/). To build the docs, you'll need a python installation and easy_install. Once you have those, you can install sphinx:

	$ easy_install -U Sphinx

And when you're done with that, clone this repository to a local directory and `cd` into it. From there:

	$ make html

You'll see something similar to:

	'sphinx-build' -b html -d build/doctrees   source build/html
	Running Sphinx v1.1.3
	loading pickled environment... done
	building [html]: targets for 1 source files that are out of date
	updating environment: 0 added, 1 changed, 0 removed
	reading sources... [100%] examples/index                                                                                
	looking for now-outdated files... none found
	pickling environment... done
	checking consistency... done
	preparing documents... done
	writing output... [100%] index                                                                                          
	writing additional files... genindex search
	copying static files... done
	dumping search index... done
	dumping object inventory... done
	build succeeded.

	Build finished. The HTML pages are in build/html.

## Editing

The `source/` directory is where the source-form of the docs are kept. Since we're using sphinx, the format of the docs are in Restructured Text, a popular markup language.

The build form of the docs end up in `build`, which is ignored by git due to the `.gitignore` file.

## Questions

Send any and all questions or feedback to katzgrau@gmail.com
