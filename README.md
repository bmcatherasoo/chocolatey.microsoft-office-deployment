# Chocolatey Package: Microsoft Office Deployment

## Description

Installiert Microsoft Office 2016 und 365.

## Package Parameters

* `/64bit` to install Office 365 ProPlus 64-bit, otherwise it will default to 32-bit.
* `/DisableUpdate` TRUE, FALSE
* `/Shared` to install with Shared Computer Licensing for Remote Desktop Services.
* `/Channel` default `Broad` [Microsoft Docs](https://docs.microsoft.com/en-us/DeployOffice/overview-of-update-channels-for-office-365-proplus?redirectSourcePath=%252fen-us%252farticle%252f9ccf0f13-28ff-4975-9bd2-7e4ea2fefef4)
* `/Language` default `MatchOS` `MatchOS, ar-sa, bg-bg, zh-cn, zh-tw, hr-hr, cs-cz, da-dk, nl-nl, en-us, et-ee, fi-fi, fr-fr, de-de, el-gr, he-il, hi-in, hu-hu, id-id, it-it, ja-jp, kk-kz, ko-kr, lv-lv, lt-lt, ms-my, nb-no, pl-pl, pt-br, pt-pt, ro-ro, ru-ru, sr-latn-cs, sk-sk, sl-si, es-es, sv-se, th-th, tr-tr, uk-ua, vi-vn`
* `/Product` default `HomeBusinessRetail` Supportet `HomeStudentRetail, PersonalRetail, HomeBusinessRetail, ProfessionalRetail, ProPlusRetail, O365HomePremRetail, O365SmallBusPremRetail, O365BusinessRetail, O365ProPlusRetail, AccessRetail, ExcelRetail, InfoPathRetail,OneNoteRetail, OutlookRetail, PowerPointRetail, PublisherRetail, WordRetail, SPDRetail, ProjectStdRetail, ProjectProRetail, ProjectStdXVolume, ProjectProXVolume, VisioStdRetail, VisioProRetail, VisioStdXVolume, VisioProXVolume, LyncEntryRetail, LyncRetail, SkypeforBusinessEntryRetail, SkypeforBusinessRetail`
* `/Exclude` `Publisher, PowerPoint, OneDrive, Outlook, OneNote, Lync, Groove, Excel, Access, Word`

## Installation

installation without parameters.

```ps1
 choco install microsoft-office-deployment
```

installation with parameters.

```ps1
 choco install microsoft-office-deployment --params="'/64bit'"
```

## ToDo

* Check if there is a factory preinstalled version on it and uninstall it.
* Support for own XML files. [Configuration XML Editor](https://officedev.github.io/Office-IT-Pro-Deployment-Scripts/XmlEditor.html)

## Disclaimer

These Chocolatey Packages only contain installation routines. The software itself is downloaded from the official sources of the software developer. ITIGO AG has no affilation with the software developer.

## Author

* [Simon Bärlocher](https://sbaerlocher.ch)
* [ITIGO AG](https://www.itigo.ch)

## License

This project is under the MIT License. See the [LICENSE](LICENSE) file for the full license text.

## Copyright

(c) 2018, ITIGO AG