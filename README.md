# ndnSIM
A basic Query solution in Ubuntu18.04 ndnSIM 2.7 Installation process
When I followed the ndnsim website however I received syntax error after running ./waf command as follows:
Traceback (most recent call last):
  File "<string>", line 3, in <module>
  File "/usr/lib/python2.7/py_compile.py", line 117, in compile
     raise py_exc
  py_compile.PyCompileError:   File
  "/usr/local/lib/python2.7/dist-packages/visualizer/base.py", line 134
   print("Could not load plugin %r: %s" % (filename, str(ex)),
  file=sys.stderr)
SyntaxError: invalid syntax
  
  However when i did this, it got solved.
  you must edit basy.py in this path:
>/ndnsim/ns-3/src/visualizer/visualizer/
>open this file with gedit
>in line 134 and 139 edit this phrase  file=stderr to file(stderr)
>then execute ./waf
