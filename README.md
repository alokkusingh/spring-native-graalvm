# Spring Native GraalVM

## Prerequisites for MacOS
### Install GraalVM Updater
Download from https://github.com/graalvm/graalvm-ce-builds/releases/download/vm-22.3.0/graalvm-ce-java17-darwin-amd64-22.3.0.tar.gz
````
tar -xvf tmpmd6img45tmpsypoxdi7.tar
````
````
sudo xattr -r -d com.apple.quarantine ~/opt/graalvm-ce-java17-22.3.0-amd/
````
````
export JAVA_HOME=~/opt/graalvm-ce-java17-22.3.0/Contents/Home
````
````
export PATH=$JAVA_HOME/bin:$PATH
````

### Performance

| Build       | Startup Time | Actuator Health API | Build Size | Memory |
|-------------|--------------|---------------------|------------|--------|
| GraalVM | ~637ms       | ~3ms                | ~21 MB     | 290 MB |
| Java | ~4.8s        | ~28ms               | ~72 MB     | 90 MB  |



