# Circuit Tracks Buddy
A simple Web MIDI app that runs as a sidecar display to your Circuit Tracks and shows the current synth patch names and categories.

Plug your phone/laptop into the CT's USB port, open this link in Chrome and you now have a little sidecar display that at least gives you some idea of what you're playing and what to look for next time.  It's not going to set the world on fire, but it helps me orientate myself around the synth preset pages and know what the name of 'that patch' is when I come across something I like.

Enjoy

![Circuit Tracks Buddy serving suggestion](http://github.com/g7uhn/circuit-tracks-buddy/CT_Buddy_serving_suggestion.png)

### Some techie details... :-)
I don't actually know much about web coding or anything to do with software really so this is me:
- understanding the form of the sysex patch dump messages described in the Circuit Tracks Programmer's Guide
- hacking together some javascript from a few Web MIDI examples around the web
- upon start and upon any subsequent Program Change message (occurs when you change patches) sending the patch dump command and reading the name and category out of the received patch dump message
- using Digital Ocean's app service to monitor this GitHub repo, detect the javascript and run it as a web app with a link, available to all...
