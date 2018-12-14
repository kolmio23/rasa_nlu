.. _demobot:

Say hi to Sara - our Rasa Demo Bot! (alpha)
===========================================

.. image:: ../_static/images/sara-mascot.png
   :width: 15%
   :alt: Sara - The Rasa Demo Bot

|
.. raw:: html

   <b>Sara</b> currently helps developers getting started with our docs - her code and training data are open source (repo <a class="reference external" href="https://github.com/RasaHQ/rasa-demo" target="_blank">here</a>) to show the inner workings of a <a class="reference external" href="http://blog.rasa.com/level-3-contextual-assistants-beyond-answering-simple-questions/" target="_blank">contextual AI assistants</a>.
   <br>
   <br>

.. button::
   :link: ../get_started_step1/
   :text: Talk to Sara


Why we built Sara
^^^^^^^^^^^^^^^^^


Contextual AI assistants are still early days and building one is not always easy. That's why we `open sourced <https://github.com/RasaHQ/rasa-demo>`_ a full example.
Sara showcases a few different features of the Rasa Stack:

- Using Rasa Core and NLU to handle contextual conversations
- Extracting entities with a CRF and Duckling
- Slot filling and form actions
- Training word vectors from scratch with the embeddings pipeline
- Generalising conversations with Rasa Core
- Connecting Rasa to a webchat on a website


Why Sara doesn't understand everything you say
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The current release is an alpha version, meaning for now she only supports a few user
goals and has a small dataset. We strongly believe that to build a great contextual AI assistant
you need to learn from real data and so we decided to throw Sara out
there while she's still not perfect.

The more you chat with her, the better she
becomes. Internally, we use `Rasa Platform <https://rasa.com/products/rasa-platform/>`_ to analyse conversations and improve Sara every day.


How you can help
^^^^^^^^^^^^^^^^
Simply by `talking to her <https://rasa.com/docs/get_started_step1/>`_!
If you’d like to give us feedback or raise any
bugs/issues, feel free to do so in the `repo <https://github.com/RasaHQ/rasa-demo>`_.
