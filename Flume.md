# Flume
* Flume agents can run on multiple servers in the enterprise, and they can communicate with each other over the network to move data. 
* Used to import straming data (server logs, tweets, and so on)
* Only a transport agent
* Buffered 

## Configuration of Flume
Flume agent configuration is specified using a text file, similar to the Java.properties format. When you create the configuration file for a Flume agent, you must configure
* Interceptor
* Sink
* Channel. Possible Flume channels include
  - The implementation of your own channel
  - File Storage
  - Database Storage
  - In Memory
* Source
