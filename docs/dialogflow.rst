:desc: Migrating from Google Dialogflow to Rasa

.. _dialogflow:

Rasa: An Open Source alternative to Google Dialogflow
=====================================================

Welcome to the wonderful world of open source! 
Congratulations on embracing a free and fully customizable solution. 
We've got the steps to migrate from LUIS here, or from LUIS :ref:`here <luis>`. 

`Join our community <https://forum.rasa.com/>`_ and be part of something really big! 

You can use Rasa NLU as an open source drop-in replacement for Google Dialogflow.

Migration from Dialogflow to Rasa is quick and easy.
Simply load the training data into Rasa and you're all set. Here's how you do it:


Step 1: Export your data from Dialogflow
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Navigate to your agent's settings by clicking the gear icon.

.. image:: ../_static/images/dialogflow_export.png
   :width: 240
   :alt: Dialogflow Export

Click on the 'Export and Import' tab and click on the 'Export as ZIP' button.

.. image:: ../_static/images/dialogflow_export_2.png
   :width: 675
   :alt: Dialogflow Export 2


This will download a file with a ``.zip`` extension. Unzip this file to create a folder.

Step 2: Train your Rasa NLU model
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Follow the instructions in the `NLU Quickstart <https://rasa.com/docs/nlu/quickstart/>`_, using your downloaded folder as the training data.

If your unzipped folder is called ``testagent``, the command would be:

.. code-block:: bash

    python -m rasa_nlu.train -c config.yml -d testagent


Step 3: Modify your app to call your Rasa NLU Server
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Your existing application will have some code to make API requests to Dialogflow. 
Modify the API url to point to your Rasa NLU server. 
If you are testing this on your development machine, that will be at ``http://localhost:5000``
When you start the Rasa NLU server, you can also pass an ``emulate`` argument:

.. code-block:: bash

    python -m rasa_nlu.server -e dialogflow

By adding this parameter, Rasa NLU's responses will be in the same format as Dialogflow provides,
so that you don't have to modify anything other than the URL in your API call.

Terminology:
^^^^^^^^^^^^


The words ``intent``, ``entity``, and ``utterance`` have the same meaning in Rasa as they do in Dialogflow.
In Dialogflow, there is a concept called ``Fulfillment``. In Rasa we call this a `Custom Action </docs/core/customactions/>`_.

Dialogflow also has a Small Talk module. One of our awesome contributors has made a Rasa compatible version of this `here <https://github.com/rahul051296/small-talk-rasa-stack>`_.


.. raw:: html
   :file: livechat.html