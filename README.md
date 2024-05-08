# YewChat 💬

> Source code for [Let’s Build a Websocket Chat Project With Rust and Yew 0.19 🦀](https://fsjohnny.medium.com/lets-build-a-websockets-project-with-rust-and-yew-0-19-60720367399f)

## Install

1. Install the required toolchain dependencies:
   ```npm i```

2. Follow the YewChat post!

## Branches

This repository is divided to branches that correspond to the blog post sections:

* main - The starter code.
* routing - The code at the end of the Routing section.
* components-part1 - The code at the end of the Components-Phase 1 section.
* websockets - The code at the end of the Hello Websockets! section.
* components-part2 - The code at the end of the Components-Phase 2 section.
* websockets-part2 - The code at the end of the WebSockets-Phase 2 section.

## Experiment 3.1: Original code

![image](https://github.com/Sirered/adprog-tutorial10-Yewchat/assets/126568984/71a7c987-c2aa-4d49-8c04-1ed5173024cb)

## Experiment 3.2: Be Creative!

![image](https://github.com/Sirered/adprog-tutorial10-Yewchat/assets/126568984/3439f1ca-4b5f-4099-ab29-2bb556b0a65a)
![image](https://github.com/Sirered/adprog-tutorial10-Yewchat/assets/126568984/3a3b3433-6bbd-43d3-a615-55c5ed04247e)


Firstly, I fixed the avatar images, because the API interface that they used was outdated. The fix is just simply changing the avatar field to the correct API link. Afterwards I changed the background of the users list to be purple instead of gray, by just changing one of the classes used in the div associated to the user list from gray to purple. Lastly I made it so that the messages sent by a user show up as blue for them, but remains the normal format for everyone else. I did this by introducing a username field in the Chat struct (which each individual person logged in has) and in the view function, there is an if statement that checks if a message's from field (meaning who sent it) matches the current chat's username field, and the div is formatted differently according to that if statement.
