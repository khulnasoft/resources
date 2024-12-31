# macOS Apple Events

{% hint style="success" %}
Learn & practice AWS Hacking:<img src="/.gitbook/assets/arte.png" alt="" data-size="line">[**Resources Training AWS Red Team Expert (ARTE)**](https://training.khulnasoft.com/courses/arte)<img src="/.gitbook/assets/arte.png" alt="" data-size="line">\
Learn & practice GCP Hacking: <img src="/.gitbook/assets/grte.png" alt="" data-size="line">[**Resources Training GCP Red Team Expert (GRTE)**<img src="/.gitbook/assets/grte.png" alt="" data-size="line">](https://training.khulnasoft.com/courses/grte)

<details>

<summary>Support Resources</summary>

* Check the [**subscription plans**](https://patreon.com/khulnasoft)!
* **Join the** 💬 [**Discord group**](https://discord.gg/hRep4RUj7f) or the [**telegram group**](https://t.me/peass) or **follow** us on **Twitter** 🐦 [**@resources\_live**](https://twitter.com/khulnasoft\_live)**.**
* **Share hacking tricks by submitting PRs to the** [**Resources**](https://github.com/khulnasoft/resources) and [**Resources Cloud**](https://github.com/khulnasoft/resources-cloud) github repos.

</details>
{% endhint %}

## Basic Information

**Apple Events** are a feature in Apple's macOS that allows applications to communicate with each other. They are part of the **Apple Event Manager**, which is a component of the macOS operating system responsible for handling interprocess communication. This system enables one application to send a message to another application to request that it perform a particular operation, like opening a file, retrieving data, or executing a command.

The mina daemon is `/System/Library/CoreServices/appleeventsd` which registers the service `com.apple.coreservices.appleevents`.

Every application that can receive events will checking with this daemon providing its Apple Event Mach Port. And when an app wants to send an event to to it, the app will request this port from the daemon.

Sandboxed applications requires privileges like `allow appleevent-send` and `(allow mach-lookup (global-name "com.apple.coreservices.appleevents))` in order to be able to send events. Noten that entitlements like `com.apple.security.temporary-exception.apple-events` could restrict who have access to send events which will need entitlements like `com.apple.private.appleevents`.

{% hint style="success" %}
It's possible to use the env variable **`AEDebugSends`** in order to log informtion about the message sent:

```bash
AEDebugSends=1 osascript -e 'tell application "iTerm" to activate'
```
{% endhint %}

{% hint style="success" %}
Learn & practice AWS Hacking:<img src="/.gitbook/assets/arte.png" alt="" data-size="line">[**Resources Training AWS Red Team Expert (ARTE)**](https://training.khulnasoft.com/courses/arte)<img src="/.gitbook/assets/arte.png" alt="" data-size="line">\
Learn & practice GCP Hacking: <img src="/.gitbook/assets/grte.png" alt="" data-size="line">[**Resources Training GCP Red Team Expert (GRTE)**<img src="/.gitbook/assets/grte.png" alt="" data-size="line">](https://training.khulnasoft.com/courses/grte)

<details>

<summary>Support Resources</summary>

* Check the [**subscription plans**](https://patreon.com/khulnasoft)!
* **Join the** 💬 [**Discord group**](https://discord.gg/hRep4RUj7f) or the [**telegram group**](https://t.me/peass) or **follow** us on **Twitter** 🐦 [**@resources\_live**](https://twitter.com/khulnasoft\_live)**.**
* **Share hacking tricks by submitting PRs to the** [**Resources**](https://github.com/khulnasoft/resources) and [**Resources Cloud**](https://github.com/khulnasoft/resources-cloud) github repos.

</details>
{% endhint %}

