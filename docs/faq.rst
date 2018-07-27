How can I get training data for my chatbot? + more FAQs
=======================================================

Getting Training Data for Chatbots and Assistants
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~



Is there a GUI for labeling data?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

You are spoiled for choice! `Rasa Platform <https://rasa.com/products/rasa-platform>`_ comes with a graphical interface
for creating both Rasa NLU and Rasa Core data. 
`rasa-trainer-ui <https://github.com/RasaHQ/rasa-nlu-trainer>`_ is an open source tool for annotating NLU data. 
`Rasa UI <https://github.com/paschmann/rasa-ui>`_ is a web application which uses Rasa NLU as its backend.



Building Advanced chatbots and assistants
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Where can I learn the fundamentals of chatbots?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Rasa has developed a course on `building chatbots in python <https://www.datacamp.com/courses/building-chatbots-in-python>`_ together with DataCamp. 

What does it mean to build machine-learning based dialogue?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Rule-based dialogue systems do not scale. There has been a lot of research on using machine learning
to overcome these limitations, `this post <https://medium.com/rasa-blog/a-new-approach-to-conversational-software-2e64a5d05f2a>`_ goes into a lot more depth. 

What are some examples of great bots built with Rasa?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

`Meekan <https://meekan.com/>`_ is a popular slack bot for scheduling meetings. 
`Tia <https://asktia.com/>`_ is a women's health company with a chatbot as part of the core experience.
`Helvetia <https://www.helvetia.com/ch/web/en/about-us/about-helvetia/information/chatbot-service.html>`_ is an
insurance company that lets you report bike thefts via a Facebook Messenger chatbot. 


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

How can I connect Rasa to backend intregrations?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

How can I coordinate work with my team?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

`Rasa Platform <https://rasa.com/products/rasa-platform/>`_ is our enterprise product
and adds a number of features for teamwork.

How can I coordinate work with my team?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

`Rasa Platform <https://rasa.com/products/rasa-platform/>`_ is our enterprise product.
Rasa Platform subscriptions come with our Customer Success program which includes enterprise grade support.

How do I deploy Rasa in production?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

`Rasa Platform <https://rasa.com/products/rasa-platform/>`_ runs on premise or on your private cloud.
Rasa Platform subscriptions come with our Customer Success program which includes enterprise grade support.

How can I add a Rasa Bot to my website?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

There are multiple open source projects for adding a Rasa-compatible chat widget to a website.
`Rasa Webchat <https://github.com/mrbot-ai/rasa-webchat>`_ is under MIT license and `Chatroom <https://github.com/scalableminds/chatroom>`_ is under AGPL 3.

How can I create a custom channel integration for Rasa?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

It is straightforward to implement a custom integration. Check out the docs `here <http://rasa.com/docs/core/connectors/#custom-channels>`_

About Rasa the Company
~~~~~~~~~~~~~~~~~~~~~~

How does Rasa make money if everything is open source?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

`Rasa Platform <https://rasa.com/products/rasa-platform/>`_ is a paid product which we offer in addition to the open source Rasa Stack.


How do I get access to your roadmap?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



I've already built a bot with the Rasa Stack. Can I easily upgrade to Rasa Platform?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Rasa Platform is installed alongside Rasa Core and NLU. Rasa Platform can work with your 
already existing Rasa NLU and Rasa Core servers.

How can I get in touch?
^^^^^^^^^^^^^^^^^^^^^^^

If you have a question about how to use Rasa, the Rasa Community is the best place to help.
For bug reports and feature requests, please go to `GitHub <https://github.com/RasaHQ>`_.
For everything else please email hi@rasa.com


