.. _thread_wiper:

====
扫线
====

扫线有两种不同的动作模式：

- 设置 `A 08`_ 为1，可以选择启用扫面线功能：

当剪线流程结束后，延迟 `T 03`_ 所设置的时间，扫线电磁铁（阀）接通，之后经过 `T 04`_ 设置的时间
后，扫线关闭。

- 设置 `A 08`_ 为2，可以选择启用扫底线功能：

当剪线流程结束后，首次抬压脚时被触发，扫线电磁铁（阀）接通，之后经过 `T 04`_ 设置的时间后，扫线
关闭。

参数列表
========

A 08
----

.. dropdown:: 扫线 <...>
   :animate: fade-in-slide-down
   
   -Max  1
   -Min  0
   -Unit  --
   -Description
     | 扫线功能开关：
     | 0 = 关闭；
     | 1 = 扫面线；
     | 2 = 扫底线。
     
T 03
----

.. dropdown:: 扫线等待时间 <...>
   :animate: fade-in-slide-down
   
   -Max  200
   -Min  1
   -Unit  毫秒
   -Description  剪线后延迟一定时间后扫线动作。

T 04
----

.. dropdown:: 扫线动作时间 <...>
   :animate: fade-in-slide-down
   
   -Max  200
   -Min  1
   -Unit  毫秒
   -Description  扫线电磁铁通电持续时间。
