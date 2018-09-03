:desc: What's new with Rasa Stack and Platform

What's New?
===========

August 2018
~~~~~~~~~~~

- Rasa Core 0.11 is out! This is a major update, which requires a little migration work, but 
greatly simplifies deploying Rasa Core in production. Custom actions are now run in a separate
server, which you can create using the new `rasa_core_sdk <https://github.com/RasaHQ/rasa_core_sdk>`_.
Check out the detailed `changelog <https://github.com/RasaHQ/rasa_core/blob/master/CHANGELOG.rst>`_, `migration instructions <http://rasa.com/docs/core/migrations/>`_, and tutorial.
- Rasa Core 0.11 also ships with the new ``EmbeddingPolicy``, implemented in tensorflow and described in a paper (link coming soon). 


July 2018
~~~~~~~~~

All new docs!
-------------

- Interactive quickstarts for Rasa NLU and Rasa Core
- Unified search across all docs, and all docs now at https://rasa.com/docs
- Reorganized Rasa NLU and Core docs, splitting 'learning' from 'reference' material

Community Forum
---------------

We felt that a lot of good discussions were getting lost on gitter. So we're moving the 
community support over to the newly created `Rasa Community Forum <https://forum.rasa.com>`_
It's going to be a great place for the Rasa community to meet, find answers to questions,
participate in discussions, share ideas and keep up to date with the most recent Rasa updates.


Released Rasa Core 0.10
-----------------------

- Ability to manage bot responses externally (instead of putting them into the domain.yml file)
- An option to ignore entities for certain intents
- New default action ActionDefaultFallback


Released Rasa NLU 0.13
----------------------

- language-agnostic NER
- support multuple training processes per project


