# HOW TO BUILD YOUR DJANGO PROJECT
At your root, create a setup.py file with this content:

<pre>
from setuptools import setup

setup()
</pre>


Then, run in your terminal:   

<pre>
python setup.py sdist      
</pre>


Finally, when you have a dist folder with a source code or a built code (executable), make use of the backend packager twine:

<pre>
twine upload dist/*
</pre>

It will ask for your credentials. You shall use...

### user: __token__
### pass: pypi-<your-secret-pypi-token>

If all dependencies and steps are good, your package setup.cfg has no typos and counts with a unique name and you have all at the correct version or in a safe virtual environment, then, you will publish your package successfully!