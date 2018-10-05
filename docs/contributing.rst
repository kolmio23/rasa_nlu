.. _contributing:

Contributing
============


There is a big community of `Rasa contributors <https://rasa.com/community/contribute/>`_. 
This page is mostly about how to contribute code to the Rasa NLU and Rasa Core libraries, but 
there are many other ways you can contribute! Read about them `here <https://rasa.com/community/contribute/>`_.

Code of conduct
---------------

Rasa NLU and Rasa Core adhere to the `Contributor Covenant Code of Conduct <http://contributor-covenant.org/version/1/4/>`_.
By participating, you are expected to uphold this code.


Creating Pull Requests
----------------------

To suggest changes, you need to create a fork of the library you want to change,
and then submit a pull request. GitHub has instructions on how to do that `here <https://help.github.com/articles/creating-a-pull-request-from-a-fork/>`_.

Typos and other Small Fixes
---------------------------

If you've noticed a small bug or typo, please mention this in an issue,
or if you feel comfortable, please create a Pull Request with your fix. 

New Features
------------

If you want to add a new feature to Rasa, **please create an issue first**. 
Please also search through existing issues in case the topic has already been discussed.

We will not automatically merge in a new feature just because you developed it,
so it is worth discussing with the maintainers before you start work to avoid
disappointment. 

If we merge in a new feature, we are taking on a lot of future work to maintain it.
There is a good discussion of these trade-offs in the `Elastic developer constitution <https://github.com/elastic/engineering/blob/master/development_constitution.md>`_ .


Tests
-----

Any new feature or change in behaviour **must** have a test written for it.
This is enforced by our code review process.
There **must** also be documentation for every feature. When you create a 
pull request, GitHub will include a checklist of everything that's required.
The code in your pull request will automatically be built by Travis CI, which
will also run all the tests. 


Python Conventions
^^^^^^^^^^^^^^^^^^

To ensure consistent style, all Python code has to follow the pep-8 specification.
This is quite strict, so it's worth installing a linter for your editor or IDE which
does this automatically for you. 


Python 2 and 3 Cross Compatibility
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Rasa runs in both Python 2 and Python 3, although Python 2 support is being phased out 
by most major Python projects, and Rasa will also drop Python 2 support eventually.

To ensure cross compatibility between Python 2 and 3 we prioritize Python 3 conventions.
Keep in mind that:

- all string literals are unicode strings
- division generates floating point numbers. Use ``//`` for truncated division
- some built-ins, e.g. ``map`` and ``filter`` return iterators in Python 3. If you want to make use of them import the Python 3 version of them from ``builtins``. Otherwise use list comprehensions, which work uniformly across versions
- use ``io.open`` instead of the builtin ``open`` when working with files
- The following imports from ``__future__`` are mandatory in every Python file: ``unicode_literals``, ``print_function``, ``division``, and ``absolute_import``

Please refer to this `cheat sheet <http://python-future.org/compatible_idioms.html#>`_ to learn how to write different constructs compatible with Python 2 and 3.

