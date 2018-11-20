## What is ASP.NET SignalR
ASP.NET SignalR is a new library for ASP.NET developers that makes it incredibly simple to add real-time web functionality to your applications. What is "real-time web" functionality? It's the ability to have your server-side code push content to the connected clients as it happens, in real-time.

You may have heard of WebSockets, a new HTML5 API that enables bi-directional communication between the browser and server. SignalR will use WebSockets under the covers when it's available, and gracefully fallback to other techniques and technologies when it isn't, while your application code stays the same.

SignalR also provides a very simple, high-level API for doing server to client RPC (call JavaScript functions in your clients' browsers from server-side .NET code) in your ASP.NET application, as well as adding useful hooks for connection management, e.g. connect/disconnect events, grouping connections, authorization. 

## What can you do with ASP.NET SignalR?
SignalR can be used to add any sort of "real-time" web functionality to your ASP.NET application. While chat is often used as an example, you can do a whole lot more. Any time a user refreshes a web page to see new data, or the page implements Ajax long polling to retrieve new data, is candidate for using SignalR.

It also enables completely new types of applications, that require high frequency updates from the server, e.g. real-time gaming. For a great example of this see the [ShootR game](http://shootr.signalr.net/)


## Documentation
See the [documentation](https://github.com/SignalR/SignalR/wiki)

## Get it on NuGet!

    Install-Package Microsoft.AspNet.SignalR -pre

## Get a sample on NuGet, straight into your app!

    Install-Package Microsoft.AspNet.SignalR.Sample
	
## LICENSE
[Apache 2.0 License](https://github.com/SignalR/SignalR/blob/master/LICENSE.md)

## Building the source

### Windows
After cloning the repository, run `build.cmd`.

### Mono
After cloning the repository, run `make`.

**NOTE:** Run `make tests` to run the unit tests. After running them it'll probably hang. If it does hang
use `Ctrl+C` to break out (We're still working on this).

Open Microsoft.AspNet.SignalR.Mono.sln to do development.

## Continuous Integration

We have a CI Server (http://ci.signalr.net/)

## Questions?
The SignalR team hangs out in the [signalr](http://jabbr.net/#/rooms/signalr) room at on [JabbR](http://jabbr.net/).