Eventbrite Event Change Notifier
======================
Notifies you when an orgnizer of the event made any modifications to the event and notifies you through SMS

The API uses ```modified``` attribute in the Eventbrite API

The script is written in [node.js](http://nodejs.org/)

## Install
```npm install```
## API Keys
Fill in ```apiconfig.sample.js``` and rename it to ```apiconfig.js```. You will need twilio and eventbrite API keys. Notice the interval is set to check every 2 mins. Eventbrite API has limit of 1k request/day.

## Run
```node app.js```

It is meant to be run in the background, so a better way maybe
```screen -dmS "Eventbrite Monitor" node app.js```

The notification you got will be like this:

![sampleSMS](https://raw.github.com/paulshi/EventbriteEventChangeNotifier/master/smsSample.png)

## License

The MIT License (MIT)

Copyright (c) 2013 Jianer Shi

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.