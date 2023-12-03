[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/mzfr/liffy/graphs/commit-activity)


<h1 align="center">gtfo</h1>

![gtfo in action](Images/gtfo.png)

<p align="center">
  <a href="https://github.com/mzfr/gtfo/wiki">gtfo Wiki</a> •
  <a href="https://github.com/mzfr/gtfo/wiki/Introduction">Introduction</a> •
  <a href="https://github.com/mzfr/gtfo/wiki/Usage">Usage</a> •
  <a href="https://github.com/mzfr/gtfo/wiki/Installation">Installation</a> •
  <a href="https://github.com/mzfr/gtfo#gallery">Gallery</a>
</p>

gtfo is a tool purely written in python3 to search binaries on [GTFOBins](https://gtfobins.github.io/) and [LOLBAS](https://lolbas-project.github.io/).

### Features

The only feature of this tool is to give you the ability to search gtfobins and lolbas from terminal.

oh and it also make you stick to your terminal. You won't have to face the bright light of your browser when you find out that vim is marked as SUID on the system you just got reverse shell on but don't know how to exploit that.

### Gallery

* __Searching GTFOBins__

![](Images/bin.png)

* __Searching lolbas__

![](Images/exe.png)

* __List exe__

![](Images/list-exe.png)

* __List binaries__

![](Images/list-bins.png)

* __Errors__ :smile:

![](Images/errors.png)

### Contribution

* Report a bug
* Fix something and open a pull request
* There are some `TODO` in the project. Help me complete those

In any case feel free to open an issue

## Credits

Thanks to [norbemi](https://twitter.com/norbemi) and [cyrus_and](https://twitter.com/cyrus_and) for creating [GTFOBins](https://gtfobins.github.io/) without that this project won't be in existence.

Also thanks to all the creators of [LOLBAS](https://lolbas-project.github.io/#)

## aslam's added option (--file)
on the target box run the find command and collect the basename. Save this output to a file on the local machine
```
find / -perm -u=s -type f 2>/dev/null -exec basename {} \; | sort
```

Next, on your local machine run `gtfobin -f suidfiles.txt`
```
./gtfobin -f suidfiles.txt
```

## Support

If you'd like you can buy me some coffee:

<a href="https://www.buymeacoffee.com/mzfr" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" style="height: 51px !important;width: 217px !important;" ></a>
