# software-update-tray
This program will check for updates every two hours and show these updates by notification.

Author: Peter Ahlers

## Install
Know what you are doing and prepare the use of this program by the following steps

1) Run the following command.
"""bash
apt install python-appindicator python-apscheduler python-notify2
  python-concurrent.futures python-funcsigs python-gtk2
"""
2) Add the content of sudo-software-update-tray to "/etc/sudoers.d". I would like to get the update list without sudo,
   but that seems impossible. This solution is to be able to run software-update-tray-get-updates without password.
3) Copy the software-update-tray and software-update-tray-get-updates to a place where you can run it.
4) Add "software-update-tray" to your startup script


## Inspiration
The following source by Neil Jagdish Patel <neil.patel@canonical.com> and Jono Bacon <jono@ubuntu.com> is used as an
inspiration.

https://wiki.ubuntu.com/DesktopExperienceTeam/ApplicationIndicators#PyGTK


## License
This program is free software: you can redistribute it and/or modify it
under the terms of either or both of the following licenses:

1) the GNU Lesser General Public License version 3, as published by the
Free Software Foundation; and/or
2) the GNU Lesser General Public License version 2.1, as published by
the Free Software Foundation.

This program is distributed in the hope that it will be useful, but
WITHOUT ANY WARRANTY; without even the implied warranties of
MERCHANTABILITY, SATISFACTORY QUALITY or FITNESS FOR A PARTICULAR
PURPOSE.  See the applicable version of the GNU Lesser General Public
License for more details.

You should have received a copy of both the GNU Lesser General Public
License version 3 and version 2.1 along with this program.  If not, see
<http://www.gnu.org/licenses/>
