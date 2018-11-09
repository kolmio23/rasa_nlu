
:desc: Migrating from Microsoft LUIS to Rasa

.. _luis:

Rasa: An Open Source Alternative to Microsoft LUIS
==================================================

If you have an application built with Microsoft LUIS and made a decision to migrate it to a
free and fully customizable solution Rasa Stack, check out the guide below on how to migrate your application from
LUIS to Rasa.

Migration from LUIS consists of just a few simple steps. Here's how you do it:


Step 1: Export your Training Data from LUIS
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Go to your list of `LUIS applications <https://www.luis.ai/applications>`_ and click 
on the three dots menu next to the app you want to export.

.. image:: ../_static/images/luis_export.png
   :width: 240
   :alt: LUIS Export

Select 'Export App'. This will download a file with a ``.json`` extension that's ready for importing to Rasa.

Step 2: Train your Rasa NLU model
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Follow the instructions in the `NLU Quickstart <https://rasa.com/docs/nlu/quickstart/>`_, using your downloaded file as the training data.


Step 3: Modify your app to call your Rasa NLU Server
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Your existing application will have some code to make API requests to LUIS. 
Modify the API url to point to your Rasa NLU server. 
If you are testing this on your development machine, that will be at ``http://localhost:5000``
When you start the Rasa NLU server, you can also pass an ``emulate`` argument:

.. code-block:: bash

    python -m rasa_nlu.server -e luis

By adding this parameter, Rasa NLU's responses will be in the same format as LUIS provides,
so that you don't have to modify anything other than the URL in your API call.

Terminology:
^^^^^^^^^^^^

The words ``intent``, ``entity``, and ``utterance`` have the same meaning in Rasa as they do
in LUIS. 
LUIS's ``patterns`` feature is very similar to Rasa NLU's `regex features </docs/nlu/dataformat/>`_
LUIS's ``phrase lists`` feature does not currently have an equivalent in Rasa NLU.

If you have migrated your LUIS application to Rasa, join the `Rasa Community Forum <https://forum.rasa.com/>`_ and share your experience with us! 


