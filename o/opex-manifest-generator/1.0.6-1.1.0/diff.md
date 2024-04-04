# Comparing `tmp/opex_manifest_generator-1.0.6.tar.gz` & `tmp/opex_manifest_generator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opex_manifest_generator-1.0.6.tar", last modified: Tue Feb 20 15:49:08 2024, max compression
+gzip compressed data, was "opex_manifest_generator-1.1.0.tar", last modified: Thu Apr  4 10:05:15 2024, max compression
```

## Comparing `opex_manifest_generator-1.0.6.tar` & `opex_manifest_generator-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-02-20 15:49:08.075791 opex_manifest_generator-1.0.6/
--rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.0.6/LICENSE.md
--rw-rw-rw-   0        0        0      701 2024-02-20 15:49:08.064919 opex_manifest_generator-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    15894 2024-02-20 15:47:17.000000 opex_manifest_generator-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-02-20 15:49:07.992468 opex_manifest_generator-1.0.6/opex_manifest_generator/
--rw-rw-rw-   0        0        0      439 2024-02-20 12:38:50.000000 opex_manifest_generator-1.0.6/opex_manifest_generator/__init__.py
--rw-rw-rw-   0        0        0     5368 2024-02-20 12:40:00.000000 opex_manifest_generator-1.0.6/opex_manifest_generator/cli.py
--rw-rw-rw-   0        0        0      611 2024-02-18 22:03:55.000000 opex_manifest_generator-1.0.6/opex_manifest_generator/common.py
--rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.0.6/opex_manifest_generator/hash.py
--rw-rw-rw-   0        0        0    19429 2024-02-20 12:41:39.000000 opex_manifest_generator-1.0.6/opex_manifest_generator/opex_manifest.py
--rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.0.6/opex_manifest_generator/test_cli.py
--rw-rw-rw-   0        0        0       21 2024-02-20 15:21:37.000000 opex_manifest_generator-1.0.6/opex_manifest_generator/version.py
-drwxrwxrwx   0        0        0        0 2024-02-20 15:49:08.064919 opex_manifest_generator-1.0.6/opex_manifest_generator.egg-info/
--rw-rw-rw-   0        0        0      701 2024-02-20 15:49:07.000000 opex_manifest_generator-1.0.6/opex_manifest_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      564 2024-02-20 15:49:07.000000 opex_manifest_generator-1.0.6/opex_manifest_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-20 15:49:07.000000 opex_manifest_generator-1.0.6/opex_manifest_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-02-20 15:49:07.000000 opex_manifest_generator-1.0.6/opex_manifest_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-02-20 15:49:07.000000 opex_manifest_generator-1.0.6/opex_manifest_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-02-20 15:49:07.000000 opex_manifest_generator-1.0.6/opex_manifest_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      819 2024-02-20 15:35:18.000000 opex_manifest_generator-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-20 15:49:08.075791 opex_manifest_generator-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 10:05:15.988477 opex_manifest_generator-1.1.0/
+-rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0      701 2024-04-04 10:05:15.985465 opex_manifest_generator-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    19695 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 10:05:15.933873 opex_manifest_generator-1.1.0/opex_manifest_generator/
+-rw-rw-rw-   0        0        0      439 2024-02-20 12:38:50.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/__init__.py
+-rw-rw-rw-   0        0        0     6190 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/cli.py
+-rw-rw-rw-   0        0        0      676 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/common.py
+-rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/hash.py
+-rw-rw-rw-   0        0        0    23661 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/opex_manifest.py
+-rw-rw-rw-   0        0        0    20008 2024-03-26 21:35:58.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/opex_manifest_v1.py
+-rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/test_cli.py
+-rw-rw-rw-   0        0        0       21 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/version.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:05:15.974175 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-04-04 10:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2024-04-04 10:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-04 10:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-04-04 10:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-04 10:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      819 2024-04-04 10:00:33.000000 opex_manifest_generator-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 10:05:15.989475 opex_manifest_generator-1.1.0/setup.cfg
```

### Comparing `opex_manifest_generator-1.0.6/LICENSE.md` & `opex_manifest_generator-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.0.6/PKG-INFO` & `opex_manifest_generator-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.0.6
+Version: 1.1.0
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.0.6/README.md` & `opex_manifest_generator-1.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -27,176 +27,228 @@
 - Assignment of standard and custom xml metadata templates. \**Custom XML's require a small bit of setup*
 - These fields are all 'drop-in', so only the fields as they are required need to be added. 
 
 All these features can be combined to create extensive and robust Opex files for transfer.
 
 ## Prerequisites
 
-Python Version 3.8+ is recommended; the program is OS independent and should work on Windows, MacOS and Linux.
+Python Version 3.8+ is recommended; the program is OS independent and works on Windows, MacOS and Linux.
 
 The following modules are utilised and installed with the package:
 - auto_classification_generator
 - pandas
 - openpyxl
 - lxml
 
 ## Installation
 
 To install the package, simply run: `pip install -U opex_manifest_generator`
 
 ## Usage
 
 ### Folder Manifest Generation
+
 The basic version of the program will generate only folder manifests, this acts recursively, so every folder within that folder will have an Opex generated.
 
 To run open up a terminal and run the command:
 
-`opex_generate {path/to/your/folder}`
-
-Replacing `{path/to/your/folder}`; for instance, on Windows this looks like:
+`opex_generate "{path/to/your/folder}"`
 
-`opex_generate "C:\Users\Christopher\Downloads\"`
+Replacing `{path/to/your/folder}` with your folder path in quotations; for instance, on Windows this looks like:
 
-This is geared towards usage with the Opex Ingest Workflow with Folder Manifest Requirement enabled. By creating these opexes, we can ensure that the workflow will check the .
+`opex_generate "C:\Users\Christopher\Downloads"`
 
 ### Fixity Generation
 
-To generate a fixity for each file within a given folder, we can add the `-fx` option.
+To generate a fixity for each file within a given folder and add it to the Opex, you can use the `-fx` option.
 
 `opex_generate "C:\Users\Christopher\Downloads\" -fx`
 
-To utilise a different algorithm:
+By default this will run with the SHA-1 algorithm. To utilise a different algorithm, specify it like so:
 
-`opex_generate "C:\Users\Christopher\Downloads\" -fx -alg SHA-256`
+`opex_generate "C:\Users\Christopher\Downloads\" -fx SHA-256`
 
-This is intended to add an additional check to the Opex Ingest Workflow and other upload methods, ensuring that the content is safely delivered with matching Hashes.
+You can utilise MD5, SHA-1, SHA-256, SHA-512 algorithms.
 
 ### Zipping 
 
-We can also utilise the zip option to bundle the opex and content into a zip file. For use with manual ingests or for Starter / UX2 users.
+You can also utilise the zip option to bundle the opex and content into a zip file. For use with manual ingests or for Starter / UX2 users.
 
-`opex_generate "C:\Users\Christopher\Downloads\" -fx -alg SHA-1 -z`
+`opex_generate "C:\Users\Christopher\Downloads\" -fx SHA-1 -z`
 
-Currently, no files will be removed after the zipping; keep in mind the available space. *Also be aware that running this command multiple times in row will break existing Opex files.
+Currently, no files will be removed after the zipping. Be aware that running this command multiple times in row will break existing Opex's.
 
 ### Clearing Opex's
 
 Mistakes happen! So, the clear option will remove all existing Opex's in a directory.
 
 `opex_generate "C:\Users\Christopher\Downloads\" -clr`
 
-Running this command with no additional options will end the program after clearing the Opex's; if other options are enabled it will proceed with the generation.
+Running this command with no additional options will end the program after clearing the Opex's; if other options are enabled it will proceed with the generation of those Opex's.
 
 ## Filtering note
 
 Currently a number of filters are applied to certain files / folders.
 
 1) Hidden directories / files and those starting with '.' are not included.
 2) Folder's titled 'meta' are not included.
 
+Hidden files and directories can be included by utilising the `--hidden` option.
+
 ## Use with the Auto Classification Generator
 
-Another tool, the Auto Classification Generator, is built-in to this program. While use of this is optional, making use of it allows for some embedding Archival References into the identifier and for Custom imports.
+The Opex Manifest generator becomes much more powerful when utilised with another tool: the Auto Classification Generator, see [here](https://github.com/CPJPRINCE/auto_classification_generator) for further details.
+
+This is built-in to the Opex Manifest Generator and can be utilised to embed identifiers and metadata directly to an Opex or through use of a spreadsheet / CSV file.
 
-Compared to `auto_class`, see here for details, instead of exporting to a spreadsheet, directly embed the references into the Opex file. To avoid potential conflicts, the behaviour differs when compared to utilising the standalone command.
+The Opex Manifest Generator makes use of the auto_class_generator as a module. It's behaviour differs somewhat when compared to utilising the standalone command `auto_class.exe`.
 
-## Basic Generation
+### Auto Classification - Code Generation
 
-To generate an auto classification code, for a given folder, with prefix `ARCH` simply run:
+To generate an auto classification code, call on `-c` option with `catalog` choice. You can also assign a prefix using `-p ARCH`:
 
 `opex_generate -c catalog -p "ARCH" C:\Users\Christopher\Downloads`
 
-This will generate Opex's with an identifier "code" added to each of the files. As described in the Auto Class module, the reference codes will take the hierarchy of the directories.
+This will generate Opex's with an identifier `code` for each of the files / folders. As described in the Auto Class module, the reference codes will take the hierarchy of the directories. You can use the `-s` option to set a starting reference.
 
-To utilising the "Accession" mode of the program:
+You can alternatively utilise the "Accession" / running number mode of generating a code using `-c accession` with prefix `2024`. *To note Accession is currently hard-coded to use "File" mode*:
 
 `opex_generate -c accession -p "2024" C:\Users\Christopher\Downloads`
 
-Or to both:
+Alternatively you can do both Catalogue / Accession at the same time:
 
 `opex_generate -c both -p "ARCH" "2024" C:\Users\Christopher\Downloads`
 
-To note: when using the catalog or accession option, the key `code` is used as the identifier. When using `both`, the Catalog Reference is given the key `code` and the 'Accession' given the key: `accref`. I will make this adjustable in a future update.
+To note: when using the `catalog` option, the key `code` is always used by default. When using `accession` the default key is `accref`. This is currently not adjustable, see [here](### XIP Metadata - Identifiers) for utilising other keys. 
 
-It's possible to also create a 'generic' set of metadata which will take the Title, Description from the basename of the folder/file and set the Security Status to 'Open'. 
+It's possible to also create a `generic` set of metadata which will take the XIP metadata for Title, Description from the basename of the folder/file and will set the Security Status to `open`. 
 
 `opex_generate -c generic C:\Users\Christopher\Downloads`
 
-Many (but not all) of the options available in Auto Classification are available here:
+You can combine generic options with catalog, accession, both to also generate an identifer.
 
-- Setting Start References
-- Clearing Empty Directories
+You can also clear Empty Directory by using `--remove-empty` option. This will also generate 
 
-### Use of the Auto Class spreadsheet as an Input 
+## Auto Classification - Spreadsheet as Input 
 
 This program also supports utilising an Auto Class spreadsheet as an input, utilising the data added into said spreadsheet, instead of generating them on command.
 
-In this way, metadata can set: XIP Metadata fields: Title, Description and Security Status; and XML metadata templates on ingest.
+In this way, metadata can be set on XIP Metadata fields, including:
+ - Title
+ - Description
+ - Security Status
+ - Identifiers
+ - SourceID
 
-#### XIP metadata
+As well as XML metadata templates, including the default templates and custom templates.
+
+### XIP metadata - Title, Description and Security Status
 
 To create the spreadsheet base spreadsheet:
 
 `opex_generate -c catalog -p "ARCH" -ex "C:\Users\Christopher\Downloads"` or `auto_class -p "ARCH" "C:\Users\Christopher\Downloads"` to avoid unnecessary OPEX creation.
 
-In the resultant spreadsheet, add in "Title", "Description", and "Security" as new columns. The column header has to match exactly, including capitalisation; these fields would then be filled in with the relevant data.
+In the resultant spreadsheet, add in "Title", "Description", and "Security" as new columns. The column headers have to match exactly, including capitalisation; these fields would then be filled in with the relevant data.
 
-Once filled in; to initialise the generation: `opex_generate -i "{/path/to/your/spreadsheet.xlsx}" "{/path/to/root/directory}"`
+Once the cells are filled in with data; to initialise the generation run: `opex_generate -i "{/path/to/your/spreadsheet.xlsx}" "{/path/to/root/directory}"`
 
 Ensure that the root directory matches the original directory of the export. In the above case this would be: `opex_generate -i "C:\Users\Christopher\Downloads\meta\Downloads_AutoClass.xlsx" "C:\Users\Christopher\Downloads"`
 
-Please note, if there are any changes to the hierarchy data after the export of the initial spreadsheet, the data may not be assigned correctly.
+To note, the column headers are drop-in, drop-out, meaning you can the columns as and when you need them. You can also leave blank data,the cell you leave blank will simply not these will not be assigned.
+
+To also note, the `Security` must match an existing tag in your system, exactly by it's name.
+
+To also also note, if there are any changes to the hierarchy data, such as a file/folder (not including a 'meta' folder) being removed or added, after the export of the initial spreadsheet, the data may not be assigned correctly.
 
-#### XML Metadata
+### XIP Metadata - Identifiers
 
-To utilise an import with XML Metadata templates, first the XML template has to be stored in the source 'metadata' directory. DC, MODS, GPDR, and EAD templates come with the package, but custom templates can be added and will work 'out-the-box', as long as they are functioning within Preservica. *I will likely change the destination of this directory for easier use.
+Custom Identifiers can be added by naming columns: `"Archive_Reference", "Accession_Reference", "Identifier", or "Identifer:Keyname"`.
+
+If named `Archive_Reference` or `Identifier` the keyname will default to `code`, if named `Accession_Reference` the keyname will default to `accref`. Using the Auto Classification Generator will always generate a column called `Archive_Reference`, you can simply rename or remove this column if not needed. 
+
+To add a custom identifier import, do so like so: `Identifier:MyCodeName`. As many identifier's as needed can be added.
+
+No additional parameter's need to be set in the command line when using Identifier's, addition is detected by default.
+
+### XML Metadata - Basic Templates
+
+To utilise an import with XML Metadata templates, first the XML template has to be stored in the source 'metadata' directory. DC, MODS, GPDR, and EAD templates come with the package.
 
 After exporting an Auto Class spreadsheet, add in additional columns to the spreadsheet; like the XIP data, all fields are optional, and can added on a 'drop-in' basis. You can add in the column header in two ways: 'exactly' or 'flatly'.
 
 An Exactly match requires that the full path from the XML document is added to the column, with parent to child separated by a `/`; 'flatly' requires only a the matching end tag. For example, the below will match to the same `recordIdentifer` field in the mods template:
 
 ```
 Exactly:
 mods:recordInfo/mods:recordIdentifier
 
 Flatly:
 mods:recordIdentifier
 ```
 
-In both cases, the header has to match both namespace and tag and is case sensitive. While using the flat method is easier, be aware that if there's non-unique tags, such as `mods:note`, the flat method will only import to the first match, which might not be it's intended destination. When using the 'exactly' and you have non-unique tags, again such as `mods:note`, you will need add an index in square brackets `[0]` to indicate which tag to assign the data to, like: `mods:note[1] mods:notes[2] ...` The number of field will simply be the order they appear in the XML.
+In both cases, the header has to match both namespace and tag and isI case sensitive. While using the flat method is easier, be aware that if there's non-unique tags, such as `mods:note`, the flat method will only import to the first match, which might not be it's intended destination.
+
+When using the 'exactly' and you have non-unique tags, again such as `mods:note`, you will need add an index in square brackets `[0]` to indicate which tag to assign the data to, like: `mods:note[1] mods:notes[2] ...` The number of field will simply be the order they appear in the XML.
 
-This is all probably easier done, than said :\). For convenance nce *I've also included* (Note to self: ADD THEM!), spreadsheet templates of DC, MODS, GDPR and EAD, with their explicit names in the headers.
+This is all probably easier done, than said :\). For convenience I've also included *(Note to self: ADD THEM!)*, spreadsheet templates of DC, MODS, GDPR and EAD, with their explicit names in the headers.
 
 Once the above is setup, and all the data added; to create the OPEX's simply add `-m` with the chosen method of import `flat|exact`, so:
 `opex_generate -i "{/path/to/your/spreadsheet.xlsx}" "{/path/to/root/directory}" -m flat` or 
 `opex_generate -i "{/path/to/your/spreadsheet.xlsx}" "{/path/to/root/directory}" -m exact`
 
+To note: when you add an XML Metadata column to the XL spreadsheet, it will always add this to the OPEX - even if the cell is left blank... This may be configurable in the future, but for now please be aware of it.
+
+### XML Metadata Templates - Custom Templates
+
+Any custom template can be added to the metadata folder and it will work 'out of the box', as long as they are functioning within Preservica.
+
+All that is necessary to do, is add the XML Template document and then add it to the 'metadata' folder within the site-package files within the program. Then in the spreadsheet you simply need to add neccesary column headers - you can utilise either flat or exact methods as described above. You can then save this as a template for reuse.
+
+*In the future I will likely allow the destination of this directory to be set by an option or adjustable in one way or aanother, for use without having to go into the Site-Packages.*
+
+#### Additional Information
+
+A SourceID can also be set by adding a `SourceID` header. The behaviour of this is not fully tested yet.
+
+Ignoring Files can also be set by adding an `Ignore` header. When this is set to `TRUE` this will skip the generation of an Opex for the specified File or Folder; when done for folder's, the folder Opex will still include any ignored file's in its manifest.
+
+Removing Files or Folders is also possible, by adding a `Removals` header. When this is set to `TRUE`, the specified File or Folder will be removed from the system. As a safeguard this must be enabled by adding the parameter `-rm, --remove`, and confirming. *Currently this process is failing...* 
+
+To note when importing a column for an XML Metadata template that needs to be a boolean IE `TRUE/FALSE`. Please ensure that none are left blank, otherwise these may be imported inaccurately as `1.0` or `0.0`. This is a pandas issue, that I'm not sure how to fix... :/
+
 ## Options
 
 The following options are currently available to run the program with, and can be utilised in various combinations with each other, although some combinations will clash:
 
 ```
 Options:
         -h,     --help          Show Help dialog
 
+        -v,     --version   Display version information                             [boolean]
+
     Opex Options:
 
         -fx,  --fixity      Generate a Fixity Check for files.                      [boolean]
         
         -alg  --algorithm   Set to specify which algorithm to use                   {SHA-1,MD5,SHA-256,SHA-512} 
                             for fixity. Defaults to SHA-1.
         
         -clr, --clear-opex  Will remove all existing Opex folders,                  [boolean]
                             When utilised with no other options, will end
                             the program.
         
         -z,   --zip         Will zip the Opex's with the file itself to create      [boolean]
                             a zip file. Existing file's are currently not removed.
                             ***Use with caution, repeating the command multiple 
-                            times, will break the Opex's.
+                            times in a row, will break the Opex's.
+        
+        --hidden            Will generate Opex's for hidden files and directories   [boolean]
+
+        -rm,  --remove      Will enable removals from a spreadsheet import          [boolean]
+                            *Currently Failing do not use*
 
     Auto Classification Options:
 
         -c,  --autoclass    This will utilise the AutoClassification                {catalog, accession, both, generic,
                             module to generate an Auto Class spreadsheet.            catalog-generic, accesison-generic,
                                                                                      both-generic}
                             There are several options, {catalog} will generate
@@ -205,24 +257,23 @@
                             (Currently this is not configurable).
                             {both} will do Both!
                             {generic} will populate the Title and 
                             Description fields with the folder/file's name,
                             if used in conjunction with one of the above options:
                             {generic-catalog,generic-accession, generic-both}
                             it will do both simultaneously.
-                            For more details on these see the 
-                            auto_classification_generator page.
+                            For more details on these see [here](https://github.com/CPJPRINCE/auto_classification_generator).
         
         -p,   --prefix      Assign a prefix to the Auto Classification,             [string]
                             when utilising {both} fill in like:
                             "catalog-prefix","accession-prefix".            
         
-        -rm,  --empty       Remove and log empty directories in a structure         [boolean]
-                            Log will bee exported to 'meta' / output folder
-
+        -rme, --remove-     Remove and log empty directories in a structure         [boolean]
+                empty       Log will bee exported to 'meta' / output folder
+       
         -o,   --output      Set's the output of the 'meta' folder when              [string] 
                             utilising AutoClass.
                                 
         -s,   --start-ref   Sets the starting Reference in the Auto Class           [int]
                             process.
 
         -i    --input       Set whether to use an Auto Class spreadsheet as an      [string]
@@ -253,19 +304,20 @@
                             Use of metadata requires, an XML document to 
                             be added to the metadata folder, see docs for
                             details (currently in site-packages *may change).
 
         -dmd, --disable-    Will, disable the creation of the meta.                 [boolean]
                 meta-dir    Can also be enabled with output.
   
-        -ex     --export    Set whether to export the Auto Class, default
+        -ex     --export    Set whether to export the Auto Class, default           [boolean]
                             behaviour will not create a new spreadsheet.
 
-        -fmt,   --format    Set whether to export as a CSV or XLSX file.           {csv,xlsx}
+        -fmt,   --format    Set whether to export as a CSV or XLSX file.            {csv,xlsx}
                             Otherwise defaults to xlsx.
+
 ```
 
 ## Future Developments
 
 - Adjust Accession so the different modes can utilised from Opex.
 - Add SourceID as option for use with Auto Class Spreadsheets.
 - Allow for multiple Identifier's to be added with Auto Class Spreadsheets. Currently only 1 or 2 identifiers can be added at a time, under "Archive_Reference" or "Accesion_Refernce". These are also tied to be either "code" or "accref". An Option needs to be added to allow custom setting of identifier...
```

### Comparing `opex_manifest_generator-1.0.6/opex_manifest_generator/common.py` & `opex_manifest_generator-1.1.0/opex_manifest_generator/common.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,11 +11,12 @@
     zip_file = f"{file_path}.zip"
     if not os.path.exists(zip_file):
         with zipfile.ZipFile(zip_file,'w') as z:
             z.write(file_path,os.path.basename(file_path))
             z.write(opex_path,os.path.basename(opex_path))
     else: print(f'A zip file already exists for: {zip_file}')
 
-def win_256_check(path):
+def win_256_check(path: str):
     if len(path) > 255 and sys.platform == "win32":
-        path = "\\\\?\\" + path
+        if path.startswith(u'\\\\?\\'): path = path
+        else: path = u"\\\\?\\" + path
     return path
```

### Comparing `opex_manifest_generator-1.0.6/opex_manifest_generator/hash.py` & `opex_manifest_generator-1.1.0/opex_manifest_generator/hash.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.0.6/opex_manifest_generator/opex_manifest.py` & `opex_manifest_generator-1.1.0/opex_manifest_generator/opex_manifest_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 """
 Opex Manifest Generator tool
 
 This tool is utilised to recusrively generate Opex files for files / directories for use in uploading to Preservica and other OPEX conformin systems.
 
 author: Christopher Prince
 license: Apache License 2.0"
@@ -64,15 +65,15 @@
         self.metadata_flag = metadata_flag
         self.metadata_dir = metadata_dir
         
     def print_running_time(self):
         print(f'Running time: {datetime.now() - self.start_time}')
         time.sleep(1)
     
-    def meta_df_lookup(self,file_path):
+    def meta_df_lookup(self,file_path: str):
         idx = self.df.index[self.df['FullName'] == file_path]
         try:
             if self.title_flag:
                 title = self.df.loc[idx].Title.item()
                 if str(title) == "nan": title = None
             else: title = None
             if self.description_flag: 
@@ -86,25 +87,40 @@
         except Exception as e:
             print(e)
             title = None
             description = None
             security = None
         return title,description,security
     
-    def df_lookup(self,file_path,code_name="code",accession_flag=None):
+    def ignore_remove_df_lookup(self,file_path):
+        pass
+
+    def ident_df_lookup(self,file_path,code_name="code",accession_flag=None):
         idx = self.df.index[self.df['FullName'] == file_path]
         if idx.empty: reference = "ERROR"
         else: 
             if accession_flag:
                 reference = self.df.loc[idx].Accession_Reference.item()
             else: 
                 reference = self.df.loc[idx].Archive_Reference.item()
-        self.identifier.text = reference
-        self.identifier.set("type",code_name)
-                        
+        if isinstance(reference,float): pass
+        else:
+            self.identifier.text = reference
+            self.identifier.set("type",code_name)
+
+        column_headers = self.df.columns.values.tolist()
+        for header in column_headers:
+            if 'Identifier' in header:
+                #self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier") 
+                #reference = self.df[header].loc[idx].item()
+                #print(reference)
+                #code_name = str(header).rsplit[':'][-1]        
+                #print(header)
+                pass
+
     def write_opex(self,file_path,opexxml):
         opex_path = str(file_path) + ".opex"
         if os.path.exists(opex_path) and not self.force_flag:
             print(f"Opex exists: {opex_path}, but force option is not set: Avoiding override")
             pass
         else:
             opex = ET.indent(opexxml,"  ")
@@ -185,14 +201,15 @@
                     xml_new = xml_file
                     for elem_dict in list_xml:
                         name = elem_dict.get('Name')
                         path = elem_dict.get('Path')
                         ns = elem_dict.get('Namespace')
                         if self.metadata_flag in {'e','exact'}:
                             try: 
+                                print(file_path)
                                 val = self.df.loc[idx,path].values[0]
                             except KeyError as e:
                                 print('Key Error: please ensure column header\'s are an exact match...')
                                 print(f'Missing Column: {e}')
                                 print('Alternatively use flat mode...')
                                 time.sleep(5)
                                 raise SystemError()
@@ -223,25 +240,25 @@
             if description:
                 self.descriptionxml = ET.SubElement(self.properties,f"{{{self.opexns}}}Description")
                 self.descriptionxml.text = str(description)      
             if security:
                 self.securityxml = ET.SubElement(self.properties,f"{{{self.opexns}}}SecurityDescriptor")
                 self.securityxml.text = str(security)
             if self.autoclass_flag in {"catalog","c","catalog-generic","cg"}:
-                self.df_lookup(file_path,code_name=code)
+                self.ident_df_lookup(file_path,code_name=code)
             elif self.autoclass_flag in {"accession","a","accession-generic","ag"}:
-                self.df_lookup(file_path,accession_flag=True)
+                self.ident_df_lookup(file_path,accession_flag=True)
             elif self.autoclass_flag in {"both","b","both-generic","bg"}:
-                self.df_lookup(file_path,code_name=code)
+                self.ident_df_lookup(file_path,code_name=code)
                 self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier")           
-                self.df_lookup(file_path,code_name="accref",accession_flag=True)
+                self.ident_df_lookup(file_path,code_name="accref",accession_flag=True)
             elif self.autoclass_flag in {"generic","g"}:
                 self.properties.remove(self.identifiers)
             elif self.input:
-                self.df_lookup(file_path)                
+                self.ident_df_lookup(file_path)                
 
     def genererate_opex_fixity(self):
         self.fixity = ET.SubElement(self.fixities,f"{{{self.opexns}}}Fixity")        
         self.hash = HashGenerator(algorithm=self.algorithm).hash_generator(self.file_path) # Double Check...
         self.fixity.set("type", self.algorithm)
         self.fixity.set("value",self.hash)
         self.OMG.list_fixity.append([self.algorithm,self.hash,self.file_path])
@@ -291,15 +308,14 @@
             if not self.OMG.metadata_flag in {'none','n'}:
                 self.xml_descmeta = ET.SubElement(self.xmlroot,f"{{{self.opexns}}}DescriptiveMetadata")
                 self.OMG.generate_descriptive_metadata(self.xml_descmeta,self.folder_path)
     
     def filter_directories(self,directory):    #Sorts the list Alphabetically and Ignores: 1. Hidden Directories starting with '.', 2. '.opex' files, 3. Folders titled 'meta', 4. Script file 5. Output file. 
         list_directories = sorted([win_256_check(os.path.join(directory,f)) for f in os.listdir(directory) \
         if not f.startswith('.') \
-        or (stat(os.stat(f).st_file_attributes) & stat.FILE_ATTRIBUTE_HIDDEN) \
         and f != 'meta'\
         and f != os.path.basename(__file__) \
         and not f.endswith('_AutoClass.xlsx') and not f.endswith('_autoclass.xlsx')\
         and not f.endswith('_EmptyDirectoriesRemoved.txt')],key=str.casefold)
         return list_directories
         
     def generate_opex_dirs(self,file_path):
```

### Comparing `opex_manifest_generator-1.0.6/opex_manifest_generator.egg-info/PKG-INFO` & `opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.0.6
+Version: 1.1.0
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.0.6/opex_manifest_generator.egg-info/SOURCES.txt` & `opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 opex_manifest_generator/__init__.py
 opex_manifest_generator/cli.py
 opex_manifest_generator/common.py
 opex_manifest_generator/hash.py
 opex_manifest_generator/opex_manifest.py
+opex_manifest_generator/opex_manifest_v1.py
 opex_manifest_generator/test_cli.py
 opex_manifest_generator/version.py
 opex_manifest_generator.egg-info/PKG-INFO
 opex_manifest_generator.egg-info/SOURCES.txt
 opex_manifest_generator.egg-info/dependency_links.txt
 opex_manifest_generator.egg-info/entry_points.txt
 opex_manifest_generator.egg-info/requires.txt
```

### Comparing `opex_manifest_generator-1.0.6/pyproject.toml` & `opex_manifest_generator-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
 00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 226f 7065 785f 6d61  .name = "opex_ma
 00000070: 6e69 6665 7374 5f67 656e 6572 6174 6f72  nifest_generator
 00000080: 220d 0a76 6572 7369 6f6e 203d 2022 312e  "..version = "1.
-00000090: 302e 3622 0d0a 6175 7468 6f72 7320 3d20  0.6"..authors = 
+00000090: 312e 3022 0d0a 6175 7468 6f72 7320 3d20  1.0"..authors = 
 000000a0: 5b0d 0a20 2020 207b 6e61 6d65 3d22 4368  [..    {name="Ch
 000000b0: 7269 7374 6f70 6865 7220 5072 696e 6365  ristopher Prince
 000000c0: 222c 2065 6d61 696c 3d22 632e 706a 2e70  ", email="c.pj.p
 000000d0: 7269 6e63 6540 676d 6169 6c2e 636f 6d22  rince@gmail.com"
 000000e0: 7d0d 0a20 2020 205d 0d0a 6465 7363 7269  }..    ]..descri
 000000f0: 7074 696f 6e20 3d20 224f 7065 7820 4d61  ption = "Opex Ma
 00000100: 6e69 6665 7374 2047 656e 6572 6174 6f72  nifest Generator
```

