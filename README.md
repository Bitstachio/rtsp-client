# RTSP Client

A Java-based RTSP (Real-Time Streaming Protocol) client application for streaming video from an RTSP server. This project was developed as part of the Computer Networks (EECS 3214) course at York University.

## Overview

This project implements a client for the RTSP protocol, enabling real-time video streaming over a network. The client establishes a TCP connection with an RTSP server for control messages and receives video data via UDP using the RTP (Real-Time Transport Protocol).

## Features

- Connect to RTSP servers using hostname/IP and port
- Setup and manage video streaming sessions
- Control video playback (setup, play, pause, teardown)
- Receive and display MJPEG video frames
- Graphical user interface for video playback control

## Architecture

The application consists of several key components:

- **UI Layer**: Swing-based graphical interface including the main window, video controls, and server selection dialog
- **Network Layer**: RTSP connection management over TCP and RTP data reception over UDP
- **Model Layer**: Session management and frame handling
- **Exception Handling**: Custom RTSP exception handling

## Usage

The client provides a simple interface to connect to an RTSP server, select a video file, and control playback. Video controls include:

- Setup: Initialize a video stream
- Play: Start video playback
- Pause: Pause the current stream
- Teardown: Close the video stream

## Requirements

- Java Runtime Environment (JRE)
- Network connectivity to an RTSP server

## Project Structure

```
RTSPClient/
└── src/
    └── ca/yorku/rtsp/client/
        ├── ui/           # User interface components
        ├── net/          # Network connection handling
        ├── model/        # Session and frame models
        └── exception/    # Custom exceptions
```

## Testing

Sample MJPEG video files (movie1.Mjpeg, movie2.Mjpeg, movie3.Mjpeg) are included for testing with the provided RTSPServer.jar.

## Authors

Original code by Jonatan Schroeder, updated March/October 2022.
