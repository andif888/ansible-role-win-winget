# ansible-role-win-winget

Role to install winget for Windows 10, 11 and Server 2022

## Table of content

- [Default Variables](#default-variables)
  - [winget_cli_download_url](#winget_cli_download_url)
  - [winget_cli_license_filename](#winget_cli_license_filename)
  - [winget_cli_license_url](#winget_cli_license_url)
  - [winget_cli_msixbundle_filename](#winget_cli_msixbundle_filename)
  - [winget_cli_version](#winget_cli_version)
  - [winget_extract_dir](#winget_extract_dir)
  - [winget_microsoft_ui_xaml_download_url](#winget_microsoft_ui_xaml_download_url)
  - [winget_microsoft_ui_xaml_major_version](#winget_microsoft_ui_xaml_major_version)
  - [winget_microsoft_ui_xaml_version](#winget_microsoft_ui_xaml_version)
  - [winget_microsoft_vclibs_download_url](#winget_microsoft_vclibs_download_url)
  - [winget_microsoft_vclibs_version](#winget_microsoft_vclibs_version)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Default Variables

### winget_cli_download_url

winget cli download url

#### Default value

```YAML
winget_cli_download_url: https://github.com/microsoft/winget-cli/releases/download/v{{
  winget_cli_version }}/{{ winget_cli_msixbundle_filename }}
```

### winget_cli_license_filename

#### Default value

```YAML
winget_cli_license_filename: 3463fe9ad25e44f28630526aa9ad5648_License1.xml
```

### winget_cli_license_url

winget cli license url

#### Default value

```YAML
winget_cli_license_url: https://github.com/microsoft/winget-cli/releases/download/v{{
  winget_cli_version }}/{{ winget_cli_license_filename }}
```

### winget_cli_msixbundle_filename

#### Default value

```YAML
winget_cli_msixbundle_filename: Microsoft.DesktopAppInstaller_8wekyb3d8bbwe.msixbundle
```

### winget_cli_version

winget cli version

#### Default value

```YAML
winget_cli_version: 1.4.10173
```

### winget_extract_dir

extract directory

#### Default value

```YAML
winget_extract_dir: C:\windows\temp\winget_extract
```

### winget_microsoft_ui_xaml_download_url

Microsoft.UI.Xaml downlaod url

#### Default value

```YAML
winget_microsoft_ui_xaml_download_url: https://www.nuget.org/api/v2/package/Microsoft.UI.Xaml/{{
  winget_microsoft_ui_xaml_version }}
```

### winget_microsoft_ui_xaml_major_version

Microsoft.UI.Xaml major version

#### Default value

```YAML
winget_microsoft_ui_xaml_major_version: '2.7'
```

### winget_microsoft_ui_xaml_version

Microsoft.UI.Xaml version

#### Default value

```YAML
winget_microsoft_ui_xaml_version: '{{ winget_microsoft_ui_xaml_major_version }}.3'
```

### winget_microsoft_vclibs_download_url

Microsoft VCLibs download url

#### Default value

```YAML
winget_microsoft_vclibs_download_url: https://aka.ms/Microsoft.VCLibs.x64.{{ winget_microsoft_vclibs_version
  }}.Desktop.appx
```

### winget_microsoft_vclibs_version

Microsoft VCLibs version

#### Default value

```YAML
winget_microsoft_vclibs_version: '14.00'
```



## Dependencies

None.

## License

license (GPL-2.0-or-later, MIT, etc)

## Author

andif888
