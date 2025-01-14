# Cloudflare Dynamic DNS IP Register
<img alt="GitHub" src="https://img.shields.io/github/license/RakhithJK/cloudflare-ddns-updater?color=black"> <img alt="GitHub last commit (branch)" src="https://img.shields.io/github/last-commit/RakhithJK/cloudflare-ddns-updater/main"> <img alt="GitHub contributors" src="https://img.shields.io/github/contributors/RakhithJK/cloudflare-ddns-updater">


This script is used to update dynamic DNS entries for accounts on Cloudflare.
This script is used to update Dynamic DNS (DDNS) service based on Cloudflare! Access your home network remotely via a custom domain name without a static IP! Written in pure BASH.



## Installation

```bash
git clone https://github.com/RakhithJK/cloudflare-ddns-updater.git
```

## Usage
This script is used with crontab. Specify the frequency of execution through crontab.

```bash
# ┌───────────── minute (0 - 59)
# │ ┌───────────── hour (0 - 23)
# │ │ ┌───────────── day of the month (1 - 31)
# │ │ │ ┌───────────── month (1 - 12)
# │ │ │ │ ┌───────────── day of the week (0 - 6) (Sunday to Saturday 7 is also Sunday on some systems)
# │ │ │ │ │ ┌───────────── command to issue                               
# │ │ │ │ │ │
# │ │ │ │ │ │
# * * * * * cd /{location of repo} && /{location of repo}/cloudflare-template.sh >> /cron.log 2>&1
# 0 0 */3 * * echo " " > /cloudflare-autoupdate.log >> /cron.log 2>&1
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Reference
This script was made with reference from [Keld Norman](https://www.youtube.com/watch?v=vSIBkH7sxos) video.

## License
[MIT](https://github.com/K0p1-Git/cloudflare-ddns-updater/blob/main/LICENSE)
