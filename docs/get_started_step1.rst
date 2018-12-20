:webchat_payload: /get_started_step1
.. _get_started_step1:

Step 1: Understand the Rasa Stack
=================================

.. raw:: html

   <div class="progress">
   <ul>
   <li class="current">1</li>
   <li><a href="../get_started_step2/">2</a></li>
   <li><a href="../get_started_step3/">3</a></li>
   <li><a href="../get_started_step4/">4</a></li>
   </ul>
   </div>

Don't feel like reading?

.. raw:: html

   <button
     class="button"
     onclick="WebChat.open()">
     Chat to Sara, the Rasa bot
   </button>
   <br>
   <br>

.. raw:: html

   <b>The Rasa Stack</b> is a set of open source machine learning tools for developers to create <a class="reference external" href="http://blog.rasa.com/level-3-contextual-assistants-beyond-answering-simple-questions/" target="_blank">contextual AI assistants and chatbots</a>:

* **Core** = a chatbot `framework` with machine learning-based dialogue management
* **NLU** = a `library` for natural language understanding with intent classification and entity extraction

NLU and Core are independent. You can use NLU without Core, and vice versa. We recommend using both.

**Lets start with an example.** Imagine you've built an AI assistant that sells renters insurance. At the end, you ask your user `Which email shall I send the confirmation to?` and they respond with `Please send the confirmation to amy@example.com`. Now it is time for the Rasa Stack to get to work:


.. image:: https://rasa.com/assets/img/rasa-ecosystem.png
   :width: 70%
   :alt: rasa stack

1. **NLU** understands the user's message based on your previous training data:

* **Intent classification**: Interpreting meaning based on predefined intents (Example: `Please send the confirmation to amy@example.com` is a ``provide_email`` intent with 93% confidence)
* **Entity extraction**: Recognizing structured data (Example: `amy@example.com` is an ``email``)

2. **Core** decides what happens next in this conversation. It's machine learning-based dialogue management predicts the **next best action** based on the input from NLU, the conversation history and your training data. (Example: Core has a confidence of 87% that ``ask_primary_change`` is the next best action to confirm with the user if they want to change their primary contact information.)

|

.. button::
   :link: ../get_started_step2/
   :text: Next Step: Try It Out

|


Looking for something specific? See what you can do with the Rasa Stack
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. tinycards::
   :title1: Turn Natural Language Into Structured Data
   :subtitle1: NLU Quickstart
   :link1: ../nlu/quickstart/
   :image_url1: ../_static/images/structured_data.png
   :title2: ML-based dialogue
   :subtitle2: Learn to handle context from real conversations
   :link2: ../core/quickstart/
   :image_url2: ../_static/images/learn_from_conversations.png
   :title3: Custom Word Vectors
   :subtitle3: Train custom word vectors for your domain
   :link3: ../nlu/master/choosing_pipeline/
   :image_url3: ../_static/images/custom_vectors.png

.. tinycards::
   :title1: Entity Extraction
   :subtitle1: Extract custom and built-in entities
   :link1: ../nlu/master/entities/
   :image_url1: ../_static/images/custom_entities.png
   :title2: Match Messages to Multiple Intents
   :subtitle2: multi-intents
   :link2: ../nlu/master/choosing_pipeline/
   :image_url2: ../_static/images/one_to_many.png
   :title3: Interactive Learning
   :subtitle3: Teach your bot new skills by talking to it.
   :link3: ../core/interactive_learning/
   :image_url3: ../_static/images/interactive_learning.png
