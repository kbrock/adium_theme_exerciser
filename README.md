# Adium Theme Exerciser

There are some great chat themes out there designed for Adium.

This project focuses on giving the developer the ability to exercise these themes

## Overview

A chat system is cut up into a few components:

1. Receive user input and translate into events
2. Send user's events to the chat server
    + send chat server request for information like users in a channel
    + send chat server a message to a channel or another user
3. Receive events from the chat server
    + receive chat message from a user
    + receive a list of users in a channel
    + receive a list of channels
4. Display chat server events to the user
    + display user chat message in a channel
    + display list of users in a channel
    + display list of channels. (allowing someone to join - see step 1)

## Focus of this project

This project focuses on letting the developer mimic the events received in 3 and leveraging Adium Message Styles to display them in a browser.

## More information about Adium

Message Styles have a good [reference][Message Styles Reference] and [tutorial][Message Styles Tutorial]. Contact List Styles also have There are some great reference articles about [Message Styles][] and [Contact List Styles][] [adium files][]. [tutorial 1]


[Message Styles Tutorial 1]: https://trac.adium.im/wiki/CreatingMessageStyles/SandBox/Tutorial1/
[Message Styles Reference]: https://trac.adium.im/wiki/CreatingMessageStyles
[Message Styles Tutorial]: https://trac.adium.im/wiki/CreatingMessageStyles/Tutorial

[Contact List Styles]: 
[adium files]: https://adium.im/help/pgs/Miscellaneous-LocationsAdiumFiles.html

## Events

The event system in irc is currently string based, but they are striving to make it more json centric.

The event system in adiumis can be sumarized by the [Template][] file, other projects are Psi are leveraging this template file and driving it using [javascript][psi-driver]

[Template]: https://github.com/adium/adium/blob/master/Plugins/WebKit%20Message%20View/Template.html
[psi-driver]: https://github.com/psi-im/psi/blob/master/themes/chatview/adium/adapter.js


## Disclaimer

I am not affiliate with Adium, and I have not dived into their code.
This is based upon the information I have read from the theme creation articles on Adium Xtras.

[Adium Xtras]: http://www.adiumxtras.com/
