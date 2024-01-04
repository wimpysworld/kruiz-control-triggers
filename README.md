# Kruiz Control Triggers

I use the excellent [Kruiz Control](https://github.com/Kruiser8/Kruiz-Control) to automate OBS Studio during my live streams and to create a Twitch chatbot.

> *Kruiz Control enables a pseudo code approach to manage and automatically handle Twitch Channel Points, Twitch Chat, OBS or SLOBS, and StreamElements or Streamlabs alerts.*

This repository contains the triggers I use for my live stream.
I have split them into two repositories, one for my Twitch channel points triggers and automation, and one for my Twitch chatbot.
They are published here for anyone to learn from, *but they are not intended to be plug-and-play*.

## KC-WimpysWorld

Integration with Twitch channel point triggers and assorted automation for OBS Studio.
This is a chatbot and also uses the Twitch API and StreamElements API.
A slightly *"patched"* version of [`index-wimpy.html`](KC-WimpysWorld/index-wimpy.html) is used to prevent VoiceMod (Windows only) from attempting to load.

## KC-BellaBotty

My Twitch chatbot, Bella. **Bella is just a **chatbot, **with **no**** Twitch API** integrations.**
As a result, a slightly *"patched"* version of [`index-bella.html`](KC-BellaBotty/index-bella.html) is used to prevent VoiceMod (Windows only) from attempting to load and also disables Twitch API integration to allow KC-BellaBotty to coexist alongside KC-WimpysWorld without causing "Invalid authorization code" errors.

### DecAPI

I use [DecAPI](https://decapi.me/) to get the data from the Twitch API and have implemented a DecAPI client using Kruiz Control.

- [dec-api.txt](KC-BellaBotty/triggers/dec-api.txt)
