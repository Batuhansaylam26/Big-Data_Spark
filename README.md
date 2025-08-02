# Install Scala on your computer

Firstly, The scala language is installed on the computer via following bash code block.</br>

```bash
curl -fL https://github.com/coursier/coursier/releases/latest/download/cs-x86_64-pc-linux.gz | gzip -d > cs && chmod +x cs && ./cs setup
```

After the installing, the computer is rebooted.</br>

Then check the scala.</br>

```bash
scala -version
```

Output:</br>
```bash
Scala code runner version: 1.8.4
Scala version (default): 3.7.2

```

After all, the scala and the compiler of scala can be launched via </br>

```bash
cs launch scala:3.7.2

cs launch scalac:3.7.2

```

# [Print "Hello World"](./hello.scala)

Firstly, the "Hello world" is printed on the screen.</br>
```bash
scala run hello.scala
```
Output:</br>
```bash
Starting compilation server
Compiling project (Scala 3.7.2, JVM (21))
Compiled project (Scala 3.7.2, JVM (21))
Hello, World!
```
