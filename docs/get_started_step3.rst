.. _get_started_step3:

Step 3: Start Building
=============================================================================================

Now it is time to build the first AI assistant yourself. If you have installed the Rasa Stack already in the step before, head to the Starterpack  - otherwise, follow the instructions here:





Install the Rasa Stack on your machine
-----------------

The recommended way to install the Rasa Stack is using pip (make sure to install both libraries Core and NLU):

.. copyable::

    pip install -U rasa_core

(Full instructions can be found `in the Core documentation <https://rasa.com/docs/core/installation/>`_.)

.. copyable::

    pip install rasa_nlu[tensorflow]

(Full instructions can be found `in the NLU documentation <https://rasa.com/docs/nlu/installation/>`_.)


Unless you've already got numpy & scipy installed, we highly recommend
that you install and use `Anaconda <https://www.continuum.io\/downloads>`_.

Get the Starterpack!
-----------------

We have prepared a starter-pack which has all the files you need to build your first custom chatbot. On top of that, the starter-pack includes a training data set ready for you to use.

.. copyable::

    git clone https://github.com/RasaHQ/starter-pack-rasa-stack.git
    cd starter-pack-rasa-stack

Now you've got everything you need to start building your first AI assistant. Learn more about how our community of makers from all over the world can help you.


.. button::
    :link: ../get_started_step4/
    :text: Next Step: Join Community

