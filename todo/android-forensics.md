# Android Forensics

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

## Locked Device

To start extracting data from an Android device it has to be unlocked. If it's locked you can:

* Check if the device has debugging via USB activated.
* Check for a possible [smudge attack](https://www.usenix.org/legacy/event/woot10/tech/full\_papers/Aviv.pdf)
* Try with [Brute-force](https://www.cultofmac.com/316532/this-brute-force-device-can-crack-any-iphones-pin-code/)

## Data Adquisition

Create an [android backup using adb](../mobile-pentesting/android-app-pentesting/adb-commands.md#backup) and extract it using [Android Backup Extractor](https://sourceforge.net/projects/adbextractor/): `java -jar abe.jar unpack file.backup file.tar`

### If root access or physical connection to JTAG interface

* `cat /proc/partitions` (search the path to the flash memory, generally the first entry is _mmcblk0_ and corresponds to the whole flash memory).
* `df /data` (Discover the block size of the system).
* dd if=/dev/block/mmcblk0 of=/sdcard/blk0.img bs=4096 (execute it with the information gathered from the block size).

### Memory

Use Linux Memory Extractor (LiME) to extract the RAM information. It's a kernel extension that should be loaded via adb.

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

