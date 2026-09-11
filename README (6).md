# Lab 2 - Compiling and Working with Java

**Author**: Justin Del Vecchio

**Edited by**: Jon Mrowczynski

This lab reinforces and/or introduces the following:

1. Compiling a Java program.
2. Looking at a compiler's output.
3. Looking at compiler options.
4. Using the `Math` library.
5. Using the Java API `math` package.

Perform the steps below and answer the questions as you go. Each question is worth 1 point unless stated otherwise.

## Part 1 (5pts.): Compiling a Java program | Looking at a compiler's output | Looking at compiler options

Perform the following steps to compile a Java program.

1. Login to a lab machine.
2. Open VS Code and its integrated terminal.
3. Create a Java source file named `Lab2.java`.
4. Add a main method to it.
5. Have this method print out **exactly** "Welcome to Lab 2!", with a newline, to the console. 
6. Compile the program with `javac`, ensuring it compiles successfully!
7. Run the compiled program using `java`.
    - You can run a compiled `.class` file, by executing the command `java NameOfClass`. Notice no `.class` extension!

You used the java compiler to compile the program. There are many compile options (or flags). You can see all these options by entering in: `javac --help`.

### Q1 (2pts.): Recompile the program you created using the `-verbose` flag. Copy and paste the resulting compilation output below, explain what the `-verbose` flag does, and the meaning of the output.

```
[[parsing started SimpleFileObject[/Users/tommyalleca/Desktop/lab2.java]]
[parsing completed 14ms]
[loading /modules/java.base/module-info.class]
[loading /modules/jdk.incubator.vector/module-info.class]
[loading /modules/jdk.httpserver/module-info.class]
[loading /modules/jdk.javadoc/module-info.class]
[loading /modules/jdk.jfr/module-info.class]
[loading /modules/jdk.graal.compiler/module-info.class]
[loading /modules/jdk.dynalink/module-info.class]
[loading /modules/java.naming/module-info.class]
[loading /modules/java.management.rmi/module-info.class]
[loading /modules/java.security.jgss/module-info.class]
[loading /modules/java.se/module-info.class]
[loading /modules/java.transaction.xa/module-info.class]
[loading /modules/java.datatransfer/module-info.class]
[loading /modules/jdk.security.jgss/module-info.class]
[loading /modules/jdk.jartool/module-info.class]
[loading /modules/jdk.attach/module-info.class]
[loading /modules/jdk.unsupported/module-info.class]
[loading /modules/jdk.crypto.cryptoki/module-info.class]
[loading /modules/jdk.jdwp.agent/module-info.class]
[loading /modules/java.compiler/module-info.class]
[loading /modules/java.instrument/module-info.class]
[loading /modules/jdk.compiler/module-info.class]
[loading /modules/jdk.hotspot.agent/module-info.class]
[loading /modules/jdk.jdi/module-info.class]
[loading /modules/jdk.jpackage/module-info.class]
[loading /modules/jdk.jsobject/module-info.class]
[loading /modules/jdk.xml.dom/module-info.class]
[loading /modules/java.smartcardio/module-info.class]
[loading /modules/jdk.naming.rmi/module-info.class]
[loading /modules/java.net.http/module-info.class]
[loading /modules/jdk.internal.vm.ci/module-info.class]
[loading /modules/jdk.management/module-info.class]
[loading /modules/jdk.internal.ed/module-info.class]
[loading /modules/jdk.localedata/module-info.class]
[loading /modules/jdk.charsets/module-info.class]
[loading /modules/jdk.management.jfr/module-info.class]
[loading /modules/java.scripting/module-info.class]
[loading /modules/jdk.crypto.ec/module-info.class]
[loading /modules/jdk.editpad/module-info.class]
[loading /modules/java.logging/module-info.class]
[loading /modules/jdk.nio.mapmode/module-info.class]
[loading /modules/jdk.unsupported.desktop/module-info.class]
[loading /modules/jdk.jdeps/module-info.class]
[loading /modules/java.sql.rowset/module-info.class]
[loading /modules/java.prefs/module-info.class]
[loading /modules/jdk.internal.md/module-info.class]
[loading /modules/jdk.jlink/module-info.class]
[loading /modules/jdk.jshell/module-info.class]
[loading /modules/jdk.security.auth/module-info.class]
[loading /modules/java.management/module-info.class]
[loading /modules/jdk.accessibility/module-info.class]
[loading /modules/java.xml.crypto/module-info.class]
[loading /modules/jdk.zipfs/module-info.class]
[loading /modules/jdk.internal.opt/module-info.class]
[loading /modules/java.security.sasl/module-info.class]
[loading /modules/jdk.sctp/module-info.class]
[loading /modules/java.xml/module-info.class]
[loading /modules/jdk.naming.dns/module-info.class]
[loading /modules/jdk.jcmd/module-info.class]
[loading /modules/jdk.graal.compiler.management/module-info.class]
[loading /modules/jdk.jstatd/module-info.class]
[loading /modules/java.rmi/module-info.class]
[loading /modules/jdk.internal.jvmstat/module-info.class]
[loading /modules/java.desktop/module-info.class]
[loading /modules/jdk.management.agent/module-info.class]
[loading /modules/jdk.internal.le/module-info.class]
[loading /modules/jdk.net/module-info.class]
[loading /modules/jdk.jconsole/module-info.class]
[loading /modules/java.sql/module-info.class]
[search path for source files: .]
[search path for class files: /Library/Java/JavaVirtualMachines/temurin-25.jdk/Contents/Home/lib/modules,.]
[loading /modules/java.base/java/lang/Object.class]
[loading /modules/java.base/java/lang/Deprecated.class]
[loading /modules/java.base/java/lang/annotation/Retention.class]
[loading /modules/java.base/java/lang/annotation/RetentionPolicy.class]
[loading /modules/java.base/java/lang/annotation/Target.class]
[loading /modules/java.base/java/lang/annotation/ElementType.class]
[checking Lab2]
[loading /modules/java.base/java/io/Serializable.class]
[loading /modules/java.base/java/lang/AutoCloseable.class]
[loading /modules/java.base/java/lang/IO.class]
[loading /modules/java.base/java/lang/String.class]
[wrote Lab2.class]
[total 136ms]]
[The verbose flag has the complier output a lot of detail about what is happening during the compilation. There was parsing going on and checking of types.]
```

### Q2: What is the name of the *type* of file generated by the `javac` compilation process?

[class file]

### Q3: Copy the *compiled* Java source file, rename it to some other valid file name, like `whatever.class`, and run it with the `java` command. Why does it not work?

[It doesn't work because the name java whatever doesn't match the lab2 name written inside the code. When the whatever.class file is opened lab2 is only there not java whatever causing a mismatch.]

## Part 2 (3pts.): Using the `Math` **Library**

Leave the existing code in the file and add the requested functionality to it:

1. Open the `Math` Java API page found
   [here](https://docs.oracle.com/en/java/javase/25/docs/api//java.base/java/lang/Math.html).
2. Call a function in the `Math` class that can help you calculate log(0). 
    - **Hint**: The `Math` class is called statically meaning that you do not have to instantiate an object.
3. Store the result in a variable.
4. Print out the variable to the console.
5. Run the program.
    - You could either use the process explained above, or...
    - You can directly run **single-source** Java files and skip the explicit compilation process using the command `java FileNameWithMainMethod.java`.

### Q4: What value does the program output for log(0)?

[-Infinity]

## Part 3 (9pts.): Using the Java API `math` **Package**.

Leave the existing code in the file and add the requested functionality to it:

1. Import the `math` package by adding this line to the top of your file:
```java
import java.math.*;
```
2. Create 2 separate integer variables and make both of their values 2,000,000,000.
3. Add these 2 numbers together and store them in a 3rd integer.
4. Print out the summed value.
5. Next, create 2 instances of the class `BigInteger` and make each instance have a value of 2,000,000,000.
6. Add these 2 `BigInteger`s together.
    - **Hint**: You need to do an object assignment here!
7. Print out their summed value.

### Q5 (2pts.): What is the value of the summed primitive `int`s? Explain why the value is either correct or incorrect.

[-294967296, Which is incorrect, this is the number because there's an overflow so the number goes into the negatives because it can't go that high.]

### Q6 (2pts.): What is the value for the summed `BigInteger` objects? Explain why the value is either correct or incorrect.

[4000000000, This is correct because unlike the primitive ints big Int can hold any whole number from small to big in it's memory, so it doesn't overflow when adding the big numbers and gives you a correct answer.]

There exists primitive types of `short`, `int`, `double`, and `long`. However, there is only a `BigInteger` type and no corresponding `BigShort` or `BigDouble` 
You can verify this by looking at the subsclasses of class `Number` listed [here](https://docs.oracle.com/en/java/javase/25/docs/api/java.base/java/lang/Number.html)

### Q7 (2pts.): Why is there no `BigShort` or `BigLong`?

[Because BigInteger can hold any whole number no matter how small or large it is, so creating a BigShort or BigLong would be redudant. To avoid not having to deal with overflow it's better to use BigInteger]

### Q8: Upload this file and your Java source code to the D2L dropbox.

[Perform steps on D2L]