# [Mozilla Hubs](https://hubs.mozilla.com/)

[![License: MPL 2.0](https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg)](https://opensource.org/licenses/MPL-2.0) [![Build Status](https://travis-ci.org/mozilla/hubs.svg?branch=master)](https://travis-ci.org/mozilla/hubs) [![Discord](https://img.shields.io/discord/498741086295031808)](https://discord.gg/CzAbuGu)

[Learn more about Hubs](https://hubs.mozilla.com/docs/welcome.html)

## Getting Started

### Development environment
I recommend using WSL on windows (WSL2) because it has much better support for VR headsets with SteamVR. Chrome / firefox do not have in browser VR support on Ubuntu yet.

WSL allows you to use all the great dev tools of Ubuntu while still being able to test things easily in VR.

As an IDE, Visual Studio Code is pretty good for Node.js

### Quick Start

[Install NodeJS](https://nodejs.org) if you haven't already. We recommend version 12 or above.

As in the hubs [documentation](https://hubs.mozilla.com/docs/hubs-cloud-custom-clients.html), run the following commands:

```bash
git clone git@github.com:PeterCarragher/hubs.git
cd hubs
git checkout hubs-cloud
npm ci
npm run login
Host (eg hubs.mozilla.com): vrgt.org
npm start
```

### Testing
```bash
npm test
```

After making your changes, visit https://localhost:8080 to test them locally(note: HTTPS is required, you'll need to accept the warning for the self-signed SSL certificate)

> Note: When running the Hubs client locally, you will still connect to the development versions of our [Janus WebRTC](https://github.com/mozilla/janus-plugin-sfu) and [reticulum](https://github.com/mozilla/reticulum) servers. These servers do not allow being accessed outside of localhost. If you want to host your own Hubs servers, please check out [Hubs Cloud](https://hubs.mozilla.com/docs/hubs-cloud-intro.html).

## Documentation

The Hubs documentation can be found [here](https://hubs.mozilla.com/docs).

## Community

Join us on our [Discord Server](https://discord.gg/CzAbuGu) or [follow us on Twitter](https://twitter.com/MozillaHubs).

## Contributing

Read our [contributor guide](./CONTRIBUTING.md) to learn how you can submit bug reports, feature requests, and pull requests.

Contributors are expected to abide by the project's [Code of Conduct](./CODE_OF_CONDUCT.md) and to be respectful of the project and people working on it. 

## Additional Resources

* [Reticulum](https://github.com/mozilla/reticulum) - Phoenix-based backend for managing state and presence.
* [NAF Janus Adapter](https://github.com/mozilla/naf-janus-adapter) - A [Networked A-Frame](https://github.com/networked-aframe) adapter for the Janus SFU service.
* [Janus Gateway](https://github.com/meetecho/janus-gateway) - A WebRTC proxy used for centralizing network traffic in this client.
* [Janus SFU Plugin](https://github.com/mozilla/janus-plugin-sfu) - Plugins for Janus which enables it to act as a SFU.
* [Hubs-Ops](https://github.com/mozilla/hubs-ops) - Infrastructure as code + management tools for running necessary backend services on AWS.

## Privacy

Mozilla and Hubs believe that privacy is fundamental to a healthy internet. Read our [privacy policy](./PRIVACY.md) for more info.

## License

Hubs is licensed with the [Mozilla Public License 2.0](./LICENSE)