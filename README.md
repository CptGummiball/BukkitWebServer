# BukkitWebServer
Java classes to add a internal webserver to your bukkit plugin

This repository provides two Java classes that can be used to seamlessly integrate an internal web server into a Bukkit/Spigot plugin. The classes, JettyServer and WebServerManager, enable easy deployment and management of a web server within the context of a Bukkit/Spigot plugin. It uses `slf4j logger` for console output.

## JettyServer.java
The JettyServer class allows you to start and stop the embedded Jetty web server.
**Don't forget to replace "path to webfiles" and "YourPluginName" in this file!**

## WebServerManager.java
The WebServerManager class simplifies the integration of the Jetty web server into a Bukkit/Spigot plugin.

## Usage
Starting the Jetty Server via WebServerManager
````
WebServerManager webServerManager = new WebServerManager(yourPluginInstance);
webServerManager.jettyStart();
````

Stopping the Jetty Server via WebServerManager
````
webServerManager.jettyStop();
````

Restarting the Jetty Server via WebServerManager
````
webServerManager.jettyRestart();
````

## Configuration
To configure the web server port, modify the webServerPort value in your plugin's configuration file.

**config.yml**
````
webServerPort: 8080
````

## Issues
If you encounter any issues or have suggestions, please [create a new issue](https://github.com/CptGummiball/BukkitWebServer/issues).

## License
This code is provided under the MIT License.

**Note:** Replace "YourPluginName" and other placeholders with your actual class names and details. This repository serves as a starting point for incorporating a Jetty web server into a Bukkit/Spigot plugin.