How can I get training data for my chatbot? + more FAQs
=======================================================

Getting Training Data for Chatbots and Assistants
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Getting a good training data set is crucial for building a chatbot or assistant. 
We have a couple of datasets to help you get started on the `Community Forum <https://forum.rasa.com/>`_.

It's also a very good idea to `pretend to be the bot yourself <https://conversations.golastmile.com/put-on-your-robot-costume-and-be-the-minimum-viable-bot-yourself-3e48a5a59308#.d4tmdan68>`_. 

But the most important factor is always real user feedback. At Rasa we strongly believe
that **real conversations are more important than hypothetical ones**.
The best data of all is the result of real humans interacting with your AI.


Is there a GUI for labeling data?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Open Source
***********

- `rasa-trainer-ui <https://github.com/RasaHQ/rasa-nlu-trainer>`_ is an open source tool for annotating NLU data.
- `Articulate <https://samtecspg.github.io/articulate/>`_ is an open source platform for building conversational interfaces.
- `Rasa UI <https://github.com/paschmann/rasa-ui>`_ is a web application which uses Rasa NLU as its backend.

Commercially Supported
**********************
`Rasa Platform <https://rasa.com/products/rasa-platform>`_ comes with a graphical interface
for creating both Rasa NLU and Rasa Core data. 


Building Advanced chatbots and assistants
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Where can I learn the fundamentals of chatbots?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Rasa has developed a course on `building chatbots in python <https://www.datacamp.com/courses/building-chatbots-in-python>`_ together with DataCamp. 

What does it mean to build machine-learning based dialogue?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In our experience, rule-based dialogue systems do not scale. 
There has been a lot of research on using machine learning
to overcome these limitations, `this post <https://medium.com/rasa-blog/a-new-approach-to-conversational-software-2e64a5d05f2a>`_ goes into a lot more depth. 

What are some examples of great bots built with Rasa?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

There are hundreds of great bots out there built with Rasa, built by everyone from startups, 
to NGOs, to the Fortune 500.
We are working on a directory, so email hi@rasa.com if you'd like to be included!

- `Meekan <https://meekan.com/>`_ is a popular slack bot for scheduling meetings. 
- `Tia <https://asktia.com/>`_ is a women's health company with a chatbot as part of the core experience.
- `Helvetia <https://www.helvetia.com/ch/web/en/about-us/about-helvetia/information/chatbot-service.html>`_ is an insurance company that lets you report bike thefts via a Facebook Messenger chatbot. 


I need help developing a bot
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Rasa works with a number of partners who can help you with your project. 
Reach out hi@rasa.com and let us know what you're looking for, and we'll recommend a partner.

How many languages does Rasa support?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

It depends on your exact setup. Rasa NLU has a number of different pipelines.
The ``tensorflow_embedding`` pipeline supports any language that you can tokenize,
whereas the ``spacy`` based pipelines work with any existing spaCy language model.
Rasa Core is independent of which language you use.

Can I create custom models for NLU and Core?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Yes! One of the big advantages of using open source code is that you can customise everything.
There is no one-size-fits-all solution to machine learning problems. You can build custom 
Rasa Core models by creating your own `Policy <https://rasa.com/docs/core/api/policy/>`_, and for Rasa NLU by creating `Custom Components <https://rasa.com/docs/nlu/customcomponents/>`_ .




Deploying Chatbots and Voice apps in Enterprises
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Is there a way to get enterprise-grade support?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Yes. `Rasa Platform <https://rasa.com/products/rasa-platform/>`_ comes with enterprise-grade
support and a choice of SLAs to suit your requirements.

How can I connect Rasa to my backend enterprise systems?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The best way to do this is with `Custom Actions <https://rasa.com/docs/core/customactions/>`_.

How do I deploy Rasa in production?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

We recommend docker for production deployments. For the Rasa Stack we provide
pre-built docker images on docker hub. 
`Rasa Platform <https://rasa.com/products/rasa-platform/>`_ is also containerized, 
and runs either on premise or on your private cloud. It ships with production-ready
container orchestration.


How can non-engineers contribute to bot development?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

`Rasa Platform <https://rasa.com/products/rasa-platform/>`_ is our enterprise product.

How can I add a Rasa Bot to my website?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

There are multiple open source projects for adding a Rasa-compatible chat widget to a website.

- `Rasa Webchat <https://github.com/mrbot-ai/rasa-webchat>`_ is under MIT license
- `Chatroom <https://github.com/scalableminds/chatroom>`_ is under AGPL 3

How can I create a custom integration for Rasa?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

It's straightforward to implement a custom channel (e.g. for company-specific chat software).
Check out the docs `here <http://rasa.com/docs/core/connectors/#custom-channels>`_.

I've already built a bot with the Rasa Stack. Can I easily upgrade to Rasa Platform?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Yes. Rasa Platform is installed alongside Rasa Core and NLU. Rasa Platform can work with your 
already existing Rasa NLU and Rasa Core servers.


About Rasa the Company
~~~~~~~~~~~~~~~~~~~~~~

How does Rasa make money if everything is open source?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

`Rasa Platform <https://rasa.com/products/rasa-platform/>`_ is a paid product which we offer in addition to the open source Rasa Stack.


How do I get access to your roadmap?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

As part of our customer success program, companies have access to our roadmap
and we work closely with them to prioritize upcoming features and get early feedback.


How can I get in touch?
^^^^^^^^^^^^^^^^^^^^^^^

If you have a question about how to use Rasa, the `Rasa Community <https://forum.rasa.com/>`_ is the best place to help.
For bug reports and feature requests, please go to `GitHub <https://github.com/RasaHQ>`_.
For everything else please email hi@rasa.com


.. raw:: html
   :file: livechat.html