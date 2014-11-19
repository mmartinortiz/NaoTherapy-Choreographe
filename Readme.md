# NaoTherapy

This repository complements to the [NaoTherapy Android app](https://github.com/mmartinortiz/NaoTherapy-Android). Here you will find 3 different directories that contains behaviours created for Choreographe, the [Nao Robot](http://www.aldebaran.com/en) software suite.

## Emotions

## Conversations

## ServerBox

The **ServerBox** is a Choreographe box for the Nao Robot that allow you to send messages to the robot within the same network. With this messages, some basic aspects of the robot can be controlled remotely, for example, stop/start different behaviours installed in the robot

ServerBox should usworks with a NaoQi version >= 1.44. The message are formed as JSON objects as sent to the server via socket. In [this](./ServerBox/docs/JSON.md) document you will find the message structure, tags and some examples

ServerBox opens a socket in the selected port. It receives JSON messages that decodes and interpret. The messages are received from the network where the robot is connected. In this version the messages are transmitted as plain text

You can install the ServerBox Behaviour in the robot and set as default behaviour. It does not require any robot resource (like motors), just the socket

# How to use the files

The different projects (Emotions, Conversations and ServerBox) have to been open with the Choreographe Suite. You can find download the suite from the [Aldebaran Website](http://www.aldebaran.com/en)

# Extending ServerBox

The box can be easily extended to accept other kind of messages or manipulate the robot behaviour according to different necessities. The ServerBox included in the Emotions behaviour has been modified, so take a look there to know the possibilities.
