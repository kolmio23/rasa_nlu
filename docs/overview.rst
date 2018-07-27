
Start building great chatbots and assistants with the open source conversational AI framework
=============================================================================================

1. **Understand the Rasa Stack**
2. Try it out (without installing anything!)
3. Install on your machine
4. Join the community and start building

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

.. smallcards::
   :title1: Try Core + NLU
   :link1: /docs/core/quickstart/
   :description1: I want a full bot framework
   :title2: Try NLU
   :link2: /docs/nlu/quickstart/
   :description2: I just need NLU for now


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
   :title1: NLU Quickstart
   :subtitle1: Turn Natural Language Into Structured Data
   :link1: ../../nlu/quickstart/
   :image_url1: ../_static/images/rasa-stack-extract-entities.png
   :title2: Match Messages to Multiple Intents
   :subtitle2: multi-intents
   :link2: ../../nlu/choosing_pipeline/
   :image_url2: ../_static/images/multi_intent.png
   :title3: Custom Word Vectors
   :subtitle3: choosing a pipeline
   :link3: ../..//nlu/choosing_pipeline/
   :image_url3: ../_static/images/word_vectors.png
   
.. tinycards::
   :title1: Entity Extraction
   :subtitle1: Extract custom and built-in entities
   :link1: ../../nlu/entities/
   :image_url1: ../_static/images/rasa-stack-extract-entities.png
   :title2: ML-based dialogue
   :subtitle2: Learn to handle context from real dialogues
   :link2: ../../core/quickstart/
   :image_url2: ../_static/images/state_machine.png
   :title3: Interactive Learning
   :subtitle3: Teach your bot new skills by talking to it.
   :link3: ../../core/interactive_learning/
   :image_url3: ../_static/images/interactive_learning.png
   

