# Burp-Suite-
Burp-Suite Professional v1.7.37 Cracked

## Download the Burp-Suite Professional Jar File: 
[Link] (https://portswigger.net/burp/releases/professional-1-7-37)

## Steps to Install JDK 8u202 on Linux and Configure Environment Variables

1. **Download JDK 8u202:**
   - Download JDK 8u202 from Oracle's website using the provided link:
     ```
     [JDK 8u202 Download Link]
     (https://mirrors.huaweicloud.com/java/jdk/8u202-b08/jdk-8u202-linux-x64.tar.gz)
   
     ```

2. **Extract JDK Archive:**
   - Open a terminal and run the following command to extract the downloaded JDK archive:
     ```bash
     tar -xvf ~/Downloads/jdk-8u202-linux-x64.tar.gz
     ```

3. **Move JDK Directory:**
   - Move the extracted JDK folder to `/usr/lib/jvm/jdk1.8.0_202`:
     ```bash
     sudo mkdir -p /usr/lib/jvm/jdk1.8.0_202
     sudo mv jdk1.8.0_202/* /usr/lib/jvm/jdk1.8.0_202/
     ```

4. **Set Alternatives:**
   - Set alternatives for `java`, `javac`, and `javaws` commands to point to the newly installed JDK:
     ```bash
     sudo update-alternatives --install "/usr/bin/java" "java" "/usr/lib/jvm/jdk1.8.0_202/bin/java" 1
     sudo update-alternatives --install "/usr/bin/javac" "javac" "/usr/lib/jvm/jdk1.8.0_202/bin/javac" 1
     sudo update-alternatives --install "/usr/bin/javaws" "javaws" "/usr/lib/jvm/jdk1.8.0_202/bin/javaws" 1
     ```

5. **Update Environment Variables:**
   - Edit `/etc/profile` to add JDK environment variables. Use a text editor (e.g., `sudo nano /etc/profile`) to add the following lines at the end:
     ```bash
     JAVA_HOME=/usr/lib/jvm/jdk1.8.0_202
     PATH=$PATH:$HOME/bin:$JAVA_HOME/bin
     export JAVA_HOME
     export PATH
     ```

6. **Reload Environment Variables:**
   - Reload the updated `/etc/profile` file to apply the changes:
     ```bash
     source /etc/profile
     ```

## Running Burp Suite with Custom Classpath

Replace the placeholders (`/path/to/burp-loader-keygen.jar` and `/path/to/burpsuite.jar`) with the actual paths to your keygen and Burp Suite JAR files:

```bash
java -Xbootclasspath/p:/path/to/burp-loader-keygen.jar -jar /path/to/burpsuite.jar
