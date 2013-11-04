==============
Android gaming
==============

This is a sample project used to study "Google game services". It is based on Google sample_ games

.. _sample: https://github.com/playgameservices/android-samples

Build system
------------

This project uses the new Android build system (Gradle_). To build the project type:

.. code-block:: python

    gradle aR --no-daemon

or you can use Gradle wrapper present in this repository (`gradlew`).

.. _Gradle: http://tools.android.com/tech-docs/new-build-system/user-guide

Gradle daemon
-------------

To get better performance during build time, Gradle is executed in daemon mode. However when you
choose a release build type, you may want to execute gradle in foreground mode (ex: you may
require user input to gather apk signing passwords). In this case be sure to stop Gradle daemon as
follows:

.. code-block:: python

    gradle --stop
    gradle aR --no-daemon

What about my project ids?
--------------------------

Inside `res/values/ids.xml` you can configure all required ids for your application, achievements
and leaderboards. Go to your `Developer console`_ and create your app and OAuth2 client. Then
you can create achievements and leaderboards according to this program. You can find more info here_.

.. _Developer Console: https://play.google.com/apps/publish/
.. _here: https://developers.google.com/games/services/console/enabling#step_3_generate_an_oauth_20_client_id

The vision
----------

Make this project a valid playground for everyone who want to start developing Android games.
