# currentActiveClientsTask

display current active clients in real time.
"client" = running app (new tab, refresh) - for each "client" we generate fake ip.

# server
webapi with signalR - save clients to cache.

# client
angular - display active clients in real time with coonection to the hub server.

# How to run?
Server: 
install nuget packages and build the project.
roslyn - sometimes it fails to create roslyn in bin folder, just for fast fix please just copy the roslyn folder in the server folder to the bin folder after the build successed.

Client:
npm install
npm start
make sure to configure the server path in environment.ts - default is signalRServerEndPoint: "http://localhost:3344"

