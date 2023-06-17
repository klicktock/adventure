# Adventure
Text &amp; audio &amp; voice adventure system. This repository will contain both the engine and the modules.
This will be a cross between traditional parser based text adventures, hyper text "twine-like" interactive fiction and tabletop roleplaying games. 
Its ultimate goal is to allow a player to go on an adventure with only sound as input and output.

## Engine

The engine will be divided into two main parts:
1. Presentation Layer. Looking at a very modern presentation modelled on today's everyday messaging apps. Presentation layer will pass commands to the story engine, receive text (and optional audio and image data) and display them.  Presentation layer will be cross platform. Intial version will use Flutter & Dart.
2. Story Engine. First the story state is initialized from modules. Then text commands will be passed to the story engine's parser. The parser will then determine what the player is trying to do and then execute the commands, modify the story's state and respond to the presentation layer. Currently I am unsure of the best language/technology to operate this. This could be local or server side.

## Modules

Looking at a TOML based file format for story modules.
Modules will likely need to be compiled in some way in order to first generate AI "scratch" audio files before finalizing voice.
Modules can also contain images
