Features
Customer registration, login (no duplicate login, duplicate registration, both have verification and error prompts)
Online user list query (you can see who is online in the current system, except yourself)
Group chat message (send a message, of course everyone online can receive it, except yourself)
Private chat message (you can chat privately with someone, if this person does not exist or is not online, there will also be corresponding prompts)
Exit system / log out (after logging out, the online list of other people will be updated, and then you can’t see me when you check the online list again)
To be continued…

Notes
After downloading the source code, please modify the redis connection information in redis.go. That is host:port, remember to change it to your own.

Remember to install go-redis first. I installed it through go mod here, which is to enter the GOPATH directory and execute the following command

go get github.com/go-redis/redis/v8
Remember to put the folder in your GOPATH/src path. The project can be opened by goland. Goland can run directly, so it’s very convenient.

A better way is to compile the client and server code separately, and then get the executable file. You can open the cmd window and run it. At this time, you can start multiple clients.

Enter GOPATH/src and execute separately
go build -o server.exe .\tcpchat\server\main\
go build -o client.exe .\tcpchat\client\main\

It is still recommended to learn some basic usage of go-redis and json format.
