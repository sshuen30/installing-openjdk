## Installing java on macos (Using Homebrew)

- Check the current java version 
```bash
java -version
```
- Install homebrew if it is not installed
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
- Install java using homebrew
```bash
brew install openjdk@11
```
- Verify the installation path of java
```bash
brew info openjdk@11
```
- Set the JAVA_HOME environment variable to point to the installed JDK
```bash
# Edit ~/.zshrc file
sudo nano ~/.zshrc

# Insert the following line and save the file
export JAVA_HOME=/opt/homebrew/opt/openjdk@11

# Apply the changes
source ~/.zshrc
```
- Verify that Java is installed and the JAVA_HOME variable is set correctly by running
```bash
java -version
echo $JAVA_HOME
```


