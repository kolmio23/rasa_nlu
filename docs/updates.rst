:desc: What's new with Rasa Stack and Platform

What's New?
===========

November 2018
~~~~~~~~~~~~~

Major release of Rasa Core (0.12) which brings a lot of new functionality:

- Vastly improved `slot filling <https://rasa.com/docs/core/slotfilling/>`_ through the new ``Forms``. You can now separate out business logic from learned behavior.
- A `new <https://rasa.com/docs/core/interactive_learning/#visualization-of-conversations>`_ interactive learning experience which renders a dynamically updated graph to the web browser.
- `End-to-end <https://rasa.com/docs/core/evaluation/#end-to-end-evaluation-of-rasa-nlu-and-core>`_ evaluation of Rasa NLU and Core models together.

New interactive learning feature in Rasa Platform. 
Jump from any point in a user conversation into interactive learning, providing corrections to the bot's actions
and taking over as the user.

October 2018
~~~~~~~~~~~~

Improved support for multiprocessing in the Rasa NLU server. 
Tensorflow training is now non-blocking in python 3. 

All Rasa Platform users now have access to experimental features.
Features can be activated via the Rasa Platform UI or programatically 
using the API. 
Experimental support for interactive learning in the Rasa Platform UI. 


September 2018
~~~~~~~~~~~~~~

The interactive learning CLI has been re-worked completely and made much
more user friendly. Users and now undo annotation mistakes, make NLU 
corrections for both intents and entities, and navigate system predictions
using arrow keys. 
Added a socket.io input channel to Rasa Core for real-time messaging.
Rasa Core's ``evaluate`` script can now be made to fail on prediction errors
for use in CI. 
Added support for JWT authentication in the Rasa Core server, improving security.
The ``UserMessage`` class now tracks which channel the user was active in (e.g. Facebook,
Slack)

A major release (0.16.0) or Rasa Platform with full support for Rasa Core 0.11.4+ 
and Rasa NLU 0.13.3+. 
Added documentation for running Rasa Platform with custom Core and NLU components / classes.
Added an API endpoint for fetching all service logs for remote debugging of 
Rasa Platform installations. 

August 2018
~~~~~~~~~~~

Rasa Core 0.11 is out!
----------------------
This is a major update, which requires a little migration work, but 
greatly simplifies deploying Rasa Core in production. Custom actions are now run in a separate
server, which you can create using the new `rasa_core_sdk <https://github.com/RasaHQ/rasa_core_sdk>`_.

- Check out the detailed `changelog <https://github.com/RasaHQ/rasa_core/blob/master/CHANGELOG.rst>`_, `migration instructions <http://rasa.com/docs/core/migrations/>`_, and `livestream <https://forum.rasa.com/t/rasa-core-sdk-live-stream/826>`_.
- Rasa Core 0.11 also ships with the new ``EmbeddingPolicy``, implemented in tensorflow and described in a paper (link coming soon). 
- **For Rasa Platform Users**: Rasa Platform 0.16 (coming September 2018) will depend on Rasa Core 0.11. Please ensure that you migrate before updating your installation. This update is necessary to enable new platform features, and to make deployment and maintenance simpler. If you have any questions about migrating to Rasa Core 0.11, please use your dedicated support email to reach out. 
- Rasa Platform can now show every conversations in story format, just click on a message in a conversation and click 'view story'. This is a convenient way to collect more stories as training data.
- Rasa Platform has an updated CMS for editing bot responses. Editing templates is instantaneous and doesn't require re-training Rasa Core. 


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

