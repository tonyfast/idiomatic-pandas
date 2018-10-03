
# Idiomatic pandas

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/tonyfast/idiomatic-pandas/master)
[NBViewer](http://nbviewer.jupyter.org/github/tonyfast/idiomatic-pandas/blob/master/readme.ipynb)

This repository will help demonstrate interactive data manipulation in [__JupyterLab__](https://jupyterlab.readthedocs.io) using a subset of the extensive [🐼 API](https://pandas.pydata.org/).  During this demo, we will treat `🐼.DataFrame` and `🐼.Series` as first 
class citizens in our notebooks. 🐼 is a [__NumFocus sponsored__](https://numfocus.org/sponsored-projects) open source Python package for working with [tidy data](https://en.wikipedia.org/wiki/Tidy_data).

This repository was created for [Munmun DeChoudhury's](http://www.munmund.net/) [Social Computing course](http://www.munmund.net/CS6474_Fall2018.html) on October 3, 2018.

> Please checkout the [`deathbeds` blog](http://deathbeds.github.io) for weekly posts about literate and scientific computing.

> To interact with the local scientific computing community join [PyData Atlanta](https://www.meetup.com/PyData-Atlanta/) or [The Atlanta Jupyter User Group](https://www.meetup.com/Atlanta-Jupyter-User-Group/).

> [A little news](https://gist.github.com/tonyfast/c7505b54166130a5836b0ece181bbb23) before we get going.

## Objective

> 10 Get into a rut early: Do the same process the same way. Accumulate idioms. Standardize. The only difference(!) between Shakespeare and you was the size of his idiom list - not the size of his vocabulary.
>> [Alan Perlis - _Perlisisms_](http://www.cs.yale.edu/homes/perlis-alan/quotes.html)

* We will treat public Github data as social data.  
* We will manipulate, combine, and explore multiple data sources from the Github API.
* We will discuss how 🐼 objects may replace common Python operations.
* We will explore how JupyterLab can augment the data analysis experience.
* We will discuss third party libraries that extend 🐼s.

> Some syntaxes in this demonstartion may look unfamiliar.  Please ask questions when you have them.  In this code, the audience will see a mixture if functional programming, asynchronous programming, and caching.

## Why does this demonstration exist?

> I feel a major difference between the [R culture](https://en.wikipedia.org/wiki/R_(programming_language)) and Python culture is that Python users seem to create code more often, whereas R users often use code. There seems to be a strong atmosphere of software engineering in the Python world: in the beginning was the custom class (with methods). For R users, in the beginning was the data.

>> [Yihui Xie - _The First Notebook War_](https://yihui.name/en/2018/09/notebook-war)

There are a lot of 🐼 examples on the web, but they _feel_ more like software rather than data analysis.  Having too many idioms may muddle data analysis & software engineering.  Hopefully, this demonstration promotes the value of 🐼 as a productivity tool for data analysis, and accelerates insight during the development process.

## Tidy Data

[![image](https://user-images.githubusercontent.com/4236275/46415900-524e8e80-c6f4-11e8-8183-6732beeecafa.png)](https://vita.had.co.nz/papers/tidy-data.pdf)


```python
    import this
```

    The Zen of Python, by Tim Peters
    
    Beautiful is better than ugly.
    Explicit is better than implicit.
    Simple is better than complex.
    Complex is better than complicated.
    Flat is better than nested.
    Sparse is better than dense.
    Readability counts.
    Special cases aren't special enough to break the rules.
    Although practicality beats purity.
    Errors should never pass silently.
    Unless explicitly silenced.
    In the face of ambiguity, refuse the temptation to guess.
    There should be one-- and preferably only one --obvious way to do it.
    Although that way may not be obvious at first unless you're Dutch.
    Now is better than never.
    Although never is often better than *right* now.
    If the implementation is hard to explain, it's a bad idea.
    If the implementation is easy to explain, it may be a good idea.
    Namespaces are one honking great idea -- let's do more of those!
    

## Modern Idioms

The Python data science ecosystem is evolving rapidly.

* [The Python 3 movement](https://python3statement.org/)
* [fstrings](https://www.python.org/dev/peps/pep-0498/)
* [Path](https://docs.python.org/3/library/pathlib.html)
* [walrus operator](https://speakerdeck.com/di_codes/pep-572-the-walrus-operator)
* [async Python](https://docs.python.org/3/library/asyncio-task.html)
* [IPython 7.0](https://blog.jupyter.org/ipython-7-0-async-repl-a35ce050f7f7)
* [conda forge](https://conda-forge.org/)


# References

I have been using 🐼 for ~4 years now.  Below are some references that have influenced my approaches to data analysis in 🐼.

* http://pandas.pydata.org/pandas-docs/stable/merging.html
* https://tomaugspurger.github.io/modern-1-intro
* https://blaze.readthedocs.io/en/latest/rosetta-pandas.html
* https://pandas.pydata.org/pandas-docs/stable/comparison_with_r.html
* http://matthewrocklin.com/blog/work/2015/06/18/Categoricals
* http://matthewrocklin.com/blog/work/2015/03/16/Fast-Serialization  
* https://pandas.pydata.org/pandas-docs/stable/indexing.html
* https://toolz.readthedocs.io/en/latest/composition.html


```python
    if __name__ == '__main__':
        !jupyter nbconvert --to markdown readme.ipynb
```

    [NbConvertApp] Converting notebook readme.ipynb to markdown
    [NbConvertApp] Writing 5103 bytes to readme.md
    
