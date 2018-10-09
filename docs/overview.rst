
Start building great chatbots and assistants with the open source conversational AI framework
=============================================================================================

Get started with our four simple steps:

  .. image:: ../_static/images/icon_number1.png
     :width: 31
     :alt: Step number 1
     :class: icon-pull-left
     :target: #
**Understand the Rasa Stack**
    
  .. image:: ../_static/images/icon_number2.png
     :width: 31
     :alt: Step number 2
     :class: icon-pull-left
     :target: https://rasa.com/docs/core/quickstart/
`Try it out <https://rasa.com/docs/core/quickstart/>`_ (without installing anything!)

  .. image:: ../_static/images/icon_number3.png
     :width: 31
     :alt: Step number 3
     :class: icon-pull-left
     :target: https://rasa.com/docs/core/installation/   
`Install Rasa <https://rasa.com/docs/core/installation/>`_ on your machine

  .. image:: ../_static/images/icon_number4.png
     :width: 31
     :alt: Step number 4
     :class: icon-pull-left
     :target: https://forum.rasa.com/
`Join the community <https://forum.rasa.com/>`_ and start building

The Rasa Stack is a pair of open source libraries (Rasa NLU and Rasa Core) that allow
developers to expand chatbots and voice assistants beyond answering simple questions.
Using state-of-the-art machine learning, your bots can hold contextual conversations with
users. Rasa is production ready and used in large companies everywhere. 

Understanding The Rasa Stack
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

TL;DR: Rasa NLU's job is to interpret messages, and Rasa Core's job is to decide what should happen next.

.. image:: ../_static/images/rasa_stack_explained.png
   :width: 1382
   :alt: rasa stack

Rasa NLU performs `Natural Language Understanding`, which means taking free-form text like 

.. pull-quote:: `Please send the confirmation to amy@example.com`

and turning it into structured data. 
Rasa Core performs `Dialog Management`, which means keeping track of a conversation, and deciding
how to proceed. Both Rasa Core and NLU use Machine Learning to learn from real example conversations.

Rasa NLU and Core are independent. You can use NLU without Core, and vice versa.

Get Started with Rasa Core and NLU
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


I want a full bot framework
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. button::
    :text: Try Core + NLU
    :link: /docs/core/quickstart/


I just need NLU for now
~~~~~~~~~~~~~~~~~~~~~~~

.. button::
   :text: Try NLU
   :link: /docs/nlu/master/quickstart/


I want to migrate to Rasa from:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. button::
   :link: ../dialogflow/
   :text: Google Dialogflow


.. button::
   :link: ../luis/
   :text: Microsoft LUIS


What you can do with the Rasa Stack
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. tinycards::
   :title1: Turn Natural Language Into Structured Data
   :subtitle1: NLU Quickstart
   :link1: ../../nlu/master/quickstart/
   :image_url1: ../_static/images/structured_data.png
   :title2: ML-based dialogue
   :subtitle2: Learn to handle context from real conversations
   :link2: ../../core/quickstart/
   :image_url2: ../_static/images/learn_from_conversations.png
   :title3: Custom Word Vectors
   :subtitle3: Train custom word vectors for your domain
   :link3: ../../nlu/master/choosing_pipeline/
   :image_url3: ../_static/images/custom_vectors.png
   
.. tinycards::
   :title1: Entity Extraction
   :subtitle1: Extract custom and built-in entities
   :link1: ../../nlu/master/entities/
   :image_url1: ../_static/images/custom_entities.png
   :title2: Match Messages to Multiple Intents
   :subtitle2: multi-intents
   :link2: ../../nlu/master/choosing_pipeline/
   :image_url2: ../_static/images/one_to_many.png
   :title3: Interactive Learning
   :subtitle3: Teach your bot new skills by talking to it.
   :link3: ../../core/interactive_learning/
   :image_url3: ../_static/images/interactive_learning.png
   

Rasa Platform: Everything you need to run the Rasa Stack in the Enterprise.
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: /_static/images/rasa-platform-diagram.png
   :width: 800
   :alt: Rasa Platform

Rasa Platform extends the open source Rasa NLU and Rasa Core libraries with APIs,
a graphical user interface, and our customer success program which includes enterprise-grade support.

.. button::
   :text: Learn More about Rasa Platform
   :link: http://rasa.com/products/rasa-platform/

.. raw:: html
   :file: livechat.html
   