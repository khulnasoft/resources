# Windows - Persistence

:warning: Content of this page has been moved to [resources/redteam/persistence/windows](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/)

- [Tools](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#tools)
- [Hide Your Binary](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#hide-your-binary)
- [Disable Antivirus and Security](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#disable-antivirus-and-security)
    - [Antivirus Removal](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#antivirus-removal)
    - [Disable Windows Defender](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#disable-windows-defender)
    - [Disable Windows Firewall](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#disable-windows-firewall)
    - [Clear System and Security Logs](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#clear-system-and-security-logs)
- [Simple User](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#simple-user)
    - [Registry HKCU](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#registry-hkcu)
    - [Startup](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#startup)
    - [Scheduled Tasks User](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#scheduled-tasks-user)
    - [BITS Jobs](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#bits-jobs)
- [Serviceland](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#serviceland)
    - [IIS](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#iis)
    - [Windows Service](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#windows-service)
- [Elevated](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#elevated)
    - [Registry HKLM](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#registry-hklm)
        - [Winlogon Helper DLL](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#)
        - [GlobalFlag](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#)
    - [Startup Elevated](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#startup-elevated)
    - [Services Elevated](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#services-elevated)
    - [Scheduled Tasks Elevated](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#scheduled-tasks-elevated)
    - [Binary Replacement](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#binary-replacement)
        - [Binary Replacement on Windows XP+](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#binary-replacement-on-windows-xp)
        - [Binary Replacement on Windows 10+](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#binary-replacement-on-windows-10)
    - [RDP Backdoor](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#rdp-backdoor)
        - [utilman.exe](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#utilman.exe)
        - [sethc.exe](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#sethc.exe)
    - [Remote Desktop Services Shadowing](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#remote-desktop-services-shadowing)
    - [Skeleton Key](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#skeleton-key)
    - [Virtual Machines](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#virtual-machines)
    - [Windows Subsystem for Linux](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#windows-subsystem-for-linux)
- [Domain](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#domain)
    - [Golden Certificate](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#golden-certificate)
    - [Golden Ticket](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#golden-ticket)
- [References](https://resources.khulnasoft.com/resources/redteam/persistence/windows-persistence/#references)