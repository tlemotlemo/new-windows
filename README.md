# new-windows
Set of custom Windows sounds

`new-windows` is a set of system sound effects originally made for Windows 10. I also use these sound effects for my NixOS setup.

These sound effects were made in FL Studio. I don't remember which plugin, but it was likely Hybrid 3, which was my go-to instrument plugin before switching to Linux. For effects, it also likely used the Kilohearts plugins, including the free ones and Convolver.

### Setup
In Windows 10, you can change the system sounds through **Control Panel > Sound**, in the Sounds tab. I believe you can change the startup sound through **Winaero Tweaker**, which I did for the `windows_login` sound. The file names of the sounds indicate which system sounds to replace them with.

With Linux, you use the system configuration to play sounds. Programs like `paplay`, `mpv`, and `ffplay` are your friends here. If you're using i3, for example, you can bind the `exec` command to the same key as another command. Below, I used `mpv` to play a sound whenever I closed a window:

```
# kill focused window
bindsym $mod+q kill; exec mpv --no-video ~/Documents/new\ windows/restore_down.wav
```
