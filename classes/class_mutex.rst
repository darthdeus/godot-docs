.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Mutex.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Mutex:

Mutex
=====

**Inherits:** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

A synchronization Mutex.

Methods
-------

+---------------------------------------+----------------------------------------------------------+
| void                                  | :ref:`lock<class_Mutex_method_lock>` **(** **)**         |
+---------------------------------------+----------------------------------------------------------+
| :ref:`Error<enum_@GlobalScope_Error>` | :ref:`try_lock<class_Mutex_method_try_lock>` **(** **)** |
+---------------------------------------+----------------------------------------------------------+
| void                                  | :ref:`unlock<class_Mutex_method_unlock>` **(** **)**     |
+---------------------------------------+----------------------------------------------------------+

Description
-----------

A synchronization Mutex. Element used to synchronize multiple :ref:`Thread<class_Thread>`\ s. Basically a binary :ref:`Semaphore<class_Semaphore>`. Guarantees that only one thread can ever acquire this lock at a time. Can be used to protect a critical section. Be careful to avoid deadlocks.

Method Descriptions
-------------------

.. _class_Mutex_method_lock:

- void **lock** **(** **)**

Lock this ``Mutex``, blocks until it is unlocked by the current owner.

.. _class_Mutex_method_try_lock:

- :ref:`Error<enum_@GlobalScope_Error>` **try_lock** **(** **)**

Try locking this ``Mutex``, does not block. Returns ``OK`` on success, ``ERR_BUSY`` otherwise.

.. _class_Mutex_method_unlock:

- void **unlock** **(** **)**

Unlock this ``Mutex``, leaving it to other threads.

