

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


Some things that could be useful to debug/deobfuscate a malicious VBS file:

## echo

```bash
Wscript.Echo "Like this?"
```

## Commnets

```bash
' this is a comment
```

## Test

```bash
cscript.exe file.vbs
```

## Write data to a file

```js
Function writeBinary(strBinary, strPath)

    Dim oFSO: Set oFSO = CreateObject("Scripting.FileSystemObject")

    ' below lines purpose: checks that write access is possible!
    Dim oTxtStream

    On Error Resume Next
    Set oTxtStream = oFSO.createTextFile(strPath)

    If Err.number <> 0 Then MsgBox(Err.message) : Exit Function
    On Error GoTo 0

    Set oTxtStream = Nothing
    ' end check of write access

    With oFSO.createTextFile(strPath)
        .Write(strBinary)
        .Close
    End With

End Function
```



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



