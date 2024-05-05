# Scripts

#### `download-youtube-videos.sh`
- Create a file which contains youtube links on separate lines
- Given the filename as an argument, this script will download each youtube video

#### `dynamic-seedbox.sh`
- Sends the IP of qbittorrent to MyAnonamouse, which requires the correct IP in order to record ratios.

#### `ha-notify.py`
- A python script to easily send a notification to the Home Assistant app on my phone.
- Make sure to fill in `HA_NOTIFY_WEBHOOK_ENDPOINT` in `sample.env`.

#### `manual-usbs-misc-backup.sh`
- Create a file named 'backupcodespass' containing the encryption password for backup_codes.txt in misc backup
   ```
   chmod 600 backupcodespass
   chown root:root backupcodespass
   ```
- As part of my 3-2-1 backup system, I have 2x USB sticks in a fireproof safe with the very basics that I would need to restore backups in a worst-case-scenario.

#### `media-perms.sh`
- This simple script sets the right file ownership/permissions for all of my media files
- Make sure to fill in `MEDIA_DIR` in `sample.env`.

#### `restart.sh`
- This script restarts all running docker containers, installs packages that Nextcloud needs to provide video file previews, and updates the MyAnonamouse seedbox IP address (see `dynamic-seedbox.sh` section)
- Make sure to fill in `SERVER_DIR` in `sample.env`.

#### `scan-nextcloud-files.sh`
- This script sets all file permissions and ownerships for my Nextcloud files. This ensures proper access controls for the Nextcloud web UI. Afterwards, it has Nextcloud scan all files, ensuring that the web UI is aware of and displays all present files.
- Make sure to fill in `FILES_DIR` in `sample.env`.

#### `smartctl-summary.sh`
- This script sends a drive health summary email to my inbox.
- Make sure to fill in `EMAIL` in `sample.env`


*Make sure to `mv sample.env .env` for environment variables to take effect*

