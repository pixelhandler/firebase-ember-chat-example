# EmberFire Chat Example

### Server

Start Server using command on console: `node ember-chat/server.js`, kill w/ CMD-C

Requires use of connect, setup w/ `npm install connect` in node_modules

## Node box

* [IDE](https://www.nitrous.io/app#/boxes/50277/ide)
* [Preview URL](http://firebase-chat-50277.usw1.actionbox.io:3000/)
  * (need to execute start server using console, runs on port 3000)
* SSH URI: ssh://action@usw1.actionbox.io:13392

If you haven’t already signed up w/ Nitrous.io, [referal link](https://www.nitrous.io/join/CoqXOGmFWfw)

## Links

* [Ember Chat example](https://github.com/andrewmp1/emberFire/tree/gh-pages/examples/chat)
* [Ember Fire](https://github.com/firebase/emberFire)

Ideas for extending the chat example:

* [Authenticating with Persona](https://www.firebase.com/docs/security/simple-login-persona.html)
  * [persona.org](https://login.persona.org/)
* [EmberJS Gauge](http://front-back.com/an-ember-js-gauge-component)
* [Leaderboard Example](https://www.firebase.com/tutorial/#session/o3zmxe1kde2)
  * [data](https://o3zmxe1kde2.firebaseio-demo.com/) 

## Firebase data

* [Collection](https://pixelhandler.firebaseio.com/chats/)

Export:

    {
      "chats" : {
        "_type" : "array",
        "0" : {
          "from" : "Guest01",
          "msg" : "Chirp."
        }
      }
    }

Security:

    {
      "rules": {
        ".read": true,
        ".write":false,
        "chats":{
          ".read": true,
          ".write": true
        }
      }
    }
