# Journal

Documenting what I do to setup ubuntu minimal.

# Initial Program Installs

- installed xinit // xinit is slightly smaller than xorg. IDK what extra things xorg has.
- installed wicp  // wicp is a graphical network manager. Easier than network-manager (for nmcli and cmtui) and better than wifi-radar (another gui).
- installed acpi  // acpi is a command line battery value checker. run with `$acpi`
- installed dwm   // remember to reboot after installing xinit and dwm
- installed chromium-browser // installed four addons: zhongwen, ublock origin, df youtube (df stands for distraction free), and vimium
- installed vim

# Configure Backlight

How do you adjust backlight? Use xbacklight.

- installed and configured xbacklight
    - create or edit the xorg.conf file with `$sudo vim /etc/X11/xorg.conf`
    - add the following code snippet:
    ```
    Section "Device"
    Identifier  "Intel Graphics" 
    Driver      "intel"
    Option      "Backlight"  "intel_backlight"
    EndSection
    ```
    - answer source: https://askubuntu.com/questions/715306/xbacklight-no-outputs-have-backlight-property-no-sys-class-backlight-folder
    - use xbacklight -set 0 to 100.


# TODO

- figure out if redshift autostarts (if not, add to xinitrc or something).
- set up github folder.
- install other programs.

# To Learn

# To Learn In Future

- fzy
- calcurse
- mutt
- ledger
- sc-im

# Interesting Programs to Look Into

- hexchat
- dtrx (extract any compressed file)
- xls2csv
- imagemagick
- scrot (cli screeshot capture)
- screenfetch (displays basic computer info and cool logo) 
- tig (graphical thing for git?)
- fd (compare with fzy?)

# Other Programs

- youtube-dl
