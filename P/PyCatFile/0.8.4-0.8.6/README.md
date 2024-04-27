# Comparing `tmp/pycatfile-0.8.4.tar.gz` & `tmp/pycatfile-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatfile-0.8.4.tar", last modified: Thu Apr 25 17:34:21 2024, max compression
+gzip compressed data, was "pycatfile-0.8.6.tar", last modified: Fri Apr 26 23:59:29 2024, max compression
```

## Comparing `pycatfile-0.8.4.tar` & `pycatfile-0.8.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:34:21.128090 pycatfile-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-25 17:34:13.000000 pycatfile-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-25 17:34:21.128090 pycatfile-0.8.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:34:21.128090 pycatfile-0.8.4/PyCatFile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-25 17:34:21.000000 pycatfile-0.8.4/PyCatFile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 17:34:21.000000 pycatfile-0.8.4/PyCatFile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:34:21.000000 pycatfile-0.8.4/PyCatFile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 17:34:21.000000 pycatfile-0.8.4/PyCatFile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:34:21.000000 pycatfile-0.8.4/PyCatFile.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 17:34:13.000000 pycatfile-0.8.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    12666 2024-04-25 17:34:13.000000 pycatfile-0.8.4/catfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4969 2024-04-25 17:34:13.000000 pycatfile-0.8.4/neocatfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   357858 2024-04-25 17:34:13.000000 pycatfile-0.8.4/pycatfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 17:34:21.128090 pycatfile-0.8.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5451 2024-04-25 17:34:13.000000 pycatfile-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:59:29.516924 pycatfile-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-26 23:59:21.000000 pycatfile-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-26 23:59:29.516924 pycatfile-0.8.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:59:29.516924 pycatfile-0.8.6/PyCatFile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-26 23:59:29.000000 pycatfile-0.8.6/PyCatFile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 23:59:29.000000 pycatfile-0.8.6/PyCatFile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 23:59:29.000000 pycatfile-0.8.6/PyCatFile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 23:59:29.000000 pycatfile-0.8.6/PyCatFile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 23:59:29.000000 pycatfile-0.8.6/PyCatFile.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 23:59:21.000000 pycatfile-0.8.6/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12671 2024-04-26 23:59:21.000000 pycatfile-0.8.6/catfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4969 2024-04-26 23:59:21.000000 pycatfile-0.8.6/neocatfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   361778 2024-04-26 23:59:21.000000 pycatfile-0.8.6/pycatfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-26 23:59:29.516924 pycatfile-0.8.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5451 2024-04-26 23:59:21.000000 pycatfile-0.8.6/setup.py
```

### Comparing `pycatfile-0.8.4/LICENSE` & `pycatfile-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycatfile-0.8.4/PKG-INFO` & `pycatfile-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.8.4
+Version: 0.8.6
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `pycatfile-0.8.4/PyCatFile.egg-info/PKG-INFO` & `pycatfile-0.8.6/PyCatFile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.8.4
+Version: 0.8.6
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `pycatfile-0.8.4/catfile.py` & `pycatfile-0.8.6/catfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: catfile.py - Last Update: 4/25/2024 Ver. 0.8.4 RC 1 - Author: cooldude2k $
+    $FileInfo: catfile.py - Last Update: 4/26/2024 Ver. 0.8.6 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import sys, argparse, pycatfile, binascii;
 
 rarfile_support = pycatfile.rarfile_support;
 py7zr_support = pycatfile.py7zr_support;
@@ -125,15 +125,15 @@
   elif(checkcompressfile=="catfile"):
    pycatfile.RePackArchiveFile(getargs.input, getargs.output, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
   elif(rarfile_support and checkcompressfile=="rarfile"):
    pycatfile.PackArchiveFileFromRarFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
   elif(py7zr_support and checkcompressfile=="7zipfile"):
    pycatfile.PackArchiveFileFromSevenZipFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
   else:
-   sys.exit(1)
+   sys.exit(1);
  else:
   pycatfile.PackArchiveFile(getargs.input, getargs.output, getargs.text, getargs.compression, getargs.level, False, getargs.checksum, [], fnamelist, getargs.verbose, False);
 
 elif should_repack:
  if getargs.convert:
   checkcompressfile = pycatfile.CheckCompressionSubType(getargs.input, fnamelist, True);
   if(checkcompressfile=="tarfile"):
@@ -143,15 +143,15 @@
   elif(checkcompressfile=="catfile"):
    pycatfile.RePackArchiveFile(getargs.input, getargs.output, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
   elif(rarfile_support and checkcompressfile=="rarfile"):
    pycatfile.PackArchiveFileFromRarFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
   elif(py7zr_support and checkcompressfile=="7zipfile"):
    pycatfile.PackArchiveFileFromSevenZipFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
   else:
-   sys.exit(1)
+   sys.exit(1);
  else:
   pycatfile.RePackArchiveFile(getargs.input, getargs.output, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
 
 elif should_extract:
  if getargs.convert:
   checkcompressfile = pycatfile.CheckCompressionSubType(getargs.input, fnamelist, True);
   tempout = BytesIO();
@@ -162,15 +162,15 @@
   elif(checkcompressfile=="catfile"):
    pycatfile.RePackArchiveFile(getargs.input, tempout, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
   elif(rarfile_support and checkcompressfile=="rarfile"):
    pycatfile.PackArchiveFileFromRarFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
   elif(py7zr_support and checkcompressfile=="7zipfile"):
    pycatfile.PackArchiveFileFromSevenZipFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
   else:
-   sys.exit(1)
+   sys.exit(1);
   getargs.input = tempout;
  pycatfile.UnPackArchiveFile(getargs.input, getargs.output, False, 0, 0, getargs.skipchecksum, fnamelist, getargs.verbose, getargs.preserve, getargs.preserve, False);
 
 elif should_list:
  if getargs.convert:
   checkcompressfile = pycatfile.CheckCompressionSubType(getargs.input, fnamelist, True);
   if(checkcompressfile=="tarfile"):
@@ -180,15 +180,15 @@
   elif(checkcompressfile=="catfile"):
    pycatfile.ArchiveFileListFiles(getargs.input, 0, 0, getargs.skipchecksum, fnamelist, getargs.verbose, False);
   elif(rarfile_support and checkcompressfile=="rarfile"):
    pycatfile.RarFileListFiles(getargs.input, getargs.verbose, False);
   elif(py7zr_support and checkcompressfile=="7zipfile"):
    pycatfile.SevenZipFileListFiles(getargs.input, getargs.verbose, False);
   else:
-   sys.exit(1)
+   sys.exit(1);
  else:
   pycatfile.ArchiveFileListFiles(getargs.input, 0, 0, getargs.skipchecksum, fnamelist, getargs.verbose, False);
 
 elif should_validate:
  if getargs.convert:
   checkcompressfile = pycatfile.CheckCompressionSubType(getargs.input, fnamelist, True);
   tempout = BytesIO();
@@ -199,15 +199,15 @@
   elif(checkcompressfile=="catfile"):
    pycatfile.RePackArchiveFile(getargs.input, tempout, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
   elif(rarfile_support and checkcompressfile=="rarfile"):
    pycatfile.PackArchiveFileFromRarFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
   elif(py7zr_support and checkcompressfile=="7zipfile"):
    pycatfile.PackArchiveFileFromSevenZipFile(getargs.input, tempout, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
   else:
-   sys.exit(1)
+   sys.exit(1);
   getargs.input = tempout;
  fvalid = pycatfile.ArchiveFileValidate(getargs.input, fnamelist, getargs.verbose, False);
  if(not getargs.verbose):
   import sys, logging;
   logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
  if(fvalid):
   pycatfile.VerbosePrintOut("File is valid: \n" + str(getargs.input));
```

### Comparing `pycatfile-0.8.4/neocatfile.py` & `pycatfile-0.8.6/neocatfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: neocatfile.py - Last Update: 4/25/2024 Ver. 0.8.4 RC 1 - Author: cooldude2k $
+    $FileInfo: neocatfile.py - Last Update: 4/26/2024 Ver. 0.8.6 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 import argparse
 import pycatfile
 
 # Compatibility layer for Python 2 and 3 input
```

### Comparing `pycatfile-0.8.4/pycatfile.py` & `pycatfile-0.8.6/pycatfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: pycatfile.py - Last Update: 4/25/2024 Ver. 0.8.4 RC 1 - Author: cooldude2k $
+    $FileInfo: pycatfile.py - Last Update: 4/26/2024 Ver. 0.8.6 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import io, os, re, sys, time, stat, zlib, base64, shutil, socket, hashlib, datetime, logging, binascii, tempfile, zipfile, platform;
 from ftplib import FTP, FTP_TLS;
 if(sys.version[0]=="2"):
  from urlparse import urlparse, urlunparse;
@@ -167,19 +167,19 @@
 __file_format_ver__ = "001";
 __use_new_style__ = True;
 __use_advanced_list__ = True;
 __use_alt_inode__ = False;
 __file_format_list__ = [__file_format_name__, __file_format_magic__, __file_format_lower__, __file_format_len__, __file_format_hex__, __file_format_delimiter__, __file_format_ver__, __use_new_style__, __use_advanced_list__, __use_alt_inode__];
 __project__ = __program_name__;
 __project_url__ = "https://github.com/GameMaker2k/PyCatFile";
-__version_info__ = (0, 8, 4, "RC 1", 1);
-__version_date_info__ = (2024, 4, 25, "RC 1", 1);
+__version_info__ = (0, 8, 6, "RC 1", 1);
+__version_date_info__ = (2024, 4, 26, "RC 1", 1);
 __version_date__ = str(__version_date_info__[0]) + "." + str(__version_date_info__[1]).zfill(2) + "." + str(__version_date_info__[2]).zfill(2);
 __revision__ = __version_info__[3];
-__revision_id__ = "$Id: 3272c8de059524fad39bf09522853fa0322dc3f6 $";
+__revision_id__ = "$Id: d45dc765c1f1cbdec9b8820a0e3bcda7bb6e3940 $";
 if(__version_info__[4] is not None):
  __version_date_plusrc__ = __version_date__ + "-" + str(__version_date_info__[4]);
 if(__version_info__[4] is None):
  __version_date_plusrc__ = __version_date__;
 if(__version_info__[3] is not None):
  __version__ = str(__version_info__[0]) + "." + str(__version_info__[1]) + "." + str(__version_info__[2]) + " " + str(__version_info__[3]);
 if(__version_info__[3] is None):
@@ -3827,14 +3827,32 @@
    return catfp
   else:
    catfp.close()
    return True;
 
 create_alias_function("Pack", __file_format_name__, "FromSevenZipFile", PackArchiveFileFromSevenZipFile);
 
+def PackArchiveFileFromInFile(infile, outfile, compression="auto", compressionlevel=None, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
+ checkcompressfile = CheckCompressionSubType(infile, formatspecs, True);
+ if(checkcompressfile=="tarfile"):
+  return PackArchiveFileFromTarFile(infile, outfile, compression, compressionlevel, checksumtype, extradata, formatspecs, verbose, returnfp);
+ elif(checkcompressfile=="zipfile"):
+  return PackArchiveFileFromZipFile(infile, outfile, compression, compressionlevel, checksumtype, extradata, formatspecs, verbose, returnfp);
+ elif(checkcompressfile=="catfile"):
+  return RePackArchiveFile(infile, outfile, compression, compressionlevel, False, 0, 0, checksumtype, False, extradata, formatspecs, verbose, returnfp);
+ elif(rarfile_support and checkcompressfile=="rarfile"):
+  return PackArchiveFileFromRarFile(infile, outfile, compression, compressionlevel, checksumtype, extradata, formatspecs, verbose, returnfp);
+ elif(py7zr_support and checkcompressfile=="7zipfile"):
+  return PackArchiveFileFromSevenZipFile(infile, outfile, compression, compressionlevel, checksumtype, extradata, formatspecs, verbose, returnfp);
+ else:
+  return False;
+ return False;
+
+create_alias_function("Pack", __file_format_name__, "FromInFile", PackArchiveFileFromInFile);
+
 def ArchiveFileSeekToFileNum(infile, seekto=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__, returnfp=False):
  if(hasattr(infile, "read") or hasattr(infile, "write")):
   catfp = infile;
   catfp.seek(0, 0);
   catfp = UncompressArchiveFile(catfp, formatspecs);
   checkcompressfile = CheckCompressionSubType(catfp, formatspecs, True);
   if(checkcompressfile=="tarfile"):
@@ -4851,14 +4869,30 @@
 if(py7zr_support):
  def SevenZipFileToArray(infile, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__, returnfp=False):
   catfp = BytesIO();
   catfp = PackArchiveFileFromSevenZipFile(infile, catfp, "auto", None, "crc32", [], formatspecs, False, True);
   listcatfiles = ArchiveFileToArray(catfp, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
   return listcatfiles;
 
+def InFileToArray(infile, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__, returnfp=False):
+ checkcompressfile = CheckCompressionSubType(infile, formatspecs, True);
+ if(checkcompressfile=="tarfile"):
+  return TarFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
+ elif(checkcompressfile=="zipfile"):
+  return ZipFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
+ elif(checkcompressfile=="catfile"):
+  return ArchiveFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
+ elif(rarfile_support and checkcompressfile=="rarfile"):
+  return RarFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
+ elif(py7zr_support and checkcompressfile=="7zipfile"):
+  return SevenZipFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
+ else:
+  return False;
+ return False;
+
 def ListDirToArrayAlt(infiles, dirlistfromtxt=False, followlink=False, listonly=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False):
  catver = formatspecs[6];
  fileheaderver = str(int(catver.replace(".", "")));
  fileheader = AppendNullByte(formatspecs[1] + fileheaderver, formatspecs[5]);
  advancedlist = formatspecs[8];
  altinode = formatspecs[9];
  infilelist = [];
@@ -6152,14 +6186,30 @@
    if(int(fsize)>0 and listonly):
     fcontents = "";
     pyhascontents = False;
    catlist['ffilelist'].update({fileidnum: {'fid': fileidnum, 'fidalt': fileidnum, 'fheadersize': int(catheaersize, 16), 'fhstart': catfhstart, 'fhend': catfhend, 'ftype': ftype, 'fname': fname, 'fbasedir': fbasedir, 'flinkname': flinkname, 'fsize': fsize, 'fatime': fatime, 'fmtime': fmtime, 'fctime': fctime, 'fbtime': fbtime, 'fmode': fmode, 'fchmode': fchmode, 'ftypemod': ftypemod, 'fwinattributes': fwinattributes, 'fuid': fuid, 'funame': funame, 'fgid': fgid, 'fgname': fgname, 'finode': finode, 'flinkcount': flinkcount, 'fminor': fdev_minor, 'fmajor': fdev_major, 'frminor': frdev_minor, 'frmajor': frdev_major, 'fchecksumtype': checksumtype, 'fnumfields': catfnumfields + 2, 'frawheader': catheaderdata, 'fextrafields': catfextrafields, 'fextrafieldsize': extrasizelen, 'fextralist': extrafieldslist, 'fheaderchecksum': int(catfileheadercshex, 16), 'fcontentchecksum': int(catfilecontentcshex, 16), 'fhascontents': pyhascontents, 'fcontentstart': catfcontentstart, 'fcontentend': catfcontentend, 'fcontents': fcontents} });
    fileidnum = fileidnum + 1;
   return catlist;
 
+def InFileToArrayAlt(infiles, listonly=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False):
+ checkcompressfile = CheckCompressionSubType(infiles, formatspecs, True);
+ if(checkcompressfile=="tarfile"):
+  return TarFileToArrayAlt(infiles, listonly, checksumtype, extradata, formatspecs, verbose);
+ elif(checkcompressfile=="zipfile"):
+  return ZipFileToArrayAlt(infiles, listonly, checksumtype, extradata, formatspecs, verbose);
+ elif(checkcompressfile=="catfile"):
+  return ArchiveFileToArray(infile, 0, 0, listonly, False, formatspecs, False);
+ elif(rarfile_support and checkcompressfile=="rarfile"):
+  return RarFileToArrayAlt(infiles, listonly, checksumtype, extradata, formatspecs, verbose);
+ elif(py7zr_support and checkcompressfile=="7zipfile"):
+  return SevenZipFileToArrayAlt(infiles, listonly, checksumtype, extradata, formatspecs, verbose);
+ else:
+  return False;
+ return False;
+
 def ListDirToArray(infiles, dirlistfromtxt=False, compression="auto", compressionlevel=None, followlink=False, seekstart=0, seekend=0, listonly=False, skipchecksum=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
  outarray = BytesIO();
  packcat = PackArchiveFile(infiles, outarray, dirlistfromtxt, compression, compressionlevel, followlink, checksumtype, extradata, formatspecs, verbose, True);
  listcatfiles = ArchiveFileToArray(outarray, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
  return listcatfiles;
 
 def ArchiveFileToArrayIndex(infile, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__, returnfp=False):
@@ -7696,14 +7746,30 @@
     VerbosePrintOut(PrintPermissionString(fmode, ftype) + " " + str(str(fuprint) + "/" + str(fgprint) + " " + str(fsize).rjust(15) + " " + member.creationtime.strftime('%Y-%m-%d %H:%M') + " " + printfname));
    lcfi = lcfi + 1;
   if(returnfp):
    return listcatfiles['catfp'];
   else:
    return True;
 
+def InFileListFiles(infile, verbose=False, formatspecs=__file_format_list__, returnfp=False):
+ checkcompressfile = CheckCompressionSubType(infile, formatspecs, True);
+ if(checkcompressfile=="tarfile"):
+  return TarFileListFiles(infile, verbose, returnfp);
+ elif(checkcompressfile=="zipfile"):
+  return ZipFileListFiles(infile, verbose, returnfp);
+ elif(checkcompressfile=="catfile"):
+  return ArchiveFileListFiles(infile, verbose, returnfp);
+ elif(rarfile_support and checkcompressfile=="rarfile"):
+  return RarFileListFiles(infile, verbose, returnfp);
+ elif(py7zr_support and checkcompressfile=="7zipfile"):
+  return SevenZipFileListFiles(infile, verbose, returnfp);
+ else:
+  return False;
+ return False;
+
 def ListDirListFiles(infiles, dirlistfromtxt=False, compression="auto", compressionlevel=None, followlink=False, seekstart=0, seekend=0, skipchecksum=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False, returnfp=False):
  outarray = BytesIO();
  packcat = PackArchiveFile(infiles, outarray, dirlistfromtxt, compression, compressionlevel, followlink, checksumtype, formatspecs, False, True);
  listcatfiles = ArchiveFileListFiles(outarray, seekstart, seekend, skipchecksum, formatspecs, verbose, returnfp);
  return listcatfiles;
 
 def ListDirListFilesAlt(infiles, dirlistfromtxt=False, followlink=False, listonly=False, seekstart=0, seekend=0, skipchecksum=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False, returnfp=False):
@@ -7738,29 +7804,27 @@
 
 if(rarfile_support):
  def PackArchiveFileFromRarFileAlt(infile, outfile, compression="auto", compressionlevel=None, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
   outarray = RarFileToArrayAlt(infile, False, checksumtype, extradata, formatspecs, False);
   listcatfiles = RePackArchiveFile(outarray, outfile, compression, compressionlevel, False, checksumtype, False, extradata, formatspecs, verbose, returnfp);
   return listcatfiles;
 
-if(rarfile_support):
- create_alias_function("Pack", __file_format_name__, "FromRarFileAlt", PackArchiveFileFromRarFileAlt);
+create_alias_function("Pack", __file_format_name__, "FromRarFileAlt", PackArchiveFileFromRarFileAlt);
 
 if(not py7zr_support):
  def PackArchiveFileFromSevenZipFileAlt(infile, outfile, compression="auto", compressionlevel=None, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
   return False;
 
 if(py7zr_support):
  def PackArchiveFileFromSevenZipFileAlt(infile, outfile, compression="auto", compressionlevel=None, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
   outarray = SevenZipFileToArrayAlt(infile, False, checksumtype, extradata, formatspecs, False);
   listcatfiles = RePackArchiveFile(outarray, outfile, compression, compressionlevel, False, checksumtype, False, extradata, formatspecs, verbose, returnfp);
   return listcatfiles;
 
-if(py7zr_support):
- create_alias_function("Pack", __file_format_name__, "FromSevenZipFileAlt", PackArchiveFileFromSevenZipFileAlt);
+create_alias_function("Pack", __file_format_name__, "FromSevenZipFileAlt", PackArchiveFileFromSevenZipFileAlt);
 
 def download_file_from_ftp_file(url):
  urlparts = urlparse(url);
  file_name = os.path.basename(urlparts.path);
  file_dir = os.path.dirname(urlparts.path);
  if(urlparts.username is not None):
   ftp_username = urlparts.username;
```

### Comparing `pycatfile-0.8.4/setup.py` & `pycatfile-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2016-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2016-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2016-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: setup.py - Last Update: 4/25/2024 Ver. 0.8.4 RC 1 - Author: cooldude2k $
+    $FileInfo: setup.py - Last Update: 4/26/2024 Ver. 0.8.6 RC 1 - Author: cooldude2k $
 '''
 
 import os, re, sys, pkg_resources;
 from setuptools import setup;
 
 verinfofilename = os.path.realpath("."+os.path.sep+os.path.sep+"pycatfile.py");
 verinfofile = open(verinfofilename, "r");
```

