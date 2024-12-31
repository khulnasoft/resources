# Office file analysis

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

<figure><img src="../../../.gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure>

\
Use [**Trickest**](https://trickest.com/?utm_source=resources&utm_medium=text&utm_campaign=ppc&utm_content=office-file-analysis) to easily build and **automate workflows** powered by the world's **most advanced** community tools.\
Get Access Today:

{% embed url="https://trickest.com/?utm_source=resources&utm_medium=banner&utm_campaign=ppc&utm_content=office-file-analysis" %}

For further information check [https://trailofbits.github.io/ctf/forensics/](https://trailofbits.github.io/ctf/forensics/). This is just a sumary:

Microsoft has created many office document formats, with two main types being **OLE formats** (like RTF, DOC, XLS, PPT) and **Office Open XML (OOXML) formats** (such as DOCX, XLSX, PPTX). These formats can include macros, making them targets for phishing and malware. OOXML files are structured as zip containers, allowing inspection through unzipping, revealing the file and folder hierarchy and XML file contents.

To explore OOXML file structures, the command to unzip a document and the output structure are given. Techniques for hiding data in these files have been documented, indicating ongoing innovation in data concealment within CTF challenges.

For analysis, **oletools** and **OfficeDissector** offer comprehensive toolsets for examining both OLE and OOXML documents. These tools help in identifying and analyzing embedded macros, which often serve as vectors for malware delivery, typically downloading and executing additional malicious payloads. Analysis of VBA macros can be conducted without Microsoft Office by utilizing Libre Office, which allows for debugging with breakpoints and watch variables.

Installation and usage of **oletools** are straightforward, with commands provided for installing via pip and extracting macros from documents. Automatic execution of macros is triggered by functions like `AutoOpen`, `AutoExec`, or `Document_Open`.

```bash
sudo pip3 install -U oletools
olevba -c /path/to/document #Extract macros
```

<figure><img src="../../../.gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure>

\
Use [**Trickest**](https://trickest.com/?utm_source=resources&utm_medium=text&utm_campaign=ppc&utm_content=office-file-analysis) to easily build and **automate workflows** powered by the world's **most advanced** community tools.\
Get Access Today:

{% embed url="https://trickest.com/?utm_source=resources&utm_medium=banner&utm_campaign=ppc&utm_content=office-file-analysis" %}

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

