### Средство перемещения приложений Synology

Легко перемещайте пакеты Synology с одного тома на другой том.

Вы просто выбираете пакет и целевой том, и сценарий остановит приложение, переместит его, обновит символические ссылки, а затем запустит приложение.

Удобно для перемещения пакетов на том SSD или на другой том, чтобы можно было удалить исходный том.

**NEW** Теперь включает [режимы резервного копирования и восстановления ](/images/backup.png).

  - Поддерживает DSM 7. Не полностью протестировано с DSM 6.


### Пакеты подтверждены рабочие

**ПРИМЕЧАНИЕ:** SНекоторые люди сообщали о проблемах с перемещением Container Manager. Сделайте резервную копию вашего докера, составьте файлы стеков портейнеров.

<details>
  <summary>Нажмите здесь, чтобы увидеть список</summary>

| Package Center Name | Name shown in script | Result |
|---------------------|-------------|--------|
| Active Backup for Business | ActiveBackup | OK - Move, Backup and Restore |
| Active Backup for Google Workspace | ActiveBackup-GSuite | OK |
| Active Backup for Microsoft 365 | ActiveBackup-Office365 | OK |
| Advanced Media Extensions | CodecPack | OK |
| AntiVirus by McAfee | AntiVirus-McAfee | OK |
| AntiVirus Essential | AntiVirus | OK |
| Apache 2.4 | Apache2.4 | OK |
| Audio Station | AudioStation | OK - Move, Backup and Restore |	
| Bitdefender for MailPlus | BitDefenderForMailPlus | OK I think |
| C2 Identity LDAP Server | C2IdentityLDAPAgent | OK - need a C2 account to fully test |
| Central Management System | CMS | OK |
| Cloud Sync | CloudSync | OK |
| Container Manager | ContainerManager | OK - Move, Backup and Restore |
| DNS Server | DNSServer | OK |
| Docker | Docker | OK - Move, Backup and Restore |
| Document Viewer | DocumentViewer | OK |
| Download Station | DownloadStation | OK |
| Emby Server | EmbyServer | OK |
| exFAT Access | exFAT-Free | OK - Move, Backup and Restore |
| git | git | OK |
| Git | Git | OK |
| Glacier Backup | GlacierBackup | OK - need a Glacier account to fully test |
| Hyper Backup | HyperBackup | OK |
| Hyper Backup Vault | HyperBackupVault | OK |
| LDAP Server | DirectoryServer | OK |
| LogAnalysis | LogAnalysis | OK - Move, Backup and Restore |
| Log Center | Log Center | OK |
| Mail Station | MailStation | OK |
| MariaDB 10 | MariaDB10 | OK |
| Media Server | MediaServer | OK |
| MediaInfo | mediainfo | OK - Move, Backup and Restore |
| MinimServer | MinimServer | OK |
| phpMyAdmin | phpMyAdmin | OK |
| Node.js v14 | Node.js_v14 | OK |
| Node.js v16 | Node.js_v16 | OK |
| Node.js v18 | Node.js_v18 | OK |
| Node.js v20 | Node.js_v20 | OK |
| Note Station | NoteStation | OK |
| PDF Viewer | PDFViewer | OK |
| Perl | Perl | OK - Move, Backup and Restore |
| PHP 7.3 | PHP7.3 | OK - Move, Backup and Restore |
| PHP 7.4 | PHP7.4 | OK - Move, Backup and Restore |
| PHP 8.0 | PHP8.0 | OK - Move, Backup and Restore |
| PHP 8.1 | PHP8.1 | OK - Move, Backup and Restore |
| PHP 8.2 | PHP8.2 | OK - Move, Backup and Restore |
| Plex Media Server | PlexMediaServer | OK |
| Presto File Server | PrestoServer | OK |
| Proxy Server | ProxyServer | OK |
| Python 3.9 | Python3.9 | OK - Move, Backup and Restore |
| Radius Server | RadiusServer | OK |
| SMI-S Provider | SynoSmisProvider | OK |
| Snapshot Replication | SnapshotReplication | OK |
| SSO Server | SSOServer | OK |
| Storage Analyzer | StorageAnalyzer | OK |
| Surveillance Station | SurveillanceStation | OK |
| SynoCli Tools | synocli-"toolname" | OK |
| Synology Application Service | SynologyApplicationService | OK |
| Synology Calendar | Calendar | OK - Move, Backup and Restore |
| Synology Chat Server | Chat | OK |
| Synology Contacts | Contacts | OK |
| Synology Directory Server | DirectoryServerForWindowsDomain | OK |
| Synology Drive Server | SynologyDrive | OK |
| Synology Mail Server | MailServer | OK |
| Synology MailPlus | MailPlus | OK |
| Synology MailPlus Server | MailPlus-Server | Still Testing... |
| Synology Office | Spreadsheet | OK |
| Synology Photos | SynologyPhotos | OK - Move, Backup and Restore |
| Tailscale | Tailscale | OK |
| Text Editor | TextEditor | OK |
| Universal Viewer | UniversalViewer | OK |
| Video Station | VideoStation | OK |
| Virtual Machine Manager | Virtualization | OK |
| VPN Server | VPNCenter | OK |
| Web Station | WebStation | OK |
| WebDAV Server | WebDAVServer | OK |

</details>

#### Packages not tested

<details>
  <summary>Нажмите здесь, чтобы увидеть список</summary>

| Package | Result |
|---------|--------|
| Archiware P5 |  |
| BRAVIA Signage | Won't install in Container Manager. It checks if Docker installed |
| Data Deposit Box |  |
| Domotz Network Monitoring |  |
| ElephantDrive |  |
| GoodSync |  |
| IDrive |  |
| Joomla |  |
| KodiExplorer |  |
| MediaWiki |  |
| MEGAcmd |  |
| NAKIVO Backup and Replication |  |
| NAKIVO Transporter |  |
| PACS |  |
| Ragic Cloud DB |  |
| Resilo Sync |  |
| TeamViewer |  |
| VirtualHere |  |
| vtigerCRM |  |
| Wordpress |  |

</details>

### Скачать сценарий

1. Загрузите исходный код последней версии (zip) с https://github.com/007revad/Synology_app_mover/releases
2. Сохраните загруженный zip-файл в папку на Synology.
3. Разархивируйте zip-файл.

### Установить место резервного копирования

Если вы хотите использовать [параметры резервного копирования и восстановления](/images/backup.png) вам необходимо отредактировать включенный файл **syno_app_mover.conf**, чтобы указать местоположение для резервного копирования.

Файл **syno_app_mover.conf** должен находиться в той же папке, что и **syno_app_mover.sh file**.

### Чтобы запустить скрипт

[Как включить SSH и войти в DSM через SSH](https://kb.synology.com/en-global/DSM/tutorial/How_to_login_to_DSM_with_root_permission_via_SSH_Telnet)

```YAML
sudo -s /volume1/scripts/syno_app_mover.sh
```

**Примечание**. Замените /volume1/scripts/ путем к расположению сценария.

### Поиск неисправностей

Если скрипт не запускается, проверьте следующее:

1.Обязательно загрузите zip-файл и разархивируйте его в папку на Synology (а не на компьютере).
2. Если путь к скрипту содержит пробелы, вам необходимо заключить путь/имя скрипта в двойные кавычки:
   ```YAML
   sudo -s "/volume1/my scripts/syno_app_mover.sh"
   ```
3. Убедитесь, что вы распаковали загруженный файл zip или rar и пытаетесь запустить файл syno_app_mover.sh.
4. Установите файл сценария как исполняемый
   ```YAML
   sudo chmod +x "/volume1/scripts/syno_app_mover.sh"
   ```

### Скриншоты ДСМ 7

<p align="center">Moving a package (with dependencies)</p>
<p align="center"><img src="/images/app2.png"></p>

<br>

<p align="center">Moving packages with shared folders</p>
<p align="center"><img src="/images/app3.png"></p>
<p align="center"><img src="/images/app4.png"></p>

<br>

<p align="center">Moving a package that has a volume location setting</p>
<p align="center"><img src="/images/app5.png"></p>

<br>

<p align="center">Moving Active Backup for Bussiness</p>
<p align="center"><img src="/images/app6.png"></p>

<br>

<p align="center">Backing up Audio Station</p>
<p align="center"><img src="/images/backup.png"></p>

### Credits
- wallacebrf for extensive beta testing of syno_app_mover v3.
