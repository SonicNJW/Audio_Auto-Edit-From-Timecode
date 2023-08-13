# Audio_Auto-Edit-From-Timecode

Given a PDF script that specifies timecodes, auto-edit source audio to extract relevant clips into their own folder so that they can then be imported into an DAW (Ableton). Created for the Coal Face project with Louise powell, Aug'23

Steps:

1. Manually prepare source-audio document - A plain text file that has the following format:  
   Filename 1  
   timecode 1  
   timecode 2  
   ..  
   timecode 10

   Filename 2

   NOTE: Timecode in hh:mm:ss:ms format

1. For each filename in the list:  
   1.1. Extract an audio file with a specific duration (i.e. 30s from timecode) for each timecode under the filename  
   1.2. Place edited clips in a sub folder with the title Extracts_Filename where each file is titled ex01.timecode.filename  
   1.3. Repeat for each filename in the list
