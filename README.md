# Caf.js

Co-design permanent, active, stateful, reliable cloud proxies with your web app and devices.

See https://www.cafjs.com

## helloiotbrowser2

Browser-based IoT example sharing a Bluetooth device (Puck.js) by exchanging a URL. It uses the Web Bluetooth API (needs Chrome for the gateway, any browser for the client).

You can also run the local Bluetooth gateway on a Raspberry PI, and then you don't need Chrome open. `Caf.js` is three-way isomorphic, allowing the same gateway code to run in both.

This example is very similar to the output of the template generator tool:

    cafjs  generate helloiotbrowser2  iotbrowser ...

The original `helloiotbrowser` used a separate Chrome tab for the gateway code, but Chrome throttles background tabs aggressively, and that created unnecessary delays.

Instead, this example uses an iframe for the gateway, making it more responsive. Consider the original `helloiotbrowser` obsolete...
