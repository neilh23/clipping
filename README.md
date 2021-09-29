# clipping
Extremely simple scripted clipboard manager using dmenu 

## Instructions

For i3 Window Manager, put the files in bin/ in your path, then add the following to ~/.config/i3/config:

> bindsym $mod+c exec clipping_copy
> 
> bindsym $mod+v exec clipping_select
> 
> bindsym $mod+x exec clipping_clear

('$mod' is the Windows key by default)

* mod+c will copy the current clipboard to the first position (moving other entries up)
* mod+v will display all entries with dmenu, allowing you to copy a desired entry to the clipboard
* mod+x will display all entries with dmenu, allowing you to delete the selected entry

That's it - code with written in 10 minutes, but it's actually pretty useful. I may refactor as a single script later

Be careful if using with a password manager, as entries are saved as plaintext files


Named in honour of the band [clipping.](clppng.bandcamp.com)
