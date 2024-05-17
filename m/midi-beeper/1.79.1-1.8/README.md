# Comparing `tmp/midi_beeper-1.79.1.tar.gz` & `tmp/midi_beeper-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midi_beeper-1.79.1.tar", last modified: Thu May 16 10:51:22 2024, max compression
+gzip compressed data, was "midi_beeper-1.8.tar", last modified: Fri May 17 08:14:01 2024, max compression
```

## Comparing `midi_beeper-1.79.1.tar` & `midi_beeper-1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 10:51:22.683353 midi_beeper-1.79.1/
--rw-r--r--   0 silbrown   (501) staff       (20)    11357 2024-05-16 08:52:25.000000 midi_beeper-1.79.1/LICENSE
--rw-r--r--   0 silbrown   (501) staff       (20)     3752 2024-05-16 10:51:22.682412 midi_beeper-1.79.1/PKG-INFO
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 10:51:22.679789 midi_beeper-1.79.1/midi_beeper/
--rw-r--r--   0 silbrown   (501) staff       (20)      117 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper/__init__.py
--rw-r--r--   0 silbrown   (501) staff       (20)    57594 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper/__main__.py
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 10:51:22.681781 midi_beeper-1.79.1/midi_beeper.egg-info/
--rw-r--r--   0 silbrown   (501) staff       (20)     3752 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper.egg-info/PKG-INFO
--rw-r--r--   0 silbrown   (501) staff       (20)      242 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper.egg-info/SOURCES.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper.egg-info/dependency_links.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       62 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper.egg-info/entry_points.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       12 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper.egg-info/top_level.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-16 10:51:22.683599 midi_beeper-1.79.1/setup.cfg
--rw-r--r--   0 silbrown   (501) staff       (20)     3872 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-17 08:14:01.085437 midi_beeper-1.8/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-17 08:13:06.000000 midi_beeper-1.8/LICENSE
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3749 2024-05-17 08:14:01.085437 midi_beeper-1.8/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-17 08:14:01.085437 midi_beeper-1.8/midi_beeper/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      117 2024-05-17 08:14:00.000000 midi_beeper-1.8/midi_beeper/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    59847 2024-05-17 08:14:00.000000 midi_beeper-1.8/midi_beeper/__main__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-17 08:14:01.085437 midi_beeper-1.8/midi_beeper.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3749 2024-05-17 08:14:01.000000 midi_beeper-1.8/midi_beeper.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      242 2024-05-17 08:14:01.000000 midi_beeper-1.8/midi_beeper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-17 08:14:01.000000 midi_beeper-1.8/midi_beeper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       62 2024-05-17 08:14:01.000000 midi_beeper-1.8/midi_beeper.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-17 08:14:01.000000 midi_beeper-1.8/midi_beeper.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-17 08:14:01.085437 midi_beeper-1.8/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3869 2024-05-17 08:14:00.000000 midi_beeper-1.8/setup.py
```

### Comparing `midi_beeper-1.79.1/LICENSE` & `midi_beeper-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `midi_beeper-1.79.1/PKG-INFO` & `midi_beeper-1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midi_beeper
-Version: 1.79.1
+Version: 1.8
 Summary: Play MIDI files using piezo beepers and other sounders
 Home-page: http://ssb22.user.srcf.net/mwrhome/midi-beeper.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
 Platform: all
 Classifier: Programming Language :: Python :: 2
```

### Comparing `midi_beeper-1.79.1/midi_beeper/__main__.py` & `midi_beeper-1.8/midi_beeper/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # (can be run in either Python 2 or Python 3)
 
 # MIDI beeper (plays MIDI without sound hardware)
-# Version 1.79, (c) 2007-2010,2015-2024 Silas S. Brown
+# Version 1.8, (c) 2007-2010,2015-2024 Silas S. Brown
 # License: Apache 2 (see below)
 
 # MIDI beeper is a Python program to play MIDI by beeping
 # through the computer's beeper instead of using proper
 # sound circuits.  It emulates chords/polyphony.
 # It sounds awful, but it might be useful when no sound device
 # is attached.  It should work on any machine that has the
@@ -45,16 +45,22 @@
 # Can also get 2 macOS voices to sing text:
 # "Organ" 2nd octave Bb to 5th octave D
 # "Joelle" (less melodious) 4th C# to 5th C#
 # force_monophonic is implied with these, and the "sox" command is also required.
 # No melisma; likely works best with patter songs.
 mac_voice = "" # or run with --Organ or --Joelle
 # put syllables into environment variable SaySyls
-# (comma separated)
+# (comma separated; may need to change spelling)
 mac_voice_praat_correction = 0 # or run with --praat requires Praat, recommended for Joelle
+voice_json = 0 # or run with --json: put environ
+# variable SingWords to space-separated words with
+# hyphen-separated syllables, preceded by singer
+# names in [...], for podcast:transcript on stdout
+# tested on Anytime Player and Anemone DAISY Maker
+Anytime_Player_bug_workaround = 1
 
 force_monophonic = 0  # set this to 1 to have only the top line (not normally necessary)
 
 maxTime = 0 # set to number of seconds (or set maxTime environment variable) to limit length of playback, 0 = unlimited
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -91,20 +97,21 @@
 if delArg('--bbc-ssd'): bbc_ssd=bbc_micro=1
 if delArg('--bbc-sdl'): bbc_sdl=bbc_micro=1
 if delArg('--grub'): grub=1
 if delArg('--qbasic'): qbasic=1
 if delArg('--Organ'): mac_voice="Organ"
 if delArg('--Joelle'): mac_voice="Joelle"
 if delArg('--praat'): mac_voice_praat_correction=1
+if delArg('--json'): voice_json=1
 assert not (bbc_sdl and (bbc_binary or bbc_ssd)), "bbc_sdl not compatible with bbc_binary or bbc_ssd"
 
 on_riscos = sys.platform.lower().find("riscos")>=0
 if on_riscos and not (bbc_micro or acorn_electron): riscos_Maestro = 1
 elif not aplay: aplay=int(os.environ.get("APLAY_VOL",0))
-if riscos_Maestro or bbc_micro or acorn_electron or grub or qbasic or mac_voice: aplay = 0
+if riscos_Maestro or bbc_micro or acorn_electron or grub or qbasic or mac_voice or voice_json: aplay = 0
 
 # To add a new type of beeper, get the following 'if' block to do any necessary global setup and to define the appropriate version of the per-file init() and of add_midi_note_chord(), then check the 'if' after 'ensure flushed' at end, and quantiseTo logic
 if aplay:
   rate = 8000 # can just about manage 3 or 4 channels on a Raspberry Pi if it isn't doing anything else
   o = os.popen("aplay -q -t raw -c 1 -f U8 -r %d" % rate,"w")
   try:
     oWrap,o = o,o.buffer # Python 3
@@ -342,14 +349,49 @@
       open('%d.praat' % pid, 'w').write('Read from file... %d.wav\nChange gender... 75.0 600.0 1.0 %d 1.0 1.0\nnowarn Write to WAV file... %d-1.wav\nRemove\n' % (pid,to_freq(note),pid)) # misnomer: this is NOT really changing gender with these parameters, it's normalising frequency (it's the same trick I did to get Yali's Mandarin first tone syllables all the same pitch for Gradint in 2008)
       os.system('/Applications/Praat.app/Contents/MacOS/Praat %d.praat' % pid)
       os.remove('%d.wav' % pid)
       os.remove('%d.praat' % pid)
       b=os.popen('sox %d-1.wav -t raw -r 44100 -c 1 -b 16 -' % pid)
       pcmData[-1] = (b.buffer if hasattr(b,'buffer') else b).read()
       os.remove('%d-1.wav' % pid)
+elif voice_json:
+  force_monophonic = 1
+  def init():
+    global SingWords,currentSpeaker,microsecsSoFar,sylsLeft
+    SingWords = os.environ["SingWords"].split()
+    SingWords.reverse() # so can use pop()
+    currentSpeaker = "singer"
+    microsecsSoFar = int(os.environ.get("SingMicrosecsOffset","0")) # (in case it won't be at the very start of the audio)
+    sylsLeft = 0
+    print('{"version":"1.0.0","segments":[')
+  def setupNextWord():
+    isSpeaker = 0
+    while True:
+      word = SingWords.pop()
+      global currentSpeaker
+      if word.startswith('[') or isSpeaker:
+        if word.startswith('['): currentSpeaker=""
+        currentSpeaker += word.replace("[","").replace("]","")
+        isSpeaker = not word.endswith(']')
+        if isSpeaker: currentSpeaker += " "
+      else:
+        global currentWord,sylsLeft ; currentWord,sylsLeft = word.replace('-',''),len(word.split('-'))
+        if Anytime_Player_bug_workaround: # v1.3.5 drops space before single-letter words
+          while SingWords and len(SingWords[-1])==1:
+            currentWord += " "+SingWords.pop()
+            sylsLeft += 1
+        break
+  def add_midi_note_chord(noteNos,microsecs):
+    global microsecsSoFar, sylsLeft, wordStartMS
+    startM,microsecsSoFar = microsecsSoFar,microsecsSoFar+microsecs
+    if not noteNos or not microsecs: return
+    if not sylsLeft:
+      wordStartMS = startM ; setupNextWord()
+    sylsLeft -= 1
+    if not sylsLeft: print('{"speaker":"%s","startTime":%g,"endTime":%g,"body":"%s"}%s' % (currentSpeaker,wordStartMS/1000000.0,microsecsSoFar/1000000.0,currentWord,(',' if SingWords else ((',{"speaker":"%s","startTime":%g,"endTime":%g,"body":""}' % (currentSpeaker,microsecsSoFar/1000000.0,microsecsSoFar/1000000.0)) if Anytime_Player_bug_workaround else '')))) # (v1.3.5 won't display last word so add a placebo)
 elif qbasic:
   def init():
     global basData, dedup_microsec_quantise
     basData = [b'PLAY "T255L64MLMB"']
     dedup_microsec_quantise = 60000000/255/(64/4)
     basData+=[b'ON PLAY(1) GOSUB playTune\nr=0:PLAY ON:GOSUB playTune\nPRINT "Press any key to stop"\nDO: LOOP UNTIL INKEY$ <> ""\nEND\nplayTune:\nIF r<=0 THEN READ p$,r\nIF p$ = "@" THEN END\nPLAY p$\nr = r - 1\nRETURN']
   def add_midi_note_chord(noteNos,microsecs):
@@ -866,15 +908,15 @@
 
 if acorn_electron: name = "MIDI to Acorn Electron"
 elif (bbc_micro or bbc_micro==[]): name = "MIDI to BBC Micro"
 elif riscos_Maestro: name = "MIDI to Maestro"
 else: name = "MIDI Beeper"
 sys.stderr.write(name+" (c) 2007-2010, 2015-2024 Silas S. Brown.  License: Apache 2\n")
 if len(sys.argv)<2:
-    sys.stderr.write("Syntax: python midi-beeper.py [options] MIDI-filename ...\nOptions: --bbc | --electron | --bbc-binary | --bbc-ssd | --maestro | --grub | --qbasic | --Organ | --Joelle\n")
+    sys.stderr.write("Syntax: python midi-beeper.py [options] MIDI-filename ...\nOptions: --bbc | --electron | --bbc-binary | --bbc-ssd | --bbc-sdl | --maestro | --grub | --qbasic | --Organ | --Joelle (--praat --json)\n")
     sys.exit(1)
 try: xrange
 except: xrange = range # Python 3
 for midiFile in sys.argv[1:]:
     init() ; dedup_chord,dedup_microsec = [],0
     dedup_microsec_error = 0
     sys.stderr.write("Parsing MIDI file "+midiFile+"\n")
@@ -903,14 +945,15 @@
         basFile = midiFile.replace(os.extsep+"midi","").replace(os.extsep+"mid","")+os.extsep+"bas"
         open(basFile,'wb').write(b'\n'.join(basData+[b'DATA @,0\n']))
         sys.stderr.write("Wrote "+basFile+"\n")
     elif mac_voice:
         wavFile = midiFile.replace(os.extsep+"midi","").replace(os.extsep+"mid","")+os.extsep+"wav"
         w=os.popen('sox -t raw -r 44100 -c 1 -b 16 -e signed-integer - '+wavFile,'w')
         (w.buffer if hasattr(w,'buffer') else w).write(b''.join(pcmData)) ; w.close() ; sys.stderr.write("Wrote "+wavFile+"\n")
+    elif voice_json: print("]}")
     elif not aplay and not grub:
         sys.stderr.write("Playing "+midiFile+"\n")
         runBeep(" ".join(cumulative_params))
 if bbc_ssd and bbc_files:
   ssdFile=os.environ.get("DFS_TITLE","tunes")+".ssd"
   sys.stderr.write("Writing output to %s\n" % ssdFile)
   open(ssdFile,"wb").write(make_bbcMicro_DFS_image(bbc_files))
```

### Comparing `midi_beeper-1.79.1/midi_beeper.egg-info/PKG-INFO` & `midi_beeper-1.8/midi_beeper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midi-beeper
-Version: 1.79.1
+Version: 1.8
 Summary: Play MIDI files using piezo beepers and other sounders
 Home-page: http://ssb22.user.srcf.net/mwrhome/midi-beeper.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
 Platform: all
 Classifier: Programming Language :: Python :: 2
```

### Comparing `midi_beeper-1.79.1/setup.py` & `midi_beeper-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages;setup(name='midi_beeper',version='1.79.1',entry_points={'console_scripts':['midi-beeper=midi_beeper.__main__:placebo']},license='Apache 2',platforms='all',url='http://ssb22.user.srcf.net/mwrhome/midi-beeper.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Play MIDI files using piezo beepers and other sounders',long_description=r'''# midi-beeper
+from setuptools import setup, find_packages;setup(name='midi_beeper',version='1.8',entry_points={'console_scripts':['midi-beeper=midi_beeper.__main__:placebo']},license='Apache 2',platforms='all',url='http://ssb22.user.srcf.net/mwrhome/midi-beeper.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Play MIDI files using piezo beepers and other sounders',long_description=r'''# midi-beeper
 MIDI Beeper from http://ssb22.user.srcf.net/mwrhome/midi-beeper.html
 
 MIDI Beeper is a program to play MIDI files on Linux/BSD by beeping through the computer’s beeper instead of using proper sound circuits. If you try to play chords or polyphony, it will rapidly switch between alternate notes like an old office telephone. It sounds awful, but it might be useful when you really have to play a MIDI file but have no sound device attached. It should work on any machine that has the “beep” command (install “beep” package from your Linux/Unix package manager). It has been tested on a PC speaker and on an NSLU2’s internal speaker.
 
 On the NSLU2, playing music with beep works in Debian 4 (Etch, 2007) but not so well in Debian 5 (Lenny, 2012); you can try compiling this [modified beep.c](http://ssb22.user.srcf.net/mwrhome/beep.c) instead (remember the chmod 4755 mentioned in the man page). I haven’t tried it on more recent distros because my NSLU2 power supply failed and I upgraded to a Raspberry Pi.
 
 MIDI Beeper can also generate polyphonic square waves itself and feed them to `aplay`, which might be useful if you need a small MIDI player on a Raspberry Pi running Linux, although too many sound channels can slow this down as it’s only a Python script.
```

