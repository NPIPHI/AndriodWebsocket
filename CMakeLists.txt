cmake_minimum_required(VERSION 3.4.1)

project(AndriodWebsocket)

add_library(AndriodWebsocket STATIC
        src/Base64.h
        src/Frame.cpp src/Frame.h
        src/InputStream.cpp include/AndroidWebsocket/InputStream.h
        include/AndroidWebsocket/Message.h
        src/message_encoder.cpp src/message_encoder.h
        src/SafeQueue.h
        src/Sha1.h
        src/Socket.cpp include/AndroidWebsocket/Socket.h
        src/SocketServer.cpp src/SocketServer.h
        src/Websocket.cpp include/AndroidWebsocket/Websocket.h
        src/Websocket_server.cpp include/AndroidWebsocket/Websocket_server.h)

target_include_directories(AndriodWebsocket PUBLIC include)