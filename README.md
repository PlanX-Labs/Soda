# Soda OS
Soda is a very simple operating system based on Raspbian for learning IoT edge programming.

## image
- [v1.4.1](https://drive.google.com/file/d/1MOgH1RgA2VneLI8kLC07-q_2amYQoyNC/view?usp=sharing)
- Upgrade soda library & bug fix<br><br>

### Serial Terminal Setting. Proceed only for the users you really need.
*Connect your storage(T-Flash or USB Memory) to your PC and check the drive letter.(ex D:)*<br><br>

*Open D:/boot/cmdline.txt and add the following to the end: (Note: Insert only one space without line breaks)* 
```console 
console=serial0,115200
```
*Open D:/boot/config.txt and add the following to the end:*
```console
arm_freq=1400
core_freq=250
```

*Serial connections don't have a standard way of setting terminal geometry.*<br>
*The assumed geometry is often 80x23 or 80x24 (terminals with zero to two status lines).*<br>
*Once you're logged in, you can set your preferred geometry via the shell, using something like*<br>
> Assume the actual terminal size is 30 rows and 120 columns<br>
```console
exit
stty rows 30 cols 120
tmux
```

## host tools
- [v1.2.3](https://drive.google.com/open?id=11tKgj8sRug7jJuA9WNzE_wPRbOChDEsk) <br>
*Rename folder and append SD Formatter*

## putty setting
- This is the same as included in the host tool.
- [putty_setting](https://drive.google.com/open?id=1Ihd6P4PGWjg0Vvux6i1XYlmIdNS-dx_1)
