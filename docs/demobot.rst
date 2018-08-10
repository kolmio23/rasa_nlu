.. _demobot:

The Rasa Demo Bot
=================

Welcome to the Rasa Demo Bot! You can try it by clicking on the bubble in the
bottom right corner. We built this to show you an example of a bot built with
Rasa. Since our libraries are open source, we decided to make the code for this
bot public too. You can find the code for the bot `here <https://github.com/RasaHQ/rasa-demo>`_.
This bot showcases how to use:

- a combination of Rasa NLU + Rasa Core + Duckling
- webchat on a website

The current release is an alpha version, meaning for now it only has two user
goals and not a very large dataset. We strongly believe that to build a real
bot you need to learn from real data and so we decided to throw the bot out
there while it’s still not perfect. The more you chat with it, the better it
becomes. This doesn’t mean we’re using some fancy reinforcement learning
algorithms, but we’ll be looking at the conversations and improving the
bot based on them with the help of our `Rasa Platform <https://rasa.com/products/rasa-platform/>`_.
In the future we will be adding more user goals dependent on the kind of
requests we get from you.

Thanks for testing the bot! If you’d like to give us feedback or raise any
bugs/issues with it, feel free to do so in the `repo <https://github.com/RasaHQ/rasa-demo>`_.

.. raw:: html
    <div id="webchat">
    <script src="https://storage.googleapis.com/mrbot-cdn/webchat-latest.js"></script>
    <script>
     WebChat.default.init({
         selector: "#webchat",
         initPayload: "/greet",
         socketUrl: "https://website-demo.rasa.com/",
         title: "",
         subtitle: "",
         profileAvatar: "https://rasa.com/assets/img/demo/rasa_avatar.png",
         showCloseButton: true,
         fullScreenMode: false,})
    </script>
    </div>
