# How to decode, edit and compile back to jar file

1. To decode a jar we can use the following services / tools
- http://java-decompiler.github.io/
- http://www.javadecompilers.com

2. After modifiyng some java files we have to compile them to classes.
3. Sometimes .java files (restored from byte code) cannot be compiled because of incompatible types.
In that case we can try to use another decode method. Different methods might surprisengly work for different classes.
The remaining issues, if any, should be fixed manually.
You don't have to recompile not touched .java files, compile only modified one.
4. Extract jar files `jar xf some-jar.jar`
5. Replace modified classes
6. To create a jar with the same structute, run the following command:
```bash
jar cvf program.jar -C path/to/classes .
```
