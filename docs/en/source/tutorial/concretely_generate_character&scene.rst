How to flesh out a character or a scene by Makamaka？
####################################################

.. note::
   
   This tutorial will teach you a methodology that can effectively plot, which does not mean that you can only plot by this method.



1.Constructing the general structure
=====================================

Firstly，you should build a rough scene and characters in your mind (like the style in the picture below).

.. image:: img/text2img_pic28.png
   :align: center
   :width: 300

At this point, you should be able to imagine a simple descriptive word in your mind

- A girl, blue hair, blue pupils, bikini swimming costume

.. code-block:: shell

    A girl, blue hair, blue pupils, bikini

It's all relatively simple, let's try to generate it first

.. image:: img/cgc_1.jpg
   :align: center
   :width: 300

We'll get a picture like this, which is still very rudimentary at this point, so it's okay, let's go ahead and add a whole new vocabulary.

2.Adding detailed descriptions
=====================================

The whole structure has been successfully built, now we just need to add a whole new vocabulary of retouching classes to it.

We have several steps for it:

   1.What do you associate with the presence of the sea? Sea water, coconut trees, beach, sun, splash, bubbles, waves

   2.Add an adjective to the base, such as dynamic light, floating hair, jewel-like eyes, diffuse, surround

   3.Add a dynamic to this subject, facing the camera

Finally we will get:

- Facing the camera, beautiful water with details, bubbles, coconut trees, beach, dynamic light, floating hair, sunlight, splash, waves, jewel-like eyes, spread, surround


.. code-block:: shell

    Facing the camera, beautiful sea water with details, bubbles, coconuts, beaches, dynamic light, floating hair, sunlight, splash, waves, jewel like eyes, diffusion, surround

.. note::

    We will add some of the adjectives to the instructions for the user to choose from, or you can modify them using the preset descriptions we provide (under construction)

When adding descriptive words, we need to try to imagine what needs to be present in the scenario you have in mind

.. image:: img/cgc_2.jpg
   :align: center
   :width: 300

The results are again generated as shown above.

At this point, you can see that the generated image has mostly met the conditions.

3.Modifying the description of the details
=================================================

For example, if you want to have an image with long yellow hair，you could switch  to a new descriptive term **Long yellow hair** from **blue hair**.


.. code-block:: shell

   A girl, Long yellow hair, blue pupils, bikini,Facing the camera, beautiful sea water with details, bubbles, coconuts, beaches, dynamic light, floating hair, sunlight, splash, waves, jewel like eyes, diffusion, surround


.. image:: img/cgc_3.jpg
   :align: center
   :width: 300

If nothing else, we will have a picture of a girl with long hair.

Similarly, if you want to generate other content, you can add or modify it.

4.Summary
=======================================================

In the process of generation, don't  imagine an overnight success, try to follow steps below:

- give priority to describing the general appearance of the character (gender, hair, clothes, etc.)

- describe the dynamics of the character, including orientation or body movements

- describe the objects present on the scene (seawater, coconuts, shells, houses, etc.)

- describe the level of detail of the objects, e.g. detailed water, real water, floating hair, etc.

- repeat 2-4 to add or remove descriptive words

- get a satisfactory picture
