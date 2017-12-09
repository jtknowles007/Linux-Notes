# BASH Notes

## 11/27/2017
*

## 12/9/2017
Found information about adding volume level display on i3bar Conky JSON file.  The commands used are as follows:
 
amixer -c 0 get Master | awk '$0~/%/{print $4}' | tr -d '[]' is the full string of commands to query the volume control and ouput the volume as a percent.

There are three commands used...amixer, awk, and tr, and of course | 'pipes' the output of the command to the next command in the line.

*  amixer -c 0 get Master
   *  amixer is a command-line mixer for ALSA soundcard driver
   *  -c  indicates that you wish to specify a specific soundcard
   *  0 is the number of the soundcard to act upon
   *  get shows the mixer control contents
   *  Master is the control selection - the Master chanel
   *  Output of above command is:
     >Simple mixer control 'Master',0
     >Capabilities: pvolume pvolume-joined pswitch pswitch-joined
     >Playback channels: Mono
     >Limits: Playback 0 - 87
     >Mono: Playback 87 [100%] [0.00dB] [on]
*  awk '$0~/%/{print $4}'
   *  awk is a pattern scanning and text processing language.  Used to define a pattern and action upon the pattern
   *  $0~/%/ tells awk to take the output of the entire line, $0 and find text that matches the characters between ~/ and / 
   *  The characters between the lines can be literal text or regular expressions.
   *  {print $4} tells awk to output the 4th "word" found in the line that contains %
   *  Output of the above command is:
     >[100%]
*  tr -d '[]'
   *  tr translates or replaces text passed to it.
   *  -d tells tr to delete instead of translate
   *  '[]' tells tr that the characters to match for deletion are the open and close brackets.
   *  Output of the above command is:
     >100%


  

