 ### About
This is the code for the website [https://web.reprozip.org](https://web.reprozip.org), an informational site for the IMLS-funded project, "Preserving the Dynamic Web." This site is built using [Nikola](https://getnikola.com/), a static site generator that relies on python 3. The instructions for compiling and building the website are below.

### Building
I would recommend you use a virtualenv to build and view this website. This is a Python tool to create isolated Python environments. The HitchHiker's Guide to Python has a [great guide](http://docs.python-guide.org/en/latest/dev/virtualenvs/) on virtual environments that I used to learn how to use/interact with virtualenvs. 

Here's how to make and activate a virtual environment:
<pre><code># install the tool virtualenv
$ pip install virtualenv

# create the Python 3 virtual environment
$ virtualenv -p python3 venv

# activate the virtual environment
$ source venv/bin/activate
</pre></code>

Now, you can get started and install all of the dependecies of this site in its own environment:

<pre><code># install the dependencies
$ pip install Nikola['extras']

# clone this repo
$ git clone git@github.com:reprozip-news-apps/website.git

# change directory (cd) so you are in the right folder for the website
$ cd website

# build the website
$ nikola build

# see the website
$ nikola serve -b
</pre></code>
