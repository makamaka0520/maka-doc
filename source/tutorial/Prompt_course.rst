Prompt 教程
########################################

基础语法教程：
:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

完整的prompt由N个tag组成，tag之间以逗号分割，每个tag属于一种对于当前图像的描述

针对基础人物的生成完整的prompt包括

  - 【基础类】：性别，头发，衣服等基础内容

  - 【动态类】：朝向，肢体动作，表情

  - 【物件】：场景上存在的物件，人物上存在的配件

  - 【细致度】：描述上述所有内容的细致程度，如 细节的水 ， 精致的脸庞 等

  - 【特效】：用于描述场景上的效果，如 动态光，BLOOM，扩散，速度线 等


细致的描述会使得生成的图像更加接近需求。

.. code-block:: shell

    如：one girl, happy, long hair, red hair, suit, flowers

.. image:: img/text2img_pic8.png
   :align: center
   :width: 300

TAG强调功能：
:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

你可以通过一些特殊的语法强调你的某一些tag使得其在画面中更突出：

- ``{tag}``: 将tag的权重放大1.05倍
- ``(tag)``: 将tag的权重放大1.1倍
- ``[tag]``:将tag的权重缩小1.05倍

多组强调符号的叠加以相乘的形式体现

- ``{{tag}}``对应权重为1.05*1.05倍
- ``((tag))``对应权重为1.1*1.1倍
- ``[tag]``对应权重缩小1.05*1.05倍

你可以通过 tag:权重的形式指定固定权重

- {tag: 1.5}, [tag: 1.5], (tag: 1.5)，全部代表直接将该tag权重设置为1.5倍，在此语法下，添加更多的{},[],()无效；

每组tag需要单独强调，如

.. code-block:: shell

    one girl, happy, long hair, red hair, {suit}, {flowers}

错误示例：

.. code-block:: shell

    one girl, happy, long hair, red hair, {suit, flowers}

.. note::

    建议权重不要超过1.5，否则会影响整体画面观感。


我们来看一下效果吧：

.. code-block:: shell

    one girl, happy, long hair, red hair, suit, {flowers：1.5}

.. image:: img/text2img_pic9.png
   :align: center
   :width: 300
