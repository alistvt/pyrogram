Welcome to Pyrogram
===================

.. raw:: html

    <div align="center">
        <a href="https://docs.pyrogram.ml">
            <div><img src="_static/logo.png" alt="Pyrogram Logo"></div>
        </a>
    </div>

    <p align="center">
        <b>Telegram MTProto API Framework for Python</b>

        <br>
        <a href="https://github.com/pyrogram/pyrogram">
            GitHub
        </a>
        •
        <a href="https://t.me/PyrogramChat">
            Community
        </a>

        •
        <a href="https://github.com/pyrogram/pyrogram/releases">
            Releases
        </a>
        •
        <a href="https://pypi.org/project/Pyrogram">
            PyPI
        </a>
        <br>
        <a href="compiler/api/source/main_api.tl">
            <img src="https://img.shields.io/badge/schema-layer%2097-eda738.svg?longCache=true&colorA=262b30"
                alt="Schema Layer">
        </a>
        <a href="https://github.com/pyrogram/tgcrypto">
            <img src="https://img.shields.io/badge/tgcrypto-v1.1.1-eda738.svg?longCache=true&colorA=262b30"
                alt="TgCrypto Version">
        </a>
    </p>

.. code-block:: python

    from pyrogram import Client, Filters

    app = Client("my_account")


    @app.on_message(Filters.private)
    def hello(client, message):
        message.reply("Hello {}".format(message.from_user.first_name))


    app.run()

**Pyrogram** is an elegant, easy-to-use Telegram_ client library and framework written from the ground up in Python and
C. It enables you to easily create custom apps for both user and bot identities (bot API alternative) via the
`MTProto API`_.

.. _Telegram: https://telegram.org
.. _MTProto API: https://core.telegram.org/api#telegram-api

How the Documentation is Organized
----------------------------------

Contents are organized into self-contained topics and can be all accessed from the sidebar, or by following them in
order using the Next button at the end of each page. Here below you can, instead, find a list of the most relevant
pages.

Getting Started
^^^^^^^^^^^^^^^

- `Quick Start`_ - Overview to get you started as fast as possible.
- `Calling Methods`_ - How to use Pyrogram's API.
- `Handling Updates`_ - How to handle Telegram updates.
- `Error Handling`_ - How to handle API errors correctly.

.. _Quick Start: intro/start
.. _Calling Methods: start/invoking
.. _Handling Updates: start/updates
.. _Error Handling: start/errors

API Reference
^^^^^^^^^^^^^
- `Client Class`_ - Details about the Client class.
- `Available Methods`_ - A list of available high-level methods.
- `Available Types`_ - A list of available high-level types.

.. _Client Class: api/client
.. _Available Methods: api/methods
.. _Available Types: api/types

Topics
^^^^^^

- `Smart Plugins`_ - How to modularize your application.
- `Advanced Usage`_ - How to use Telegram's raw API.
- `Release Notes`_ - Release notes for Pyrogram releases.
- `Pyrogram FAQ`_ - Answers to common Pyrogram questions.

.. _Smart Plugins: topics/smart-plugins
.. _Advanced Usage: topics/advanced-usage
.. _Release Notes: topics/releases
.. _Pyrogram FAQ: topics/faq

.. toctree::
    :hidden:
    :caption: Introduction

    intro/start
    intro/install
    intro/setup

.. toctree::
    :hidden:
    :caption: Getting Started

    intro/auth
    start/invoking
    start/updates
    start/errors

.. toctree::
    :hidden:
    :caption: API Reference

    api/client
    api/methods
    api/types
    api/handlers
    api/decorators
    api/filters
    api/errors

.. toctree::
    :hidden:
    :caption: Topic Guides

    topics/filters
    topics/more-on-updates
    topics/config-file
    topics/smart-plugins
    topics/auto-auth
    topics/session-settings
    topics/tgcrypto
    topics/text-formatting
    topics/proxy
    topics/bots-interaction
    topics/test-servers
    topics/advanced-usage
    topics/voice-calls
    topics/releases
    topics/faq

.. toctree::
    :hidden:
    :caption: Telegram API

    telegram/functions/index
    telegram/types/index