# Audio_Auto-Edit-From-Timecode

Given a PDF script that specifies timecodes, auto-edit source audio to extract relevant clips into their own folder so that they can then be imported into an DAW (Ableton). Created for the Coal Face project with Louise powell, Aug'23

Steps:

1. Manually prepare source-audio document as plain text document- The plain text document should have the following format (Example timecode document is included in the repo):  
   SOURCE: Filename 1  
   timecode 1  
   timecode 2  
   ..  
   timecode 10

   SOURCE: Filename 2

   NOTE: Timecode in hh:mm:ss:ms format  
    example:  
    SOURCE: Michael Banes Interview.mp3  
    00.00.24.00  
    00.01.34.23  
    ..

2. Run the Audio_Auto-Edit-Timcode script that does the following:  
   2.1. Asks:  
    A. What SOURCE to extract from the given timecode document (i.e. do you want to extract all edits at once or just one source file's extracts (useful if there is an error with one of the timecodes and you want to amend the timecode document, correct it, and re-extract only that source files edits)  
    B. How long each extract should be (i.e. 30s, 60s). Ensure that the length will be enough to encapsulate each of the sentences that you want to extract.  
    C. Where to save the extracted files (each SOURCE to get it's own 'EXTRACTS_Filename sub folder).  
    D. Confirm/Cancel (COnfirm = Extracts Audio from selected Source)

   2.2. For each filename in the list:  
    A. Extract an audio file with a specific duration (i.e. 30s from timecode) for each timecode under the filename  
    B. Place edited clips in a sub folder with the title Extracts_Filename where each file is titled timecode.filename.extract: Example: 00.00.24.00.thisFile.extract.mp3  
    C. Repeat for each filename in the list
