### Rest reqres API Performance Testing with Report
This project demonstrates Performance testing using JMeter of tests to load testing of the API.
## Feature
- Load Testing
- Tests for GET, POST, PUT, DELETE requests
## Technology Used
- JMeter
## Perrequisite
- Java jdk
## Installation
1. Java jdk: [download and install java jdk.](https://www.oracle.com/apac/java/technologies/downloads/)
- To verify the version of java which version is installed
- Go to cmd and write this command:
```Console
java -version
```
2. JMeter: [download and install JMeter.](https://jmeter.apache.org/download_jmeter.cgi)
- Unzip the folder to your computer.
- Go to Bin folder inside your JMeter folder and launch the .bat file.
-After click bat file wait few seconds JMeter UI will be show.
```Console
Note: Make sure that you do not close the .exe file as that will also close JMeter UI.
```
## JMeter from command line
### Why use command line?
- GUI consumes memory, slower the process.
- Intergrate with any external process CI and CD.
### How is the process?
1. Go to JMeter bin folder.
2. Go to the folder address bar, write cmd then enter. You see command window
3. Run the Command like below:
```Console
jmeter -n -t “location of your test file” -l “location of results file.jtl”
```
- -n == non gui mode
- -t == your test file
- -l == your location result
4. Create html report end of the test. Open cmd line go to JMeter bin folder go to cmd.
5. Run the command like below:
```Console
jmeter -g “location of results file.jtl” -o “location of results file.html”
```

