### Rest reqres API Performance Testing with Report
This project demonstrates performance testing using JMeter of tests for load testing of the API.
## Feature
- Load Testing
- Tests for GET, POST, PUT, DELETE requests
## Technology Used
- JMeter
## Perrequisite
- Java jdk
## Installation
1. Java jdk: [download and install java jdk.](https://www.oracle.com/apac/java/technologies/downloads/)
- To verify the version of Java which version is installed
- Go to cmd and write this command:
```Console
java -version
```
2. JMeter: [download and install JMeter.](https://jmeter.apache.org/download_jmeter.cgi)
- Unzip the folder to your computer.
- Go to the Bin folder inside your JMeter folder and launch the .bat file.
-After clicking the bat file, wait a few seconds JMeter UI will be shown.
```Console
Note: Make sure that you do not close the .exe file, as that will also close JMeter UI.
```
## JMeter from command line
### Why use the command line?
- GUI consumes memory, slowing down the process.
- Integrate with any external process CI and CD.
### How is the process?
1. Go to the JMeter bin folder.
2. Go to the folder address bar, write cmd then enter. You see the command window
3. Run the Command like below:
```Console
jmeter -n -t “location of your test file” -l “location of results file.jtl”
```
- -n == non gui mode
- -t == your test file
- -l == your location result
4. Create html report end of the test. Open cmd line, go to the JMeter bin folder go to cmd.
5. Run the command like below:
```Console
jmeter -g “location of results file.jtl” -o “location of results file.html”
```
### Test Setup
The performance tests were conducted using JMeter with different levels of concurrency. Each test executed a specified number of concurrent requests with a fixed loop count to evaluate the system's response time, throughput, and error rate.

The following tests were performed:
1. 10 Concurrent Requests with 1 Loop Count:
- Average Transactions Per Second (TPS) for Total Samples: ~1
- Total Concurrent API Requests: 50
2. 15 Concurrent Requests with 1 Loop Count:
- Average Transactions Per Second (TPS) for Total Samples: ~2
- Total Concurrent API Requests: 75
3. 20 Concurrent Requests with 1 Loop Count:
- Average Transactions Per Second (TPS) for Total Samples: ~3
- Total Concurrent API Requests: 100
The test execution with 20 concurrent requests resulted in an error rate of 10%.
## Test Result
1. 10 Concurrent Requests with 1 Loop Count:

<img width="1000" height="407" alt="Screenshot 2025-07-31 010122" src="https://github.com/user-attachments/assets/b4106d04-65d6-4da7-9eae-a97cd77f250f" />

2. 15 Concurrent Requests with 1 Loop Count:

<img width="1000" height="402" alt="Screenshot 2025-07-31 010339" src="https://github.com/user-attachments/assets/e26be73d-aafd-42b5-97d4-0ac47e3e0617" />

3. 20 Concurrent Requests with 1 Loop Count:

<img width="1000" height="406" alt="Screenshot 2025-07-31 010503" src="https://github.com/user-attachments/assets/966b1d37-184b-4f50-a5c9-841fde4f2655" />
<img width="1000" height="368" alt="Screenshot 2025-07-31 010524" src="https://github.com/user-attachments/assets/607e90b3-f877-4c6c-832f-b216991d714a" />

 
 




