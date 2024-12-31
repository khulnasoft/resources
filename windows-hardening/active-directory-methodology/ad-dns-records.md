# AD DNS Records

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

By default **any user** in Active Directory can **enumerate all DNS records** in the Domain or Forest DNS zones, similar to a zone transfer (users can list the child objects of a DNS zone in an AD environment).

The tool [**adidnsdump**](https://github.com/dirkjanm/adidnsdump) enables **enumeration** and **exporting** of **all DNS records** in the zone for recon purposes of internal networks.

```bash
git clone https://github.com/dirkjanm/adidnsdump
cd adidnsdump
pip install .

adidnsdump -u domain_name\\username ldap://10.10.10.10 -r
cat records.csv
```

For more information read [https://dirkjanm.io/getting-in-the-zone-dumping-active-directory-dns-with-adidnsdump/](https://dirkjanm.io/getting-in-the-zone-dumping-active-directory-dns-with-adidnsdump/)

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

