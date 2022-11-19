如何具象的去生成一个人物以及场景
########################################

.. note::
   
   此教程将教会大家一种能够有效出图的方法论，不代表只能通过此方法出图。



1.构建大体结构
=====================================

先在脑海中构建出一个大致的场景以及人物（比如下图的中表现的感觉）

.. image:: img/text2img_pic28.png
   :align: center
   :width: 300

此时，你脑海中应该能够想象出一个简单的描述词汇

- 一个女孩，蓝色头发，蓝色瞳孔，比基尼泳衣

.. code-block:: shell

    A girl, blue hair, blue pupils, bikini

都是比较简单的，我们先尝试生成下

.. image:: img/cgc_1.jpg
   :align: center
   :width: 300

将得到这样的一幅图片，此时还是十分简陋的，没关系，我们继续往上添加全新的词汇

2.添加细节描述
=====================================

整个结构我们已经成功构建完成，现在只需要在上面添加全新的修饰类词汇

- 面向镜头，漂亮的带细节的海水，气泡，椰树，海滩，动态光，漂浮的头发，阳光，飞溅，海浪，宝石般的眼睛，扩散，环绕


.. code-block:: shell

    Facing the camera, beautiful sea water with details, bubbles, coconuts, beaches, dynamic light, floating hair, sunlight, splash, waves, jewel like eyes, diffusion, surround

.. note::

    我们将在说明书中添加部分形容词给到用户选择，用户也可以使用我们提供的预设描述进行修改（施工中）

在添加描述词汇时，我们需要尽量的去想象你所构想的场景中所需要存在的内容

.. image:: img/cgc_2.jpg
   :align: center
   :width: 300

再次生成结果如上图

此时可以看到生成的图片已经能够大部分满足条件

3.修改细节描述
=====================================

例如，我想要为黄色长发，就可以修改描述词 ``blue hair`` 为 ``Long yellow hair``


.. code-block:: shell

   A girl, Long yellow hair, blue pupils, bikini,Facing the camera, beautiful sea water with details, bubbles, coconuts, beaches, dynamic light, floating hair, sunlight, splash, waves, jewel like eyes, diffusion, surround


.. image:: img/cgc_3.jpg
   :align: center
   :width: 300

如果不出意外的话，我们就将得到一张长发的少女图

同理，如果想要生成其他的内容，也可以进行添加或者修改

4.总结
=======================================================

在生成的过程中，不要去想象一蹴而就，遵循几点:

- 优先描述人物的大致样式（性别，头发，衣服等基础内容）

- 描述出人物的动态，包括朝向或者肢体动作

- 描述出场景上存在的物件（海水，椰子，贝壳，房屋等）

- 描述物件的细致程度，比如细节的水，真实的水，漂浮的头发等

- 重复 2-4 添加或者删除描述词汇

- 得到满意的图片
