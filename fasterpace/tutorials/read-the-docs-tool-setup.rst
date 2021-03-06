read-the-docs-tool-setup
========================

By `Jack Henderson`_

In this tutorial, we will ...

.. contents:: Sections:
  :local:
  :depth: 1

Prerequisites
-------------

http://www.sphinx-doc.org/en/stable/install.html#windows-install-python-and-sphinx


Install Python
--------------
https://www.python.org/downloads/windows/

.. image:: read-the-docs-tool-setup/_static/read-the-docs-tool-setup-1.png


.. image:: read-the-docs-tool-setup/_static/read-the-docs-tool-setup-2.png


.. image:: read-the-docs-tool-setup/_static/read-the-docs-tool-setup-3.png


.. image:: read-the-docs-tool-setup/_static/read-the-docs-tool-setup-4.png


.. image:: read-the-docs-tool-setup/_static/read-the-docs-tool-setup-5.png


At command prompt, type “python” and Enter. The version will display.
.. image:: read-the-docs-tool-setup/_static/read-the-docs-tool-setup-6.png


EXPERIMENTAL: Upgrade pip
C:\> python -m pip install --upgrade pip

.. image:: read-the-docs-tool-setup/_static/read-the-docs-tool-setup-7.png


Install sphinx with pip

C:\> pip install sphinx

After installation, type sphinx-build -h on the command prompt. If everything worked fine, you will get a Sphinx version number and a list of options for this command

Install auto build
C:\> pip install sphinx sphinx-autobuild

Install the theme file for read the docs
D:\>pip install sphinx_rtd_theme

D:\>pip install sphinxcontrib-httpdomain
D:\>pip install sphinxcontrib-dotnetdomain


Download and install PyCharm editor.
https://www.jetbrains.com/pycharm/



Create your first project
-------------------------

D:\>md myproject
D:\>cd myproject
D:\myproject>md docs
D:\myproject>cd docs
D:\myproject\docs>

D:\myproject\docs>sphinx-quickstart
Welcome to the Sphinx 1.4.1 quickstart utility.

Please enter values for the following settings (just press Enter to
accept a default value, if one is given in brackets).

Enter the root path for documentation.
> Root path for the documentation [.]:

You have two options for placing the build directory for Sphinx output.
Either, you use a directory "_build" within the root path, or you separate
"source" and "build" directories within the root path.
> Separate source and build directories (y/n) [n]: y

Inside the root directory, two more directories will be created; "_templates"
for custom HTML templates and "_static" for custom stylesheets and other static
files. You can enter another prefix (such as ".") to replace the underscore.
> Name prefix for templates and static dir [_]:

The project name will occur in several places in the built documentation.
> Project name: My Project Docs
> Author name(s): Jack Henderson

Sphinx has the notion of a "version" and a "release" for the
software. Each version can have multiple releases. For example, for
Python the version is something like 2.5 or 3.0, while the release is
something like 2.5.1 or 3.0a1.  If you don't need this dual structure,
just set both to the same value.
> Project version: 0.0
> Project release [0.0]: 0.0.1

If the documents are to be written in a language other than English,
you can select a language here by its language code. Sphinx will then
translate text that it generates into that language.

For a list of supported codes, see
http://sphinx-doc.org/config.html#confval-language.
> Project language [en]:

The file name suffix for source files. Commonly, this is either ".txt"
or ".rst".  Only files with this suffix are considered documents.
> Source file suffix [.rst]:

One document is special in that it is considered the top node of the
"contents tree", that is, it is the root of the hierarchical structure
of the documents. Normally, this is "index", but if your "index"
document is a custom template, you can also set this to another filename.
> Name of your master document (without suffix) [index]:

Sphinx can also add configuration for epub output:
> Do you want to use the epub builder (y/n) [n]: y

Please indicate if you want to use one of the following Sphinx extensions:
> autodoc: automatically insert docstrings from modules (y/n) [n]: y
> doctest: automatically test code snippets in doctest blocks (y/n) [n]:
> intersphinx: link between Sphinx documentation of different projects (y/n) [n]: y
> todo: write "todo" entries that can be shown or hidden on build (y/n) [n]: y
> coverage: checks for documentation coverage (y/n) [n]: y
> imgmath: include math, rendered as PNG or SVG images (y/n) [n]:
> mathjax: include math, rendered in the browser by MathJax (y/n) [n]:
> ifconfig: conditional inclusion of content based on config values (y/n) [n]:
> viewcode: include links to the source code of documented Python objects (y/n) [n]:
> githubpages: create .nojekyll file to publish the document on GitHub pages (y/n) [n]:

A Makefile and a Windows command file can be generated for you so that you
only have to run e.g. `make html' instead of invoking sphinx-build
directly.
> Create Makefile? (y/n) [y]: y
> Create Windows command file? (y/n) [y]: y

Creating file .\source\conf.py.
Creating file .\source\index.rst.
Creating file .\Makefile.
Creating file .\make.bat.

Finished: An initial directory structure has been created.

You should now populate your master file .\source\index.rst and create other documentation
source files. Use the Makefile to build the docs, like so:
   make builder
where "builder" is one of the supported builders, e.g. html, latex or linkcheck.


D:\myproject\docs>

D:\myproject\docs>make html

D:\myproject\docs>cd source

D:\myproject\docs\source>sphinx-autobuild . build\html

+--------- manually triggered build ---------------------------------------------
Error: Config directory doesn't contain a conf.py file.
+--------------------------------------------------------------------------------

[I 160412 12:05:30 server:281] Serving on http://127.0.0.1:8000
[I 160412 12:05:30 handlers:59] Start watching changes
[I 160412 12:05:30 handlers:61] Start detecting changes
[I 160412 12:05:35 handlers:132] Browser Connected: http://127.0.0.1:8000/

Open your browser to http://127.0.0.1:8000

.. image:: read-the-docs-tool-setup/_static/read-the-docs-tool-setup-8.png



Open index.rst using PyCharm and change description.

.. image:: read-the-docs-tool-setup/_static/read-the-docs-tool-setup-9.png


Save the file and look at the browser:

http://127.0.0.1:8000

Finished!


