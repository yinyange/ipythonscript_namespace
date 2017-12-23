# ipythonscript_namespace

Simple scripts to test ipython_namespace

如果在IPython中执行main.py，在IPython shell中将访问不到任何结果以及main函数中定义的对象。

main2.py直接在该模块的全局命名空间中执行main中的代码，这样在IPython 中运行main2.py时，就能看到main中定义的所有变量。如下：


    $ ipython

    In [1]: %run main.py

    In [2]: result
    ---------------------------------------------------------------------------
    NameError                                 Traceback (most recent call last)
    <ipython-input-2-a5b1e83cd027> in <module>()
    ----> 1 result

    NameError: name 'result' is not defined

    In [3]: %run main2.py

    In [4]: result
    Out[4]: 14

    In [5]: 
