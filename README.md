# ipythonscript_namespace

Simple scripts to test ipython_namespace

如果在IPython中执行main.py，在IPython shell中将访问不到任何结果以及main函数中定义的对象。

main2.py直接在该模块的全局命名空间中执行main中的代码，这样在IPython 中运行main2.py时，就能看到main中定义的所有变量。
