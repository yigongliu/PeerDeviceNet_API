PeerDeviceNet_API
=================

PeerDeviceNet, as a mobile framework, supports the following three functional areas for developing connected mobile apps:

* Remote intenting. Intents are android's internal messaging bus to glue components such as activities and services. PeerDeviceNet's remote intenting extends this bus to connected devices, enables remote start of activities and services.
* Group communication. Allow mobile apps set up simple multicast groups among peer devices to enable various communication patterns.
* Device connection. Provide reusable component (Connection Manager) and API to connect peer devices.

There are three native communication mechanisms used by android system components and apps: intents, messenger and IDL(aidl). PeerDeviceNet exposes the above mentioned functionalities thru all these three mechanisms. 

Intents and messenger apis are message based. Intents use action name strings as message ids and messengers use integer message ids. They all package message data as items inside a bundle. Normally IDL(aidl) interfaces are RPC based. Following "messaging" paradigm,  all PeerDeviceNet IDL api methods are asynchronous, ie. marked as "oneway" in definition. And results or responses are returned thru callback/Handler interfaces.

For more detailed descriptions, please refer to "Developer API introduction"(http://www.peerdevicenet.net/api.html).

