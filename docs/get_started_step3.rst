.. _get_started_step3:

Step 3: Start Building
======================

Now it is time to build the first AI assistant yourself. If you have installed the Rasa Stack already in the step before, head to the Starterpack  - otherwise, follow the instructions here:





Install the Rasa Stack on your machine
--------------------------------------

The recommended way to install the Rasa Stack is using pip (make sure to install both libraries Core and NLU):

.. copyable::

    pip install -U rasa_core


.. raw:: html

     (Full instructions can be found <a class="reference external" href="https://rasa.com/docs/core/" target="_blank">in the Core Documentation</a>.)



.. copyable::

    pip install rasa_nlu[tensorflow]


.. raw:: html

     (Full instructions can be found <a class="reference external" href="https://rasa.com/docs/nlu/" target="_blank">in the NLU Documentation</a>.)



Unless you've already got numpy & scipy installed, we highly recommend
that you install and use `Anaconda <https://www.continuum.io\/downloads>`_.

Get the Starter Pack!
---------------------

We have prepared a starter pack which has all the files you need to build your first custom chatbot. On top of that, the starter-pack includes a training data set ready for you to use.

.. copyable::

    git clone https://github.com/RasaHQ/starter-pack-rasa-stack.git
    cd starter-pack-rasa-stack


.. raw:: html

     Now you've got everything you need to start building your first AI assistant. You can find detailed docs for Rasa NLU <a class="reference external" href="https://rasa.com/docs/nlu/" target="_blank">here</a> and for Rasa Core <a class="reference external" href="https://rasa.com/docs/core/" target="_blank">here</a>.

Learn more about how our community of makers from all over the world can help you.


.. button::
    :link: ../get_started_step4/
    :text: Next Step: Join Community
