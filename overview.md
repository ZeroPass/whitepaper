# Overview

Overview of whole cryptographic schematics.![](https://zeropass.gitbooks.io/whitepaper/content/all.svg)

The second device is not included in this scheme. All \(smart\) devices under the same account have the whole scheme independently deployed. Fully encrypted syncing \(with two factor signatures\) ensures consistency between devices. The second device is not needed cryptographically, it only confirms that the user behind the device is really you by sending a signed message to the ZeroPass server.

Source code for all our apps will be made publicly available on GitHub \(asap\).

Let us unwind this a bit, and see how ZeroPass scheme comes to life;

