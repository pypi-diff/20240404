# Comparing `tmp/slcode-0.4.1.tar.gz` & `tmp/slcode-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slcode-0.4.1.tar", last modified: Mon Mar 11 13:27:31 2024, max compression
+gzip compressed data, was "slcode-1.0.0.tar", last modified: Thu Apr  4 09:55:02 2024, max compression
```

## Comparing `slcode-0.4.1.tar` & `slcode-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 13:27:31.752330 slcode-0.4.1/
--rw-rw-rw-   0        0        0    35801 2024-03-11 12:33:05.000000 slcode-0.4.1/LICENCE.md
--rw-rw-rw-   0        0        0     1656 2024-03-11 13:27:31.751333 slcode-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      599 2022-07-26 08:31:43.000000 slcode-0.4.1/README.md
--rw-rw-rw-   0        0        0      532 2023-01-24 07:38:15.000000 slcode-0.4.1/README.rst
--rw-rw-rw-   0        0        0     1112 2024-03-11 13:27:21.000000 slcode-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-11 13:27:31.752330 slcode-0.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-11 13:27:31.736189 slcode-0.4.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-11 13:27:31.744136 slcode-0.4.1/src/SL_C0de/
--rw-rw-rw-   0        0        0     6211 2023-12-12 17:47:21.000000 slcode-0.4.1/src/SL_C0de/Load.py
--rw-rw-rw-   0        0        0    78777 2024-02-29 10:30:23.000000 slcode-0.4.1/src/SL_C0de/SOLVER.py
--rw-rw-rw-   0        0        0        0 2022-03-23 10:35:02.000000 slcode-0.4.1/src/SL_C0de/__init__.py
--rw-rw-rw-   0        0        0    80314 2024-01-31 14:22:35.000000 slcode-0.4.1/src/SL_C0de/grid.py
--rw-rw-rw-   0        0        0    18118 2024-01-31 13:34:25.000000 slcode-0.4.1/src/SL_C0de/love.py
--rw-rw-rw-   0        0        0     8560 2023-10-17 13:46:31.000000 slcode-0.4.1/src/SL_C0de/spharm.py
-drwxrwxrwx   0        0        0        0 2024-03-11 13:27:31.751333 slcode-0.4.1/src/slcode.egg-info/
--rw-rw-rw-   0        0        0     1656 2024-03-11 13:27:31.000000 slcode-0.4.1/src/slcode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-03-11 13:27:31.000000 slcode-0.4.1/src/slcode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 13:27:31.000000 slcode-0.4.1/src/slcode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-03-11 13:27:31.000000 slcode-0.4.1/src/slcode.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-11 13:27:31.000000 slcode-0.4.1/src/slcode.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-11 13:27:31.750333 slcode-0.4.1/tests/
--rw-rw-rw-   0        0        0        0 2022-03-23 10:36:10.000000 slcode-0.4.1/tests/test_SL_C0de_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:55:02.225880 slcode-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-04-04 09:54:58.000000 slcode-1.0.0/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-04 09:55:02.225880 slcode-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 09:54:58.000000 slcode-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 09:55:02.225880 slcode-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-04 09:54:58.000000 slcode-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:55:02.221880 slcode-1.0.0/slcode/
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-04-04 09:54:58.000000 slcode-1.0.0/slcode/Load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79351 2024-04-04 09:54:58.000000 slcode-1.0.0/slcode/SOLVER.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:54:58.000000 slcode-1.0.0/slcode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79394 2024-04-04 09:54:59.000000 slcode-1.0.0/slcode/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21466 2024-04-04 09:54:59.000000 slcode-1.0.0/slcode/love.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-04 09:54:59.000000 slcode-1.0.0/slcode/spharm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:55:02.225880 slcode-1.0.0/slcode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-04 09:55:02.000000 slcode-1.0.0/slcode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 09:55:02.000000 slcode-1.0.0/slcode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:55:02.000000 slcode-1.0.0/slcode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 09:55:02.000000 slcode-1.0.0/slcode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 09:55:02.000000 slcode-1.0.0/slcode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:55:02.225880 slcode-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:54:59.000000 slcode-1.0.0/tests/test_SL_C0de_lib.py
```

### Comparing `slcode-0.4.1/LICENCE.md` & `slcode-1.0.0/LICENCE.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
+GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `slcode-0.4.1/PKG-INFO` & `slcode-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,33 @@
-Metadata-Version: 2.1
-Name: slcode
-Version: 0.4.1
-Summary: SL_C0de is a python library based on the matlab code SL_code. This module is used to calculate GIA over the world but alse the sediment isostasy. It include function to calculate radial symetric auto gravitational earth visco-elastic response. This module also include the possibility to resolve the Sea level equation based on the publication of Mitrovica and Austermann ... ajouter des refs. The aim of this library is to be easy to include new sources of load and link to other python library.
-Author-email: HENRY-LARROZE Adrien <adrien.henry@univ-lr.fr>
-Project-URL: Homepage, https://github.com/AHenryLarroze/Py_SL_C0de
-Project-URL: Bug Tracker, https://github.com/AHenryLarroze/Py_SL_C0de/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENCE.md
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: pyshtools
-Requires-Dist: matplotlib
-
-version 0.1.0 First realise of the library. 
-version 0.2.0 Paralelisation of several functions in the code. 
-version 0.3.0 Modification of the code to decompose the perturbation of the Sea level.
-version 0.3.1 New love number importation based on love numbers calculated by ALMA3
-version 0.3.2 Output function added as a csv writer for using in other application
-version 0.3.3 Add of the sediment import as in the matlab code
-version 0.3.4 Revision of the code to calculate the ground motion at the end of the computation
-version 0.3.5 Integration of saving and loading data from previous run
+Metadata-Version: 2.1
+Name: slcode
+Version: 1.0.0
+Summary: SL_C0de is a python library based on the matlab code SL_code. This module is used to calculate GIA over the world but alse the sediment isostasy. It include function to calculate radial symetric auto gravitational earth visco-elastic response. This module also include the possibility to resolve the Sea level equation based on the publication of Mitrovica and Austermann ... ajouter des refs. The aim of this library is to be easy to include new sources of load and link to other python library.
+Home-page: https://github.com/AHenryLarroze/Py_SL_C0de
+Author: Adrien Henry-Larroze
+Author-email: adrien_henry@orange.fr
+License: GPL-3.0
+Project-URL: Homepage, https://py-sl-c0de.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/AHenryLarroze/Py_SL_C0de
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENCE.md
+Requires-Dist: joblib==1.2.0
+Requires-Dist: matplotlib==3.7.0
+Requires-Dist: numpy==1.24.2
+Requires-Dist: plotly==5.13.0
+Requires-Dist: pyshtools==4.10.1
+Requires-Dist: scipy==1.10.0
+Requires-Dist: sphinx_rtd_theme==1.2.0
+Requires-Dist: tomli==2.0.1
+Requires-Dist: stripy==2.2
+Requires-Dist: netcdf4==1.6.2
+Requires-Dist: jupyter==1.0.0
+
+SL_C0de
+=======
+
+**SL_C0de** (/lu'make/) is a python library based on the matlab code SL_code. This module allows to calculate GIA over the world but also the sediment isostasy. It includes function to calculate radial symetric auto gravitational earth visco-elastic response. This module also includes the option to resolve the Sea level equation. This library has been benchmarked with the following Matlab code (jaustermann/SLcode/tree/master/GRL_2022_proglacial_lakes).The aim of this library is to be easy to include new sources of load and can be linked to other python library.
+
+documentation :
```

### Comparing `slcode-0.4.1/src/SL_C0de/SOLVER.py` & `slcode-1.0.0/slcode/SOLVER.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,1290 +1,1316 @@
-from .grid import ICE_TIME_GRID
-from .grid import SEDIMENT_TIME_GRID
-from .grid import TOPOGRAPHIC_TIME_GRID
-from .grid import OCEAN_TIME_GRID
-from .grid import LOAD_TIME_GRID
-from .spharm import sphericalobject
-from .love import LOVE
-import numpy as np
-import copy
-import os
-import sys
-
-def Precomputation(ice_grid,sed_grid,topo_grid,Output_way,stop=26,step=0.5,maxdeg=512,irregular_time_step=None,backend=False,plot=False):
-    '''
-    The _`Precomputation` method prepare the different data to match temporal and spatial resolution of the modelisation. spatial resolution (m,n) and temporal resolution (step). The input data format is described in :ref:`Mass grid format<grid_format>`.
-
-    Attribute :
-    ----------- 
-        ice_grid : dict(name = str, grid = np.array((n_i,m_i,t_i)), time = np.array((t_i,)), lon = np.array((n_i)), lat = np.array((m_i)))
-            ice thickness grid
-        sed_grid : dict(name = str, grid = np.array((n_j,m_j,t_j)), time = np.array((t_j,)), lon = np.array((n_j)), lat = np.array((m_j)),frame = (lon1,lon2,lat1,lat2))
-            sediment thickness
-        topo_grid : dict(name = str, grid = np.array((n_k,m_k)), lon = np.array((n_j)), lat = np.array((m_j)))
-            present topography 
-        Output_way : str
-            The filepath toward wich the different grid will be saved
-        stop : float 
-            age at wich the computation stop
-        step : float
-            time step used for the temporal resolution of the model
-        maxdeg : int 
-            The maximum degree of spherical harmonics, that define the spatial resolution of the model. (m = 2*maxdeg, n = maxdeg)
-        irregular_time_step : np.array((time_step_number,))
-            An irregular time array to compute the model over non regular time step
-        backend : bool
-            If required you can ask a backend during the run of each computation. True, will generate a backend, False will not. Defaul is False
-        Plot : bool
-            If needed you can ask plot of each output compared to the initial plot. You will need the cartopy doc.
-    Returns : 
-    --------- 
-        None 
-
-    The data output of the function are saved to the output way.
-
-    '''
-
-    time_step=np.arange(start=stop,stop=-step,step=-step)
-    if not(irregular_time_step is None):
-        time_step=irregular_time_step
-
-    ice_time_grid=ICE_TIME_GRID(time_step,maxdeg,grid_name=ice_grid['name'])
-    ice_time_grid.interp_on_time_and_space(ice_grid['grid'],ice_grid['time'],ice_grid['lon'],ice_grid['lat'],grid_type='global',backend=backend)
-    ice_time_grid.save(save_way=Output_way)
-
-    sed_time_grid=SEDIMENT_TIME_GRID(time_step,maxdeg,grid_name=sed_grid['name'])
-    sed_time_grid.interp_on_time_and_space(sed_grid['grid'],sed_grid['time'],sed_grid['lon'],sed_grid['lat'],backend=backend,grid_type='local')
-    sed_time_grid.height_time_grid=sed_time_grid.height_time_grid=sed_time_grid.height_time_grid[:,::-1,:]# latitude are inverted ! 
-    sed_time_grid.save(save_way=Output_way)
-
-
-    topo_time_grid=TOPOGRAPHIC_TIME_GRID(time_step,maxdeg,grid_name=topo_grid['name'])
-    topo_time_grid.topo_pres=topo_time_grid.interp_on(topo_grid['grid'],topo_grid['lon'],topo_grid['lat'],grid_type='global')+ice_time_grid.height_time_grid.sum(0)
-
-    # there is no ice in topo_sl
-
-    for i in range(topo_time_grid.time_step_number-1):
-        if i==0:
-            topo_time_grid.height_time_grid[i,:,:]=topo_time_grid.topo_pres-sed_time_grid.height_time_grid.sum(0)-ice_time_grid.height_time_grid[1:,:,:].sum(0)
-        else :
-            topo_time_grid.height_time_grid[i,:,:]=topo_time_grid.topo_pres-sed_time_grid.height_time_grid[i:,:,:].sum(0)-ice_time_grid.height_time_grid[i:,:,:].sum(0)
-    
-    topo_time_grid.save(save_way=Output_way)
-
-    if plot :
-        plot_precomputation(ice_grid['time'],ice_grid['grid'],ice_time_grid,save_way=Output_way)
-        plot_precomputation(sed_grid['time'],sed_grid['grid'],sed_time_grid,area=sed_grid['frame'],lon_init=sed_grid['lon'],lat_init=sed_grid['lat'],save_way=Output_way)
-        plot_precomputation(np.array([1]),topo_grid['grid'],topo_time_grid,topo=True,save_way=Output_way)
-
-def SLE_forward_modeling(Input_way,ice_name,sed_name,topo_name,ocean_name,love_way,love_file,conv_lim,Output_way):
-    '''
-    The _`SLE_forward_modeling` method solve the SLE with no constrain on final topography. This result in a forward modeling of the SL. It can be used for test and exploration of models. For informations on iterations see :ref:`description of iteration <iteration_desc>`.
-
-    Attribute : 
-    ------------
-        Input_way : str
-            File location of the input data (ice, sediment and topography)
-        ice_name : str
-            The name of the ice data file
-        sed_name : str
-            The name of the sediment data file
-        topo_name : str
-            The name of the topographic data file
-        ocean_name : str
-            The name of the output file containig the data on the ocean
-        love_way : str 
-            way of the love numbers file used to compute earth visco elastic deformation
-        conv_lim : float
-            Limit of precision required for the convergence of the SLE resolution (10^-3)
-        output_way : str 
-            filepath for saving results of the modelisation
-
-    Returns :
-    --------- 
-        None 
-
-    The resulting ocean class object (:ref:`OCEAN_TIME_GRID <OCEAN_TIME_GRID>`) containing the ocean thickness is saved in the outputway under the name ocean. 
-    '''
-    ice_time_grid=ICE_TIME_GRID(from_file=(True,Input_way+'/'+ice_name))
-    sed_time_grid=SEDIMENT_TIME_GRID(from_file=(True,Input_way+'/'+sed_name))
-    topo_time_grid=TOPOGRAPHIC_TIME_GRID(from_file=(True,Input_way+'/'+topo_name))
-
-    ocean_time_grid=OCEAN_TIME_GRID(ice_time_grid.time_step,ice_time_grid.maxdeg,grid_name=ocean_name)
-    ocean_time_grid.time_step_number=ocean_time_grid.time_step_number
-
-    love_number=LOVE(ice_time_grid.maxdeg,love_way+'/'+love_file,ice_time_grid.time_step,6371000,5.9742e24,type='time')
-    love_number.dev_beta()
-
-    TO=sphericalobject(coeff=np.zeros(ice_time_grid.height_time_coeff[0,:].shape))
-    TO.prev=np.zeros(ice_time_grid.height_time_coeff[0,:].shape)
-
-    
-
-    ice_time_grid.ice_correction(topo_time_grid,ocean_time_grid)
-    ice_time_grid.timegrdtotimecoeff()
-
-    load=LOAD_TIME_GRID(sdelL=ice_time_grid.height_time_coeff[1:t_it,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[1:t_it,:]*sed_time_grid.rho+ocean_time_grid.height_time_coeff[1:t_it,:]*ocean_time_grid.rho,beta_l=love_number.beta_l,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg)
-
-    topo_time_grid.update_0()
-    ocean_time_grid.evaluate_ocean(topo_time_grid.grd_0).grdtocoeff()
-    ocean_time_grid.update_0()
-    ocean_time_grid.save_prev()
-    topo_time_grid.grid_from_step(0)
-    # grd correspond donc au topo_j défini dans le code de kendal et al.
-    ocean_time_grid.evaluate_ocean(topo_time_grid.grd).grdtocoeff()
-    TO.grd=topo_time_grid.grd_0*(ocean_time_grid.grd-ocean_time_grid.grd_0)
-    TO.grdtocoeff()
-
-    track_conv=np.array([])
-
-    for t_it in range (1,ice_time_grid.time_step_number-1):
-        topo_time_grid.grid_from_step(t_it)
-        # grd correspond donc au topo_j défini dans le code de kendal et al.
-        ocean_time_grid.evaluate_ocean(topo_time_grid.grd).grdtocoeff()
-        TO.grd=topo_time_grid.grd_0*(ocean_time_grid.grd-ocean_time_grid.grd_0)
-        TO.grdtocoeff()
-        sed_time_grid.coeff_from_step(t_it)
-        ice_time_grid.coeff_from_step(t_it)
-        
-        conv_it=0
-        conv_it=ocean_time_grid.sea_level_solver(load,ice_time_grid,sed_time_grid,love_number,TO,t_it,conv_it,conv_lim)
-
-        track_conv=np.append(track_conv,conv_it)     
-        
-        TO.prev=TO.coeff.copy()
-
-        ocean_time_grid.save_prev()
-        
-        topo_time_grid.height_time_grid[t_it,:,:]=topo_time_grid.grd_0-(ocean_time_grid.delSLcurl.grd+ocean_time_grid.delPhi_g)
-    
-    if not(os.path.exists(Output_way+'/model_output')):
-            os.mkdir(Output_way+'/model_output')
-    Output_way=Output_way+'/model_output'
-
-    if not(os.path.exists(Output_way+'/'+love_file)):
-        os.mkdir(Output_way+'/'+love_file)
-    ocean_time_grid.save(Output_way+'/'+love_file)
-    ice_time_grid.save(Output_way+'/'+love_file)
-    topo_time_grid.save(Output_way+'/'+love_file)
-    print(sed_time_grid.time_grid_name)
-    sed_time_grid.save(Output_way+'/'+love_file)
-
-def SLE_solver(Input_way,ice_name,sed_name,topo_name,ocean_name,love_way,love_file,topo_lim,conv_lim,Output_way):
-    '''
-    The _`SLE_solver` solve the SLE and converge toward the actual topography. The computation of the SLE resolution is describe in :ref:`Sea level equation resolution <SLE_res>`. For informations on iterations see :ref:`description of iteration <iteration_desc>`.
-
-    Attribute :
-    ----------- 
-        Input_way : str
-            File location of the input data (ice, sediment and topography)
-        ice_name : str
-            The name of the ice data file
-        sed_name : str
-            The name of the sediment data file
-        topo_name : str
-            The name of the topographic data file
-        ocean_name : str
-            The name of the output file containig the data on the ocean
-        love_way : str 
-            way of the love numbers file used to compute earth visco elastic deformation
-        conv_lim : float
-            Limit of precision required for the convergence of the SLE resolution (10^-3)
-        topo_lim : float
-            Topography convergence limit toward wich the iteration will converge (1 m)
-        output_way : str 
-            filepath for saving results of the modelisation
-
-    Returns : 
-    --------- 
-        None 
-
-    The resulting ocean class object (:ref:`OCEAN_TIME_GRID <OCEAN_TIME_GRID>`), updated ice thickness (:ref:`ICE_TIME_GRID <ICE_TIME_GRID>`) and updated  topography (:ref:`TOPOGRAPHIC_TIME_GRID <TOPOGRAPHIC_TIME_GRID>`) are saved to output_way. 
-    '''
-    
-    ice_time_grid=ICE_TIME_GRID(from_file=(True,Input_way+'/'+ice_name))
-    sed_time_grid=SEDIMENT_TIME_GRID(from_file=(True,Input_way+'/'+sed_name))
-    topo_time_grid=TOPOGRAPHIC_TIME_GRID(from_file=(True,Input_way+'/'+topo_name))
-
-    maxdeg=ice_time_grid.maxdeg
-
-    time_step=ice_time_grid.time_step.copy()
-
-    # Initiate the base elements
-    from SL_C0de.spharm import sphericalobject
-    from SL_C0de.Load import LOAD
-
-    ocean_time_grid=OCEAN_TIME_GRID(time_step,maxdeg,grid_name=ocean_name)
-    ocean_time_grid.time_step_number=ocean_time_grid.time_step_number
-
-    ice_time_grid.timegrdtotimecoeff()
-    sed_time_grid.timegrdtotimecoeff()
-
-    love_number=LOVE(maxdeg,love_way+'/'+love_file,time_step,6371000,5.9742e24)
-    love_number.dev_beta()
-    love_number.dev_beta_tide()
-    TO=sphericalobject(coeff=np.zeros(ice_time_grid.height_time_coeff[0,:].shape))
-
-
-    topo_diff_median=np.inf
-    #sdel_topo_diff=np.inf
-    topo_it=0
-    while topo_diff_median>topo_lim : #and sdel_topo_diff>10**(-1):
-        delPhi_g_time=np.array([])
-        TO.prev=np.zeros(ice_time_grid.height_time_coeff[0,:].shape)
-
-        if topo_diff_median != np.inf :
-            topo_time_grid.height_time_grid[0,:,:]=topo_initial.copy()
-        # topo_time_grid.height_time_grid = topo_time_grid.height_time_grid - ice_time_grid.height_time_grid + ice_time_grid.ice # for resetting the corrected ice.
-        ice_time_grid.ice_correction(topo_time_grid,ocean_time_grid)
-        ice_time_grid.timegrdtotimecoeff()
-
-        t_it=-1
-
-        load=LOAD_TIME_GRID(sdelL=ice_time_grid.height_time_coeff[1:t_it,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[1:t_it,:]*sed_time_grid.rho+ocean_time_grid.height_time_coeff[1:t_it,:]*ocean_time_grid.rho,beta_l=love_number.beta_l,E=love_number.E,E_T=love_number.E_T,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg)
-        
-        topo_time_grid.update_0()
-        ocean_time_grid.evaluate_ocean(topo_time_grid.grd_0).grdtocoeff()
-        ocean_time_grid.update_0()
-        ocean_time_grid.save_prev()
-        topo_time_grid.grid_from_step(0)
-        # grd correspond donc au topo_j défini dans le code de kendal et al.
-        ocean_time_grid.evaluate_ocean(topo_time_grid.grd).grdtocoeff()
-        TO.grd=topo_time_grid.grd_0*(ocean_time_grid.grd-ocean_time_grid.grd_0)
-        TO.grdtocoeff()
-
-        track_conv=np.array([])
-
-        for t_it in range (1,ice_time_grid.time_step_number-1):
-            topo_time_grid.grid_from_step(t_it)
-            # grd correspond donc au topo_j défini dans le code de kendal et al.
-            ocean_time_grid.evaluate_ocean(topo_time_grid.grd).grdtocoeff()
-            TO.grd=topo_time_grid.grd_0*(ocean_time_grid.grd-ocean_time_grid.grd_0)
-            TO.grdtocoeff()
-            sed_time_grid.coeff_from_step(t_it)
-            ice_time_grid.coeff_from_step(t_it)
-            
-
-
-            print('time_iteration : ',ice_time_grid.time_step[t_it])
-            if topo_it==0 : 
-                conv_it=0
-            else :
-                conv_it=1
-            conv_it=ocean_time_grid.sea_level_solver(load,ice_time_grid,sed_time_grid,love_number,TO,t_it,conv_it,conv_lim)
-
-            print(conv_it)
-
-            track_conv=np.append(track_conv,conv_it)     
-            
-            TO.prev=TO.coeff.copy()
-
-            ocean_time_grid.save_prev()
-            
-            topo_time_grid.height_time_grid[t_it,:,:]=topo_time_grid.grd_0-(ocean_time_grid.delSLcurl.grd+ocean_time_grid.delPhi_g)
-            
-
-            #delPhi_g_time=np.append(delPhi_g_time,ocean_time_grid.delPhi_g)
-
-        topo_it+=1
-        topo_pres_ice_corrected=topo_time_grid.topo_pres-ice_time_grid.ice.sum(0)+ice_time_grid.height_time_grid.sum(0)
-        topo_diff=np.abs(topo_time_grid.height_time_grid[-1,:,:]-topo_pres_ice_corrected).max().max()
-        sdel_topo_diff=np.abs(topo_diff-np.abs(topo_time_grid.height_time_grid[-1,:,:]-topo_pres_ice_corrected).max().max())
-        topo_diff_mean=np.abs(topo_time_grid.height_time_grid[-1,:,:]-topo_pres_ice_corrected).mean().mean()
-        topo_diff_median=np.median(np.median(np.abs(topo_time_grid.height_time_grid[-1,:,:]-topo_pres_ice_corrected)))
-        print(topo_it,' : ',topo_diff, topo_diff_mean, topo_diff_median, sdel_topo_diff,track_conv-(topo_it>0))
-        topo_initial=topo_pres_ice_corrected - (topo_time_grid.height_time_grid[-1,:,:]-topo_time_grid.height_time_grid[0,:,:])
-
-    if not(os.path.exists(Output_way+'/model_output')):
-        os.mkdir(Output_way+'/model_output')
-    Output_way=Output_way+'/model_output'
-
-    if not(os.path.exists(Output_way+'/'+love_file)):
-        os.mkdir(Output_way+'/'+love_file)
-    ocean_time_grid.save(Output_way+'/'+love_file)
-    ice_time_grid.save(Output_way+'/'+love_file)
-    topo_time_grid.save(Output_way+'/'+love_file)
-    sed_time_grid.save(Output_way+'/'+love_file)
-    return load
-
-def find_files(filename, search_path):
-    result = []
-
-    # Wlaking top-down from the root
-    for root, dir, files in os.walk(search_path):
-        if filename in dir:
-            result.append(os.path.join(root, filename))
-    return result
-
-def calculate_deformation(love_number,ice_time_grid,sed_time_grid,ocean_time_grid,a,Me,Output_way,backend=False,plot=dict(plot=False)) :
-
-    '''
-    The _`calculate_deformation` method calculate the earth viscoelastic response resulting from the different masses caculated with the :ref:`SLE_solver <SLE_solver>`. This computation follows the decomposition of the SLE described in :ref:`Computation of ground and geoid subsidence from different load source <G_R_comp>`
-
-    Attribute :
-    ----------- 
-        love_number : :ref:`LOVE <LOVE>` 
-            The loaded love number in the form of a LOVE class object
-        ice_time_grid : :ref:`grid.ICE_TIME_GRID <ICE_TIME_GRID>`
-            ice thickness in the form of ICE_TIME_GRID class object
-        sed_time_grid : :ref:`grid.SEDIMENT_TIME_GRID <SEDIMENT_TIME_GRID>` 
-            sediment thickness in the form of SEDIMENT_TIME_GRID class object
-        ocean_time_grid : :ref:`grid.OCEAN_TIME_GRID <OCEAN_TIME_GRID>` 
-            ocean thickness calculated using the SLE solver in the form of OCEAN_TIME_GRID class object
-        a : float
-            radius of earth in meter
-        Me : float
-            mass of earth (kg)
-        Output_way : str
-            way of the output where the load is calculated
-        backend : bool
-            set if the function is writing its state of computation
-
-    Returns :  
-    ---------
-        None 
-
-    The resulting LOAD and GEOID are stored in a LOAD file in the same file then the input files. The structure is based on the :ref:`LOAD_TIME_GRID <LOAD_TIME_GRID>`  class object.
-    '''
-    beta_l=love_number.beta_R_l
-
-    ice_load_time_grid=LOAD_TIME_GRID(sdelL=ice_time_grid.height_time_coeff*ice_time_grid.rho,beta_l=beta_l,E=love_number.h_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='ICE_LOAD')
-    ice_load_time_grid.calc_elastic_time()
-    ice_load_time_grid.calc_viscuous_time(backend=backend)
-    ice_load_time_grid.save(save_way=Output_way)    
-    ice_load_time_grid=0
-
-    sediment_load_time_grid=LOAD_TIME_GRID(sdelL=sed_time_grid.height_time_coeff*sed_time_grid.rho,beta_l=beta_l,E=love_number.h_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='SEDIMENT_LOAD')
-    sediment_load_time_grid.calc_elastic_time()
-    sediment_load_time_grid.calc_viscuous_time(backend=backend)
-    sediment_load_time_grid.save(save_way=Output_way)
-    sediment_load_time_grid=0
-
-    ocean_load_time_grid=LOAD_TIME_GRID(sdelL=ocean_time_grid.height_time_coeff*ocean_time_grid.rho,beta_l=beta_l,E=love_number.h_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='OCEAN_LOAD')
-    ocean_load_time_grid.calc_elastic_time()
-    ocean_load_time_grid.calc_viscuous_time(backend=backend)
-    ocean_load_time_grid.save(save_way=Output_way)
-    ocean_load_time_grid=0
-
-    total_load_time_grid=LOAD_TIME_GRID(sdelL=ice_time_grid.height_time_coeff*ice_time_grid.rho+sed_time_grid.height_time_coeff*sed_time_grid.rho+ocean_time_grid.height_time_coeff*ocean_time_grid.rho,beta_l=beta_l,E=love_number.h_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='TOTAL_LOAD')
-    total_load_time_grid.calc_elastic_time()
-    total_load_time_grid.calc_viscuous_time(backend=backend)
-    total_load_time_grid.save(save_way=Output_way)
-    total_load_time_grid=0
-
-    #Calculating the geoïd deformation
-
-    beta_l=love_number.beta_G_l
-
-    ice_geoid_time_grid=LOAD_TIME_GRID(sdelL=ice_time_grid.height_time_coeff*ice_time_grid.rho,beta_l=beta_l,E=1+love_number.k_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='ICE_GEOID')
-    ice_geoid_time_grid.calc_elastic_time()
-    ice_geoid_time_grid.calc_viscuous_time(backend=backend)
-    ice_geoid_time_grid.save(save_way=Output_way)
-    ice_geoid_time_grid=0
-
-    sediment_geoid_time_grid=LOAD_TIME_GRID(sdelL=sed_time_grid.height_time_coeff*sed_time_grid.rho,beta_l=beta_l,E=1+love_number.k_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='SEDIMENT_GEOID')
-    sediment_geoid_time_grid.calc_elastic_time()
-    sediment_geoid_time_grid.calc_viscuous_time(backend=backend)
-    sediment_geoid_time_grid.save(save_way=Output_way)
-    sediment_geoid_time_grid=0
-
-    ocean_geoid_time_grid=LOAD_TIME_GRID(sdelL=ocean_time_grid.height_time_coeff*ocean_time_grid.rho,beta_l=beta_l,E=love_number.k_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='OCEAN_GEOID')
-    ocean_geoid_time_grid.calc_elastic_time()
-    ocean_geoid_time_grid.calc_viscuous_time(backend=backend)
-    ocean_geoid_time_grid.save(save_way=Output_way)
-    ocean_geoid_time_grid=0
-
-    total_geoid_time_grid=LOAD_TIME_GRID(sdelL=ice_time_grid.height_time_coeff*ice_time_grid.rho+sed_time_grid.height_time_coeff*sed_time_grid.rho+ocean_time_grid.height_time_coeff*ocean_time_grid.rho,beta_l=beta_l,E=love_number.k_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='TOTAL_GEOID')
-    total_geoid_time_grid.calc_elastic_time()
-    total_geoid_time_grid.calc_viscuous_time(backend=backend)
-    total_geoid_time_grid.save(save_way=Output_way)
-    total_geoid_time_grid=0
-
-
-
-def calculate_sediment_ocean_interaction(love_number,ice_time_grid,sed_time_grid,ocean_time_grid,a,Me,topo_time_grid,Output_way,backend=False,plot=dict(plot=False)) :
-
-    '''
-    The _`calculate_sediment_ocean_interaction` method calculate the earth viscoelastic response resulting from sediment under sea surface. This is used to retrieve the effect of ocean replacement by sediment on the sediment load. The resulting subsidence is the true subsidence induced by sediment. The problems and resolution in equation is described in :ref:`True sediment subsidence <sed_subs>`.
-
-    Attribute :
-    ----------- 
-        love_number : :ref:`LOVE <LOVE>` 
-            The loaded love number in the form of a LOVE class object
-        ice_time_grid : :ref:`grid.ICE_TIME_GRID <ICE_TIME_GRID>`
-            ice thickness in the form of ICE_TIME_GRID class object
-        sed_time_grid : :ref:`grid.SEDIMENT_TIME_GRID <SEDIMENT_TIME_GRID>` 
-            sediment thickness in the form of SED_TIME_GRID class object
-        ocean_time_grid : :ref:`grid.OCEAN_TIME_GRID <OCEAN_TIME_GRID>` 
-            ocean thickness calculated using the SLE solver in the form of OCEAN_TIME_GRID class object
-        a : float
-            radius of earth in meter
-        Me : float
-            mass of earth (kg)
-        Output_way : str
-            way of the output where the load is calculated
-        backend : bool
-            set if the function is writing its state of computation
-
-    Returns : 
-    --------- 
-        None 
-
-    The resulting LOAD and GEOID are stored in a LOAD file in the same file then the input files. The structure is based on the :ref:`LOAD_TIME_GRID <LOAD_TIME_GRID>` class object.
-    '''
-
-    beta_l=love_number.beta_R_l # Load the earth love numbers
-    #Preparing a new grid that compute the load of the substracted sediment volume to the ocean.
-    #We create a new object to compute the oceanic sediment
-    oceanic_sediment_time_grid=copy.copy(sed_time_grid)
-    oceanic_sediment_time_grid.rho=ocean_time_grid.rho
-    
-
-    for t_it in range (oceanic_sediment_time_grid.time_step_number-1): # At each time step we apply the ocean function to the sediment height grid
-        oceanic_sediment_time_grid.height_time_grid[t_it,:,:]=oceanic_sediment_time_grid.height_time_grid[t_it,:,:]*ocean_time_grid.evaluate_ocean(topo_time_grid.height_time_grid[t_it,:,:]).grd
-    oceanic_sediment_time_grid.timegrdtotimecoeff()
-
-
-    oceanic_sediment_load_time_grid=LOAD_TIME_GRID(sdelL=oceanic_sediment_time_grid.height_time_coeff*oceanic_sediment_time_grid.rho,beta_l=beta_l,E=love_number.h_e,a=a,Me=Me,time_step=oceanic_sediment_time_grid.time_step,maxdeg=oceanic_sediment_time_grid.maxdeg,grid_name='OCEANIC_SEDIMENT_LOAD')    
-    #computing the earth deformation
-    oceanic_sediment_load_time_grid.calc_elastic_time()
-    oceanic_sediment_load_time_grid.calc_viscuous_time(backend=backend)
-    oceanic_sediment_load_time_grid.save(save_way=Output_way)
-    oceanic_sediment_load_time_grid.clean_memory()
-
-    beta_l=love_number.beta_G_l # Load the ocean love numbers
-
-    #computing the geoid deformation
-    oceanic_sediment_geoid_time_grid=LOAD_TIME_GRID(sdelL=oceanic_sediment_time_grid.height_time_coeff*oceanic_sediment_time_grid.rho,beta_l=beta_l,E=love_number.h_e,a=a,Me=Me,time_step=oceanic_sediment_time_grid.time_step,maxdeg=oceanic_sediment_time_grid.maxdeg,grid_name='OCEANIC_SEDIMENT_GEOID')
-    oceanic_sediment_geoid_time_grid.calc_elastic_time()
-    oceanic_sediment_geoid_time_grid.calc_viscuous_time(backend=backend)
-    oceanic_sediment_geoid_time_grid.save(save_way=Output_way)
-    oceanic_sediment_geoid_time_grid.clean_memory()
-
-
-
-def Post_process(Input_way,sed_name,ice_name,ocean_name,topo_name,love_way):
-    '''
-    The _`Post_process` calculate the earth viscoelastic response resulting from the different masses caculated with the SLE_solver. This computation is made for all models available in the files. 
-
-    Attribute :
-    ----------- 
-        input_way_sed : str
-            way where the sediment precomputed are stored
-        input_way_model_output : str
-            filepath to the different masses calculated by the SLE solver
-        love_way : str
-            way to the love number output
-
-    Returns : 
-    --------- 
-        None 
-
-    The resulting LOAD and GEOID are stored in a LOAD file in the same file then the input files. The structure is based on the :ref:`LOAD_TIME_GRID <LOAD_TIME_GRID>` class object.
-    '''
-    
-
-
-    earth_model_name_list=os.listdir(Input_way)
-
-    for earth_model_name in earth_model_name_list :
-
-        print('calculation for : ' + earth_model_name)
-
-        Output_way=Input_way+'/'+earth_model_name+'/LOAD/'
-
-        if not(os.path.exists(Output_way)):
-            os.mkdir(Output_way)
-
-        sed_time_grid=SEDIMENT_TIME_GRID(from_file=(True,Input_way+'/'+earth_model_name+'/'+sed_name))
-        sed_time_grid.timegrdtotimecoeff()
-
-        ocean_time_grid=OCEAN_TIME_GRID(from_file=(True,Input_way+'/'+earth_model_name+'/'+ocean_name))
-        #print(ocean_time_grid.height_time_coeff.shape)
-        ice_time_grid=ICE_TIME_GRID(from_file=(True,Input_way+'/'+earth_model_name+'/'+ice_name))
-        #print(ice_time_grid.time_step_number)
-
-        np.set_printoptions(threshold=sys.maxsize)
-        a=6371000
-        Me=5.9742e24
-        love_way_found=find_files(earth_model_name,love_way)[0]
-        love_number=LOVE(ice_time_grid.maxdeg,love_way_found,ice_time_grid.time_step,a,Me)
-
-        ice_time_grid.timegrdtotimecoeff()
-
-        calculate_deformation(love_number,ice_time_grid,sed_time_grid,ocean_time_grid,a,Me,Output_way)
-
-        #Loading the topography to compute the ocean function at each time step
-        topo_time_grid=TOPOGRAPHIC_TIME_GRID(from_file=(True,Input_way+'/'+earth_model_name+'/'+topo_name))
-
-        print('Oceanic sediment calculation')
-        calculate_sediment_ocean_interaction(love_number,ice_time_grid,sed_time_grid,ocean_time_grid,a,Me,topo_time_grid,Output_way)
-
-def plot_model_result_map(Input_way,plot):
-    '''
-    The _`plot_model_result_map` function run the plot functions for all type of load. This function use the `plot_frame`_ function, see this function for more details. 
-
-    Attribute :
-    ----------- 
-        input_way_sed : str
-            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
-        plot : dict(plot=True,times=[n_t],frames=[n_f*(lon1,lon1,lat1,lat2)],frames_resolution=[n_f],frames_min_max=np.array([[[min_load],max_load,min_geoid,max_geoid]]),contours_v=[n_f*2*[contours...]],transects=[n_t*(lat1,lon1,lat2,lon2)],point_density=[n_t], transect_min_max=[n_t(min_load,max_load,min_geoid,max_geoid)], points=np.array([n_p[lat,lon]]))
-            The plot dictionnary used to define all the plot parameters of the output. In this dictionary, there is three main group of parameters, the frame plot parameters, the transect plot parameters and the points plot parameters. The frame plot parameters contain the frame locations in frames, the frames resolution in frames_resolution, the frames min and max value to plot in frames_min_max and the contours value to plot in contours_v. The transect plot parameters contains the location of the begining and end of the transects in transects, the point density along the transect in point_density and the min max value of the transect in transect_min_max. The points plot parameters contains the locations of the differents plots in points. 
-
-    Returns : 
-    --------- 
-        None 
-
-    '''
-    Input_way=Input_way+'/LOAD'
-    plot_frame(Input_way,plot,Input_way,'ICE')
-    plot_frame(Input_way,plot,Input_way,'SEDIMENT')
-    plot_frame(Input_way,plot,Input_way,'OCEAN')
-    plot_frame(Input_way,plot,Input_way,'NO_SEDIMENT')
-    plot_frame(Input_way,plot,Input_way,'TOTAL')
-
-def calc_transect(Input_way,time,transect,point_density,type,type_bis):
-    '''
-    The _`calc_transect` function evaluate the spherical harmonics coefficient function run the plot functions for all type of load. This function use the `plot_frame`_ function, see this function for more details. 
-
-    Attribute :
-    ----------- 
-        input_way_sed : str
-            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
-        time : float
-            The selected time to plot the transect.
-        transect : (lat1,lon1,lat2,lon2)
-            The coordinate of the beginning and the end of the transect.
-        point_dentity : int
-            Number of points along the transect, this will define the resolution
-        type : str
-            This define the type of load considered. Must be "SEDIMENT", "NO_SEDIMENT", "OCEAN", "ICE" or "TOTAL".
-        type_bis : str
-            This define if the plot concern the geoid of the ground deformation. Must be "LOAD" or "GEOID".
-
-    Returns : 
-    --------- 
-        None 
-        
-    '''
-    
-    if type is 'OCEAN' :
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_{type_bis}'))
-        t_it=np.where(load_time_grid.time_step==time)[0][0]
-        load_time_grid.coeff=load_time_grid.viscuous_deformation[t_it-2,:]-load_time_grid.viscuous_deformation[t_it-3,:]+load_time_grid.elastic_deformation[t_it-2,:]-load_time_grid.elastic_deformation[t_it-3,:]
-        load_time_grid.coeff=load_time_grid.coeff/(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
-        tr_ocean=load_time_grid.along_transect(coord=transect,point_density=point_density)
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_{type_bis}'))
-        load_time_grid.coeff=load_time_grid.viscuous_deformation[t_it-2,:]-load_time_grid.viscuous_deformation[t_it-3,:]+load_time_grid.elastic_deformation[t_it-2,:]-load_time_grid.elastic_deformation[t_it-3,:]
-        load_time_grid.coeff=load_time_grid.coeff/(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
-        tr_oceanic_sediment=load_time_grid.along_transect(coord=transect,point_density=point_density)
-        tr=tr_ocean+tr_oceanic_sediment
-    elif type is 'SEDIMENT' :
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_{type_bis}'))
-        t_it=np.where(load_time_grid.time_step==time)[0][0]
-        load_time_grid.coeff=load_time_grid.viscuous_deformation[t_it-2,:]-load_time_grid.viscuous_deformation[t_it-3,:]+load_time_grid.elastic_deformation[t_it-2,:]-load_time_grid.elastic_deformation[t_it-3,:]
-        load_time_grid.coeff=load_time_grid.coeff/(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
-        tr_sediment=load_time_grid.along_transect(coord=transect,point_density=point_density)
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_{type_bis}'))
-        load_time_grid.coeff=load_time_grid.viscuous_deformation[t_it-2,:]-load_time_grid.viscuous_deformation[t_it-3,:]+load_time_grid.elastic_deformation[t_it-2,:]-load_time_grid.elastic_deformation[t_it-3,:]
-        load_time_grid.coeff=load_time_grid.coeff/(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
-        tr_oceanic_sediment=load_time_grid.along_transect(coord=transect,point_density=point_density)
-        tr=tr_sediment-tr_oceanic_sediment
-    elif type is 'NO_SEDIMENT' :
-        ice_load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\ICE_{type_bis}'))
-        ocean_load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEAN_{type_bis}'))
-        t_it=np.where(ice_load_time_grid.time_step==time)[0][0]
-
-        ice_load_time_grid.coeff=ice_load_time_grid.viscuous_deformation[t_it-2,:]-ice_load_time_grid.viscuous_deformation[t_it-3,:]+ice_load_time_grid.elastic_deformation[t_it-2,:]-ice_load_time_grid.elastic_deformation[t_it-3,:]
-        ice_load_time_grid.coeff=ice_load_time_grid.coeff/(ice_load_time_grid.time_step[t_it-1]-ice_load_time_grid.time_step[t_it])
-
-        ocean_load_time_grid.coeff=ocean_load_time_grid.viscuous_deformation[t_it-2,:]-ocean_load_time_grid.viscuous_deformation[t_it-3,:]+ocean_load_time_grid.elastic_deformation[t_it-2,:]-ocean_load_time_grid.elastic_deformation[t_it-3,:]
-        ocean_load_time_grid.coeff=ocean_load_time_grid.coeff/(ocean_load_time_grid.time_step[t_it-1]-ocean_load_time_grid.time_step[t_it])
-
-        tr_ice=ice_load_time_grid.along_transect(coord=transect,point_density=point_density)
-        tr_ocean=ocean_load_time_grid.along_transect(coord=transect,point_density=point_density)
-
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_{type_bis}'))
-        load_time_grid.coeff=load_time_grid.viscuous_deformation[t_it-2,:]-load_time_grid.viscuous_deformation[t_it-3,:]+load_time_grid.elastic_deformation[t_it-2,:]-load_time_grid.elastic_deformation[t_it-3,:]
-        load_time_grid.coeff=load_time_grid.coeff/(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
-        tr_oceanic_sediment=load_time_grid.along_transect(coord=transect,point_density=point_density)
-        tr=tr_ice+tr_ocean+tr_oceanic_sediment
-    else :
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_{type_bis}'))
-        t_it=np.where(load_time_grid.time_step==time)[0][0]
-        load_time_grid.coeff=load_time_grid.viscuous_deformation[t_it-2,:]-load_time_grid.viscuous_deformation[t_it-3,:]+load_time_grid.elastic_deformation[t_it-2,:]-load_time_grid.elastic_deformation[t_it-3,:]
-        load_time_grid.coeff=load_time_grid.coeff/(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
-        tr=load_time_grid.along_transect(coord=transect,point_density=point_density)
-    dt=(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
-    return tr,dt
-
-
-def plot_model_result_cross_section(Input_way,plot):
-    '''
-    The _`plot_model_result_cross_section` function evaluate the spherical harmonics coefficient function and plot the results along a defined transect in plot.
-
-    Attribute :
-    ----------- 
-        Input_way_sed : str
-            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
-        plot : dict(plot=True,times=[n_t],frames=[n_f*(lon1,lon1,lat1,lat2)],frames_resolution=[n_f],frames_min_max=np.array([[[min_load],max_load,min_geoid,max_geoid]]),contours_v=[n_f*2*[contours...]],transects=[n_t*(lat1,lon1,lat2,lon2)],point_density=[n_t], transect_min_max=[n_t(min_load,max_load,min_geoid,max_geoid)], points=np.array([n_p[lat,lon]]))
-            The plot dictionnary used to define all the plot parameters of the output. In this dictionary, there is three main group of parameters, the frame plot parameters, the transect plot parameters and the points plot parameters. The frame plot parameters contain the frame locations in frames, the frames resolution in frames_resolution, the frames min and max value to plot in frames_min_max and the contours value to plot in contours_v. The transect plot parameters contains the location of the begining and end of the transects in transects, the point density along the transect in point_density and the min max value of the transect in transect_min_max. The points plot parameters contains the locations of the differents plots in points. 
-
-    Returns : 
-    --------- 
-        None 
-        
-    '''
-    Input_way=Input_way+'/LOAD'
-    sediment_color=(0.4,0.7,0.5)
-    sediment_color_dark=(0.2,0.4,0.25)
-    ice_color=(0.1,0.8,0.8)
-    ocean_color=(0.2,0.2,0.6)
-    glaciohydrostatic_color=(0.1,0.1,0.4)
-    if len(plot['transects'])>0 :
-        fig,ax=plt.subplots(len(plot['transects'])*len(plot['times']),2,figsize=(29.7,5*len(plot['transects'])*len(plot['times'])))
-        fig_loc,ax_map=plt.subplots(1,1,subplot_kw={'projection': ccrs.PlateCarree(), "aspect": 1})
-        alpha_ocean=0
-        coast_line_width=0.2
-        ax_map.set_global()
-        cartopy.mpl.geoaxes.GeoAxes.gridlines(ax_map,crs=ccrs.PlateCarree(),draw_labels=True)
-        ax_map.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
-        ax_map.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
-        for i_transect in range(len(plot['transects'])):
-            ax_map.plot((plot['transects'][i_transect][1],plot['transects'][i_transect][3]),(plot['transects'][i_transect][0],plot['transects'][i_transect][2]),color='r',linewidth=0.5)
-            ax_map.annotate(f'{i_transect})', # this is the text
-                 (plot['transects'][i_transect][1],plot['transects'][i_transect][0]), # these are the coordinates to position the label
-                 textcoords="offset points", # how to position the text
-                 xytext=(0,1), # distance from text to points (x,y)
-                 ha='center',
-                 fontsize=3)
-        plt.close(fig_loc)
-        fig_loc.savefig(f'{Input_way}/transect_localisation.pdf')
-        k=0
-        for i_time in range(len(plot['times'])):
-            for i_transect in range(len(plot['transects'])):
-                coord=plot['transects'][i_transect]
-                theta=np.linspace(coord[0],coord[2],plot['point_density'][i_transect])/180*2*np.pi
-                phi=np.linspace(coord[1],coord[3],plot['point_density'][i_transect])/180*2*np.pi
-                phiA=np.append(phi,0)
-                phiB=np.append(0,phi)
-                D= np.append(0,6371*np.arccos(np.sin(phiA)*np.sin(phiB)+np.cos(phiA)*np.cos(phiB)*np.cos(np.append(0,np.append(np.diff(theta),0))))[1:-1].cumsum())/2
-                axes=ax[k,:]
-                type_bis='LOAD'
-                tr_ice_load,dt=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'ICE',type_bis)
-                tr_sed_load,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'SEDIMENT',type_bis)
-                tr_oc_load,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'OCEAN',type_bis)
-                tr_nosed_load,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'NO_SEDIMENT',type_bis)
-                tr_tot_load,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'TOTAL',type_bis)
-                axes[0].plot(D,tr_ice_load,label='ice_load',color=ice_color)
-                axes[0].plot(D,tr_sed_load,label='sediment_load',color=sediment_color)
-                axes[0].plot(D,tr_oc_load,label='ocean_load',color=ocean_color)
-                axes[0].plot(D,tr_nosed_load,label='glaciohydrostatic_load',color=glaciohydrostatic_color)
-                axes[0].plot(D,tr_tot_load,label='total load',color='k')
-                axes[0].set_ylim(plot['transect_min_max'][i_transect][0],plot['transect_min_max'][i_transect][1])
-                axes[0].set_xlabel(f'distance (km)')
-                axes[0].set_ylabel(f'Vertical Land motion averaged over {dt*1000} year (mm/yr)')
-                t=plot['times'][i_time]
-                axes[0].grid()
-                axes[0].set_title(f'VLM estimated at {t} kyr along transect {i_transect})')
-                axes[0].legend()
-                type_bis='GEOID'
-                tr_ice_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'ICE',type_bis)
-                tr_sed_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'SEDIMENT',type_bis)
-                tr_oc_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'OCEAN',type_bis)
-                tr_nosed_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'NO_SEDIMENT',type_bis)
-                tr_tot_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'TOTAL',type_bis)
-                axes[1].plot(D,tr_ice_geoid,label='ice_geoid',color=ice_color)
-                axes[1].plot(D,tr_sed_geoid,label='sediment_geoid',color=sediment_color)
-                axes[1].plot(D,tr_oc_geoid,label='ocean_geoid',color=ocean_color)
-                axes[1].plot(D,tr_nosed_geoid,label='glaciohydrostatic_geoid',color=glaciohydrostatic_color)
-                axes[1].plot(D,tr_tot_geoid,label='total geoid',color='k')
-                axes[1].set_xlabel(f'distance (km)')
-                axes[1].set_ylabel(f'Vertical Geoid motion averaged over {dt*1000} year (mm/yr)')
-                t=plot['times'][i_time]
-                axes[1].set_title(f'VGM estimated at {t} kyr along transect {i_transect})')
-                axes[1].grid()
-                axes[1].set_ylim(plot['transect_min_max'][i_transect][2],plot['transect_min_max'][i_transect][3])
-                axes[1].legend()
-                k+=1
-        plt.close(fig)
-        fig.savefig(f'{Input_way}/transect_deformation.pdf')
-
-    
-
-def calc_point(Input_way,points,type,type_bis):
-    '''
-    The _`calc_point` function evaluate the spherical harmonics coefficient for a type of model output at precise points locations.
-
-    Attribute :
-    ----------- 
-        Input_way : str
-            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
-        time : float
-            The selected time to plot the transect.
-        points : np.array(n_p*[lat,lon])
-            The locations of the different points you wan't to extract data.
-        type : str
-            This define the type of load considered. Must be "SEDIMENT", "NO_SEDIMENT", "OCEAN", "ICE" or "TOTAL".
-        type_bis : str
-            This define if the plot concern the geoid of the ground deformation. Must be "LOAD" or "GEOID".
-
-    Returns : 
-    --------- 
-        None 
-        
-    '''
-    
-    if type is 'OCEAN' :
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_{type_bis}'))
-        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
-        points_ocean=load_time_grid.point_time(points)
-
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_{type_bis}'))
-        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
-        points_oceanic_sediment=load_time_grid.point_time(points)
-
-        points=points_ocean+points_oceanic_sediment
-    elif type is 'SEDIMENT' :
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_{type_bis}'))
-        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
-        points_sediment=load_time_grid.point_time(points)
-
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_{type_bis}'))
-        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
-        points_oceanic_sediment=load_time_grid.point_time(points)
-
-        points=points_sediment-points_oceanic_sediment
-
-    elif type is 'NO_SEDIMENT' :
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEAN_{type_bis}'))
-        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
-        points_ocean=load_time_grid.point_time(points)
-
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\ICE_{type_bis}'))
-        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
-        points_ice=load_time_grid.point_time(points)
-
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_{type_bis}'))
-        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
-        points_oceanic_sediment=load_time_grid.point_time(points)
-
-        points=points_ocean+points_oceanic_sediment+points_ice
-    else :
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_{type_bis}'))
-        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
-        points=load_time_grid.point_time(points)
-
-    return points,load_time_grid.time_step
-
-def plot_model_output_points(Input_way,plot):
-    '''
-    The _`plot_model_output_points` function plot the output of the model at different points.
-    
-    Attribute :
-    ----------- 
-        Input_way : str
-            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
-        plot : dict(plot=True,times=[n_t],frames=[n_f*(lon1,lon1,lat1,lat2)],frames_resolution=[n_f],frames_min_max=np.array([[[min_load],max_load,min_geoid,max_geoid]]),contours_v=[n_f*2*[contours...]],transects=[n_t*(lat1,lon1,lat2,lon2)],point_density=[n_t], transect_min_max=[n_t(min_load,max_load,min_geoid,max_geoid)], points=np.array([n_p[lat,lon]]))
-            The plot dictionnary used to define all the plot parameters of the output. In this dictionary, there is three main group of parameters, the frame plot parameters, the transect plot parameters and the points plot parameters. The frame plot parameters contain the frame locations in frames, the frames resolution in frames_resolution, the frames min and max value to plot in frames_min_max and the contours value to plot in contours_v. The transect plot parameters contains the location of the begining and end of the transects in transects, the point density along the transect in point_density and the min max value of the transect in transect_min_max. The points plot parameters contains the locations of the differents plots in points. 
-        
-
-    Returns : 
-    --------- 
-        None 
-        
-    '''
-    sediment_color=(0.4,0.7,0.5)
-    sediment_color_dark=(0.2,0.4,0.25)
-    ice_color=(0.1,0.8,0.8)
-    ocean_color=(0.2,0.2,0.6)
-    glaciohydrostatic_color=(0.7,0.2,0.2)
-    if len(plot['transects'])>0 :
-        fig,axes=plt.subplots(len(plot['points']),3,figsize=(29.7,4*len(plot['points'])))
-        fig_loc,ax_map=plt.subplots(1,1,subplot_kw={'projection': ccrs.PlateCarree(), "aspect": 1})
-        alpha_ocean=0
-        coast_line_width=0.2
-        ax_map.set_global()
-        cartopy.mpl.geoaxes.GeoAxes.gridlines(ax_map,crs=ccrs.PlateCarree(),draw_labels=True)
-        ax_map.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
-        ax_map.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
-        for i_point in range(len(plot['points'])):
-            ax_map.scatter((plot['points'][i_point,1],plot['points'][i_point,1]),(plot['points'][i_point,0],plot['points'][i_point,0]),color='r',s=0.05)
-            ax_map.annotate(f'{i_point})', # this is the text
-                 (plot['points'][i_point,1],plot['points'][i_point,0]), # these are the coordinates to position the label
-                 textcoords="offset points", # how to position the text
-                 xytext=(0,0.2), # distance from text to points (x,y)
-                 ha='center',
-                 fontsize=1)
-        plt.close(fig_loc)
-        fig_loc.savefig(f'{Input_way}/LOAD/Points_localisation.pdf')
-        coord=plot['points']
-        type_bis='LOAD'
-        points_ice_load,time_step=calc_point(Input_way+'/LOAD',plot['points'],'ICE',type_bis)
-        points_sed_load,_=calc_point(Input_way+'/LOAD',plot['points'],'SEDIMENT',type_bis)
-        points_oc_load,_=calc_point(Input_way+'/LOAD',plot['points'],'OCEAN',type_bis)
-        points_nosed_load,_=calc_point(Input_way+'/LOAD',plot['points'],'NO_SEDIMENT',type_bis)
-        points_tot_load,_=calc_point(Input_way+'/LOAD',plot['points'],'TOTAL',type_bis)
-        for i_point in range(len(plot['points'])):
-            axes[i_point,0].plot(time_step,points_ice_load[i_point,:],label='ice_load',color=ice_color)
-            axes[i_point,0].plot(time_step,points_sed_load[i_point,:],label='sediment_load',color=sediment_color)
-            axes[i_point,0].plot(time_step,points_oc_load[i_point,:],label='ocean_load',color=ocean_color)
-            axes[i_point,0].plot(time_step,points_nosed_load[i_point,:],label='glaciohydrostatic_load',color=glaciohydrostatic_color)
-            axes[i_point,0].plot(time_step,points_tot_load[i_point,:],label='total load',color='k')
-            #axes[i_point,0].set_ylim(plot['transect_min_max'][i_transect][0],plot['transect_min_max'][i_transect][1])
-            axes[i_point,0].set_xlabel(f'time (kyr)')
-            axes[i_point,0].set_ylabel(f'Vertical Land motion (mm/yr)')
-            axes[i_point,0].grid()
-            axes[i_point,0].set_title(f'VLM at point {i_point})')
-            axes[i_point,0].legend()
-        type_bis='GEOID'
-        points_ice_geoid,time_step=calc_point(Input_way+'/LOAD',plot['points'],'ICE',type_bis)
-        points_sed_geoid,_=calc_point(Input_way+'/LOAD',plot['points'],'SEDIMENT',type_bis)
-        points_oc_geoid,_=calc_point(Input_way+'/LOAD',plot['points'],'OCEAN',type_bis)
-        points_nosed_geoid,_=calc_point(Input_way+'/LOAD',plot['points'],'NO_SEDIMENT',type_bis)
-        points_tot_geoid,_=calc_point(Input_way+'/LOAD',plot['points'],'TOTAL',type_bis)
-        for i_point in range(len(plot['points'])):
-            axes[i_point,1].plot(time_step,points_ice_geoid[i_point,:],label='ice_geoid',color=ice_color)
-            axes[i_point,1].plot(time_step,points_sed_geoid[i_point,:],label='sediment_geoid',color=sediment_color)
-            axes[i_point,1].plot(time_step,points_oc_geoid[i_point,:],label='ocean_geoid',color=ocean_color)
-            axes[i_point,1].plot(time_step,points_nosed_geoid[i_point,:],label='glaciohydrostatic_geoid',color=glaciohydrostatic_color)
-            axes[i_point,1].plot(time_step,points_tot_geoid[i_point,:],label='total_geoid',color='k')
-            #axes[i_point,0].set_ylim(plot['transect_min_max'][i_transect][0],plot['transect_min_max'][i_transect][1])
-            axes[i_point,1].set_xlabel(f'time (kyr)')
-            axes[i_point,1].set_ylabel(f'Vertical Geoid motion (mm/yr)')
-            axes[i_point,1].grid()
-            axes[i_point,1].set_title(f'VGM at point {i_point})')
-            axes[i_point,1].legend()
-        dESL=calculate_dESL(Input_way)
-        for i_point in range(len(plot['points'])):
-            axes[i_point,2].plot(time_step,dESL[:].cumsum()-dESL[:].cumsum()[-1],label='ESL',linestyle='dashed',color='k')
-            axes[i_point,2].plot(time_step,(dESL[:]+points_tot_geoid[i_point,:]-points_tot_load[i_point,:]).cumsum()-(dESL[:]+points_tot_geoid[i_point,:]-points_tot_load[i_point,:]).cumsum()[-1],label='RSL',color='k')
-            axes[i_point,2].legend()
-            axes[i_point,2].grid()
-            axes[i_point,2].set_xlabel(f'time (kyr)')
-            axes[i_point,2].set_ylabel(f'Depth below present sea level (mbpsl)')
-            axes[i_point,2].set_title(f'RSL and ESL at point {i_point})')
-
-        # type_bis='GEOID'
-        # tr_ice_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'ICE',type_bis)
-        # tr_sed_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'SEDIMENT',type_bis)
-        # tr_oc_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'OCEAN',type_bis)
-        # tr_tot_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'TOTAL',type_bis)
-        # axes[1].plot(D,tr_ice_geoid,label='ice_load',color=ice_color)
-        # axes[1].plot(D,tr_sed_geoid,label='sediment_load',color=sediment_color)
-        # axes[1].plot(D,tr_oc_geoid,label='ocean_load',color=ocean_color)
-        # axes[1].plot(D,tr_tot_geoid,label='total load',color='k')
-        # axes[1].set_xlabel(f'distance (km)')
-        # axes[1].set_ylabel(f'Vertical Geoid motion averaged over {dt*1000} year (mm/yr)')
-        # t=plot['times'][i_time]
-        # axes[1].set_title(f'VGM estimated at {t} kyr along transect {i_transect})')
-        # axes[1].grid()
-        # axes[1].set_ylim(plot['transect_min_max'][i_transect][2],plot['transect_min_max'][i_transect][3])
-        # axes[1].legend()
-        plt.close(fig)
-        fig.savefig(f'{Input_way}/LOAD/Points_deformation.pdf')
-
-def plot_frame(Input_way,plot,Output_way,type):
-    '''
-    The _`plot_frame` function define the spherical harmonic coefficient to be expanded into a grid and plot in the frame defined in plot. This function make the difference between sediment subsidence and true sediment subsidence where water replaced by sediment is included. 
-    
-    Attribute :
-    ----------- 
-        Input_way : str
-            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
-        plot : dict(plot=True,times=[n_t],frames=[n_f*(lon1,lon1,lat1,lat2)],frames_resolution=[n_f],frames_min_max=np.array([[[min_load],max_load,min_geoid,max_geoid]]),contours_v=[n_f*2*[contours...]],transects=[n_t*(lat1,lon1,lat2,lon2)],point_density=[n_t], transect_min_max=[n_t(min_load,max_load,min_geoid,max_geoid)], points=np.array([n_p[lat,lon]]))
-            The plot dictionnary used to define all the plot parameters of the output. In this dictionary, there is three main group of parameters, the frame plot parameters, the transect plot parameters and the points plot parameters. The frame plot parameters contain the frame locations in frames, the frames resolution in frames_resolution, the frames min and max value to plot in frames_min_max and the contours value to plot in contours_v. The transect plot parameters contains the location of the begining and end of the transects in transects, the point density along the transect in point_density and the min max value of the transect in transect_min_max. The points plot parameters contains the locations of the differents plots in points. 
-        Output_way : str
-            way where the plot will be saved.
-        type : str
-            This define the type of load considered. Must be "SEDIMENT", "NO_SEDIMENT", "OCEAN", "ICE" or "TOTAL".
-
-        
-
-    Returns : 
-    --------- 
-        None 
-        
-    '''
-    if type is "SEDIMENT" :
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_LOAD'))
-        sediment_load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_LOAD'))
-        load_time_grid.viscuous_deformation=sediment_load_time_grid.viscuous_deformation-load_time_grid.viscuous_deformation
-        load_time_grid.elastic_deformation=sediment_load_time_grid.elastic_deformation-load_time_grid.elastic_deformation
-        geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_GEOID'))
-        sediment_geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_GEOID'))
-        geoid_time_grid.viscuous_deformation=sediment_geoid_time_grid.viscuous_deformation-geoid_time_grid.viscuous_deformation
-        geoid_time_grid.elastic_deformation=sediment_geoid_time_grid.elastic_deformation-geoid_time_grid.elastic_deformation
-    if type is "OCEAN" :
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_LOAD'))
-        sediment_load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_LOAD'))
-        load_time_grid.viscuous_deformation=sediment_load_time_grid.viscuous_deformation+load_time_grid.viscuous_deformation
-        load_time_grid.elastic_deformation=sediment_load_time_grid.elastic_deformation+load_time_grid.elastic_deformation
-        geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_GEOID'))
-        sediment_geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_GEOID'))
-        geoid_time_grid.viscuous_deformation=sediment_geoid_time_grid.viscuous_deformation+geoid_time_grid.viscuous_deformation
-        geoid_time_grid.elastic_deformation=sediment_geoid_time_grid.elastic_deformation+geoid_time_grid.elastic_deformation
-    elif type is "NO_SEDIMENT":
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\TOTAL_LOAD'))
-        sediment_load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\SEDIMENT_LOAD'))
-        oceanic_sediment_load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_LOAD'))
-        load_time_grid.viscuous_deformation=-sediment_load_time_grid.viscuous_deformation+load_time_grid.viscuous_deformation+oceanic_sediment_load_time_grid.viscuous_deformation
-        load_time_grid.elastic_deformation=-sediment_load_time_grid.elastic_deformation+load_time_grid.elastic_deformation+oceanic_sediment_load_time_grid.elastic_deformation
-        
-        ocean_geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEAN_GEOID'))
-        geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\ICE_GEOID'))
-        oceanic_sediment_geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_GEOID'))
-        geoid_time_grid.viscuous_deformation=ocean_geoid_time_grid.viscuous_deformation+geoid_time_grid.viscuous_deformation+oceanic_sediment_geoid_time_grid.viscuous_deformation
-        geoid_time_grid.elastic_deformation=ocean_geoid_time_grid.elastic_deformation+geoid_time_grid.elastic_deformation+oceanic_sediment_geoid_time_grid.elastic_deformation
-    else :
-        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_LOAD'))
-        geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_GEOID'))
-    plot_model_output(load_time_grid,plot,Output_way,f'load_{type}',vmin=(plot['frames_min_max'][:,0]),vmax=plot['frames_min_max'][:,1],contours_v=plot['contours_v'][0])
-    plot_model_output(geoid_time_grid,plot,Output_way,f'geoid_{type}',vmin=(plot['frames_min_max'][:,2]),vmax=plot['frames_min_max'][:,3],contours_v=plot['contours_v'][1])
-
-def plot_model_output(time_grid,plot,Output_way,type=None,vmin=None,vmax=None,contours_v=None):
-    '''
-    The _`plot_model_output` function plot the frames for each frames and at each time steps. 
-    
-    Attribute :
-    ----------- 
-        time_grid : TIME_GRID from `ref`:{TIME_GRID <TIME_GRID>}
-        plot : dict(plot=True,times=[n_t],frames=[n_f*(lon1,lon1,lat1,lat2)],frames_resolution=[n_f],frames_min_max=np.array([[[min_load],max_load,min_geoid,max_geoid]]),contours_v=[n_f*2*[contours...]],transects=[n_t*(lat1,lon1,lat2,lon2)],point_density=[n_t], transect_min_max=[n_t(min_load,max_load,min_geoid,max_geoid)], points=np.array([n_p[lat,lon]]))
-            The plot dictionnary used to define all the plot parameters of the output. In this dictionary, there is three main group of parameters, the frame plot parameters, the transect plot parameters and the points plot parameters. The frame plot parameters contain the frame locations in frames, the frames resolution in frames_resolution, the frames min and max value to plot in frames_min_max and the contours value to plot in contours_v. The transect plot parameters contains the location of the begining and end of the transects in transects, the point density along the transect in point_density and the min max value of the transect in transect_min_max. The points plot parameters contains the locations of the differents plots in points. 
-        Output_way : str
-            way where the plot will be saved.
-        type : str
-            This define the type of load considered. Must be "SEDIMENT", "NO_SEDIMENT", "OCEAN", "ICE" or "TOTAL".
-        vmin : float 
-            The minimal value for the colormap of your plot
-        vmax : float
-            The maximal value for the colormap of your plot
-        contours_v : list
-            List of the contours values to be plot
-
-    Returns : 
-    --------- 
-        None 
-        
-    '''
-    if plot['plot']:
-        if len(plot['frames'])>0 :
-            fig,ax=plt.subplots(len(plot['frames'])*len(plot['times']),3,figsize=(29.7,10*len(plot['frames'])*len(plot['times'])),subplot_kw={'projection': ccrs.PlateCarree(), "aspect": 1})
-            k=0
-            for i_time in range(len(plot['times'])):
-                for i_frame in range(len(plot['frames'])):
-                    axes=ax[k,:]
-                    time=plot['times'][i_time]
-                    central_longitude=0
-                    #ax_total  = plt.subplot(subplot_size+i_time*3+1, projection=ccrs.PlateCarree(central_longitude=central_longitude))
-                    time_grid.height_time_coeff=time_grid.viscuous_deformation+time_grid.elastic_deformation
-                    ax_total=plot_load_frame(axes[0],time_grid,plot['frames'][i_frame],time,plot['frames_resolution'][i_frame],name=f'total {type}',vmin=vmin[i_frame],vmax=vmax[i_frame],contour=contours_v[i_frame])
-
-                    #ax_viscous  = plt.subplot(subplot_size+i_time*3+2, projection=ccrs.PlateCarree(central_longitude=central_longitude))
-                    time_grid.height_time_coeff=time_grid.viscuous_deformation
-                    ax_viscous=plot_load_frame(axes[1],time_grid,plot['frames'][i_frame],time,plot['frames_resolution'][i_frame],name=f'viscous {type}',vmin=vmin[i_frame],vmax=vmax[i_frame],contour=contours_v[i_frame])
-
-                    #ax_elastic = plt.subplot(subplot_size+i_time*3+3, projection=ccrs.PlateCarree(central_longitude=central_longitude))
-                    time_grid.height_time_coeff=time_grid.elastic_deformation
-                    ax_elastic=plot_load_frame(axes[2],time_grid,plot['frames'][i_frame],time,plot['frames_resolution'][i_frame],name=f'elastic {type}',vmin=vmin[i_frame],vmax=vmax[i_frame],contour=contours_v[i_frame]) 
-                    k+=1
-        plt.close(fig)
-        fig.savefig(f'{Output_way}/{type}_deformation.pdf')
-
-import cartopy
-import matplotlib.pyplot as plt
-import cartopy.crs as ccrs
-from matplotlib import cm
-import matplotlib.colors as colors
-
-def plot_precomputation(initial_time_step,initial_grid,precomputed_grid,selected_time=1,area=None,save_way='',lon_init=None,lat_init=None,topo=False,vmin=None,vmax=None):
-    '''
-    The _`plot_precomputation` function plot the output of the precomputation as the ice, sediment and totpography. These plot allow you to compare the entry and the output to be sure there is no errors.
-    
-    Attribute :
-    ----------- 
-        Input_way : str
-            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
-        plot : dict(plot=True,times=[n_t],frames=[n_f*(lon1,lon1,lat1,lat2)],frames_resolution=[n_f],frames_min_max=np.array([[[min_load],max_load,min_geoid,max_geoid]]),contours_v=[n_f*2*[contours...]],transects=[n_t*(lat1,lon1,lat2,lon2)],point_density=[n_t], transect_min_max=[n_t(min_load,max_load,min_geoid,max_geoid)], points=np.array([n_p[lat,lon]]))
-            The plot dictionnary used to define all the plot parameters of the output. In this dictionary, there is three main group of parameters, the frame plot parameters, the transect plot parameters and the points plot parameters. The frame plot parameters contain the frame locations in frames, the frames resolution in frames_resolution, the frames min and max value to plot in frames_min_max and the contours value to plot in contours_v. The transect plot parameters contains the location of the begining and end of the transects in transects, the point density along the transect in point_density and the min max value of the transect in transect_min_max. The points plot parameters contains the locations of the differents plots in points. 
-        Output_way : str
-            way where the plot will be saved.
-        type : str
-            This define the type of load considered. Must be "SEDIMENT", "NO_SEDIMENT", "OCEAN", "ICE" or "TOTAL".
-        vmin : float 
-            The minimal value for the colormap of your plot
-        vmax : float
-            The maximal value for the colormap of your plot
-
-    Returns : 
-    --------- 
-        None 
-        
-    '''
-    our_ind=np.where((precomputed_grid.time_step-selected_time)==0)[0][0]
-    in_ind=np.where((initial_time_step-selected_time)==0)[0][0]
-
-    cmap=cm.get_cmap('bwr', 255)
-    alpha_ocean=0
-    coast_line_width=0.5
-    norm1 = colors.TwoSlopeNorm(vmin=-0.1,vmax=None,vcenter=0)
-    fig = plt.figure(figsize=(12, 6), facecolor="none")
-
-    # plot the initial data
-
-    norm = colors.TwoSlopeNorm(vmin=vmin,vmax=vmax,vcenter=0)
-
-    if area is None :
-        ax_init  = plt.subplot(121, projection=ccrs.Mollweide())
-        ax_init.set_global()
-    else :
-        ax_init  = plt.subplot(121, projection=ccrs.PlateCarree())
-        ax_init.set_extent(area)
-
-    if not(lon_init is None) :
-        m_init = ax_init.scatter(lon_init,lat_init,c=initial_grid[:in_ind+1,:].sum(0),transform=ccrs.PlateCarree(),zorder=0,norm=norm,cmap=cmap)
-        cbar_init=plt.colorbar(mappable=m_init, orientation="horizontal")
-        cbar_init.set_label(precomputed_grid.time_grid_name + '(m)')
-        #cbar_init.set_ticks([0, initial_grid[:in_ind+1].sum(0).max()])
-        ax_init.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
-        ax_init.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
-        cartopy.mpl.geoaxes.GeoAxes.gridlines(ax_init,crs=ccrs.PlateCarree(),draw_labels=True)
-    else : 
-        if topo : 
-            m_init = ax_init.imshow(initial_grid, origin='lower', transform=ccrs.PlateCarree(),extent=[0,360, -89, 89], zorder=0, cmap=cmap, interpolation="gaussian",norm=norm)
-            cbar_init=plt.colorbar(mappable=m_init, orientation="horizontal")
-            cbar_init.set_label(precomputed_grid.time_grid_name + '(m)')
-            #cbar_init.set_ticks([0, initial_grid[:in_ind+1].sum(0).max()])
-            ax_init.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
-            ax_init.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
-        else : 
-            m_init = ax_init.imshow(initial_grid[:in_ind+1].sum(0), origin='lower', transform=ccrs.PlateCarree(),extent=[0,360, -89, 89], zorder=0, cmap=cmap, interpolation="gaussian",norm=norm)
-            cbar_init=plt.colorbar(mappable=m_init, orientation="horizontal")
-            cbar_init.set_label(precomputed_grid.time_grid_name + '(m)')
-            #cbar_init.set_ticks([0, initial_grid[:in_ind+1].sum(0).max()])
-            ax_init.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
-            ax_init.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
-        cartopy.mpl.geoaxes.GeoAxes.gridlines(ax_init,crs=ccrs.PlateCarree(),draw_labels=True)
-
-    if area is None :
-        ax_precomp  = plt.subplot(122, projection=ccrs.Mollweide())
-        ax_precomp.set_global()
-    else :
-        ax_precomp  = plt.subplot(122, projection=ccrs.PlateCarree())
-        ax_precomp.set_extent(area)
-
-    colormap = cmap
-    if topo :
-        m2 = ax_precomp.imshow(precomputed_grid.height_time_grid[-1,:,:], origin='lower', transform=ccrs.PlateCarree(),extent=[0,360, -89, 89], zorder=0, cmap=colormap, interpolation="gaussian",norm=norm)
-        cbar2=plt.colorbar(mappable=m2, orientation="horizontal")
-        cbar2.set_label(precomputed_grid.time_grid_name + ' interpolated (m)')
-        #cbar2.set_ticks([0, precomputed_grid.height_time_grid[:our_ind+1,:,:].sum(0).max()])
-        ax_precomp.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
-        ax_precomp.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
-
-    else : 
-        m2 = ax_precomp.imshow(precomputed_grid.height_time_grid[:our_ind+1,:,:].sum(0), origin='lower', transform=ccrs.PlateCarree(),extent=[0,360, -89, 89], zorder=0, cmap=colormap, interpolation="gaussian",norm=norm)
-        cbar2=plt.colorbar(mappable=m2, orientation="horizontal")
-        cbar2.set_label(precomputed_grid.time_grid_name + ' interpolated (m)')
-        #cbar2.set_ticks([0, precomputed_grid.height_time_grid[:our_ind+1,:,:].sum(0).max()])
-        ax_precomp.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
-        ax_precomp.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
-    cartopy.mpl.geoaxes.GeoAxes.gridlines(ax_precomp,crs=ccrs.PlateCarree(),draw_labels=True)
-
-    plt.close(fig)
-
-    fig.savefig(save_way+'/'+precomputed_grid.time_grid_name+'.pdf')
-
-def calculate_dESL(Input_way):
-    '''
-    The _`calculate_dESL` function compute the ESL variation over time including a varaible ocean surface.
-    
-    Attribute :
-    ----------- 
-        Input_way : str
-            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
-
-    Returns : 
-    --------- 
-        dESL : np.array([time_step_number,])
-            The variation of the ESL at each time step.
-        
-    '''
-    ocean_grid=OCEAN_TIME_GRID(from_file=(True,Input_way+"/OCE"))
-
-    ice=ICE_TIME_GRID(from_file=(True,Input_way+"/ICE_ICE6G"))
-
-    topo=TOPOGRAPHIC_TIME_GRID(from_file=(True,Input_way+"/topo_SL"))
-    dESL=np.zeros(ice.time_step_number)
-    for t_it in range(ice.time_step_number-1):
-        ocean_grid.evaluate_ocean(topo.height_time_grid[t_it,:,:]).grdtocoeff()
-        dESL[t_it]=np.real(1/ocean_grid.coeff[0] * (- ice.rho/ocean_grid.rho*ice.height_time_coeff[t_it,0]))
-    return dESL
-
-import cartopy
-import cartopy.crs as ccrs
-import matplotlib
-from matplotlib import cm
-import matplotlib as mpl
-import matplotlib.colors as colors
-import numpy as np
-import matplotlib.pyplot as plt
-
-def plot_load_frame(ax,data,frame,time,resolution,name,add_contour=None,vmin=None,vmax=None,vcenter=0,contour=None,color=None):
-    '''
-    The _`plot_load_frame` function plot the data in entry into a defined frame following different arguments fro the plot.
-    
-    Attribute :
-    ----------- 
-        ax : matplotlib.pyplot.axes
-            The axis on wich the data will be plot.
-        data : LOAD_TIME_GRID
-            A LOAD_TIME_GRID object with the LOAD_TIME_GRID.coeff to be ploted.
-        frame : (lon1,lon2,lat1,lat2)
-            The coordinate of the frame to plot.
-        time : float
-            The time of the plot that will be plot
-        resolution : int
-            The resolution of the plot, the resulting resolution will be resolution x resolution*2
-        name : str
-            The name of the plot, will be used in the title and legend of the plot
-        vmin : float
-            The minimal value of the plot colormap
-        vmax : float
-            The maximal value of the plot colormap
-        vcenter : float
-            The central value of the plot colormap
-        contour : np.array([n_c])
-            The contour that will be ploted on the map
-        color : np.array([n_c])
-            The contour fill color to be ploted
-        
-
-    Returns : 
-    --------- 
-        ax : matplotlib.pyplot.axes
-            The axis updated from the plots
-        
-    '''
-    t_it=np.where(data.time_step==time)[0][0]
-    data.coeff=(data.coeff_from_step(t_it-2).coeff-data.coeff_from_step(t_it-3).coeff)/(data.time_step[t_it-1]-data.time_step[t_it])
-    grid,lon_hd,lat_hd=data.coefftogrdhd(resolution)
-    lon_hd-=180
-    grid=np.concatenate((grid[:,resolution-1:],grid[:,:resolution]),axis=1)
-    lon_lim_min=np.abs(lon_hd-frame[0]).argmin()
-    lon_lim_max=np.abs(lon_hd-frame[1]).argmin()
-    lat_lim_min=np.abs(lat_hd-frame[2]).argmin()
-    lat_lim_max=np.abs(lat_hd-frame[3]).argmin()
-    lon=lon_hd[lon_lim_min:lon_lim_max+1]
-    lat=lat_hd[lat_lim_min:lat_lim_max+1]
-    grid=grid[lat_lim_min:lat_lim_max+1,lon_lim_min:lon_lim_max+1]
-
-
-    alpha_ocean=0
-    coast_line_width=0.5
-    #cmap=cm.get_cmap('rainbow', 100)
-    cmap=mpl.colors.LinearSegmentedColormap.from_list('hsv_2',mpl.colormaps['hsv_r'].resampled(255)(range(255))[20:-20],gamma=1.0)
-    if not(color is None):
-        cmap=None
-
-    norm = colors.TwoSlopeNorm(vmin=vmin,vmax=vmax,vcenter=vcenter)
-    if not(contour[0] is None):
-        if contour[0]<0 and contour[-1]>0 :
-            norm = colors.TwoSlopeNorm(vmin=contour[0],vmax=contour[-1],vcenter=0)
-        elif contour[0]<0 and contour[-1]<0 :
-            norm  = colors.TwoSlopeNorm(vmin=contour[0],vmax=contour[-1],vcenter=contour[-1])
-        elif contour[0]>0 and contour[-1]>0 :
-            norm  = colors.TwoSlopeNorm(vmin=contour[0],vmax=contour[-1],vcenter=contour[0])
-    
-    #print(frame_corr)
-    ax.set_extent(frame)
-    #ax.set_global()
-    if contour[0] is None :
-        m2 = ax.contourf(lon,lat,grid,origin='lower', transform=ccrs.PlateCarree(central_longitude=0),extent=frame, zorder=0, cmap=cmap,colors=color,norm=norm)
-    else :
-        m2 = ax.contourf(lon,lat,grid,levels=contour,origin='lower', transform=ccrs.PlateCarree(central_longitude=0),extent=frame, zorder=0, cmap=cmap,colors=color,norm=norm)
-    if not(add_contour is None):
-        CS=ax.contour(lat,lon,add_contour,5,colors='k',linewidths=0.5,linestyles='solid')
-        ax.clabel(CS, CS.levels, inline=True, fontsize=10)
-    
-    cbar2=plt.colorbar(mappable=m2, orientation="horizontal")
-    cbar2.set_label(f'{name} VGM at {time} kyr, averaged over {(data.time_step[t_it-1]-data.time_step[t_it])*1000} year (mm/yr); maximum subsidenc : {np.min(np.min(grid))}')
-    # if not(contour is None):
-    #     cbar2.set_ticks(contour)
-    # elif not(vmax is None) and not(vmin is None):
-    #     cbar2.set_ticks([vmin, 0, vmax])
-    # elif not(vmin is None):
-    #     cbar2.set_ticks([vmin, 0, grid.max()])
-    # elif not(vmax is None):
-    #     cbar2.set_ticks([grid.min(), 0, vmax])
-    # else:
-    #     cbar2.set_ticks([grid.min(), 0, grid.max()])
-    cartopy.mpl.geoaxes.GeoAxes.gridlines(ax,crs=ccrs.PlateCarree(),draw_labels=True)
-    ax.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
-    ax.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
-
-    return ax
-
-from netCDF4 import Dataset
-
-
-
-def export_to_netcdf(Input_way,time,resolution,frame,save_way,type,type_bis):
-    '''
-    The _`export_to_netcdf` function export the data from the input_way, type and type_bis, of the frame shape into a netcdf file. This file can be open in any gis software.
-
-    Attribute : 
-    -----------
-        Input_way : str
-            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
-        time : float
-            The time of the plot in kyr
-        resolution : int
-            the spatial resolution of the plot. ! This resolution concern the entire globe and not juste the frame.
-        frame : (lon1,lon2,lat1,lat2)
-            The coordinate of the frame to plot.
-        save_way : str
-            The filepath to save the netcdf file
-        type : str 
-            The type of loading taken into account. Can be : "SEDIMENT", "OCEAN", "ICE", "NO_SEDIMENT".
-        type_bis : str
-            The type of affected surface by the loading. Can be : "GEOID", "LOAD".
-            
-    ''' 
-    data=LOAD_TIME_GRID(from_file=(True,f'{Input_way}/LOAD/{type}_{type_bis}'))
-    t_it=np.where(data.time_step==time)[0][0]
-    data.height_time_coeff=data.viscuous_deformation+data.elastic_deformation
-    data.coeff=(data.coeff_from_step(t_it-2).coeff-data.coeff_from_step(t_it-3).coeff)/(data.time_step[t_it-1]-data.time_step[t_it])
-    grid,lon_hd,lat_hd=data.coefftogrdhd(resolution)
-    lon_hd-=180
-    grid=np.concatenate((grid[:,resolution-1:],grid[:,:resolution]),axis=1)
-    lon_lim_min=np.abs(lon_hd-frame[0]).argmin()
-    lon_lim_max=np.abs(lon_hd-frame[1]).argmin()
-    lat_lim_min=np.abs(lat_hd-frame[2]).argmin()
-    lat_lim_max=np.abs(lat_hd-frame[3]).argmin()
-    lon=lon_hd[lon_lim_min:lon_lim_max+1]
-    lat=lat_hd[lat_lim_min:lat_lim_max+1]
-    grid=grid[lat_lim_min:lat_lim_max+1,lon_lim_min:lon_lim_max+1]
-
-    data.ncgrid=Dataset(f'{save_way}/{data.time_grid_name}{frame}.nc','w','NETCDF4_CLASSIC')
-    data.ncgrid.title=data.time_grid_name
-
-    data.ncgrid.createDimension('lon',len(lon))
-    data.ncgrid.createDimension('lat',len(lat))
-
-
-    lati=data.ncgrid.createVariable('lat', np.float32, ('lat',))
-    lati.units = 'degrees_north'
-    lati.long_name = 'latitude'
-    lati[:]=lat
-
-    long=data.ncgrid.createVariable('lon', np.float32, ('lon',))
-    long.units = 'degrees_east'
-    long.long_name = 'longitude'
-    long[:]=lon
-
-    grided=data.ncgrid.createVariable('grid', np.float32, ('lat','lon'))
-    grided.units = 'mm/yr'
-    grided.long_name = 'grid'
-    grided[:,:]=grid
-
-    data.ncgrid.close()
+from .grid import ICE_TIME_GRID
+from .grid import SEDIMENT_TIME_GRID
+from .grid import TOPOGRAPHIC_TIME_GRID
+from .grid import OCEAN_TIME_GRID
+from .grid import LOAD_TIME_GRID
+from .spharm import sphericalobject
+from .love import LOVE
+import numpy as np
+import copy
+import os
+import sys
+
+def Precomputation(ice_grid,sed_grid,topo_grid,Output_way,stop=26,step=0.5,maxdeg=512,irregular_time_step=None,backend=False,plot=False):
+    '''
+    The _`Precomputation` method prepare the different data to match temporal and spatial resolution of the modelisation. spatial resolution (m,n) and temporal resolution (step). The input data format is described in :ref:`Mass grid format<grid_format>`.
+
+    Attribute :
+    ----------- 
+        ice_grid : dict(name = str, grid = np.array((n_i,m_i,t_i)), time = np.array((t_i,)), lon = np.array((n_i)), lat = np.array((m_i)))
+            ice thickness grid
+        sed_grid : dict(name = str, grid = np.array((n_j,m_j,t_j)), time = np.array((t_j,)), lon = np.array((n_j)), lat = np.array((m_j)),frame = (lon1,lon2,lat1,lat2))
+            sediment thickness
+        topo_grid : dict(name = str, grid = np.array((n_k,m_k)), lon = np.array((n_j)), lat = np.array((m_j)))
+            present topography 
+        Output_way : str
+            The filepath toward wich the different grid will be saved
+        stop : float 
+            age at wich the computation stop
+        step : float
+            time step used for the temporal resolution of the model
+        maxdeg : int 
+            The maximum degree of spherical harmonics, that define the spatial resolution of the model. (m = 2*maxdeg, n = maxdeg)
+        irregular_time_step : np.array((time_step_number,))
+            An irregular time array to compute the model over non regular time step
+        backend : bool
+            If required you can ask a backend during the run of each computation. True, will generate a backend, False will not. Defaul is False
+        Plot : bool
+            If needed you can ask plot of each output compared to the initial plot. You will need the cartopy doc.
+    Returns : 
+    --------- 
+        None 
+
+    The data output of the function are saved to the output way.
+
+    '''
+
+    time_step=np.arange(start=stop,stop=-step,step=-step)
+    if time_step[-1]<0:
+        time_step[-1]=0
+    if not(irregular_time_step is None):
+        time_step=irregular_time_step
+
+    ice_time_grid=ICE_TIME_GRID(time_step,maxdeg,grid_name=ice_grid['name'])
+    ice_time_grid.interp_on_time_and_space(ice_grid['grid'],ice_grid['time'],ice_grid['lon'],ice_grid['lat'],grid_type='global',backend=backend)
+    ice_time_grid.save(save_way=Output_way)
+
+    sed_time_grid=SEDIMENT_TIME_GRID(time_step,maxdeg,grid_name=sed_grid['name'])
+    sed_time_grid.interp_on_time_and_space(sed_grid['grid'],sed_grid['time'],sed_grid['lon'],sed_grid['lat'],backend=backend,grid_type='local')
+    sed_time_grid.height_time_grid=sed_time_grid.height_time_grid=sed_time_grid.height_time_grid[:,::-1,:]# latitude are inverted ! 
+    sed_time_grid.save(save_way=Output_way)
+
+
+    topo_time_grid=TOPOGRAPHIC_TIME_GRID(time_step,maxdeg,grid_name=topo_grid['name'])
+    topo_time_grid.topo_pres=topo_time_grid.interp_on(topo_grid['grid'],topo_grid['lon'],topo_grid['lat'],grid_type='global')+ice_time_grid.height_time_grid.sum(0)
+
+    # there is no ice in topo_sl
+
+    for i in range(topo_time_grid.time_step_number-1):
+        if i==0:
+            topo_time_grid.height_time_grid[i,:,:]=topo_time_grid.topo_pres-sed_time_grid.height_time_grid.sum(0)-ice_time_grid.height_time_grid[1:,:,:].sum(0)
+        else :
+            topo_time_grid.height_time_grid[i,:,:]=topo_time_grid.topo_pres-sed_time_grid.height_time_grid[i:,:,:].sum(0)-ice_time_grid.height_time_grid[i:,:,:].sum(0)
+    
+    topo_time_grid.save(save_way=Output_way)
+
+    if plot :
+        plot_precomputation(ice_grid['time'],ice_grid['grid'],ice_time_grid,save_way=Output_way)
+        plot_precomputation(sed_grid['time'],sed_grid['grid'],sed_time_grid,area=sed_grid['frame'],lon_init=sed_grid['lon'],lat_init=sed_grid['lat'],save_way=Output_way)
+        colors_undersea = plt.cm.terrain(np.linspace(0, 0.17, 256))
+        colors_land = plt.cm.terrain(np.linspace(0.25, 1, 256))
+        all_colors = np.vstack((colors_undersea, colors_land))
+        terrain_map = colors.LinearSegmentedColormap.from_list('terrain_map',all_colors)
+        plot_precomputation(np.array([1]),topo_grid['grid'],topo_time_grid,topo=True,save_way=Output_way,vcenter=0,cmap=terrain_map)
+
+def SLE_forward_modeling(Input_way,ice_name,sed_name,topo_name,ocean_name,love_way,love_file,conv_lim,Output_way):
+    '''
+    The _`SLE_forward_modeling` method solve the SLE with no constrain on final topography. This result in a forward modeling of the SL. It can be used for test and exploration of models. For informations on iterations see :ref:`description of iteration <iteration_desc>`.
+
+    Attribute : 
+    ------------
+        Input_way : str
+            File location of the input data (ice, sediment and topography)
+        ice_name : str
+            The name of the ice data file
+        sed_name : str
+            The name of the sediment data file
+        topo_name : str
+            The name of the topographic data file
+        ocean_name : str
+            The name of the output file containig the data on the ocean
+        love_way : str 
+            way of the love numbers file used to compute earth visco elastic deformation
+        conv_lim : float
+            Limit of precision required for the convergence of the SLE resolution (10^-3)
+        output_way : str 
+            filepath for saving results of the modelisation
+
+    Returns :
+    --------- 
+        None 
+
+    The resulting ocean class object (:ref:`OCEAN_TIME_GRID <OCEAN_TIME_GRID>`) containing the ocean thickness is saved in the outputway under the name ocean. 
+    '''
+    ice_time_grid=ICE_TIME_GRID(from_file=(True,Input_way+'/'+ice_name))
+    sed_time_grid=SEDIMENT_TIME_GRID(from_file=(True,Input_way+'/'+sed_name))
+    topo_time_grid=TOPOGRAPHIC_TIME_GRID(from_file=(True,Input_way+'/'+topo_name))
+
+    ocean_time_grid=OCEAN_TIME_GRID(ice_time_grid.time_step,ice_time_grid.maxdeg,grid_name=ocean_name)
+    ocean_time_grid.time_step_number=ocean_time_grid.time_step_number
+
+    love_number=LOVE(ice_time_grid.maxdeg,love_way+'/'+love_file,ice_time_grid.time_step,6371000,5.9742e24,type='time')
+    love_number.dev_beta()
+
+    TO=sphericalobject(coeff=np.zeros(ice_time_grid.height_time_coeff[0,:].shape))
+    TO.prev=np.zeros(ice_time_grid.height_time_coeff[0,:].shape)
+
+    
+
+    ice_time_grid.ice_correction(topo_time_grid,ocean_time_grid)
+    ice_time_grid.timegrdtotimecoeff()
+
+    load=LOAD_TIME_GRID(sdelL=ice_time_grid.height_time_coeff[1:t_it,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[1:t_it,:]*sed_time_grid.rho+ocean_time_grid.height_time_coeff[1:t_it,:]*ocean_time_grid.rho,beta_l=love_number.beta_l,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg)
+
+    topo_time_grid.update_0()
+    ocean_time_grid.evaluate_ocean(topo_time_grid.grd_0).grdtocoeff()
+    ocean_time_grid.update_0()
+    ocean_time_grid.save_prev()
+    topo_time_grid.grid_from_step(0)
+    # grd correspond donc au topo_j défini dans le code de kendal et al.
+    ocean_time_grid.evaluate_ocean(topo_time_grid.grd).grdtocoeff()
+    TO.grd=topo_time_grid.grd_0*(ocean_time_grid.grd-ocean_time_grid.grd_0)
+    TO.grdtocoeff()
+
+    track_conv=np.array([])
+
+    for t_it in range (1,ice_time_grid.time_step_number-1):
+        topo_time_grid.grid_from_step(t_it)
+        # grd correspond donc au topo_j défini dans le code de kendal et al.
+        ocean_time_grid.evaluate_ocean(topo_time_grid.grd).grdtocoeff()
+        TO.grd=topo_time_grid.grd_0*(ocean_time_grid.grd-ocean_time_grid.grd_0)
+        TO.grdtocoeff()
+        sed_time_grid.coeff_from_step(t_it)
+        ice_time_grid.coeff_from_step(t_it)
+        
+        conv_it=0
+        conv_it=ocean_time_grid.sea_level_solver(load,ice_time_grid,sed_time_grid,love_number,TO,t_it,conv_it,conv_lim)
+
+        track_conv=np.append(track_conv,conv_it)     
+        
+        TO.prev=TO.coeff.copy()
+
+        ocean_time_grid.save_prev()
+        
+        topo_time_grid.height_time_grid[t_it,:,:]=topo_time_grid.grd_0-(ocean_time_grid.delSLcurl.grd+ocean_time_grid.delPhi_g)
+    
+    if not(os.path.exists(Output_way+'/model_output')):
+            os.mkdir(Output_way+'/model_output')
+    Output_way=Output_way+'/model_output'
+
+    if not(os.path.exists(Output_way+'/'+love_file)):
+        os.mkdir(Output_way+'/'+love_file)
+    ocean_time_grid.save(Output_way+'/'+love_file)
+    ice_time_grid.save(Output_way+'/'+love_file)
+    topo_time_grid.save(Output_way+'/'+love_file)
+    print(sed_time_grid.time_grid_name)
+    sed_time_grid.save(Output_way+'/'+love_file)
+
+def SLE_solver(Input_way,ice_name,sed_name,topo_name,ocean_name,love_way,love_file,topo_lim,conv_lim,Output_way):
+    '''
+    The _`SLE_solver` solve the SLE and converge toward the actual topography. The computation of the SLE resolution is describe in :ref:`Sea level equation resolution <SLE_res>`. For informations on iterations see :ref:`description of iteration <iteration_desc>`.
+
+    Attribute :
+    ----------- 
+        Input_way : str
+            File location of the input data (ice, sediment and topography)
+        ice_name : str
+            The name of the ice data file
+        sed_name : str
+            The name of the sediment data file
+        topo_name : str
+            The name of the topographic data file
+        ocean_name : str
+            The name of the output file containig the data on the ocean
+        love_way : str 
+            way of the love numbers file used to compute earth visco elastic deformation
+        conv_lim : float
+            Limit of precision required for the convergence of the SLE resolution (10^-3)
+        topo_lim : float
+            Topography convergence limit toward wich the iteration will converge (1 m)
+        output_way : str 
+            filepath for saving results of the modelisation
+
+    Returns : 
+    --------- 
+        None 
+
+    The resulting ocean class object (:ref:`OCEAN_TIME_GRID <OCEAN_TIME_GRID>`), updated ice thickness (:ref:`ICE_TIME_GRID <ICE_TIME_GRID>`) and updated  topography (:ref:`TOPOGRAPHIC_TIME_GRID <TOPOGRAPHIC_TIME_GRID>`) are saved to output_way. 
+    '''
+    
+    ice_time_grid=ICE_TIME_GRID(from_file=(True,Input_way+'/'+ice_name))
+    sed_time_grid=SEDIMENT_TIME_GRID(from_file=(True,Input_way+'/'+sed_name))
+    topo_time_grid=TOPOGRAPHIC_TIME_GRID(from_file=(True,Input_way+'/'+topo_name))
+
+    maxdeg=ice_time_grid.maxdeg
+
+    time_step=ice_time_grid.time_step.copy()
+
+    # Initiate the base elements
+    from SL_C0de.spharm import sphericalobject
+    from SL_C0de.Load import LOAD
+
+    ocean_time_grid=OCEAN_TIME_GRID(time_step,maxdeg,grid_name=ocean_name)
+    ocean_time_grid.time_step_number=ocean_time_grid.time_step_number
+
+    ice_time_grid.timegrdtotimecoeff()
+    sed_time_grid.timegrdtotimecoeff()
+
+    love_number=LOVE(maxdeg,love_way+'/'+love_file,time_step,6371000,5.9742e24)
+    love_number.dev_beta()
+    love_number.dev_beta_tide()
+    TO=sphericalobject(coeff=np.zeros(ice_time_grid.height_time_coeff[0,:].shape))
+
+
+    topo_diff_median=np.inf
+    #sdel_topo_diff=np.inf
+    topo_it=0
+    while topo_diff_median>topo_lim : #and sdel_topo_diff>10**(-1):
+        delPhi_g_time=np.array([])
+        TO.prev=np.zeros(ice_time_grid.height_time_coeff[0,:].shape)
+
+        if topo_diff_median != np.inf :
+            topo_time_grid.height_time_grid[0,:,:]=topo_initial.copy()
+        # topo_time_grid.height_time_grid = topo_time_grid.height_time_grid - ice_time_grid.height_time_grid + ice_time_grid.ice # for resetting the corrected ice.
+        ice_time_grid.ice_correction(topo_time_grid,ocean_time_grid)
+        ice_time_grid.timegrdtotimecoeff()
+
+        t_it=-1
+
+        load=LOAD_TIME_GRID(sdelL=ice_time_grid.height_time_coeff[1:t_it,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[1:t_it,:]*sed_time_grid.rho+ocean_time_grid.height_time_coeff[1:t_it,:]*ocean_time_grid.rho,beta_l=love_number.beta_l,E=love_number.E,E_T=love_number.E_T,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg)
+        
+        topo_time_grid.update_0()
+        ocean_time_grid.evaluate_ocean(topo_time_grid.grd_0).grdtocoeff()
+        ocean_time_grid.update_0()
+        ocean_time_grid.save_prev()
+        topo_time_grid.grid_from_step(0)
+        # grd correspond donc au topo_j défini dans le code de kendal et al.
+        ocean_time_grid.evaluate_ocean(topo_time_grid.grd).grdtocoeff()
+        TO.grd=topo_time_grid.grd_0*(ocean_time_grid.grd-ocean_time_grid.grd_0)
+        TO.grdtocoeff()
+
+        track_conv=np.array([])
+
+        for t_it in range (1,ice_time_grid.time_step_number-1):
+            topo_time_grid.grid_from_step(t_it)
+            # grd correspond donc au topo_j défini dans le code de kendal et al.
+            ocean_time_grid.evaluate_ocean(topo_time_grid.grd).grdtocoeff()
+            TO.grd=topo_time_grid.grd_0*(ocean_time_grid.grd-ocean_time_grid.grd_0)
+            TO.grdtocoeff()
+            sed_time_grid.coeff_from_step(t_it)
+            ice_time_grid.coeff_from_step(t_it)
+            
+
+
+            print('time_iteration : ',ice_time_grid.time_step[t_it])
+            if topo_it==0 : 
+                conv_it=0
+            else :
+                conv_it=1
+            conv_it=ocean_time_grid.sea_level_solver(load,ice_time_grid,sed_time_grid,love_number,TO,t_it,conv_it,conv_lim)
+
+            print(conv_it)
+
+            track_conv=np.append(track_conv,conv_it)     
+            
+            TO.prev=TO.coeff.copy()
+
+            ocean_time_grid.save_prev()
+            
+            topo_time_grid.height_time_grid[t_it,:,:]=topo_time_grid.grd_0-(ocean_time_grid.delSLcurl.grd+ocean_time_grid.delPhi_g)
+            
+
+            #delPhi_g_time=np.append(delPhi_g_time,ocean_time_grid.delPhi_g)
+
+        topo_it+=1
+        topo_pres_ice_corrected=topo_time_grid.topo_pres-ice_time_grid.ice.sum(0)+ice_time_grid.height_time_grid.sum(0)
+        topo_diff=np.abs(topo_time_grid.height_time_grid[-1,:,:]-topo_pres_ice_corrected).max().max()
+        sdel_topo_diff=np.abs(topo_diff-np.abs(topo_time_grid.height_time_grid[-1,:,:]-topo_pres_ice_corrected).max().max())
+        topo_diff_mean=np.abs(topo_time_grid.height_time_grid[-1,:,:]-topo_pres_ice_corrected).mean().mean()
+        topo_diff_median=np.median(np.median(np.abs(topo_time_grid.height_time_grid[-1,:,:]-topo_pres_ice_corrected)))
+        print(topo_it,' : ',topo_diff, topo_diff_mean, topo_diff_median, sdel_topo_diff,track_conv-(topo_it>0))
+        topo_initial=topo_pres_ice_corrected - (topo_time_grid.height_time_grid[-1,:,:]-topo_time_grid.height_time_grid[0,:,:])
+
+    if not(os.path.exists(Output_way+'/model_output')):
+        os.mkdir(Output_way+'/model_output')
+    Output_way=Output_way+'/model_output'
+
+    if not(os.path.exists(Output_way+'/'+love_file)):
+        os.mkdir(Output_way+'/'+love_file)
+    ocean_time_grid.save(Output_way+'/'+love_file)
+    ice_time_grid.save(Output_way+'/'+love_file)
+    topo_time_grid.save(Output_way+'/'+love_file)
+    sed_time_grid.save(Output_way+'/'+love_file)
+    return load
+
+def find_files(filename, search_path):
+    result = []
+
+    # Wlaking top-down from the root
+    for root, dir, files in os.walk(search_path):
+        if filename in dir:
+            result.append(os.path.join(root, filename))
+    return result
+
+def calculate_deformation(love_number,ice_time_grid,sed_time_grid,ocean_time_grid,a,Me,Output_way,backend=False,plot=dict(plot=False)) :
+
+    '''
+    The _`calculate_deformation` method calculate the earth viscoelastic response resulting from the different masses caculated with the :ref:`SLE_solver <SLE_solver>`. This computation follows the decomposition of the SLE described in :ref:`Computation of ground and geoid subsidence from different load source <G_R_comp>`
+
+    Attribute :
+    ----------- 
+        love_number : :ref:`LOVE <LOVE>` 
+            The loaded love number in the form of a LOVE class object
+        ice_time_grid : :ref:`grid.ICE_TIME_GRID <ICE_TIME_GRID>`
+            ice thickness in the form of ICE_TIME_GRID class object
+        sed_time_grid : :ref:`grid.SEDIMENT_TIME_GRID <SEDIMENT_TIME_GRID>` 
+            sediment thickness in the form of SEDIMENT_TIME_GRID class object
+        ocean_time_grid : :ref:`grid.OCEAN_TIME_GRID <OCEAN_TIME_GRID>` 
+            ocean thickness calculated using the SLE solver in the form of OCEAN_TIME_GRID class object
+        a : float
+            radius of earth in meter
+        Me : float
+            mass of earth (kg)
+        Output_way : str
+            way of the output where the load is calculated
+        backend : bool
+            set if the function is writing its state of computation
+
+    Returns :  
+    ---------
+        None 
+
+    The resulting LOAD and GEOID are stored in a LOAD file in the same file then the input files. The structure is based on the :ref:`LOAD_TIME_GRID <LOAD_TIME_GRID>`  class object.
+    '''
+    beta_l=love_number.beta_R_l
+
+    ice_load_time_grid=LOAD_TIME_GRID(sdelL=ice_time_grid.height_time_coeff*ice_time_grid.rho,beta_l=beta_l,E=love_number.h_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='ICE_LOAD')
+    ice_load_time_grid.calc_elastic_time()
+    ice_load_time_grid.calc_viscuous_time(backend=backend)
+    ice_load_time_grid.save(save_way=Output_way)    
+    ice_load_time_grid=0
+
+    sediment_load_time_grid=LOAD_TIME_GRID(sdelL=sed_time_grid.height_time_coeff*sed_time_grid.rho,beta_l=beta_l,E=love_number.h_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='SEDIMENT_LOAD')
+    sediment_load_time_grid.calc_elastic_time()
+    sediment_load_time_grid.calc_viscuous_time(backend=backend)
+    sediment_load_time_grid.save(save_way=Output_way)
+    sediment_load_time_grid=0
+
+    ocean_load_time_grid=LOAD_TIME_GRID(sdelL=ocean_time_grid.height_time_coeff*ocean_time_grid.rho,beta_l=beta_l,E=love_number.h_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='OCEAN_LOAD')
+    ocean_load_time_grid.calc_elastic_time()
+    ocean_load_time_grid.calc_viscuous_time(backend=backend)
+    ocean_load_time_grid.save(save_way=Output_way)
+    ocean_load_time_grid=0
+
+    total_load_time_grid=LOAD_TIME_GRID(sdelL=ice_time_grid.height_time_coeff*ice_time_grid.rho+sed_time_grid.height_time_coeff*sed_time_grid.rho+ocean_time_grid.height_time_coeff*ocean_time_grid.rho,beta_l=beta_l,E=love_number.h_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='TOTAL_LOAD')
+    total_load_time_grid.calc_elastic_time()
+    total_load_time_grid.calc_viscuous_time(backend=backend)
+    total_load_time_grid.save(save_way=Output_way)
+    total_load_time_grid=0
+
+    #Calculating the geoïd deformation
+
+    beta_l=love_number.beta_G_l
+
+    ice_geoid_time_grid=LOAD_TIME_GRID(sdelL=ice_time_grid.height_time_coeff*ice_time_grid.rho,beta_l=beta_l,E=1+love_number.k_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='ICE_GEOID')
+    ice_geoid_time_grid.calc_elastic_time()
+    ice_geoid_time_grid.calc_viscuous_time(backend=backend)
+    ice_geoid_time_grid.save(save_way=Output_way)
+    ice_geoid_time_grid=0
+
+    sediment_geoid_time_grid=LOAD_TIME_GRID(sdelL=sed_time_grid.height_time_coeff*sed_time_grid.rho,beta_l=beta_l,E=1+love_number.k_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='SEDIMENT_GEOID')
+    sediment_geoid_time_grid.calc_elastic_time()
+    sediment_geoid_time_grid.calc_viscuous_time(backend=backend)
+    sediment_geoid_time_grid.save(save_way=Output_way)
+    sediment_geoid_time_grid=0
+
+    ocean_geoid_time_grid=LOAD_TIME_GRID(sdelL=ocean_time_grid.height_time_coeff*ocean_time_grid.rho,beta_l=beta_l,E=love_number.k_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='OCEAN_GEOID')
+    ocean_geoid_time_grid.calc_elastic_time()
+    ocean_geoid_time_grid.calc_viscuous_time(backend=backend)
+    ocean_geoid_time_grid.save(save_way=Output_way)
+    ocean_geoid_time_grid=0
+
+    total_geoid_time_grid=LOAD_TIME_GRID(sdelL=ice_time_grid.height_time_coeff*ice_time_grid.rho+sed_time_grid.height_time_coeff*sed_time_grid.rho+ocean_time_grid.height_time_coeff*ocean_time_grid.rho,beta_l=beta_l,E=love_number.k_e,a=a,Me=Me,time_step=ice_time_grid.time_step,maxdeg=ice_time_grid.maxdeg,grid_name='TOTAL_GEOID')
+    total_geoid_time_grid.calc_elastic_time()
+    total_geoid_time_grid.calc_viscuous_time(backend=backend)
+    total_geoid_time_grid.save(save_way=Output_way)
+    total_geoid_time_grid=0
+
+
+
+def calculate_sediment_ocean_interaction(love_number,ice_time_grid,sed_time_grid,ocean_time_grid,a,Me,topo_time_grid,Output_way,backend=False,plot=dict(plot=False)) :
+
+    '''
+    The _`calculate_sediment_ocean_interaction` method calculate the earth viscoelastic response resulting from sediment under sea surface. This is used to retrieve the effect of ocean replacement by sediment on the sediment load. The resulting subsidence is the true subsidence induced by sediment. The problems and resolution in equation is described in :ref:`True sediment subsidence <sed_subs>`.
+
+    Attribute :
+    ----------- 
+        love_number : :ref:`LOVE <LOVE>` 
+            The loaded love number in the form of a LOVE class object
+        ice_time_grid : :ref:`grid.ICE_TIME_GRID <ICE_TIME_GRID>`
+            ice thickness in the form of ICE_TIME_GRID class object
+        sed_time_grid : :ref:`grid.SEDIMENT_TIME_GRID <SEDIMENT_TIME_GRID>` 
+            sediment thickness in the form of SED_TIME_GRID class object
+        ocean_time_grid : :ref:`grid.OCEAN_TIME_GRID <OCEAN_TIME_GRID>` 
+            ocean thickness calculated using the SLE solver in the form of OCEAN_TIME_GRID class object
+        a : float
+            radius of earth in meter
+        Me : float
+            mass of earth (kg)
+        Output_way : str
+            way of the output where the load is calculated
+        backend : bool
+            set if the function is writing its state of computation
+
+    Returns : 
+    --------- 
+        None 
+
+    The resulting LOAD and GEOID are stored in a LOAD file in the same file then the input files. The structure is based on the :ref:`LOAD_TIME_GRID <LOAD_TIME_GRID>` class object.
+    '''
+
+    beta_l=love_number.beta_R_l # Load the earth love numbers
+    #Preparing a new grid that compute the load of the substracted sediment volume to the ocean.
+    #We create a new object to compute the oceanic sediment
+    oceanic_sediment_time_grid=copy.copy(sed_time_grid)
+    oceanic_sediment_time_grid.rho=ocean_time_grid.rho
+    
+
+    for t_it in range (oceanic_sediment_time_grid.time_step_number-1): # At each time step we apply the ocean function to the sediment height grid
+        oceanic_sediment_time_grid.height_time_grid[t_it,:,:]=oceanic_sediment_time_grid.height_time_grid[t_it,:,:]*ocean_time_grid.evaluate_ocean(topo_time_grid.height_time_grid[t_it,:,:]).grd
+    oceanic_sediment_time_grid.timegrdtotimecoeff()
+
+
+    oceanic_sediment_load_time_grid=LOAD_TIME_GRID(sdelL=oceanic_sediment_time_grid.height_time_coeff*oceanic_sediment_time_grid.rho,beta_l=beta_l,E=love_number.h_e,a=a,Me=Me,time_step=oceanic_sediment_time_grid.time_step,maxdeg=oceanic_sediment_time_grid.maxdeg,grid_name='OCEANIC_SEDIMENT_LOAD')    
+    #computing the earth deformation
+    oceanic_sediment_load_time_grid.calc_elastic_time()
+    oceanic_sediment_load_time_grid.calc_viscuous_time(backend=backend)
+    oceanic_sediment_load_time_grid.save(save_way=Output_way)
+    oceanic_sediment_load_time_grid.clean_memory()
+
+    beta_l=love_number.beta_G_l # Load the ocean love numbers
+
+    #computing the geoid deformation
+    oceanic_sediment_geoid_time_grid=LOAD_TIME_GRID(sdelL=oceanic_sediment_time_grid.height_time_coeff*oceanic_sediment_time_grid.rho,beta_l=beta_l,E=love_number.h_e,a=a,Me=Me,time_step=oceanic_sediment_time_grid.time_step,maxdeg=oceanic_sediment_time_grid.maxdeg,grid_name='OCEANIC_SEDIMENT_GEOID')
+    oceanic_sediment_geoid_time_grid.calc_elastic_time()
+    oceanic_sediment_geoid_time_grid.calc_viscuous_time(backend=backend)
+    oceanic_sediment_geoid_time_grid.save(save_way=Output_way)
+    oceanic_sediment_geoid_time_grid.clean_memory()
+
+
+
+def Post_process(Input_way,sed_name,ice_name,ocean_name,topo_name,love_way):
+    '''
+    The _`Post_process` calculate the earth viscoelastic response resulting from the different masses caculated with the SLE_solver. This computation is made for all models available in the files. 
+
+    Attribute :
+    ----------- 
+        input_way_sed : str
+            way where the sediment precomputed are stored
+        input_way_model_output : str
+            filepath to the different masses calculated by the SLE solver
+        love_way : str
+            way to the love number output
+
+    Returns : 
+    --------- 
+        None 
+
+    The resulting LOAD and GEOID are stored in a LOAD file in the same file then the input files. The structure is based on the :ref:`LOAD_TIME_GRID <LOAD_TIME_GRID>` class object.
+    '''
+    
+
+
+    earth_model_name_list=os.listdir(Input_way)
+
+    for earth_model_name in earth_model_name_list :
+
+        print('calculation for : ' + earth_model_name)
+
+        Output_way=Input_way+'/'+earth_model_name+'/LOAD/'
+
+        if not(os.path.exists(Output_way)):
+            os.mkdir(Output_way)
+
+        sed_time_grid=SEDIMENT_TIME_GRID(from_file=(True,Input_way+'/'+earth_model_name+'/'+sed_name))
+        sed_time_grid.timegrdtotimecoeff()
+
+        ocean_time_grid=OCEAN_TIME_GRID(from_file=(True,Input_way+'/'+earth_model_name+'/'+ocean_name))
+        #print(ocean_time_grid.height_time_coeff.shape)
+        ice_time_grid=ICE_TIME_GRID(from_file=(True,Input_way+'/'+earth_model_name+'/'+ice_name))
+        #print(ice_time_grid.time_step_number)
+
+        np.set_printoptions(threshold=sys.maxsize)
+        a=6371000
+        Me=5.9742e24
+        love_way_found=find_files(earth_model_name,love_way)[0]
+        love_number=LOVE(ice_time_grid.maxdeg,love_way_found,ice_time_grid.time_step,a,Me)
+
+        ice_time_grid.timegrdtotimecoeff()
+
+        calculate_deformation(love_number,ice_time_grid,sed_time_grid,ocean_time_grid,a,Me,Output_way)
+
+        #Loading the topography to compute the ocean function at each time step
+        topo_time_grid=TOPOGRAPHIC_TIME_GRID(from_file=(True,Input_way+'/'+earth_model_name+'/'+topo_name))
+
+        print('Oceanic sediment calculation')
+        calculate_sediment_ocean_interaction(love_number,ice_time_grid,sed_time_grid,ocean_time_grid,a,Me,topo_time_grid,Output_way)
+
+def plot_model_RSL(plot,Input_way,Output_way):
+    load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}/LOAD/TOTAL_LOAD'))
+    geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}/LOAD/TOTAL_GEOID'))
+    dESL=calculate_dESL(Input_way)
+    load_time_grid.height_time_coeff=(geoid_time_grid.viscuous_deformation+geoid_time_grid.elastic_deformation-load_time_grid.viscuous_deformation-load_time_grid.elastic_deformation)*dESL[2:,np.newaxis].repeat(load_time_grid.viscuous_deformation.shape[1],axis=1)
+    time_grid=load_time_grid
+    if plot['plot']:
+        if len(plot['frames'])>0 :
+            fig,ax=plt.subplots(len(plot['frames'])*len(plot['times']),1,figsize=(29.7,10*len(plot['frames'])*len(plot['times'])),subplot_kw={'projection': ccrs.PlateCarree(), "aspect": 1})
+            k=0
+            for i_time in range(len(plot['times'])):
+                for i_frame in range(len(plot['frames'])):
+                    axes=ax[k]
+                    time=plot['times'][i_time]
+                    central_longitude=0
+                    #ax_total  = plt.subplot(subplot_size+i_time*3+1, projection=ccrs.PlateCarree(central_longitude=central_longitude))
+                    ax_total=plot_load_frame(axes,time_grid,plot['frames'][i_frame],time,plot['frames_resolution'][i_frame],name=f'RSL',vmin=plot['frames_min_max'][i_frame][0],vmax=plot['frames_min_max'][i_frame][1])
+                    k+=1
+        plt.close(fig)
+        fig.savefig(f'{Output_way}/RSL.pdf')
+
+def plot_model_result_map(Input_way,plot):
+    '''
+    The _`plot_model_result_map` function run the plot functions for all type of load. This function use the `plot_frame`_ function, see this function for more details. 
+
+    Attribute :
+    ----------- 
+        input_way_sed : str
+            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
+        plot : dict(plot=True,times=[n_t],frames=[n_f*(lon1,lon1,lat1,lat2)],frames_resolution=[n_f],frames_min_max=np.array([[[min_load],max_load,min_geoid,max_geoid]]),contours_v=[n_f*2*[contours...]],transects=[n_t*(lat1,lon1,lat2,lon2)],point_density=[n_t], transect_min_max=[n_t(min_load,max_load,min_geoid,max_geoid)], points=np.array([n_p[lat,lon]]))
+            The plot dictionnary used to define all the plot parameters of the output. In this dictionary, there is three main group of parameters, the frame plot parameters, the transect plot parameters and the points plot parameters. The frame plot parameters contain the frame locations in frames, the frames resolution in frames_resolution, the frames min and max value to plot in frames_min_max and the contours value to plot in contours_v. The transect plot parameters contains the location of the begining and end of the transects in transects, the point density along the transect in point_density and the min max value of the transect in transect_min_max. The points plot parameters contains the locations of the differents plots in points. 
+
+    Returns : 
+    --------- 
+        None 
+
+    '''
+    Input_way=Input_way+'/LOAD'
+    plot_frame(Input_way,plot,Input_way,'ICE')
+    plot_frame(Input_way,plot,Input_way,'SEDIMENT')
+    plot_frame(Input_way,plot,Input_way,'OCEAN')
+    plot_frame(Input_way,plot,Input_way,'NO_SEDIMENT')
+    plot_frame(Input_way,plot,Input_way,'TOTAL')
+
+def calc_transect(Input_way,time,transect,point_density,type,type_bis):
+    '''
+    The _`calc_transect` function evaluate the spherical harmonics coefficient function run the plot functions for all type of load. This function use the `plot_frame`_ function, see this function for more details. 
+
+    Attribute :
+    ----------- 
+        input_way_sed : str
+            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
+        time : float
+            The selected time to plot the transect.
+        transect : (lat1,lon1,lat2,lon2)
+            The coordinate of the beginning and the end of the transect.
+        point_dentity : int
+            Number of points along the transect, this will define the resolution
+        type : str
+            This define the type of load considered. Must be "SEDIMENT", "NO_SEDIMENT", "OCEAN", "ICE" or "TOTAL".
+        type_bis : str
+            This define if the plot concern the geoid of the ground deformation. Must be "LOAD" or "GEOID".
+
+    Returns : 
+    --------- 
+        None 
+        
+    '''
+    
+    if type is 'OCEAN' :
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_{type_bis}'))
+        t_it=np.where(load_time_grid.time_step==time)[0][0]
+        load_time_grid.coeff=load_time_grid.viscuous_deformation[t_it-2,:]-load_time_grid.viscuous_deformation[t_it-3,:]+load_time_grid.elastic_deformation[t_it-2,:]-load_time_grid.elastic_deformation[t_it-3,:]
+        load_time_grid.coeff=load_time_grid.coeff/(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
+        tr_ocean=load_time_grid.along_transect(coord=transect,point_density=point_density)
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_{type_bis}'))
+        load_time_grid.coeff=load_time_grid.viscuous_deformation[t_it-2,:]-load_time_grid.viscuous_deformation[t_it-3,:]+load_time_grid.elastic_deformation[t_it-2,:]-load_time_grid.elastic_deformation[t_it-3,:]
+        load_time_grid.coeff=load_time_grid.coeff/(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
+        tr_oceanic_sediment=load_time_grid.along_transect(coord=transect,point_density=point_density)
+        tr=tr_ocean+tr_oceanic_sediment
+    elif type is 'SEDIMENT' :
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_{type_bis}'))
+        t_it=np.where(load_time_grid.time_step==time)[0][0]
+        load_time_grid.coeff=load_time_grid.viscuous_deformation[t_it-2,:]-load_time_grid.viscuous_deformation[t_it-3,:]+load_time_grid.elastic_deformation[t_it-2,:]-load_time_grid.elastic_deformation[t_it-3,:]
+        load_time_grid.coeff=load_time_grid.coeff/(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
+        tr_sediment=load_time_grid.along_transect(coord=transect,point_density=point_density)
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_{type_bis}'))
+        load_time_grid.coeff=load_time_grid.viscuous_deformation[t_it-2,:]-load_time_grid.viscuous_deformation[t_it-3,:]+load_time_grid.elastic_deformation[t_it-2,:]-load_time_grid.elastic_deformation[t_it-3,:]
+        load_time_grid.coeff=load_time_grid.coeff/(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
+        tr_oceanic_sediment=load_time_grid.along_transect(coord=transect,point_density=point_density)
+        tr=tr_sediment-tr_oceanic_sediment
+    elif type is 'NO_SEDIMENT' :
+        ice_load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\ICE_{type_bis}'))
+        ocean_load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEAN_{type_bis}'))
+        t_it=np.where(ice_load_time_grid.time_step==time)[0][0]
+
+        ice_load_time_grid.coeff=ice_load_time_grid.viscuous_deformation[t_it-2,:]-ice_load_time_grid.viscuous_deformation[t_it-3,:]+ice_load_time_grid.elastic_deformation[t_it-2,:]-ice_load_time_grid.elastic_deformation[t_it-3,:]
+        ice_load_time_grid.coeff=ice_load_time_grid.coeff/(ice_load_time_grid.time_step[t_it-1]-ice_load_time_grid.time_step[t_it])
+
+        ocean_load_time_grid.coeff=ocean_load_time_grid.viscuous_deformation[t_it-2,:]-ocean_load_time_grid.viscuous_deformation[t_it-3,:]+ocean_load_time_grid.elastic_deformation[t_it-2,:]-ocean_load_time_grid.elastic_deformation[t_it-3,:]
+        ocean_load_time_grid.coeff=ocean_load_time_grid.coeff/(ocean_load_time_grid.time_step[t_it-1]-ocean_load_time_grid.time_step[t_it])
+
+        tr_ice=ice_load_time_grid.along_transect(coord=transect,point_density=point_density)
+        tr_ocean=ocean_load_time_grid.along_transect(coord=transect,point_density=point_density)
+
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_{type_bis}'))
+        load_time_grid.coeff=load_time_grid.viscuous_deformation[t_it-2,:]-load_time_grid.viscuous_deformation[t_it-3,:]+load_time_grid.elastic_deformation[t_it-2,:]-load_time_grid.elastic_deformation[t_it-3,:]
+        load_time_grid.coeff=load_time_grid.coeff/(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
+        tr_oceanic_sediment=load_time_grid.along_transect(coord=transect,point_density=point_density)
+        tr=tr_ice+tr_ocean+tr_oceanic_sediment
+    else :
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_{type_bis}'))
+        t_it=np.where(load_time_grid.time_step==time)[0][0]
+        load_time_grid.coeff=load_time_grid.viscuous_deformation[t_it-2,:]-load_time_grid.viscuous_deformation[t_it-3,:]+load_time_grid.elastic_deformation[t_it-2,:]-load_time_grid.elastic_deformation[t_it-3,:]
+        load_time_grid.coeff=load_time_grid.coeff/(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
+        tr=load_time_grid.along_transect(coord=transect,point_density=point_density)
+    dt=(load_time_grid.time_step[t_it-1]-load_time_grid.time_step[t_it])
+    return tr,dt
+
+
+def plot_model_result_cross_section(Input_way,plot):
+    '''
+    The _`plot_model_result_cross_section` function evaluate the spherical harmonics coefficient function and plot the results along a defined transect in plot.
+
+    Attribute :
+    ----------- 
+        Input_way_sed : str
+            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
+        plot : dict(plot=True,times=[n_t],frames=[n_f*(lon1,lon1,lat1,lat2)],frames_resolution=[n_f],frames_min_max=np.array([[[min_load],max_load,min_geoid,max_geoid]]),contours_v=[n_f*2*[contours...]],transects=[n_t*(lat1,lon1,lat2,lon2)],point_density=[n_t], transect_min_max=[n_t(min_load,max_load,min_geoid,max_geoid)], points=np.array([n_p[lat,lon]]))
+            The plot dictionnary used to define all the plot parameters of the output. In this dictionary, there is three main group of parameters, the frame plot parameters, the transect plot parameters and the points plot parameters. The frame plot parameters contain the frame locations in frames, the frames resolution in frames_resolution, the frames min and max value to plot in frames_min_max and the contours value to plot in contours_v. The transect plot parameters contains the location of the begining and end of the transects in transects, the point density along the transect in point_density and the min max value of the transect in transect_min_max. The points plot parameters contains the locations of the differents plots in points. 
+
+    Returns : 
+    --------- 
+        None 
+        
+    '''
+    Input_way=Input_way+'/LOAD'
+    sediment_color=(0.4,0.7,0.5)
+    sediment_color_dark=(0.2,0.4,0.25)
+    ice_color=(0.1,0.8,0.8)
+    ocean_color=(0.2,0.2,0.6)
+    glaciohydrostatic_color=(0.1,0.1,0.4)
+    if len(plot['transects'])>0 :
+        fig,ax=plt.subplots(len(plot['transects'])*len(plot['times']),2,figsize=(29.7,5*len(plot['transects'])*len(plot['times'])))
+        fig_loc,ax_map=plt.subplots(1,1,subplot_kw={'projection': ccrs.PlateCarree(), "aspect": 1})
+        alpha_ocean=0
+        coast_line_width=0.2
+        ax_map.set_global()
+        cartopy.mpl.geoaxes.GeoAxes.gridlines(ax_map,crs=ccrs.PlateCarree(),draw_labels=True)
+        ax_map.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
+        ax_map.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
+        for i_transect in range(len(plot['transects'])):
+            ax_map.plot((plot['transects'][i_transect][1],plot['transects'][i_transect][3]),(plot['transects'][i_transect][0],plot['transects'][i_transect][2]),color='r',linewidth=0.5)
+            ax_map.annotate(f'{i_transect})', # this is the text
+                 (plot['transects'][i_transect][1],plot['transects'][i_transect][0]), # these are the coordinates to position the label
+                 textcoords="offset points", # how to position the text
+                 xytext=(0,1), # distance from text to points (x,y)
+                 ha='center',
+                 fontsize=3)
+        plt.close(fig_loc)
+        fig_loc.savefig(f'{Input_way}/transect_localisation.pdf')
+        k=0
+        for i_time in range(len(plot['times'])):
+            for i_transect in range(len(plot['transects'])):
+                coord=plot['transects'][i_transect]
+                theta=np.linspace(coord[0],coord[2],plot['point_density'][i_transect])/180*2*np.pi
+                phi=np.linspace(coord[1],coord[3],plot['point_density'][i_transect])/180*2*np.pi
+                phiA=np.append(phi,0)
+                phiB=np.append(0,phi)
+                D= np.append(0,6371*np.arccos(np.sin(phiA)*np.sin(phiB)+np.cos(phiA)*np.cos(phiB)*np.cos(np.append(0,np.append(np.diff(theta),0))))[1:-1].cumsum())/2
+                axes=ax[k,:]
+                type_bis='LOAD'
+                tr_ice_load,dt=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'ICE',type_bis)
+                tr_sed_load,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'SEDIMENT',type_bis)
+                tr_oc_load,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'OCEAN',type_bis)
+                tr_nosed_load,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'NO_SEDIMENT',type_bis)
+                tr_tot_load,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'TOTAL',type_bis)
+                axes[0].plot(D,tr_ice_load,label='ice_load',color=ice_color)
+                axes[0].plot(D,tr_sed_load,label='sediment_load',color=sediment_color)
+                axes[0].plot(D,tr_oc_load,label='ocean_load',color=ocean_color)
+                axes[0].plot(D,tr_nosed_load,label='glaciohydrostatic_load',color=glaciohydrostatic_color)
+                axes[0].plot(D,tr_tot_load,label='total load',color='k')
+                axes[0].set_ylim(plot['transect_min_max'][i_transect][0],plot['transect_min_max'][i_transect][1])
+                axes[0].set_xlabel(f'distance (km)')
+                axes[0].set_ylabel(f'Vertical Land motion averaged over {dt*1000} year (mm/yr)')
+                t=plot['times'][i_time]
+                axes[0].grid()
+                axes[0].set_title(f'VLM estimated at {t} kyr along transect {i_transect})')
+                axes[0].legend()
+                type_bis='GEOID'
+                tr_ice_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'ICE',type_bis)
+                tr_sed_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'SEDIMENT',type_bis)
+                tr_oc_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'OCEAN',type_bis)
+                tr_nosed_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'NO_SEDIMENT',type_bis)
+                tr_tot_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'TOTAL',type_bis)
+                axes[1].plot(D,tr_ice_geoid,label='ice_geoid',color=ice_color)
+                axes[1].plot(D,tr_sed_geoid,label='sediment_geoid',color=sediment_color)
+                axes[1].plot(D,tr_oc_geoid,label='ocean_geoid',color=ocean_color)
+                axes[1].plot(D,tr_nosed_geoid,label='glaciohydrostatic_geoid',color=glaciohydrostatic_color)
+                axes[1].plot(D,tr_tot_geoid,label='total geoid',color='k')
+                axes[1].set_xlabel(f'distance (km)')
+                axes[1].set_ylabel(f'Vertical Geoid motion averaged over {dt*1000} year (mm/yr)')
+                t=plot['times'][i_time]
+                axes[1].set_title(f'VGM estimated at {t} kyr along transect {i_transect})')
+                axes[1].grid()
+                axes[1].set_ylim(plot['transect_min_max'][i_transect][2],plot['transect_min_max'][i_transect][3])
+                axes[1].legend()
+                k+=1
+        plt.close(fig)
+        fig.savefig(f'{Input_way}/transect_deformation.pdf')
+
+    
+
+def calc_point(Input_way,points,type,type_bis):
+    '''
+    The _`calc_point` function evaluate the spherical harmonics coefficient for a type of model output at precise points locations.
+
+    Attribute :
+    ----------- 
+        Input_way : str
+            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
+        time : float
+            The selected time to plot the transect.
+        points : np.array(n_p*[lat,lon])
+            The locations of the different points you wan't to extract data.
+        type : str
+            This define the type of load considered. Must be "SEDIMENT", "NO_SEDIMENT", "OCEAN", "ICE" or "TOTAL".
+        type_bis : str
+            This define if the plot concern the geoid of the ground deformation. Must be "LOAD" or "GEOID".
+
+    Returns : 
+    --------- 
+        None 
+        
+    '''
+    
+    if type is 'OCEAN' :
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_{type_bis}'))
+        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
+        points_ocean=load_time_grid.point_time(points)
+
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_{type_bis}'))
+        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
+        points_oceanic_sediment=load_time_grid.point_time(points)
+
+        points=points_ocean+points_oceanic_sediment
+    elif type is 'SEDIMENT' :
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_{type_bis}'))
+        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
+        points_sediment=load_time_grid.point_time(points)
+
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_{type_bis}'))
+        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
+        points_oceanic_sediment=load_time_grid.point_time(points)
+
+        points=points_sediment-points_oceanic_sediment
+
+    elif type is 'NO_SEDIMENT' :
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEAN_{type_bis}'))
+        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
+        points_ocean=load_time_grid.point_time(points)
+
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\ICE_{type_bis}'))
+        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
+        points_ice=load_time_grid.point_time(points)
+
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_{type_bis}'))
+        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
+        points_oceanic_sediment=load_time_grid.point_time(points)
+
+        points=points_ocean+points_oceanic_sediment+points_ice
+    else :
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_{type_bis}'))
+        load_time_grid.height_time_coeff=load_time_grid.viscuous_deformation+load_time_grid.elastic_deformation
+        points=load_time_grid.point_time(points)
+
+    return points,load_time_grid.time_step
+
+def plot_model_output_points(Input_way,plot):
+    '''
+    The _`plot_model_output_points` function plot the output of the model at different points.
+    
+    Attribute :
+    ----------- 
+        Input_way : str
+            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
+        plot : dict(plot=True,times=[n_t],frames=[n_f*(lon1,lon1,lat1,lat2)],frames_resolution=[n_f],frames_min_max=np.array([[[min_load],max_load,min_geoid,max_geoid]]),contours_v=[n_f*2*[contours...]],transects=[n_t*(lat1,lon1,lat2,lon2)],point_density=[n_t], transect_min_max=[n_t(min_load,max_load,min_geoid,max_geoid)], points=np.array([n_p[lat,lon]]))
+            The plot dictionnary used to define all the plot parameters of the output. In this dictionary, there is three main group of parameters, the frame plot parameters, the transect plot parameters and the points plot parameters. The frame plot parameters contain the frame locations in frames, the frames resolution in frames_resolution, the frames min and max value to plot in frames_min_max and the contours value to plot in contours_v. The transect plot parameters contains the location of the begining and end of the transects in transects, the point density along the transect in point_density and the min max value of the transect in transect_min_max. The points plot parameters contains the locations of the differents plots in points. 
+        
+
+    Returns : 
+    --------- 
+        None 
+        
+    '''
+    sediment_color=(0.4,0.7,0.5)
+    sediment_color_dark=(0.2,0.4,0.25)
+    ice_color=(0.1,0.8,0.8)
+    ocean_color=(0.2,0.2,0.6)
+    glaciohydrostatic_color=(0.7,0.2,0.2)
+    if len(plot['transects'])>0 :
+        fig,axes=plt.subplots(len(plot['points']),3,figsize=(29.7,4*len(plot['points'])))
+        fig_loc,ax_map=plt.subplots(1,1,subplot_kw={'projection': ccrs.PlateCarree(), "aspect": 1})
+        alpha_ocean=0
+        coast_line_width=0.2
+        ax_map.set_global()
+        cartopy.mpl.geoaxes.GeoAxes.gridlines(ax_map,crs=ccrs.PlateCarree(),draw_labels=True)
+        ax_map.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
+        ax_map.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
+        for i_point in range(len(plot['points'])):
+            ax_map.scatter((plot['points'][i_point,1],plot['points'][i_point,1]),(plot['points'][i_point,0],plot['points'][i_point,0]),color='r',s=0.05)
+            ax_map.annotate(f'{i_point})', # this is the text
+                 (plot['points'][i_point,1],plot['points'][i_point,0]), # these are the coordinates to position the label
+                 textcoords="offset points", # how to position the text
+                 xytext=(0,0.2), # distance from text to points (x,y)
+                 ha='center',
+                 fontsize=1)
+        plt.close(fig_loc)
+        fig_loc.savefig(f'{Input_way}/LOAD/Points_localisation.pdf')
+        coord=plot['points']
+        type_bis='LOAD'
+        points_ice_load,time_step=calc_point(Input_way+'/LOAD',plot['points'],'ICE',type_bis)
+        points_sed_load,_=calc_point(Input_way+'/LOAD',plot['points'],'SEDIMENT',type_bis)
+        points_oc_load,_=calc_point(Input_way+'/LOAD',plot['points'],'OCEAN',type_bis)
+        points_nosed_load,_=calc_point(Input_way+'/LOAD',plot['points'],'NO_SEDIMENT',type_bis)
+        points_tot_load,_=calc_point(Input_way+'/LOAD',plot['points'],'TOTAL',type_bis)
+        for i_point in range(len(plot['points'])):
+            axes[i_point,0].plot(time_step,points_ice_load[i_point,:],label='ice_load',color=ice_color)
+            axes[i_point,0].plot(time_step,points_sed_load[i_point,:],label='sediment_load',color=sediment_color)
+            axes[i_point,0].plot(time_step,points_oc_load[i_point,:],label='ocean_load',color=ocean_color)
+            axes[i_point,0].plot(time_step,points_nosed_load[i_point,:],label='glaciohydrostatic_load',color=glaciohydrostatic_color)
+            axes[i_point,0].plot(time_step,points_tot_load[i_point,:],label='total load',color='k')
+            #axes[i_point,0].set_ylim(plot['transect_min_max'][i_transect][0],plot['transect_min_max'][i_transect][1])
+            axes[i_point,0].set_xlabel(f'time (kyr)')
+            axes[i_point,0].set_ylabel(f'Vertical Land motion (mm/yr)')
+            axes[i_point,0].grid()
+            axes[i_point,0].set_title(f'VLM at point {i_point})')
+            axes[i_point,0].legend()
+        type_bis='GEOID'
+        points_ice_geoid,time_step=calc_point(Input_way+'/LOAD',plot['points'],'ICE',type_bis)
+        points_sed_geoid,_=calc_point(Input_way+'/LOAD',plot['points'],'SEDIMENT',type_bis)
+        points_oc_geoid,_=calc_point(Input_way+'/LOAD',plot['points'],'OCEAN',type_bis)
+        points_nosed_geoid,_=calc_point(Input_way+'/LOAD',plot['points'],'NO_SEDIMENT',type_bis)
+        points_tot_geoid,_=calc_point(Input_way+'/LOAD',plot['points'],'TOTAL',type_bis)
+        for i_point in range(len(plot['points'])):
+            axes[i_point,1].plot(time_step,points_ice_geoid[i_point,:],label='ice_geoid',color=ice_color)
+            axes[i_point,1].plot(time_step,points_sed_geoid[i_point,:],label='sediment_geoid',color=sediment_color)
+            axes[i_point,1].plot(time_step,points_oc_geoid[i_point,:],label='ocean_geoid',color=ocean_color)
+            axes[i_point,1].plot(time_step,points_nosed_geoid[i_point,:],label='glaciohydrostatic_geoid',color=glaciohydrostatic_color)
+            axes[i_point,1].plot(time_step,points_tot_geoid[i_point,:],label='total_geoid',color='k')
+            #axes[i_point,0].set_ylim(plot['transect_min_max'][i_transect][0],plot['transect_min_max'][i_transect][1])
+            axes[i_point,1].set_xlabel(f'time (kyr)')
+            axes[i_point,1].set_ylabel(f'Vertical Geoid motion (mm/yr)')
+            axes[i_point,1].grid()
+            axes[i_point,1].set_title(f'VGM at point {i_point})')
+            axes[i_point,1].legend()
+        dESL=calculate_dESL(Input_way)
+        for i_point in range(len(plot['points'])):
+            axes[i_point,2].plot(time_step,dESL[:].cumsum()-dESL[:].cumsum()[-1],label='ESL',linestyle='dashed',color='k')
+            axes[i_point,2].plot(time_step,(dESL[:]+points_tot_geoid[i_point,:]-points_tot_load[i_point,:]).cumsum()-(dESL[:]+points_tot_geoid[i_point,:]-points_tot_load[i_point,:]).cumsum()[-1],label='RSL',color='k')
+            axes[i_point,2].legend()
+            axes[i_point,2].grid()
+            axes[i_point,2].set_xlabel(f'time (kyr)')
+            axes[i_point,2].set_ylabel(f'Depth below present sea level (mbpsl)')
+            axes[i_point,2].set_title(f'RSL and ESL at point {i_point})')
+
+        # type_bis='GEOID'
+        # tr_ice_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'ICE',type_bis)
+        # tr_sed_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'SEDIMENT',type_bis)
+        # tr_oc_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'OCEAN',type_bis)
+        # tr_tot_geoid,_=calc_transect(Input_way,plot['times'][i_time],plot['transects'][i_transect],plot['point_density'][i_transect],'TOTAL',type_bis)
+        # axes[1].plot(D,tr_ice_geoid,label='ice_load',color=ice_color)
+        # axes[1].plot(D,tr_sed_geoid,label='sediment_load',color=sediment_color)
+        # axes[1].plot(D,tr_oc_geoid,label='ocean_load',color=ocean_color)
+        # axes[1].plot(D,tr_tot_geoid,label='total load',color='k')
+        # axes[1].set_xlabel(f'distance (km)')
+        # axes[1].set_ylabel(f'Vertical Geoid motion averaged over {dt*1000} year (mm/yr)')
+        # t=plot['times'][i_time]
+        # axes[1].set_title(f'VGM estimated at {t} kyr along transect {i_transect})')
+        # axes[1].grid()
+        # axes[1].set_ylim(plot['transect_min_max'][i_transect][2],plot['transect_min_max'][i_transect][3])
+        # axes[1].legend()
+        plt.close(fig)
+        fig.savefig(f'{Input_way}/LOAD/Points_deformation.pdf')
+
+def plot_frame(Input_way,plot,Output_way,type):
+    '''
+    The _`plot_frame` function define the spherical harmonic coefficient to be expanded into a grid and plot in the frame defined in plot. This function make the difference between sediment subsidence and true sediment subsidence where water replaced by sediment is included. 
+    
+    Attribute :
+    ----------- 
+        Input_way : str
+            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
+        plot : dict(plot=True,times=[n_t],frames=[n_f*(lon1,lon1,lat1,lat2)],frames_resolution=[n_f],frames_min_max=np.array([[[min_load],max_load,min_geoid,max_geoid]]),contours_v=[n_f*2*[contours...]],transects=[n_t*(lat1,lon1,lat2,lon2)],point_density=[n_t], transect_min_max=[n_t(min_load,max_load,min_geoid,max_geoid)], points=np.array([n_p[lat,lon]]))
+            The plot dictionnary used to define all the plot parameters of the output. In this dictionary, there is three main group of parameters, the frame plot parameters, the transect plot parameters and the points plot parameters. The frame plot parameters contain the frame locations in frames, the frames resolution in frames_resolution, the frames min and max value to plot in frames_min_max and the contours value to plot in contours_v. The transect plot parameters contains the location of the begining and end of the transects in transects, the point density along the transect in point_density and the min max value of the transect in transect_min_max. The points plot parameters contains the locations of the differents plots in points. 
+        Output_way : str
+            way where the plot will be saved.
+        type : str
+            This define the type of load considered. Must be "SEDIMENT", "NO_SEDIMENT", "OCEAN", "ICE" or "TOTAL".
+
+        
+
+    Returns : 
+    --------- 
+        None 
+        
+    '''
+    if type is "SEDIMENT" :
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_LOAD'))
+        sediment_load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_LOAD'))
+        load_time_grid.viscuous_deformation=sediment_load_time_grid.viscuous_deformation-load_time_grid.viscuous_deformation
+        load_time_grid.elastic_deformation=sediment_load_time_grid.elastic_deformation-load_time_grid.elastic_deformation
+        geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_GEOID'))
+        sediment_geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_GEOID'))
+        geoid_time_grid.viscuous_deformation=sediment_geoid_time_grid.viscuous_deformation-geoid_time_grid.viscuous_deformation
+        geoid_time_grid.elastic_deformation=sediment_geoid_time_grid.elastic_deformation-geoid_time_grid.elastic_deformation
+    if type is "OCEAN" :
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_LOAD'))
+        sediment_load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_LOAD'))
+        load_time_grid.viscuous_deformation=sediment_load_time_grid.viscuous_deformation+load_time_grid.viscuous_deformation
+        load_time_grid.elastic_deformation=sediment_load_time_grid.elastic_deformation+load_time_grid.elastic_deformation
+        geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_GEOID'))
+        sediment_geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_GEOID'))
+        geoid_time_grid.viscuous_deformation=sediment_geoid_time_grid.viscuous_deformation+geoid_time_grid.viscuous_deformation
+        geoid_time_grid.elastic_deformation=sediment_geoid_time_grid.elastic_deformation+geoid_time_grid.elastic_deformation
+    elif type is "NO_SEDIMENT":
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\TOTAL_LOAD'))
+        sediment_load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\SEDIMENT_LOAD'))
+        oceanic_sediment_load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_LOAD'))
+        load_time_grid.viscuous_deformation=-sediment_load_time_grid.viscuous_deformation+load_time_grid.viscuous_deformation+oceanic_sediment_load_time_grid.viscuous_deformation
+        load_time_grid.elastic_deformation=-sediment_load_time_grid.elastic_deformation+load_time_grid.elastic_deformation+oceanic_sediment_load_time_grid.elastic_deformation
+        
+        ocean_geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEAN_GEOID'))
+        geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\ICE_GEOID'))
+        oceanic_sediment_geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\OCEANIC_SEDIMENT_GEOID'))
+        geoid_time_grid.viscuous_deformation=ocean_geoid_time_grid.viscuous_deformation+geoid_time_grid.viscuous_deformation+oceanic_sediment_geoid_time_grid.viscuous_deformation
+        geoid_time_grid.elastic_deformation=ocean_geoid_time_grid.elastic_deformation+geoid_time_grid.elastic_deformation+oceanic_sediment_geoid_time_grid.elastic_deformation
+    else :
+        load_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_LOAD'))
+        geoid_time_grid=LOAD_TIME_GRID(from_file=(True,f'{Input_way}\{type}_GEOID'))
+    plot_model_output(load_time_grid,plot,Output_way,f'load_{type}',vmin=(plot['frames_min_max'][:,0]),vmax=plot['frames_min_max'][:,1],contours_v=plot['contours_v'][0])
+    plot_model_output(geoid_time_grid,plot,Output_way,f'geoid_{type}',vmin=(plot['frames_min_max'][:,2]),vmax=plot['frames_min_max'][:,3],contours_v=plot['contours_v'][1])
+
+def plot_model_output(time_grid,plot,Output_way,type=None,vmin=None,vmax=None,contours_v=None):
+    '''
+    The _`plot_model_output` function plot the frames for each frames and at each time steps. 
+    
+    Attribute :
+    ----------- 
+        time_grid : TIME_GRID from `ref`:{TIME_GRID <TIME_GRID>}
+        plot : dict(plot=True,times=[n_t],frames=[n_f*(lon1,lon1,lat1,lat2)],frames_resolution=[n_f],frames_min_max=np.array([[[min_load],max_load,min_geoid,max_geoid]]),contours_v=[n_f*2*[contours...]],transects=[n_t*(lat1,lon1,lat2,lon2)],point_density=[n_t], transect_min_max=[n_t(min_load,max_load,min_geoid,max_geoid)], points=np.array([n_p[lat,lon]]))
+            The plot dictionnary used to define all the plot parameters of the output. In this dictionary, there is three main group of parameters, the frame plot parameters, the transect plot parameters and the points plot parameters. The frame plot parameters contain the frame locations in frames, the frames resolution in frames_resolution, the frames min and max value to plot in frames_min_max and the contours value to plot in contours_v. The transect plot parameters contains the location of the begining and end of the transects in transects, the point density along the transect in point_density and the min max value of the transect in transect_min_max. The points plot parameters contains the locations of the differents plots in points. 
+        Output_way : str
+            way where the plot will be saved.
+        type : str
+            This define the type of load considered. Must be "SEDIMENT", "NO_SEDIMENT", "OCEAN", "ICE" or "TOTAL".
+        vmin : float 
+            The minimal value for the colormap of your plot
+        vmax : float
+            The maximal value for the colormap of your plot
+        contours_v : list
+            List of the contours values to be plot
+
+    Returns : 
+    --------- 
+        None 
+        
+    '''
+    if plot['plot']:
+        if len(plot['frames'])>0 :
+            fig,ax=plt.subplots(len(plot['frames'])*len(plot['times']),3,figsize=(29.7,10*len(plot['frames'])*len(plot['times'])),subplot_kw={'projection': ccrs.PlateCarree(), "aspect": 1})
+            k=0
+            for i_time in range(len(plot['times'])):
+                for i_frame in range(len(plot['frames'])):
+                    axes=ax[k,:]
+                    time=plot['times'][i_time]
+                    central_longitude=0
+                    #ax_total  = plt.subplot(subplot_size+i_time*3+1, projection=ccrs.PlateCarree(central_longitude=central_longitude))
+                    time_grid.height_time_coeff=time_grid.viscuous_deformation+time_grid.elastic_deformation
+                    ax_total=plot_load_frame(axes[0],time_grid,plot['frames'][i_frame],time,plot['frames_resolution'][i_frame],name=f'total {type}',vmin=vmin[i_frame],vmax=vmax[i_frame],contour=contours_v[i_frame])
+
+                    #ax_viscous  = plt.subplot(subplot_size+i_time*3+2, projection=ccrs.PlateCarree(central_longitude=central_longitude))
+                    time_grid.height_time_coeff=time_grid.viscuous_deformation
+                    ax_viscous=plot_load_frame(axes[1],time_grid,plot['frames'][i_frame],time,plot['frames_resolution'][i_frame],name=f'viscous {type}',vmin=vmin[i_frame],vmax=vmax[i_frame],contour=contours_v[i_frame])
+
+                    #ax_elastic = plt.subplot(subplot_size+i_time*3+3, projection=ccrs.PlateCarree(central_longitude=central_longitude))
+                    time_grid.height_time_coeff=time_grid.elastic_deformation
+                    ax_elastic=plot_load_frame(axes[2],time_grid,plot['frames'][i_frame],time,plot['frames_resolution'][i_frame],name=f'elastic {type}',vmin=vmin[i_frame],vmax=vmax[i_frame],contour=contours_v[i_frame]) 
+                    k+=1
+        plt.close(fig)
+        fig.savefig(f'{Output_way}/{type}_deformation.pdf')
+
+import cartopy
+import matplotlib.pyplot as plt
+import cartopy.crs as ccrs
+from matplotlib import cm
+import matplotlib.colors as colors
+
+def plot_precomputation(initial_time_step,initial_grid,precomputed_grid,selected_time=1,area=None,save_way='',lon_init=None,lat_init=None,topo=False,vmin=None,vmax=None,vcenter=0,cmap=cm.get_cmap('bwr', 255)):
+    '''
+    The _`plot_precomputation` function plot the output of the precomputation as the ice, sediment and totpography. These plot allow you to compare the entry and the output to be sure there is no errors.
+    
+    Attribute :
+    ----------- 
+        Input_way : str
+            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
+        plot : dict(plot=True,times=[n_t],frames=[n_f*(lon1,lon1,lat1,lat2)],frames_resolution=[n_f],frames_min_max=np.array([[[min_load],max_load,min_geoid,max_geoid]]),contours_v=[n_f*2*[contours...]],transects=[n_t*(lat1,lon1,lat2,lon2)],point_density=[n_t], transect_min_max=[n_t(min_load,max_load,min_geoid,max_geoid)], points=np.array([n_p[lat,lon]]))
+            The plot dictionnary used to define all the plot parameters of the output. In this dictionary, there is three main group of parameters, the frame plot parameters, the transect plot parameters and the points plot parameters. The frame plot parameters contain the frame locations in frames, the frames resolution in frames_resolution, the frames min and max value to plot in frames_min_max and the contours value to plot in contours_v. The transect plot parameters contains the location of the begining and end of the transects in transects, the point density along the transect in point_density and the min max value of the transect in transect_min_max. The points plot parameters contains the locations of the differents plots in points. 
+        Output_way : str
+            way where the plot will be saved.
+        type : str
+            This define the type of load considered. Must be "SEDIMENT", "NO_SEDIMENT", "OCEAN", "ICE" or "TOTAL".
+        vmin : float 
+            The minimal value for the colormap of your plot
+        vmax : float
+            The maximal value for the colormap of your plot
+
+    Returns : 
+    --------- 
+        None 
+        
+    '''
+    our_ind=np.where((precomputed_grid.time_step-selected_time)==0)[0][0]
+    in_ind=np.where((initial_time_step-selected_time)==0)[0][0]
+    alpha_ocean=0
+    coast_line_width=0.5
+    norm1 = colors.TwoSlopeNorm(vmin=-0.1,vmax=None,vcenter=0)
+    fig = plt.figure(figsize=(12, 6), facecolor="none")
+
+    # plot the initial data
+
+    norm = colors.TwoSlopeNorm(vmin=vmin,vmax=vmax,vcenter=vcenter)
+
+    if area is None :
+        ax_init  = plt.subplot(121, projection=ccrs.Mollweide())
+        ax_init.set_global()
+    else :
+        ax_init  = plt.subplot(121, projection=ccrs.PlateCarree())
+        ax_init.set_extent(area)
+
+    if not(lon_init is None) :
+        m_init = ax_init.scatter(lon_init,lat_init,c=initial_grid[:in_ind+1,:].sum(0),transform=ccrs.PlateCarree(),zorder=0,norm=norm,cmap=cmap)
+        cbar_init=plt.colorbar(mappable=m_init, orientation="horizontal")
+        cbar_init.set_label(precomputed_grid.time_grid_name + '(m)')
+        #cbar_init.set_ticks([0, initial_grid[:in_ind+1].sum(0).max()])
+        ax_init.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
+        ax_init.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
+        cartopy.mpl.geoaxes.GeoAxes.gridlines(ax_init,crs=ccrs.PlateCarree(),draw_labels=True)
+    else : 
+        if topo : 
+            m_init = ax_init.imshow(initial_grid, origin='lower', transform=ccrs.PlateCarree(),extent=[0,360, -89, 89], zorder=0, cmap=cmap, interpolation="gaussian",norm=norm)
+            cbar_init=plt.colorbar(mappable=m_init, orientation="horizontal")
+            cbar_init.set_label(precomputed_grid.time_grid_name + '(m)')
+            #cbar_init.set_ticks([0, initial_grid[:in_ind+1].sum(0).max()])
+            ax_init.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
+            ax_init.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
+        else : 
+            m_init = ax_init.imshow(initial_grid[:in_ind+1].sum(0), origin='lower', transform=ccrs.PlateCarree(),extent=[0,360, -89, 89], zorder=0, cmap=cmap, interpolation="gaussian",norm=norm)
+            cbar_init=plt.colorbar(mappable=m_init, orientation="horizontal")
+            cbar_init.set_label(precomputed_grid.time_grid_name + '(m)')
+            #cbar_init.set_ticks([0, initial_grid[:in_ind+1].sum(0).max()])
+            ax_init.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
+            ax_init.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
+        cartopy.mpl.geoaxes.GeoAxes.gridlines(ax_init,crs=ccrs.PlateCarree(),draw_labels=True)
+
+    if area is None :
+        ax_precomp  = plt.subplot(122, projection=ccrs.Mollweide())
+        ax_precomp.set_global()
+    else :
+        ax_precomp  = plt.subplot(122, projection=ccrs.PlateCarree())
+        ax_precomp.set_extent(area)
+
+    colormap = cmap
+    if topo :
+        m2 = ax_precomp.imshow(precomputed_grid.height_time_grid[-1,:,:], origin='lower', transform=ccrs.PlateCarree(),extent=[0,360, -89, 89], zorder=0, cmap=colormap, interpolation="gaussian",norm=norm)
+        cbar2=plt.colorbar(mappable=m2, orientation="horizontal")
+        cbar2.set_label(precomputed_grid.time_grid_name + ' interpolated (m)')
+        #cbar2.set_ticks([0, precomputed_grid.height_time_grid[:our_ind+1,:,:].sum(0).max()])
+        ax_precomp.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
+        ax_precomp.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
+
+    else : 
+        m2 = ax_precomp.imshow(precomputed_grid.height_time_grid[:our_ind+1,:,:].sum(0), origin='lower', transform=ccrs.PlateCarree(),extent=[0,360, -89, 89], zorder=0, cmap=colormap, interpolation="gaussian",norm=norm)
+        cbar2=plt.colorbar(mappable=m2, orientation="horizontal")
+        cbar2.set_label(precomputed_grid.time_grid_name + ' interpolated (m)')
+        #cbar2.set_ticks([0, precomputed_grid.height_time_grid[:our_ind+1,:,:].sum(0).max()])
+        ax_precomp.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
+        ax_precomp.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
+    cartopy.mpl.geoaxes.GeoAxes.gridlines(ax_precomp,crs=ccrs.PlateCarree(),draw_labels=True)
+
+    plt.close(fig)
+
+    fig.savefig(save_way+'/'+precomputed_grid.time_grid_name+'.pdf')
+
+def calculate_dESL(Input_way):
+    '''
+    The _`calculate_dESL` function compute the ESL variation over time including a varaible ocean surface.
+    
+    Attribute :
+    ----------- 
+        Input_way : str
+            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
+
+    Returns : 
+    --------- 
+        dESL : np.array([time_step_number,])
+            The variation of the ESL at each time step.
+        
+    '''
+    ocean_grid=OCEAN_TIME_GRID(from_file=(True,Input_way+"/OCE"))
+
+    ice=ICE_TIME_GRID(from_file=(True,Input_way+"/ICE_ICE6G"))
+
+    topo=TOPOGRAPHIC_TIME_GRID(from_file=(True,Input_way+"/topo_SL"))
+    dESL=np.zeros(ice.time_step_number)
+    for t_it in range(ice.time_step_number-1):
+        ocean_grid.evaluate_ocean(topo.height_time_grid[t_it,:,:]).grdtocoeff()
+        dESL[t_it]=np.real(1/ocean_grid.coeff[0] * (- ice.rho/ocean_grid.rho*ice.height_time_coeff[t_it,0]))
+    return dESL
+
+import cartopy
+import cartopy.crs as ccrs
+import matplotlib
+from matplotlib import cm
+import matplotlib as mpl
+import matplotlib.colors as colors
+import numpy as np
+import matplotlib.pyplot as plt
+
+def plot_load_frame(ax,data,frame,time,resolution,name,add_contour=None,vmin=None,vmax=None,vcenter=0,contour=[None],color=None):
+    '''
+    The _`plot_load_frame` function plot the data in entry into a defined frame following different arguments fro the plot.
+    
+    Attribute :
+    ----------- 
+        ax : matplotlib.pyplot.axes
+            The axis on wich the data will be plot.
+        data : LOAD_TIME_GRID
+            A LOAD_TIME_GRID object with the LOAD_TIME_GRID.coeff to be ploted.
+        frame : (lon1,lon2,lat1,lat2)
+            The coordinate of the frame to plot.
+        time : float
+            The time of the plot that will be plot
+        resolution : int
+            The resolution of the plot, the resulting resolution will be resolution x resolution*2
+        name : str
+            The name of the plot, will be used in the title and legend of the plot
+        vmin : float
+            The minimal value of the plot colormap
+        vmax : float
+            The maximal value of the plot colormap
+        vcenter : float
+            The central value of the plot colormap
+        contour : np.array([n_c])
+            The contour that will be ploted on the map
+        color : np.array([n_c])
+            The contour fill color to be ploted
+        
+
+    Returns : 
+    --------- 
+        ax : matplotlib.pyplot.axes
+            The axis updated from the plots
+        
+    '''
+    t_it=np.where(data.time_step==time)[0][0]
+    data.coeff=(data.coeff_from_step(t_it-2).coeff-data.coeff_from_step(t_it-3).coeff)/(data.time_step[t_it-1]-data.time_step[t_it])
+    grid,lon_hd,lat_hd=data.coefftogrdhd(resolution)
+    lon_hd-=180
+    grid=np.concatenate((grid[:,resolution-1:],grid[:,:resolution]),axis=1)
+    lon_lim_min=np.abs(lon_hd-frame[0]).argmin()
+    lon_lim_max=np.abs(lon_hd-frame[1]).argmin()
+    lat_lim_min=np.abs(lat_hd-frame[2]).argmin()
+    lat_lim_max=np.abs(lat_hd-frame[3]).argmin()
+    lon=lon_hd[lon_lim_min:lon_lim_max+1]
+    lat=lat_hd[lat_lim_min:lat_lim_max+1]
+    grid=grid[lat_lim_min:lat_lim_max+1,lon_lim_min:lon_lim_max+1]
+
+
+    alpha_ocean=0
+    coast_line_width=0.5
+    cmap=cm.get_cmap('bwr', 100)
+    #cmap=mpl.colors.LinearSegmentedColormap.from_list('hsv_2',mpl.colormaps['hsv_r'].resampled(255)(range(255))[20:-20],gamma=1.0)
+    
+    if not(color is None):
+        cmap=None
+
+    norm = colors.TwoSlopeNorm(vmin=vmin,vmax=vmax,vcenter=vcenter)
+    if not(contour[0] is None):
+        if contour[0]<0 and contour[-1]>0 :
+            norm = colors.TwoSlopeNorm(vmin=contour[0],vmax=contour[-1],vcenter=0)
+        elif contour[0]<0 and contour[-1]<0 :
+            norm  = colors.TwoSlopeNorm(vmin=contour[0],vmax=contour[-1],vcenter=contour[-1])
+        elif contour[0]>0 and contour[-1]>0 :
+            norm  = colors.TwoSlopeNorm(vmin=contour[0],vmax=contour[-1],vcenter=contour[0])
+    
+    #print(frame_corr)
+    ax.set_extent(frame)
+    #ax.set_global()
+    if contour[0] is None :
+        m2 = ax.contourf(lon,lat,grid,levels=50,origin='lower', transform=ccrs.PlateCarree(central_longitude=0),extent=frame, zorder=0, cmap=cmap,colors=color,norm=norm)
+    else :
+        m2 = ax.contourf(lon,lat,grid,levels=contour,origin='lower', transform=ccrs.PlateCarree(central_longitude=0),extent=frame, zorder=0, cmap=cmap,colors=color,norm=norm)
+    if not(add_contour is None):
+        CS=ax.contour(lat,lon,add_contour,5,colors='k',linewidths=0.5,linestyles='solid')
+        ax.clabel(CS, CS.levels, inline=True, fontsize=10)
+    
+    cbar2=plt.colorbar(mappable=m2, orientation="horizontal")
+    cbar2.set_label(f'{name} VGM at {time} kyr, averaged over {(data.time_step[t_it-1]-data.time_step[t_it])*1000} year (mm/yr); maximum subsidenc : {np.min(np.min(grid))}')
+    # if not(contour is None):
+    #     cbar2.set_ticks(contour)
+    # elif not(vmax is None) and not(vmin is None):
+    #     cbar2.set_ticks([vmin, 0, vmax])
+    # elif not(vmin is None):
+    #     cbar2.set_ticks([vmin, 0, grid.max()])
+    # elif not(vmax is None):
+    #     cbar2.set_ticks([grid.min(), 0, vmax])
+    # else:
+    #     cbar2.set_ticks([grid.min(), 0, grid.max()])
+    cartopy.mpl.geoaxes.GeoAxes.gridlines(ax,crs=ccrs.PlateCarree(),draw_labels=True)
+    ax.add_feature(cartopy.feature.OCEAN, alpha=alpha_ocean, zorder=99, facecolor="#BBBBBB")
+    ax.coastlines(resolution="50m", zorder=100, linewidth=coast_line_width)
+
+    return ax
+
+from netCDF4 import Dataset
+
+
+
+def export_to_netcdf(Input_way,time,resolution,frame,save_way,type,type_bis):
+    '''
+    The _`export_to_netcdf` function export the data from the input_way, type and type_bis, of the frame shape into a netcdf file. This file can be open in any gis software.
+
+    Attribute : 
+    -----------
+        Input_way : str
+            way where the load data are located. If you are using the function from SL_C0de.SOLVER library, this way should be xxx/model_output/earth_model_name.
+        time : float
+            The time of the plot in kyr
+        resolution : int
+            the spatial resolution of the plot. ! This resolution concern the entire globe and not juste the frame.
+        frame : (lon1,lon2,lat1,lat2)
+            The coordinate of the frame to plot.
+        save_way : str
+            The filepath to save the netcdf file
+        type : str 
+            The type of loading taken into account. Can be : "SEDIMENT", "OCEAN", "ICE", "NO_SEDIMENT".
+        type_bis : str
+            The type of affected surface by the loading. Can be : "GEOID", "LOAD".
+            
+    ''' 
+    data=LOAD_TIME_GRID(from_file=(True,f'{Input_way}/LOAD/{type}_{type_bis}'))
+    t_it=np.where(data.time_step==time)[0][0]
+    data.height_time_coeff=data.viscuous_deformation+data.elastic_deformation
+    data.coeff=(data.coeff_from_step(t_it-2).coeff-data.coeff_from_step(t_it-3).coeff)/(data.time_step[t_it-1]-data.time_step[t_it])
+    grid,lon_hd,lat_hd=data.coefftogrdhd(resolution)
+    lon_hd-=180
+    grid=np.concatenate((grid[:,resolution-1:],grid[:,:resolution]),axis=1)
+    lon_lim_min=np.abs(lon_hd-frame[0]).argmin()
+    lon_lim_max=np.abs(lon_hd-frame[1]).argmin()
+    lat_lim_min=np.abs(lat_hd-frame[2]).argmin()
+    lat_lim_max=np.abs(lat_hd-frame[3]).argmin()
+    lon=lon_hd[lon_lim_min:lon_lim_max+1]
+    lat=lat_hd[lat_lim_min:lat_lim_max+1]
+    grid=grid[lat_lim_min:lat_lim_max+1,lon_lim_min:lon_lim_max+1]
+
+    data.ncgrid=Dataset(f'{save_way}/{data.time_grid_name}{frame}.nc','w','NETCDF4_CLASSIC')
+    data.ncgrid.title=data.time_grid_name
+
+    data.ncgrid.createDimension('lon',len(lon))
+    data.ncgrid.createDimension('lat',len(lat))
+
+
+    lati=data.ncgrid.createVariable('lat', np.float32, ('lat',))
+    lati.units = 'degrees_north'
+    lati.long_name = 'latitude'
+    lati[:]=lat
+
+    long=data.ncgrid.createVariable('lon', np.float32, ('lon',))
+    long.units = 'degrees_east'
+    long.long_name = 'longitude'
+    long[:]=lon
+
+    grided=data.ncgrid.createVariable('grid', np.float32, ('lat','lon'))
+    grided.units = 'mm/yr'
+    grided.long_name = 'grid'
+    grided[:,:]=grid
+
+    data.ncgrid.close()
```

### Comparing `slcode-0.4.1/src/SL_C0de/grid.py` & `slcode-1.0.0/slcode/grid.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,1489 +1,1497 @@
-import numpy as np
-import math
-from .spharm import sphericalobject
-import matplotlib.pyplot as plt
-from matplotlib import cm
-import matplotlib as mpl
-import stripy
-from netCDF4 import Dataset
-import pyshtools as pysh
-from .Load import LOAD
-import math
-
-from scipy import io
-
-def sph2cart(az, el, r):
-    rsin_theta = r * np.sin(el)
-    x = rsin_theta * np.cos(az)
-    y = rsin_theta * np.sin(az)
-    z = r * np.cos(el)
-    return x, y, z
-
-class GRID(object):
-        """
-        The class _`GRID` is used to represent the Gaussian Grid.
-
-        Attributes
-        ----------
-
-            .. note::
-
-                This grid have no attribute * this might be changed in future version to be used as stand alone. The absence of attribute is the result of the use of this function in :ref:`TIME_GRID <TIME_GRID>` that use that define all parameters used in the init function of GRID.
-
-        Methods
-        -------
-            `interp_on`_ : 
-                method used to interpolate the grid over the model grid.
-            `smooth_on`_ : 
-                method used to smooth the grid to reduce noise effect.
-            `disk`_ : 
-                method used to create a disk of certain shape to test parameters.
-                     
-
-        """
-        def __init__(self):
-            self.nlons = (self.maxdeg) * 2 
-            self.nlats = (self.maxdeg)
-            x,w=pysh.expand.SHGLQ(self.maxdeg-1)
-            x_GL = np.arccos(x[::-1])*180/math.pi - 90
-            lon_GL = np.linspace(0,360,2*self.maxdeg+1)
-            lon_GL = lon_GL[:-1]
-            self.lats=x_GL
-            self.elons=lon_GL
-            self.colats = 90 - self.lats
-            #self.elons,self.lats=np.meshgrid(self.elons,self.lats)
-        
-        # def add_time(self,time_step):
-        #     '''
-            
-        #     This function add time field to the object.
-        
-        # Parameters :  
-        #     time_step (np.array): a vector array of length number of time step.
-             
-        # See the documentation of the cited class object for more information on different parameters used in the function.
-        
-        # Returns :
-            
-        # Added fields : 
-        #     time_step (np.array): an array of each time step of length number of time step.
-        
-        #     '''
-        #     self.time_step=time_step # à ajouter dans ice grid definition
-            
-        def interp_on(self,grd,lon,lat,smoothing=False,grid_type='global',error=False):
-            '''
-            The method _`interp_on` interpolate a grid of data on the grid of the model calculated in the init function of `GRID`_. This function is using stripy library to pursue the interpolation (`Stripy library <https://underworldcode.github.io/stripy/2.0.5b2/FrontPage.html>`_).
-        
-            Attribute
-            --------- 
-                grd : np.array([m,n])
-                    The grid data over space.
-                lon : np.array([m,])
-                    The longitude of the data.
-                lat : np.array([n,])
-                    The latitude of the data.   
-                smoothing : bool
-                    If a smoothing is applied to the grid before the interpolation, see `smooth_on`_.
-                grid_type : str
-                    grid type define if it's a grid over the whole world or over a small area. This is used to avoid long computation for the interpolation in the case of interpolating small areas over the world. There is two possible 'global' and 'local'. The global interpolation is using `stripy.sTriangulaion <https://underworldcode.github.io/stripy/2.0.5b2/SphericalMeshing/SphericalTriangulations/Ex3-Interpolation.html>`_. The local interpolation is using `stripyt.Triangulation <https://underworldcode.github.io/stripy/2.0.5b2/SphericalMeshing/CartesianTriangulations/Ex3-Interpolation.html>`_.        
-                error : bool
-                    If true, the method return the error of the interpolation calculated by stripy.
-                
-            Return
-            ------
-                grd : np.array([maxdeg*2,maxdeg])
-                    The grid interpolated on the model grid.
-            '''
-            if grid_type=='global':
-                lon,lat=np.meshgrid(lon,lat)
-                vertices_lat=np.radians(lat.flatten())
-                vertices_lon=np.radians(lon.flatten())
-                spherical_triangulation = stripy.sTriangulation(lons=vertices_lon, lats=vertices_lat,refinement_levels=0,permute=True)
-                if smoothing :
-                    grd,dds,err=spherical_triangulation.smoothing(grd.flatten(),np.ones_like(grd.flatten()),0.1,0.1,0.01)
-                elons,lats=np.meshgrid(self.elons,self.lats)
-                vertices_lats=np.radians(lats.flatten())
-                vertices_elons=np.radians(elons.flatten())
-                grd,err=spherical_triangulation.interpolate_nearest(vertices_elons,vertices_lats,data=grd.flatten())
-                grd[np.isnan(grd)]=0
-            elif grid_type=='local':
-                # Select the points inside the local studied zone.
-                spherical_triangulation = stripy.Triangulation(x=lon, y=lat,permute=True)
-                if smoothing :
-                    grd,dds,err=spherical_triangulation.smoothing(grd,np.ones_like(grd),0.1,0.1,0.01)
-                elons,lats=np.meshgrid(self.elons,self.lats)
-                lats=lats.flatten()
-                elons=elons.flatten()
-                point_in=((elons>lon.min())*(elons<lon.max()))*((lats>lat.min())*(lats<lat.max()))
-                elons_in=elons[point_in]
-                lats_in=lats[point_in]
-                grd_in,err=spherical_triangulation.interpolate_nearest(elons_in,lats_in,grd)
-                # I need to complete the grid where the is no data
-                grd=np.zeros(elons.shape)
-                grd[point_in]=grd_in
-            else:
-                print('No such grid type, please select one between : regular or samples')
-            if error : 
-                return grd.reshape((self.nlats,self.nlons)), err.reshape((self.nlats,self.nlons))
-            return grd.reshape((self.nlats,self.nlons))
-        
-        def smooth_on(self,grd,lon,lat):
-
-            '''
-            The method _`smooth_on` is smoothing the grid over the area whith `smoothing <https://underworldcode.github.io/stripy/2.0.5b2/SphericalMeshing/CartesianTriangulations/Ex5-Smoothing.html>`_. This function can be used to correct values before the interpolation over time and space. This way, you can have better results on topographic convergence.
-
-            Attribute
-            ---------
-                grd : np.array([m,n])
-                    Array containig the grid values over the space.
-                lat : nparray([n,])
-                    latitude.
-                lon : nparray([m,])
-                    longitude.
-            
-            Return
-            ------
-                grd : np.array([m,n])
-                    smoothed array with the same shape then the initial grid.
-            '''
-
-            lon,lat=np.meshgrid(lon,lat)
-            vertices_lat=np.radians(lat.ravel())
-            vertices_lon=np.radians(lon.ravel())
-            spherical_triangulation = stripy.sTriangulation(lons=vertices_lon, lats=vertices_lat,refinement_levels=0)
-            grd,dds,err=spherical_triangulation.smoothing(grd.flatten(),np.ones_like(grd.flatten()),10,0.1,0.01)
-            elons,lats=np.meshgrid(self.elons,self.lats)
-            vertices_lats=np.radians(lats.ravel())
-            vertices_elons=np.radians(elons.ravel())
-            grd,err=spherical_triangulation.interpolate_nearest(vertices_elons,vertices_lats,data=grd.flatten())
-            grd[np.isnan(grd)]=0
-            grd=grd.reshape(elons.shape)
-            return grd
-
-        def disk(self,lat,lon,radius,high,tx=1):
-            '''
-            _`disk` is a method used to create a thickness grid. This grid can be used to test different parameters.
-
-            Attribute
-            ---------
-                lat : nparray([1,])
-                    Array contaning the latitudinal coordinate in degree of the center of the disk.
-                lon : nparray(1,[])
-                    Array containing the longitudinal coordinate in degree of the center of the disk.
-                radius : double
-                    The radius in degree of the disk in degree.
-                high : double
-                    The thickness in meter of the disk over the considered area.
-            
-            Return
-            ------
-                grd : np.array([maxdeg*2,maxdeg])
-                    The grid as defined by the `GRID`_ class with a disk of thikness high at lon,lat position with the size of radius.
-        
-            '''
-
-            grd=np.zeros((tx,self.lats.size,self.elons.size))
-            lon_g,lat_g=np.meshgrid(self.elons,self.lats)
-            grd[:,((lon-lon_g)**2+(lat-lat_g)**2)<radius]=high
-            grd[:,:2,:]=grd[:,:2,:]*0
-            return grd
-
-        def zeros(self,tx=1):
-            '''
-            _`zeros` is a method used to generate a zero array with the caracteristics of the grid. 
-            
-            Attribute : 
-            -----------
-                tx : int
-                    times the thickness is repeated
-
-            Return :
-            --------
-                np.zeros((tx,self.lats.size,self.elons.size))
-                    An array containing only zeros 
-            '''
-            return np.zeros((tx,self.lats.size,self.elons.size))
-        
-        def along_transect(self,coord=('lat_start','lon_start','lat_stop','lon_stop'),point_density=None,point_distance=None):
-            if not(point_density is None):
-                theta=np.linspace(coord[0],coord[2],point_density)
-                phi=np.linspace(coord[1],coord[3],point_density)
-            if not(point_distance is None):
-                theta=np.arange(coord[0],coord[2],point_distance)
-                phi=np.arange(coord[1],coord[3],point_distance)
-            i=0
-            Y_lm=np.expand_dims(pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[0]+pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[1]*1j,axis=1)
-            
-            for i in range(1,len(phi)):
-                Y_lm=np.concatenate((Y_lm,np.expand_dims((pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[0]+pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[1]*1j),axis=1)),axis=1)
-            return (Y_lm*np.repeat(np.expand_dims(self.coeff,axis=1),point_density,axis=1)).sum(0)
-
-class TIME_GRID(GRID,sphericalobject):
-    """
-    The _`TIME_GRID` class is used to manage the mass grids. These grids have a time dimenssion this way wa can manage the time variation of the mass. We can define the mass grid by it's mass directly or by coupling a height with a density. If needed you can load spherical harmonics coefficient.Tis class is inheriting the methods from :ref:`sphericalobject <sphericalobject>` and :ref:`GRID <GRID>`. 
-
-    Attributes
-    ----------
-        time_step : np.array([time_step_number,])
-            This array contains the time step of the data you are importing. They will be use for temporal interpolation.
-        maxdeg : int
-            Maximum harmonic coefficient degree of the data. this define the chape of the grid and coefficient arrays
-        height_time_grid : np.array([maxedg*2,maxdeg])
-            This array is the height grid at each time steps defined in grid_time_step
-        mass_time_grid : np.array([maxedg*2,maxdeg])
-            This array is the mass grid at each time steps defined in grid_time_step
-        height_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
-            This array is the height spherical harmonic coefficient at each time steps defined in grid_time_step
-        mass_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
-            This array is the mass spherical harmonic coefficient at each time steps defined in grid_time_step
-        rho : float
-            The density of the considered layer. 
-        
-        .. note::
-
-            In future development the density may vary threw space and time. We'll have to make a variable object more then a constant density. 
-
-        grid_name : str
-            The name of the grid. We recommand you to choose a specific name for each grid you create. This name is used to save the grid in an nc file with `save`_. 
-        from_file : (bool,way)
-            This parameter define if the data are new or loaded from a previously saved model in a nc file. If the first element is False, the code will create a blank object, based on provided datas. If the first element is True, the method will get the data from the file way specified in the second element of this attribute.
-        superinit : bool
-            This parameter is used to specify if the object is used as herited method in an initialisation of a child class object.
-    
-    Methods
-    -------
-        `interp_on_time`_ 
-            Interpolate a grid over the time considered in the model  
-        `interp_on_time_and_space`_ :
-            Interpolate the grid over time and space as in the defined Grid during the initialisation of the class
-        `grid_from_step`_ :
-            Get the grid for a defined time iteration
-        `coeff_from_step`_ :
-            Get the spherical harmonics coefficient for a defined time iteration
-        `timegrdtotimecoeff`_ :
-            Convert the grid into spherical harmonics coefficient for all time steps
-        `timecoefftotimegrd`_ :
-            Convert the spherical harmonics coefficient into grid for all time steps
-        `zeros_time`_ :
-            Generate a zero grid for all time steps
-        `disk_time`_ :
-            Generate a disk of a specified thickness at a specified location over all time steps
-        `update_0`_ :
-            Update the 0 time step data of the grid
-        `save`_ :
-            Save the grid in a specified nc file with the name of the grid
-
-    """
-
-    def __init__(self,time_step=np.array([1,2]),maxdeg=64,height_time_grid=None,mass_time_grid=None,mass_time_coeff=None,height_time_coeff=None,rho=0,grid_name='time_grid',from_file=(False,),superinit=False):
-        if not(from_file[0]) :
-            self.maxdeg=maxdeg
-            super().__init__()
-            self.isgrd=False
-            self.iscoeff=False
-
-
-            self.time_grid_name=grid_name
-
-            self.saved=np.array([]) # initialize the save of the spherical harmonic object
-
-            self.rho=rho
-
-            self.time_step=time_step
-            self.time_step_number=len(time_step)
-
-            self.height_time_grid=np.zeros((self.time_step_number-1,self.nlats,self.nlons))
-            self.mass_time_grid=np.zeros((self.time_step_number-1,self.nlats,self.nlons))
-            self.height_time_coeff=np.zeros((self.time_step_number-1,int(maxdeg*(maxdeg+1)/2)))+0j
-            self.mass_time_coeff=np.zeros((self.time_step_number-1,int(maxdeg*(maxdeg+1)/2)))+0j
-
-            if not(height_time_grid is None):
-                self.height_time_grid=height_time_grid
-                self.mass_time_grid=height_time_grid*rho
-                self.grd_0=self.mass_time_grid[0,:,:]
-            elif not(mass_time_grid is None):
-                self.mass_time_grid=mass_time_grid
-                self.grd_0=self.mass_time_grid[0,:,:]
-            elif not(height_time_coeff is None):
-                self.height_time_coeff=height_time_coeff
-                self.mass_time_coeff=height_time_coeff*rho
-                self.coeff_0=self.mass_time_coeff[0,:]
-            elif not(mass_time_coeff is None):
-                self.mass_time_coeff=mass_time_coeff
-                self.coeff_0=self.mass_time_coeff[0,:]
-
-        elif from_file[0] :
-            self.ncgrid = Dataset(from_file[1]+'.nc',mode='r',format='NETCDF4_CLASSIC') 
-            self.time_grid_name=self.ncgrid.title
-            self.maxdeg=len(self.ncgrid['lat'][:].data)
-            super().__init__()
-
-            self.time_step=self.ncgrid['time'][:].data
-            self.time_step_number=len(self.time_step)
-            self.maxdeg=self.ncgrid.dimensions['maxdeg'].size
-
-            self.rho=self.ncgrid['rho'][:].data
-
-            self.height_time_grid=self.ncgrid['thickness'][:].data
-            self.mass_time_grid=np.zeros((self.time_step_number,self.nlats,self.nlons))
-            self.height_time_coeff=self.ncgrid['coeff_real'][:].data+self.ncgrid['coeff_imag'][:].data*1j
-            self.mass_time_coeff=np.zeros((self.time_step_number,int(self.maxdeg*(self.maxdeg+1)/2)))+0j
-
-            self.mass_time_grid=self.height_time_grid*rho
-
-            if not(superinit):
-                self.ncgrid.close()
-
-    def interp_on_time(self,grid_to_interp,grid_time_step,model_time_step,interp_type='Thickness_divide',backend='False',grid_type='regular'):
-        """
-        The function _`interp_on_time` is used for interpolation upon time and space it call the interpolation function of the :ref:`GRID <GRID>` parameter. This function adapt the order of time and space interpolation to reduce computation time. The temporal interpolation try to preserve the thickness of the overall time. Tis is down by cutting and merging time steps of the original grid to match the model time_step. 
-
-        Attributes
-        ----------
-            grid_to_interp : np.array([k,n,m])
-                The grid to be interpreted.
-            grid_time_step : np.array([k,])
-                The time value of each time step of the grid model.
-            model_time_step ; np.array([time_step_number,])
-                The time values of the model.
-            interp_type : str
-                No use of this parameter anymore
-            backend : bool 
-                Define if the function retur, backends. True it will return the backends, False (default value) don't give any backend. 
-        
-        Return :
-        --------
-            grid_interpolated : np.array([time_step_number,n,m])
-                The interpolated grid over time. Depending of the model parameters. 
-        """
-
-        if interp_type=="Thickness_divide":
-            grid_time_step=grid_time_step[::-1]
-            model_time_step=model_time_step[::-1]
-            if grid_type=='global':
-                grid_to_interp=grid_to_interp[::-1,:,:]
-                d_grid_time_step=np.diff(grid_time_step)
-                d_grid_to_interp=grid_to_interp/d_grid_time_step[:,np.newaxis,np.newaxis]
-
-                Merge_time_step=np.unique(np.concatenate((grid_time_step,model_time_step)), return_index=True)
-                Merge_time_step=(Merge_time_step[0],Merge_time_step[1]+1)
-                Merge_time_step[1][Merge_time_step[1]>len(grid_time_step)]=0
-
-                out=len(model_time_step[model_time_step>grid_time_step.max()])
-
-                count=np.diff(np.nonzero(Merge_time_step[1])).squeeze()
-                to_merge=np.searchsorted(Merge_time_step[0],grid_time_step[np.isin(grid_time_step,model_time_step,invert=True)].squeeze())-1
-                grd_interpolated=np.zeros((len(Merge_time_step[0])-1,d_grid_to_interp.shape[1],d_grid_to_interp.shape[2]))
-                grd_interpolated=np.array(np.concatenate((d_grid_to_interp.repeat(count,axis=0),np.zeros((out,d_grid_to_interp.shape[1],d_grid_to_interp.shape[2]))))*np.diff(Merge_time_step[0])[:,np.newaxis,np.newaxis])
-
-                for i in range(len(to_merge)):
-                    if backend :
-                        print('time slicing : ' + str(i))
-                    grd_interpolated[to_merge[i]-1,:,:]+=grd_interpolated[to_merge[i],:,:]
-                    grd_interpolated=np.delete(grd_interpolated,to_merge[i],0)
-                    to_merge-=1
-                return grd_interpolated[::-1,:,:]
-            elif grid_type=='local':
-                grid_to_interp=grid_to_interp[::-1,:]
-                d_grid_time_step=np.diff(grid_time_step)
-                d_grid_to_interp=grid_to_interp/d_grid_time_step[:,np.newaxis]
-
-                Merge_time_step=np.unique(np.concatenate((grid_time_step,model_time_step)), return_index=True)
-                Merge_time_step=(Merge_time_step[0],Merge_time_step[1]+1)
-                Merge_time_step[1][Merge_time_step[1]>len(grid_time_step)]=0
-
-                out=len(model_time_step[model_time_step>grid_time_step.max()])
-
-
-                count=np.diff(np.nonzero(Merge_time_step[1])).squeeze()
-                to_merge=np.searchsorted(Merge_time_step[0],grid_time_step[np.isin(grid_time_step,model_time_step,invert=True)].squeeze())-1
-                grd_interpolated=np.zeros((len(Merge_time_step[0])-1,d_grid_to_interp.shape[1]))
-                grd_interpolated=np.array(np.concatenate((d_grid_to_interp.repeat(count,axis=0),np.zeros((out,d_grid_to_interp.shape[1]))))*np.diff(Merge_time_step[0])[:,np.newaxis])
-
-                for i in range(len(to_merge)):
-                    if backend :
-                        print('time slicing : ' + str(i))
-                    grd_interpolated[to_merge[i]-1,:]+=grd_interpolated[to_merge[i],:]
-                    grd_interpolated=np.delete(grd_interpolated,to_merge[i],0)
-                    to_merge-=1
-                return grd_interpolated[::-1,:]
-            else :
-                print('no such grid type avaiable. try local or global')
-
-    def interp_on_time_and_space(self,grid_to_interp,grid_time_step,grid_lon,grid_lat,interp_type='Thickness_divide',backend=False,grid_type='global'):
-        """
-        The _`interp_on_time_and_space` function is used for interpolation upon time and space it call the interpolation function of the :ref:`GRID <GRID>` parameter. This function perform the temporal and spatial interpolation in different order to ameliorate the computation time. If the temporal resolution of the input grid is higher than the model time resolution the temporal resolution will be perform first. The spatial resolution is performed first in the other case.
-
-        Attributes
-        ----------
-            grid_to_interp : np.array([k,n,m])
-                The grid to be interpreted.
-            grid_time_step : np.array([k,])
-                The time value of each time step of the grid_to_interp.
-            grid_lon : np.array([n])
-                The longitudinal coordinates of the grid_to_interp.
-            grid_lat : np.array([m])
-                The latitudinal coordinate of the grid_to_interp.
-            interp_type : str
-                No use of this parameter anymore
-            backend : bool 
-                Define if the function retur, backends. True it will return the backends, False (default value) don't give any backend. 
-        
-        Return :
-        --------
-            grid_interpolated : np.array([time_step_number,maxdeg*2,maxdeg])
-                The interpolated grid over time. Depending of the model parameters. 
-        """
-        if len(grid_time_step)<self.time_step_number:
-            time_grid_pre_interp=np.zeros((len(grid_time_step)-1,self.nlats,self.nlons))
-            for i in range(len(grid_time_step)-1):
-                if backend :
-                    print('interpolation number : ' + str(i))
-
-                time_grid_pre_interp[i,:,:]=self.interp_on(grid_to_interp[i],grid_lon,grid_lat,grid_type=grid_type)
-            grid_type='global'
-            self.height_time_grid=self.interp_on_time(time_grid_pre_interp,grid_time_step,self.time_step,interp_type,backend=backend,grid_type=grid_type)
-        else :
-            grd_to_interpolate=self.interp_on_time(grid_to_interp,grid_time_step,self.time_step,interp_type,backend=backend,grid_type=grid_type)
-            for i in range(self.time_step_number-1):
-                if backend :
-                    print('interpolation number : ' + str(i))
-                self.height_time_grid[i,:,:]=self.interp_on(grd_to_interpolate[i,:],grid_lon,grid_lat,grid_type=grid_type)
-
-    
-    def grid_from_step(self,t_it):
-        """
-        The _`grid_from_step` method is used to get the value of the grid at the defined time step.
-        
-        Attributes :
-        ------------
-            t_it : int
-                This is the value of the time step iteration on wich you are trying to retreave the grid. It must inside the time_step interpolation you have used during the initialisation of the time grid. 
-        
-        Return :
-        --------
-            None
-        """
-        # if not(self.mass_time_grid is None) :
-        #     self.grd=self.mass_time_grid[t_it,:,:]
-        # elif not(self.height_time_grid is None):
-        self.grd=self.height_time_grid[t_it,:,:].copy()
-        return self
-
-    def coeff_from_step(self,t_it):
-        """
-        The _`coeff_from_step` method is used to get the value of the coefficient at the requested time iteration.
-        
-        Attributes :
-        ------------
-            t_it : double
-                This is the value of the time step iteration on wich you are trying to retreave the coefficient. It must be inside the time_step interpolation you have used during the initialisation of the time grid.
-
-        Return :
-        --------
-            None
-        """
-        # if not(self.mass_time_coeff is None) :
-        #     self.coeff=self.mass_time_coeff[t_it,:]
-        # elif not(self.height_time_coeff is None):
-        self.coeff=self.height_time_coeff[t_it,:].copy()
-        return self
-    
-    def timegrdtotimecoeff(self):
-        """
-        The _`timegrdtotimecoeff` method transform for each time step the grid into spherical harmonics coefficient. 
-
-        Attribute :
-        -----------
-            None
-        
-        Result :
-        --------
-            None
-
-        """
-        for i in range(self.time_step_number-1):
-            self.grd=self.height_time_grid[i,:,:]
-            self.height_time_coeff[i,:]=self.grdtocoeff().coeff
-        return self
-    
-    def timecoefftotimegrd(self):
-        """
-        The _`timecoefftotimegrd` method transform for each time step the spherical harmonic coefficient into a grid. 
-
-        Attribute :
-        -----------
-            None
-        
-        Result :
-        --------
-            None
-        """
-        for i in range(self.time_step_number-1):
-            self.coeff=self.height_time_coeff[i,:]
-            self.height_time_grid[i,:,:]=self.coefftogrd().grd
-        return self
-    
-    def zeros_time(self,time_step_number):
-        """
-        The _`zeros_time` method is used to define a grid over time with only 0 value. It is based on :ref:`GRID.zeros <zeros>`. 
-
-        Attribute :
-        -----------
-            time_step_number : int
-                The number of time step on wich we apply the zeros grid.
-        
-        Return :
-        --------
-            None
-        """
-        self.height_time_grid=self.zeros(time_step_number)
-    
-    def disk_time(self,time_step_number,lat,lon,radius,high):
-        """
-        The _`disk_time` method is used to define a grid over time with a disk defined with it's center coordinate and the height. This function is based on :ref:`GRID.disk <disk>`.
-
-        Attribute :
-        -----------
-            time_step_number : int
-                The number of time step on wich the disk load will be applyed.
-            lat : double
-                The latitude of the center of the disk (°).
-            lon : double
-                The longitude of the center of the disk (°).
-            radius : double
-                The radius of the disk (°).
-            high : double
-                The high of the disk (m).
-        Return :
-        --------
-            None
-        """
-        self.height_time_grid=self.disk(lat,lon,radius,high,time_step_number)
-    
-    def update_0(self):
-        """
-        The _`update_0` function is used to save the first time iteration of the object before it's modification to be called at any moment in the code without alteration.
-
-        Attribute :
-        -----------
-            None
-        Return :
-        --------
-            None
-
-        """
-        if not(self.height_time_grid is None) :
-            self.grd_0=self.height_time_grid[0,:,:].copy()
-        if not(self.height_time_coeff is None) :
-            self.coeff_0=self.height_time_coeff[0,:].copy()
-
-    def plot_step_on_sphere(self,time_step,cmap=cm.inferno,vmin=None,vmax=None,clip=False,inverse=False):
-        colormap=cmap
-        if vmin==None and vmax==None :
-            normaliser = mpl.colors.Normalize(vmin=np.min(self.height_time_grid[time_step,:,:]), vmax=np.max(self.height_time_grid[time_step,:,:]),clip=clip)
-        elif vmax==None and not(vmin==None):
-            normaliser = mpl.colors.Normalize(vmin=vmin, vmax=np.max(self.height_time_grid[time_step,:,:]),clip=clip)
-        elif vmin==None and not(vmax==None):
-            normaliser = mpl.colors.Normalize(vmin=np.min(self.height_time_grid[time_step,:,:]), vmax=vmax,clip=clip)
-        if inverse:
-            normaliser.inverse()
-        
-        elons,lats=np.meshgrid(self.elons,self.lats)
-        
-        u=elons/360*2*math.pi
-        v=(lats+90)/180*math.pi
-        x,y,z=sph2cart(u.flatten(),v.flatten(),np.ones((u.flatten().shape)))
-        fig = plt.figure()
-        ax = fig.add_subplot(111, projection="3d")
-        ax.plot_surface(np.reshape(x,(self.lats.shape[0],self.elons.shape[0])),np.reshape(y,(self.lats.shape[0],self.elons.shape[0])),np.reshape(z,(self.lats.shape[0],self.elons.shape[0])),facecolors=colormap(normaliser(self.height_time_grid[time_step,:,:])),cmap=colormap)
-        ax.set_aspect('equal')
-
-    def scatter_step_on_sphere(self,time_step,cmap=cm.inferno,vmin=None,vmax=None,clip=False,inverse=False,marker='.',s=0.2):
-        colormap=cmap
-        if vmin==None and vmax==None :
-            normaliser = mpl.colors.Normalize(vmin=np.min(self.height_time_grid[time_step,:,:]), vmax=np.max(self.height_time_grid[time_step,:,:]),clip=clip)
-        elif vmax==None and not(vmin==None):
-            normaliser = mpl.colors.Normalize(vmin=vmin, vmax=np.max(self.height_time_grid[time_step,:,:]),clip=clip)
-        elif vmin==None and not(vmax==None):
-            normaliser = mpl.colors.Normalize(vmin=np.min(self.height_time_grid[time_step,:,:]), vmax=vmax,clip=clip)
-        if inverse:
-            normaliser.inverse()
-
-        elons,lats=np.meshgrid(self.elons,self.lats)
-        
-        u=elons/360*2*math.pi
-        v=(lats+90)/180*math.pi
-        x,y,z=sph2cart(u.flatten(),v.flatten(),np.ones((u.flatten().shape)))
-        fig = plt.figure()
-        ax = fig.add_subplot(111, projection="3d")
-        ax.scatter(x,y,z,marker=marker,c=colormap(normaliser(self.height_time_grid[time_step,:,:].flatten())),s=s)
-        ax.set_aspect('equal')
-
-    def plot_step(self,time_step):
-        fig = plt.figure()
-        ax = fig.add_subplot(111)
-        elons,lats=np.meshgrid(self.elons,self.lats)
-        ax.pcolor(elons,lats,self.height_time_grid[time_step,:,:])
-
-    def point_time(self,coords):
-        points=np.zeros((coords.shape[0],self.time_step_number))
-        for t_it in range(self.time_step_number):
-            coeff=(self.height_time_coeff[t_it-2,:]-self.height_time_coeff[t_it-3,:])/(self.time_step[t_it-2]-self.time_step[t_it-3])
-            coeff=np.stack((coeff.real,coeff.imag))
-            coeff=pysh.shio.SHCindexToCilm(coeff)
-            points[:,t_it]=-pysh.expand.MakeGridPoint(coeff,-coords[:,0],coords[:,1])
-        return points
-    
-    def along_transect(self,coord=('lat_start','lon_start','lat_stop','lon_stop'),point_density=None,point_distance=None,backend=False):
-        if not(point_density is None):
-            theta=np.linspace(-coord[0],-coord[2],point_density)
-            phi=np.linspace(coord[1],coord[3],point_density)
-        if not(point_distance is None):
-            theta=np.arange(-coord[0],-coord[2],point_distance)
-            phi=np.arange(coord[1],coord[3],point_distance)
-        coeff=np.stack((self.coeff.real,self.coeff.imag))
-        coeff=pysh.shio.SHCindexToCilm(coeff)
-        transect=pysh.expand.MakeGridPoint(coeff,theta,phi)
-        # Y_lm=np.expand_dims(pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[0]+pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[1]*1j,axis=1)
-        # for i in range(1,len(phi)):
-        #     Y_lm=np.concatenate((Y_lm,np.expand_dims((pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[0]+pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[1]*1j),axis=1)),axis=1)
-        # self.coeff_from_step(0)
-        # transect=np.expand_dims((Y_lm*np.repeat(np.expand_dims(self.coeff,axis=1),point_density,axis=1)).sum(0),axis=1)
-        # for t_it in range(1,self.height_time_coeff.shape[0]):
-        #     if backend :
-        #         print(t_it)
-        #     self.coeff_from_step(t_it)
-        #     transect=np.concatenate((transect,np.expand_dims((Y_lm*np.repeat(np.expand_dims(self.coeff,axis=1),point_density,axis=1)).sum(0),axis=1)),axis=1)
-        return transect
-
-    def save(self,save_way='',supersave=False):
-
-        """
-        The _`save` function is used to save the grid and all it's parameters inside a nc file. Parameters saved are, longitude, latitude, maximum degree, the time steps of the grid, the thickness of the grid, the harmonic coefficient, grid density. The harmonic coefficient, due to complexe data type management of nc, are saved separately in there complexe and real part. The created file will have the name of the grid. 
-
-        Attribute :
-        -----------
-            save_way : str
-                The filepath where the data will be saved. Default value is the current file
-            supersave : bool
-                Define if the save is called as a super method from an object that inherit the function. This precise if this method has to close the nc file (False) of if the herited class will do it (True). Default value is False.
-        Return :
-        --------
-            None
-
-        """
-
-        self.ncgrid=Dataset(save_way+'/'+self.time_grid_name+'.nc','w','NETCDF4_CLASSIC')
-        self.ncgrid.title=self.time_grid_name
-
-        self.ncgrid.createDimension('maxdeg',self.maxdeg)
-        self.ncgrid.createDimension('maxdeg_order',(self.maxdeg)*(self.maxdeg+1)/2)
-        self.ncgrid.createDimension('lon',self.nlons)
-        self.ncgrid.createDimension('lat',self.nlats)
-        self.ncgrid.createDimension('time_diff',self.time_step_number-1)
-        self.ncgrid.createDimension('time_step',self.time_step_number)
-
-        lat=self.ncgrid.createVariable('lat', np.float32, ('lat',))
-        lat.units = 'degrees_north'
-        lat.long_name = 'latitude'
-        lat[:]=self.lats
-
-        lon=self.ncgrid.createVariable('lon', np.float32, ('lon',))
-        lon.units = 'degrees_east'
-        lon.long_name = 'longitude'
-        lon[:]=self.elons
-
-        time=self.ncgrid.createVariable('time', np.float32, ('time_step',))
-        time.units = 'kyr'
-        time.long_name = 'time'
-        time[:]=self.time_step
-
-        thickness=self.ncgrid.createVariable('thickness',np.float32,('time_diff','lat','lon'))
-        thickness.units='m'
-        thickness.long_name='layer_thickness'
-        thickness[:,:,:]=self.height_time_grid
-
-        coeff_real=self.ncgrid.createVariable('coeff_real',np.float32,('time_diff','maxdeg_order'))
-        coeff_real.units='m'
-        coeff_real.long_name='layer thickness in spherical harmonics'
-        coeff_real[:,:]=np.real(self.height_time_coeff)
-
-        coeff_imag=self.ncgrid.createVariable('coeff_imag',np.float32,('time_diff','maxdeg_order'))
-        coeff_imag.units='m'
-        coeff_imag.long_name='layer thickness in spherical harmonics'
-        coeff_imag[:,:]=np.imag(self.height_time_coeff)
-
-        rho=self.ncgrid.createVariable('rho',np.float32)
-        rho.units='kg/m3'
-        rho.long_name='density of the considered grid'
-        rho[:]=self.rho
-        
-        if not(supersave) :
-            self.ncgrid.close()
-
-class SEDIMENT_TIME_GRID(TIME_GRID):
-    """
-    The _`SEDIMENT_TIME_GRID` class is used to represent sediment deposited thickness and time over time. It inherit from :ref:`TIME_GRID <TIME_GRID>` and just add a default value of sediment density at 2600 kg/m3. 
-
-    .. note::
-        This class must include the developement of :cite:`ferrier_2017` on sediment compaction and it's effect on water redistriution. 
-
-    Attributes
-    ----------
-        time_step : np.array([time_step_number,])
-            This array contains the time step of the data you are importing. They will be use for temporal interpolation.
-        maxdeg : int
-            Maximum harmonic coefficient degree of the data. this define the chape of the grid and coefficient arrays
-        height_time_grid : np.array([maxedg*2,maxdeg])
-            This array is the height grid at each time steps defined in grid_time_step
-        mass_time_grid : np.array([maxedg*2,maxdeg])
-            This array is the mass grid at each time steps defined in grid_time_step
-        height_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
-            This array is the height spherical harmonic coefficient at each time steps defined in grid_time_step
-        mass_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
-            This array is the mass spherical harmonic coefficient at each time steps defined in grid_time_step
-        rho : float
-            The density of the considered layer. Default value is 2600.
-        
-        .. note::
-
-            In future development the density may vary threw space and time. We'll have to make a variable object more then a constant density. 
-
-        grid_name : str
-            The name of the grid. We recommand you to choose a specific name for each grid you create. This name is used to save the grid in an nc file with `save`_. 
-        from_file : (bool,way)
-            This parameter define if the data are new or loaded from a previously saved model in a nc file. If the first element is False, the code will create a blank object, based on provided datas. If the first element is True, the method will get the data from the file way specified in the second element of this attribute.
-
-    Method
-    ------
-        :ref:`save <sed_save>` 
-            used to save data
-
-    """
-    def __init__(self,time_step=np.array([1,2]),maxdeg=64,height_time_grid=None,mass_time_grid=None,mass_time_coeff=None,height_time_coeff=None,rho=2600,grid_name='time_grid',from_file=(False,)) : 
-        """
-        Parameters
-        ----------
-        """
-        # preset the grid and coefficient to none. The sediment density is set to 2300 
-        super().__init__(time_step,maxdeg,height_time_grid,mass_time_grid,height_time_coeff,mass_time_coeff,rho,grid_name,from_file,superinit=True)
-        self.isgrd=False
-        self.iscoeff=False
-        self.saved=np.array([])
-        if from_file[0] :
-            self.ncgrid.close()
-
-    def save(self,save_way=''):
-        """
-        .. _sed_save:
-
-        The save method is used to save the grid data to a file. It call the super method :ref:`save <save>` method with no additional saved parameters.   
-
-        .. note::
-            Because we need to include :cite:`ferrier_2017` works, this save function will be modified to include data about the sediment compaction.  
-
-        Attributes
-        ----------
-            rho : float
-                Density value of the sediment as a constant, default value is 2600.
-
-        Return
-        ------
-            None
-
-        """
-        super().save(save_way,supersave=True)
-        self.ncgrid.close()
-
-class ICE_TIME_GRID(TIME_GRID):
-    """
-    The _`ICE_TIME_GRID` class is used to represent the ice thickness evolution threw time. This class inherit of :ref:`TIME_GRID <TIME_GRID>`. 
-
-    ...
-
-    Attributes
-    ----------
-        time_step : np.array([time_step_number,])
-            This array contains the time step of the data you are importing. They will be use for temporal interpolation.
-        maxdeg : int
-            Maximum harmonic coefficient degree of the data. this define the chape of the grid and coefficient arrays
-        height_time_grid : np.array([maxedg*2,maxdeg])
-            This array is the height grid at each time steps defined in grid_time_step
-        mass_time_grid : np.array([maxedg*2,maxdeg])
-            This array is the mass grid at each time steps defined in grid_time_step
-        height_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
-            This array is the height spherical harmonic coefficient at each time steps defined in grid_time_step
-        mass_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
-            This array is the mass spherical harmonic coefficient at each time steps defined in grid_time_step
-        rho : float
-            The density of the considered layer. Default is 916.7 kg/m3.
-        
-        .. note::
-
-            In future development the density may vary threw space and time. We'll have to make a variable object more then a constant density. 
-
-        grid_name : str
-            The name of the grid. We recommand you to choose a specific name for each grid you create. This name is used to save the grid in an nc file with `save`_. 
-        from_file : (bool,way)
-            This parameter define if the data are new or loaded from a previously saved model in a nc file. If the first element is False, the code will create a blank object, based on provided datas. If the first element is True, the method will get the data from the file way specified in the second element of this attribute.
-        
-        
-    Methods
-    -------
-        `ice_correction`_ 
-            correct the grounded ice thickness from the created floating ice by ground vertical mouvement
-        :ref:`save <ice_save>` 
-            used to save data
-        
-    """
-    def __init__(self,time_step=np.array([1,2]),maxdeg=64,height_time_grid=None,mass_time_grid=None,mass_time_coeff=None,height_time_coeff=None,rho=916.7,grid_name='time_grid',from_file=(False,)) : 
-        """
-        Parameters
-        ----------
-        """
-        # initialize to false the grid and coefficient (no grid or coefficient pre loaded). The ice volumetric masse is set to 916.7 kg/m3.
-        super().__init__(time_step,maxdeg,height_time_grid,mass_time_grid,height_time_coeff,mass_time_coeff,rho,grid_name,from_file,superinit=True)
-        # self.isgrd=False
-        # self.iscoeff=False
-        self.saved=np.array([])
-        self.sdeli_00=0
-        self.deli_00_prev=0
-
-        if from_file[0] :
-            self.ice=self.ncgrid['ice'][:].data
-            self.ncgrid.close()
-
-    def ice_correction(self,topo,oc):
-        """
-        The _`ice_correction` method is used to correct the grounded ice thickness from the floating ice generted by vertical ground motion. This correction is done for each time step to remove the floating ice.  The correction of grounded ice is based on :ref:`Grounded ice correction <Ice_corr>`.
-
-        Attributes
-        ----------
-            topo : :ref:`TOPOGRAPHIC_TIME_GRID <TOPOGRAPHIC_TIME_GRID>` class object
-                A topogrphic grid object, used to check if grounded ice become floating ice. The topography is then modified to by this function. 
-            oc : :ref:`OCEAN_TIME_GRID <OCEAN_TIME_GRID>` class object
-                An oceanic time grid object used only to get the density of ocean set for the model. 
-
-            .. note::
-                To avoid memory consumption the oc parameter should be replace simply by oc_rho the ocean density. 
-                 
-
-        Return
-        ------
-            None
-
-        """
-        for t_it in range(self.time_step_number-1):
-            if t_it==0 :
-                topo.height_time_grid[t_it,:,:]=topo.height_time_grid[t_it,:,:]-self.height_time_grid[t_it,:,:]+self.ice[t_it,:,:]
-            else :
-                topo.height_time_grid[t_it,:,:]=topo.height_time_grid[t_it,:,:]-self.height_time_grid[:t_it+1,:,:].sum(0)+self.ice[:t_it+1,:,:].sum(0)
-        for t_it in range(self.time_step_number-1): 
-            if t_it==0:
-                check1 = OCEAN_TIME_GRID().evaluate_ocean(-topo.height_time_grid[t_it,:,:]+self.ice[t_it,:,:]) # generate the ocean function for ice-topo
-                check2 = OCEAN_TIME_GRID().evaluate_ocean(topo.height_time_grid[t_it,:,:]-self.ice[t_it,:,:]).grd*(OCEAN_TIME_GRID().evaluate_ocean(-self.ice[t_it,:,:]*self.rho-(topo.height_time_grid[t_it,:,:]-self.ice[t_it,:,:])*oc.rho).grd)
-                self.height_time_grid[t_it,:,:] = check1.grd*self.ice[t_it,:,:]+check2*self.ice[t_it,:,:] # add the two part of ice over the check1 nd check2 positive area.
-            else :
-                check1 = OCEAN_TIME_GRID().evaluate_ocean(-topo.height_time_grid[t_it,:,:]+self.ice[:t_it+1,:,:].sum(0)) # generate the ocean function for ice-topo
-                check2 = OCEAN_TIME_GRID().evaluate_ocean(topo.height_time_grid[t_it,:,:]-self.ice[:t_it+1,:,:].sum(0)).grd*(OCEAN_TIME_GRID().evaluate_ocean(-self.ice[:t_it+1,:,:].sum(0)*self.rho-(topo.height_time_grid[t_it,:,:]-self.ice[:t_it+1,:,:].sum(0))*oc.rho).grd)
-                self.height_time_grid[t_it,:,:] = check1.grd*self.ice[:t_it+1,:,:].sum(0)+check2*self.ice[:t_it+1,:,:].sum(0)-self.height_time_grid[:t_it,:,:].sum(0) # add the two part of ice over the check1 nd check2 positive area.
-        for t_it in range(self.time_step_number-1):    
-            if t_it==0 :
-                topo.height_time_grid[t_it,:,:]=topo.height_time_grid[t_it,:,:]+self.height_time_grid[t_it,:,:]-self.ice[t_it,:,:]
-            else :
-                topo.height_time_grid[t_it,:,:]=topo.height_time_grid[t_it,:,:]+self.height_time_grid[:t_it+1,:,:].sum(0)-self.ice[:t_it+1,:,:].sum(0)
-
-    def save(self,save_way=''):
-
-        """
-        .. _ice_save:
-
-        The save method is used to save the data of the ice grid. Because of the `ice_correction`_ method that update the grid we choosed to preserve the original ice thickness data in a ice parameter that is saved inside the nc file. Otherwise this method use the super method :ref:`save` to save the rest of the data.  
-
-        Attributes
-        ----------
-            save_way :str
-                The way where the nc file is saved. Default value is the current file (an empty str).              
-
-        Return
-        ------
-            None
-
-        """
-
-        super().save(save_way,supersave=True)
-        ice=self.ncgrid.createVariable('ice',np.float32,('time_diff','lat','lon'))
-        ice.units='m'
-        ice.long_name='initial_ice_thickness'
-
-        if self.__dict__.keys().__contains__('ice'):
-            ice[:,:,:]=self.ice
-        else :
-            ice[:,:,:]=self.height_time_grid.copy()
-
-        self.ncgrid.close()
-
-class OCEAN_TIME_GRID(TIME_GRID):
-    """
-    The _`OCEAN_TIME_GRID` class is used to represent the ocean thickness variation and contains the method to resolve the sea level equation. This method inherit from :ref:`TIME_GRID <TIME_GRID>`.
-
-    ...
-
-    Attributes
-    ----------
-        time_step : np.array([time_step_number,])
-            This array contains the time step of the data you are importing. They will be use for temporal interpolation.
-        maxdeg : int
-            Maximum harmonic coefficient degree of the data. this define the chape of the grid and coefficient arrays
-        height_time_grid : np.array([maxedg*2,maxdeg])
-            This array is the height grid at each time steps defined in grid_time_step
-        mass_time_grid : np.array([maxedg*2,maxdeg])
-            This array is the mass grid at each time steps defined in grid_time_step
-        height_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
-            This array is the height spherical harmonic coefficient at each time steps defined in grid_time_step
-        mass_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
-            This array is the mass spherical harmonic coefficient at each time steps defined in grid_time_step
-        rho : float
-            The density of the considered layer. Default is 1000 kg/m3.
-        
-        .. note::
-
-            In future development the density may vary threw space and time. We'll have to make a variable object more then a constant density. 
-
-        grid_name : str
-            The name of the grid. We recommand you to choose a specific name for each grid you create. This name is used to save the grid in an nc file with `save`_. 
-        from_file : (bool,way)
-            This parameter define if the data are new or loaded from a previously saved model in a nc file. If the first element is False, the code will create a blank object, based on provided datas. If the first element is True, the method will get the data from the file way specified in the second element of this attribute.
-           
-    Methods
-    -------
-        :ref:`update_0 <update_0_oce>`
-            set the grd_0 from the actual grd loaded in the grid
-        `evaluate_ocean`_
-            evaluate the ocean function based on the Gaussian grid of the topography 
-
-    """
-    def __init__(self,time_step=np.array([1,2]),maxdeg=64,height_time_grid=None,mass_time_grid=None,mass_time_coeff=None,height_time_coeff=None,rho=1000,grid_name='time_grid',from_file=(False,)) :
-        """
-        Parameters
-        ----------
-        """
-        # initialize the ocean with no grid and no coefficient. The saved is also initialized. The volumetric mass of water is set to 1000 
-
-        super().__init__(time_step,maxdeg,height_time_grid,mass_time_grid,height_time_coeff,mass_time_coeff,rho,grid_name,from_file,superinit=True)
-        self.saved=np.array([])
-        if from_file[0] :
-            self.ncgrid.close()
-        
-    def update_0(self):
-        """
-        .. _update_0_oce:
-
-        The update_0 method update the grd_0 parameter of the object to the currend loaded grd. 
-
-        Attributes
-        ----------
-            None
-            
-        Return
-        -------
-            None
-
-        """
-        self.grd_0=self.grd.copy()
-        
-    def evaluate_ocean(self,topo) :
-        '''
-        The _`evaluate_ocean` method evaluate the ocean function using the topography. It create a 0-1 matrix wich is 1 where topo<0 and 0 where topo>0.  The ocean function is described in :ref:`ocean function <oc_func>`.
-    
-        Attribute
-        ---------
-            topo : np.array(maxdeg,maxdegx2)
-                topographic gaussian grid.
-        
-        Returns :
-            None
-
-        '''
-        # use sign function to optimize the conversion from positive negative value to boolean value.
-        out = -0.5*np.sign(topo)+0.5
-        out = 0.5*np.sign(out-0.6)+0.5
-        # set the grd to the output of the previous computation.
-        self.grd=out
-        return self
-    
-    def sea_level_solver(self,load,ice_time_grid,sed_time_grid,love_number,TO,t_it,conv_it,conv_lim):
-        '''
-        The _`sea_level_solver` method solve the sea level equation until. Beacause of the iterative type of the resolution of the SLE, this method define also a first guess of the Sea level at the first iteration and the first time step. This function is based on the convergence iteration for the estimation of the variability defined in :ref:`Convergence parameter <conv>`.
-
-        Attribute
-        ---------
-            load : :ref:`LOAD_TIME_GRID <LOAD_TIME_GRID>` class object
-                The load time grid as specified in the class object. This grid needs to be of the same shape (maxdeg) then the one of the current object. 
-            ice_time_grid : :ref:`ICE_TIME_GRID <ICE_TIME_GRID>` class object
-                The ice time grid as specified in the class object. This grid needs to be of the same shape (maxdeg) then the one of the current object. 
-            sed_time_grid : :ref:`SEDIMENT_TIME_GRID <SEDIMENT_TIME_GRID>` class object
-                The sediment time grid as specified in the class object. This grid needs to be of the same shape (maxdeg) then the one of the current object. 
-            love_number : :ref:`LOVE <LOVE>` class object 
-                The love numbers as specified in the class object. The love numbers must have been set up with the same maximm degree thne the currend object.
-            TO : :ref:`sphericalobject <sphericalobject>` class object
-                The ocean contours variability area computed as a sphericalobject class computed for the previous iteration. !Trouver où définir ce calcul!. 
-            t_it : int
-                The time iteration of the current computation on wich apply the resolution of the SLE.
-            conv_it : int
-                convergence iteration set to 0 if it's for a simple resolution of the SLE on one time step. This is used when you are working on a topographic convergence. In the code, the first guess for the SLE will be if it's not the first topographic convergence iteration, the guess of the previuous one.
-            conv_lim : float
-                To stop the convergence of the solution, the conv_lim is usually set to 10^-3. The number of required step is then between 13 and 7. 
-        Return 
-        ------
-            None 
-
-        '''
-        if conv_it==0 :
-            if t_it==0:
-                self.height_time_coeff[t_it,:]=self.prev/self.prev[0]*(TO.coeff[0]-TO.prev[0])-TO.coeff-TO.prev
-            else :
-                self.height_time_coeff[t_it,:]=self.prev/self.prev[0]*(-ice_time_grid.rho/self.rho*ice_time_grid.height_time_coeff[:t_it+1,:].sum(0) + TO.coeff[0]-TO.prev[0])-TO.coeff-TO.prev
-        chi=np.inf
-        while chi>conv_lim:
-            chi=self.sea_level_equation(load,ice_time_grid,sed_time_grid,love_number,TO,t_it)
-            conv_it+=1
-        #if t_it >1 :
-            #print(load.rot_pot[t_it-1,:],sed_time_grid.height_time_coeff[t_it,:].max())
-        return conv_it
-    
-    def sea_level_equation(self,load,ice_time_grid,sed_time_grid,love_number,TO,t_it):
-        '''
-        The _`sea_level_equation` method calculate the Sea level variation following the SLE. Tis function is resolving both the conservation of mass equation and the SL variation. This follows the method described in :ref:`Resolution of SLE including the deconvolution<spec_sol>`.
-
-        Attribute
-        ---------
-            load : :ref:`LOAD_TIME_GRID <LOAD_TIME_GRID>` class object
-                The load time grid as specified in the class object. This grid needs to be of the same shape (maxdeg) then the one of the current object. 
-            ice_time_grid : :ref:`ICE_TIME_GRID <ICE_TIME_GRID>` class object
-                The ice time grid as specified in the class object. This grid needs to be of the same shape (maxdeg) then the one of the current object. 
-            sed_time_grid : :ref:`SEDIMENT_TIME_GRID <SEDIMENT_TIME_GRID>` class object
-                The sediment time grid as specified in the class object. This grid needs to be of the same shape (maxdeg) then the one of the current object. 
-            love_number : :ref:`LOVE <LOVE>` class object 
-                The love numbers as specified in the class object. The love numbers must have been set up with the same maximm degree thne the currend object.
-            TO : :ref:`sphericalobject <sphericalobject>` class object
-                The ocean contours variability area computed as a sphericalobject class computed for the previous iteration. !Trouver où définir ce calcul!. 
-            t_it : int
-                The time iteration of the current computation on wich apply the resolution of the SLE.
-        Return 
-        ------
-            None 
-            
-        '''
-        if t_it==0 :
-            delSLcurl_fl=love_number.E* love_number.T.coeff *(ice_time_grid.height_time_coeff[0,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[0,:]*sed_time_grid.rho+self.height_time_coeff[0,:]*self.rho)
-            self.delSLcurl=sphericalobject(coeff=delSLcurl_fl - ice_time_grid.height_time_coeff[0,:]- sed_time_grid.height_time_coeff[0,:]).coefftogrd()
-            load.calc_rot_visc(ice_time_grid.height_time_coeff[1:t_it,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[1:t_it,:]*sed_time_grid.rho+self.height_time_coeff[1:t_it,:]*self.rho,0,love_number)
-            RO=sphericalobject(grd=self.delSLcurl.grd*self.grd).grdtocoeff()
-            self.delPhi_g=np.real(1/self.coeff[0] * (- ice_time_grid.rho/self.rho*ice_time_grid.coeff[0] - RO.coeff[0] + TO.coeff[0]))
-            chi = np.abs( (np.sum(np.abs(RO.coeff + self.delPhi_g*self.coeff -  TO.coeff)) - np.sum(np.abs(self.height_time_coeff[t_it,:]))) / np.sum(np.abs(self.height_time_coeff[t_it,:])))
-            self.height_time_coeff[t_it,:]=RO.coeff + self.delPhi_g*self.coeff -  TO.coeff
-        else :
-            
-            if t_it == 1 : 
-                #load.calc_viscuous_load(ice_time_grid.height_time_coeff[0,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[0,:]*sed_time_grid.rho+self.height_time_coeff[0,:]*self.rho,love_number.beta_l,0)
-                load.calc_rot_visc(ice_time_grid.height_time_coeff[1,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[1,:]*sed_time_grid.rho+self.height_time_coeff[1,:]*self.rho,t_it,love_number)
-                load.rot_pot[t_it,:]=load.rot_pot[t_it,:]
-                load.calc_rotational_viscuous(np.zeros(6),love_number.beta_l_tide,0)
-                load.calc_viscuous(np.zeros(ice_time_grid.height_time_coeff[0,:].shape),love_number.beta_l,0)
-
-            else : 
-                load.calc_rot_visc(ice_time_grid.height_time_coeff[1:t_it,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[1:t_it,:]*sed_time_grid.rho+self.height_time_coeff[1:t_it,:]*self.rho,t_it,love_number)
-                load.rot_pot[t_it,:]=load.rot_pot[t_it,:]-load.rot_pot[:t_it,:].sum(0) # calc small variation
-                load.calc_viscuous(ice_time_grid.height_time_coeff[1:t_it,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[1:t_it,:]*sed_time_grid.rho+self.height_time_coeff[1:t_it,:]*self.rho,love_number.beta_l,t_it)
-                load.calc_rotational_viscuous(load.rot_pot[1:t_it,:],love_number.beta_l_tide,t_it)
-            # print(t_it)
-            # print('rot_pot : ',load.rot_pot[:t_it])
-            # print('m : ',load.sdelm[:t_it])
-            # print('I : ', load.sdelI[:t_it])
-            # print('V_lm_T : ', load.V_lm_tide.coeff)
-            delSLcurl_tide_fl=1/load.g*load.V_lm_tide.coeff+1/load.g*love_number.E_T[:6]*load.rot_pot[:t_it,:].sum(0)
-            
-            delSLcurl_fl=love_number.E* love_number.T.coeff *(ice_time_grid.height_time_coeff[1:t_it+1,:].sum(0)*ice_time_grid.rho+sed_time_grid.height_time_coeff[1:t_it+1,:].sum(0)*sed_time_grid.rho+self.height_time_coeff[1:t_it+1,:].sum(0)*self.rho)+love_number.T.coeff*load.V_lm.coeff
-
-            #print(load.V_lm_tide.coeff.shape,load.V_lm.coeff.shape)
-
-            delSLcurl_tide_fl=np.concatenate((delSLcurl_tide_fl,np.zeros(delSLcurl_fl.shape[0]-delSLcurl_tide_fl.shape[0])))
-
-            self.delSLcurl=sphericalobject(coeff=delSLcurl_fl + delSLcurl_tide_fl - ice_time_grid.height_time_coeff[1:t_it+1,:].sum(0)- sed_time_grid.height_time_coeff[1:t_it+1,:].sum(0)).coefftogrd()
-            RO=sphericalobject(grd=self.delSLcurl.grd*self.grd).grdtocoeff()
-            self.delPhi_g=np.real(1/self.coeff[0] * (- ice_time_grid.rho/self.rho*ice_time_grid.height_time_coeff[1:t_it+1,0].sum() - RO.coeff[0] + TO.coeff[0]))
-            #print(t_it,':',self.coeff[0])
-            if t_it==1:
-                chi = np.abs((np.sum(np.abs(RO.coeff + self.delPhi_g*self.coeff -  TO.coeff - self.height_time_coeff[0,:])) - np.sum(np.abs(self.height_time_coeff[t_it,:]))) / np.sum(np.abs(self.height_time_coeff[t_it,:])))
-                self.height_time_coeff[t_it,:]=RO.coeff + self.delPhi_g*self.coeff -  TO.coeff - self.height_time_coeff[0,:]
-            else :
-                chi = np.abs((np.sum(np.abs(RO.coeff + self.delPhi_g*self.coeff -  TO.coeff - self.height_time_coeff[:t_it,:].sum(0))) - np.sum(np.abs(self.height_time_coeff[t_it,:]))) / np.sum(np.abs(self.height_time_coeff[t_it,:])))
-                self.height_time_coeff[t_it,:]=RO.coeff + self.delPhi_g*self.coeff -  TO.coeff - self.height_time_coeff[:t_it,:].sum(0)
-            # print('chi : ',chi)
-        return chi
-
-class TOPOGRAPHIC_TIME_GRID(TIME_GRID):
-    """
-    The _`TOPOGRAPHIC_TIME_GRID` class is used to save and include all the topographic variations. This class inherits of :ref:`TIME_GRID <TIME_GRID>`. This class main difference with TIME_GRID is the presence of a parameter called topo_pres wich is the present topography. It is created using :ref:`Precomputation <Precomputation>`.
-
-    Attributes
-    ----------
-        time_step : np.array([time_step_number,])
-            This array contains the time step of the data you are importing. They will be use for temporal interpolation.
-        maxdeg : int
-            Maximum harmonic coefficient degree of the data. this define the chape of the grid and coefficient arrays
-        height_time_grid : np.array([maxedg*2,maxdeg])
-            This array is the height grid at each time steps defined in grid_time_step
-        mass_time_grid : np.array([maxedg*2,maxdeg])
-            This array is the mass grid at each time steps defined in grid_time_step
-        height_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
-            This array is the height spherical harmonic coefficient at each time steps defined in grid_time_step
-        mass_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
-            This array is the mass spherical harmonic coefficient at each time steps defined in grid_time_step
-        rho : float
-            The density of the considered layer.
-        
-        .. note::
-
-            In future development the density may vary threw space and time. We'll have to make a variable object more then a constant density. 
-
-        grid_name : str
-            The name of the grid. We recommand you to choose a specific name for each grid you create. This name is used to save the grid in an nc file with `save`_. 
-        from_file : (bool,way)
-            This parameter define if the data are new or loaded from a previously saved model in a nc file. If the first element is False, the code will create a blank object, based on provided datas. If the first element is True, the method will get the data from the file way specified in the second element of this attribute.
-
-    Methods
-    -------
-        :ref:`save <topo_save>` 
-            Method to save the topographic datas   
-
-    """
-    def __init__(self,time_step=np.array([1,2]),maxdeg=64,height_time_grid=None,mass_time_grid=None,mass_time_coeff=None,height_time_coeff=None,rho=0,grid_name='time_grid',from_file=(False,)) : 
-        """
-        Parameters
-        ----------
-        """
-        super().__init__(time_step,maxdeg,height_time_grid,mass_time_grid,height_time_coeff,mass_time_coeff,rho,grid_name,from_file,superinit=True)
-        if from_file[0] :
-            self.topo_pres=self.ncgrid['topo_pres'][:].data
-            self.ncgrid.close()
-        
-        # initialize coefficient and grid to 0 because no grid or coefficient has been created
-        # self.isgrd=False
-        # self.iscoeff=False
-        #self.saved=np.array([])
-
-    def save(self,save_way=''):
-        """
-        .. _topo_save:
-
-        The save method is used to save the data of the topographic grid. Particularity of the topography is the present day topography used in the code to converge toward it. The function save is. Otherwise this method use the super method :ref:`save` to save the rest of the data.  
-
-        Attributes
-        ----------
-            save_way :str
-                The way where the nc file is saved. Default value is the current file (an empty str).              
-
-        Return
-        ------
-            None
-
-        """
-        super().save(save_way,supersave=True)
-        topo_pres=self.ncgrid.createVariable('topo_pres',np.float32,('lat','lon'))
-        topo_pres.units='m'
-        topo_pres.long_name='present topography'
-
-        if self.__dict__.keys().__contains__('topo_pres'):
-            topo_pres[:,:]=self.topo_pres
-
-        self.ncgrid.close()
-
-
-from .love import get_tlm
-
-class LOAD_TIME_GRID(TIME_GRID) :
-    """
-    The _`LOAD_TIME_GRID` class is used to save and include all the topographic variations. This class inherits of :ref:`TIME_GRID <TIME_GRID>` and :ref:`LOAD <LOAD>`.
-
-    Attributes
-    ---------- 
-        sdelL : np.array([time_step_number,maxdeg,maxdegx2])
-            The load variation grid used to compute earth vertical motion.
-        betal : np.array([time_step_number,time_step_number,maxdeg])
-            The beta love number as described in :ref:`Variation of geoïd and ground Equations <geoid_ground_variation_theory>` section. There calculated in the :ref:`LOVE <LOVE>` class.
-        E : np.array([(maxdeg+1)(maxdeg+2)/2,])
-            The elastic component of the earth as love numbers computed form :ref:`LOVE <LOVE>` class.
-        a : float
-            The earth radius in meter, set by default to 7371000 meters.
-        Me : float
-            The earth mass in set by default to 5000. 
-        time_step : np.array([time_step_number,])
-            This array contains the time step of the data you are importing. They will be use for temporal interpolation.
-        maxdeg : int
-            Maximum harmonic coefficient degree of the data. this define the chape of the grid and coefficient arrays
-        height_time_grid : np.array([maxedg*2,maxdeg])
-            This array is the height grid at each time steps defined in grid_time_step
-        mass_time_grid : np.array([maxedg*2,maxdeg])
-            This array is the mass grid at each time steps defined in grid_time_step
-        height_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
-            This array is the height spherical harmonic coefficient at each time steps defined in grid_time_step
-        mass_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
-            This array is the mass spherical harmonic coefficient at each time steps defined in grid_time_step
-        rho : float
-            The density of the considered layer.
-        grid_name : str
-            The name of the grid. We recommand you to choose a specific name for each grid you create. This name is used to save the grid in an nc file with `save`_. 
-        from_file : (bool,way)
-            This parameter define if the data are new or loaded from a previously saved model in a nc file. If the first element is False, the code will create a blank object, based on provided datas. If the first element is True, the method will get the data from the file way specified in the second element of this attribute.
-
-    Methods
-    -------
-        `calc_viscuous`_:
-            Compute the viscous motion of the geoïd and ground for one time step.
-        `calc_viscuous_time`_ :
-            Compute the viscous ground motion of the earth on all time steps.    
-        `calc_elastic_time`_ :
-            Compute the elastic ground motion of the earth on all time steps.
-        :ref:`save <load_save>` :
-            Save the load data
-
-    """
-    def __init__(self,sdelL=np.array([]),beta_l=np.array([]),E=np.array([]),E_T=np.array([]),a=7371000,Me=5000,time_step=np.array([1,2]),maxdeg=64,height_time_grid=None,mass_time_grid=None,mass_time_coeff=None,height_time_coeff=None,rho=0,grid_name='time_grid',from_file=(False,),g=9.80665):
-        TIME_GRID.__init__(self,time_step,maxdeg,height_time_grid,mass_time_grid,height_time_coeff,mass_time_coeff,rho,grid_name,from_file,superinit=True)
-        #LOAD.__init__(self,maxdeg,time_step)
-        self.beta_counter=np.repeat(np.arange(0,self.maxdeg),np.arange(1,self.maxdeg+1))
-        if from_file[0]:
-            self.a=self.ncgrid['a'][:].data
-            self.Me=self.ncgrid['Me'][:].data
-            self.viscuous_deformation=self.ncgrid['viscuous_deformation_real'][:].data+self.ncgrid['viscuous_deformation_imag'][:].data*1j
-            self.elastic_deformation=self.ncgrid['elastic_deformation_real'][:].data+self.ncgrid['elastic_deformation_imag'][:].data*1j
-            #self.beta_l=self.ncgrid['beta_l'][:].data
-            self.elastic_love=self.ncgrid['elastic_love'][:].data
-            self.load=self.ncgrid['load_real'][:].data+self.ncgrid['load_imag'][:].data*1j
-        else :
-            self.g=g
-            self.viscuous_deformation=np.zeros((self.time_step_number-2,int(maxdeg*(maxdeg+1)/2)))+0j
-            self.elastic_deformation=np.zeros((self.time_step_number-2,int(maxdeg*(maxdeg+1)/2)))+0j
-            self.load=sdelL[1:,:]
-            self.elastic_love=E[self.beta_counter.astype(int)]
-            self.elastic_tidal_love=E_T
-            self.a=a
-            self.Me=Me
-            self.beta_l=beta_l
-            self.viscuous_love=self.beta_l[:,:,self.beta_counter.astype(int)]
-            self.V_lm=sphericalobject(coeff=np.zeros((int(maxdeg*(maxdeg+1)/2)))+0j)
-            self.V_lm_tide=sphericalobject(coeff=np.zeros((6,))+0j)
-            self.rot_pot=np.zeros((self.time_step_number-1,6))+0j
-            self.sdelI=np.zeros((self.time_step_number-2,3))+0j
-            self.sdelm=np.zeros((self.time_step_number-2,3))+0j
-        self.T = sphericalobject(coeff=get_tlm(self.maxdeg-1,self.a,self.Me))
-
-    def calc_viscuous(self,sdelL,beta,t_it):
-        '''
-        The _`calc_viscuous` method is used to calculate the ground and geoïd deformation based on viscuous love numbers.
-
-        Attribute
-        ---------
-            sdelL : np.array([t_it,(maxdeg+1)(maxdeg+20/2)])
-                The load grid used to estimate the ground vertical mouvement. This include all previous loading history because of the viscous comportment of earth. 
-            beta : np.array([time_step_number,time_step_number,(maxdeg+1)(maxdeg+2)/2])
-                The beta love numbers used to compute the earth deformation to include the viscous part. These love numbers are particularly heavy in the memory due to the representation of the time. 
-            t_it : int
-                The time iteration at wich the computation is performed.
-            
-        '''
-        if t_it==1 :
-            self.V_lm.coeff=np.zeros(beta.shape[2])
-        else :
-            self.V_lm.coeff=(beta[t_it-1,:t_it-1]*sdelL).sum(0)
-
-    def calc_rotational_viscuous(self,rot_pot,beta_tide,t_it):
-        if t_it==1 :
-            self.V_lm_tide.coeff=np.zeros(6)
-        else :
-            self.V_lm_tide.coeff=(beta_tide[t_it-1,:t_it-1]*rot_pot).sum(0)
-
-    def calc_viscuous_time(self,backend=False) :
-        '''
-        The _`calc_viscuous_time` method compute the vicuous vertical ground motion. This method call the :ref:`LOAD <LOAD>` method for this. 
-
-        Attribute
-        ---------
-            backend : bool
-                Specifie if the method give backend (True) or not (False). Default is False.
-
-        Return
-        ------
-            None
-
-        '''
-        for t_it in range(1,self.time_step_number-1):
-            if t_it+1==1 :
-                self.calc_viscuous(np.zeros(self.height_time_coeff[0,:].shape),self.viscuous_love,0)
-            else :
-                self.calc_viscuous(self.load[1:t_it,:],self.viscuous_love,t_it)
-            self.viscuous_deformation[t_it-1,:]=self.T.coeff*np.squeeze(self.V_lm.coeff.T)
-            if backend:
-                print(f'viscuous calculation at {self.time_step[t_it]} kyr done')
-    
-    def calc_elastic_time(self):
-        '''
-        The _`calc_elastic_time` method compute the elactic vertical ground motion. This method call the :ref:`LOAD <LOAD>` method for this. 
-
-        Attribute
-        ---------
-            None
-
-        Return
-        ------
-            None
-             
-        '''
-        self.elastic_deformation=np.repeat(np.expand_dims(self.T.coeff,axis=0),self.time_step_number-2,axis=0)*np.repeat(np.expand_dims(self.elastic_love,axis=0),self.time_step_number-2,axis=0)*self.load
-
-    def save(self,save_way=''):
-        '''
-        .. _load_save:
-
-        The save method is used to save the data from the class. It is based on the inherited :ref:`save <save>` method. Because of the particularity of this TIME_GRID, we had to save the new parameters, and calculated data. This function save for each data the real and complex part of the data due to the nc file particularity. The saved data are, The load (load), the viscuous groud motion (viscous_deformation), the elastic ground motion (elastic_deformation), the elastic love numbers (elastic_love), earth radius (a), earth mass (Me). 
-
-        Attribute
-        ---------
-            save_way : str
-                file path to where the grid will be saved. 
-
-        Return
-        ------
-            None
-             
-        '''
-        super().save(save_way,supersave=True)
-
-        self.ncgrid.createDimension('time_no_init',self.time_step_number-2)
-
-        load_real=self.ncgrid.createVariable('load_real',np.float32,('time_no_init','maxdeg_order'))
-        load_real.units='kg'
-        load_real.long_name='load grid used to compute the earth deformation.'
-        load_real[:,:]=np.real(self.load)
-
-        load_imag=self.ncgrid.createVariable('load_imag',np.float32,('time_no_init','maxdeg_order'))
-        load_imag.units='kg'
-        load_imag.long_name='load grid used to compute the earth deformation.'
-        load_imag[:,:]=np.imag(self.load)
-
-        viscuous_deformation_real=self.ncgrid.createVariable('viscuous_deformation_real',np.float32,('time_no_init','maxdeg_order'))
-        viscuous_deformation_real.units='mm/yr'
-        viscuous_deformation_real.long_name='viscuous component of the earth deformation due to load.'
-        viscuous_deformation_real[:,:]=np.real(self.viscuous_deformation)
-
-        viscuous_deformation_imag=self.ncgrid.createVariable('viscuous_deformation_imag',np.float32,('time_no_init','maxdeg_order'))
-        viscuous_deformation_imag.units='mm/yr'
-        viscuous_deformation_imag.long_name='viscuous component of the earth deformation due to load.'
-        viscuous_deformation_imag[:,:]=np.imag(self.viscuous_deformation)
-
-        elastic_deformation_real=self.ncgrid.createVariable('elastic_deformation_real',np.float32,('time_no_init','maxdeg_order'))
-        elastic_deformation_real.units='mm/yr'
-        elastic_deformation_real.long_name='elastic component of the earth deformation due to load.'
-        elastic_deformation_real[:,:]=np.real(self.elastic_deformation)
-
-        elastic_deformation_imag=self.ncgrid.createVariable('elastic_deformation_imag',np.float32,('time_no_init','maxdeg_order'))
-        elastic_deformation_imag.units='mm/yr'
-        elastic_deformation_imag.long_name='elastic component of the earth deformation due to load.'
-        elastic_deformation_imag[:,:]=np.imag(self.elastic_deformation)
-
-        elastic_love=self.ncgrid.createVariable('elastic_love',np.float32,('maxdeg_order'))
-        elastic_love.units='none'
-        elastic_love.long_name='elastic load love numbers used to compute the earth deformation'
-        elastic_love[:]=self.elastic_love
-
-        # beta_l=self.ncgrid.createVariable('beta_l',np.float32,('time_diff','time_diff','maxdeg'))
-        # beta_l.units='none'
-        # beta_l.long_name='viscuous load love numbers used to compute the earth deformation'
-        # beta_l[:,:]=self.beta_l
-
-        a=self.ncgrid.createVariable('a',np.float32)
-        a.units='m'
-        a.long_name='earth radius'
-        a=self.a
-
-        Me=self.ncgrid.createVariable('Me',np.float32)
-        Me.units='kg'
-        Me.long_name='earth mass'
-        Me=self.Me
-
-        self.ncgrid.close()
-
-    def clean_memory(self):
-        '''
-        This method is used to clean the memory to avoïd over charging RAM. 
-        '''
-        self.viscuous_love=0
-
-    def calc_rot_visc(self,sdelL,t_it,love_number,G=6.67408E-11,a=6371000,C=8.034e37,k_f=0.942,omega=7.292E-5):
-        '''
-        .. note::
-            This function must be updated to work with the new versions of the code.
-
-        '''
-        # extract degree 2 coefficient from the load
-        CminA = (k_f*(a**5)*(omega)**2)/(3*G)
-
-        if t_it==1 :
-            L00 = sdelL[0]
-            L20 = sdelL[3]
-            L21 = sdelL[4]
-        else :
-            L00 = sdelL[:,0].sum(0)
-            L20 = sdelL[:,3].sum(0)
-            L21 = sdelL[:,4].sum(0)
-
-        # calculate the load effect constant 
-        I1=math.sqrt(32/15)*math.pi*a**4*np.real(L21)
-        I2=math.sqrt(32/15)*math.pi*a**4*np.imag(L21)   
-        I3=8/3*math.pi*a**4*(L00-L20/math.sqrt(5))
-        I=np.array([I1,I2,I3])
-        if t_it==1 :
-            V_lm=np.zeros(3)
-            V_lm_T=np.zeros(3)
-        if t_it==2 :
-            V_lm = love_number.beta_konly_l[t_it-2,:t_it-1]*self.sdelI[:t_it-1,:].squeeze()
-            V_lm_T = love_number.beta_konly_l_tide[t_it-2,:t_it-1]*self.sdelm[:t_it-1,:].squeeze()
-        else : #apply the visco elastic properties of the earth on the rotation using the load.
-            V_lm = np.dot(love_number.beta_konly_l[t_it-2,:t_it-1],self.sdelI[:t_it-1,:].squeeze())
-            V_lm_T = np.dot(love_number.beta_konly_l_tide[t_it-2,:t_it-1],self.sdelm[:t_it-1,:].squeeze())
-        
-        temp = 1/(1-love_number.k_tide_e[1]/k_f)*(1/CminA * ((1+love_number.k_e[1])*I + V_lm.squeeze()) + V_lm_T.squeeze()/k_f)
-        # calculate the perturbation to the rotational potential from Milne 1998
-        m1=temp[0]
-        m2=temp[1]
-        temp = -1/(1-love_number.k_tide_e[1]/k_f)*(1/C * ((1+love_number.k_e[1])*I + V_lm.squeeze()))
-        m3=temp[2]
-
-        m=np.array([m1,m2,m3])
-        # print(t_it)
-        # print('L : ', sdelL)
-        # print('L : ', L00,L20,L21)
-        # print('temp : ',(1/CminA * ((1+love_number.k_e[1])*I + V_lm.squeeze()) + V_lm_T.squeeze()/k_f))
-        # print('CminA : ',CminA)
-        # print(t_it)
-        # print('V_lm : ',V_lm)
-        # print('V_lm_T : ', V_lm_T)
-        # print('I : ',I)
-        # print('m : ',m)
-        #update the rotational load using.
-        #print(self.sdelI[:t_it-1,:].sum(0),self.sdelI[:t_it-1,:].sum(0).shape,I.T.squeeze(),I.T.squeeze().shape,self.sdelI[t_it-1,:],self.sdelI[t_it-1,:].shape)
-        self.sdelI[t_it-1,:] = I.T.squeeze() - self.sdelI[:t_it-2,:].sum(0)
-        self.sdelm[t_it-1,:] = m.T.squeeze() - self.sdelm[:t_it-2,:].sum(0)
-
-        #print('m : ',self.sdelm[t_it-1,:])
-        # calculate the rotational perturbation of the earth potential, just for the 6 first coefficient (no use to calculate further)
-        self.rot_pot[t_it-1,0] = a**2 * omega**2/3 * (np.sum(m**2) + 2*m3)+0j
-        self.rot_pot[t_it-1,3] = a**2 * omega**2/(6*np.sqrt(5)) * (m1**2 + m2**2 - 2*m3**2 - 4*m3)+1j*0
-        self.rot_pot[t_it-1,4] = a**2 * omega**2/np.sqrt(30) * (m1*(1+m3) - 1j*m2*(1+m3))+1j*0
-        self.rot_pot[t_it-1,5] = a**2 * omega**2/(np.sqrt(5) * np.sqrt(24)) * ( (m2**2-m1**2) + 1j*2*m1*m2 )+1j*0
-        
+import numpy as np
+import math
+from .spharm import sphericalobject
+import matplotlib.pyplot as plt
+from matplotlib import cm
+import matplotlib as mpl
+import stripy
+from netCDF4 import Dataset
+import pyshtools as pysh
+from .Load import LOAD
+import math
+
+from scipy import io
+
+def sph2cart(az, el, r):
+    rsin_theta = r * np.sin(el)
+    x = rsin_theta * np.cos(az)
+    y = rsin_theta * np.sin(az)
+    z = r * np.cos(el)
+    return x, y, z
+
+class GRID(object):
+        """
+        The class _`GRID` is used to represent the Gaussian Grid.
+
+        Attributes
+        ----------
+
+            .. note::
+
+                This grid have no attribute * this might be changed in future version to be used as stand alone. The absence of attribute is the result of the use of this function in :ref:`TIME_GRID <TIME_GRID>` that use that define all parameters used in the init function of GRID.
+
+        Methods
+        -------
+            `interp_on`_ : 
+                method used to interpolate the grid over the model grid.
+            `smooth_on`_ : 
+                method used to smooth the grid to reduce noise effect.
+            `disk`_ : 
+                method used to create a disk of certain shape to test parameters.
+                     
+
+        """
+        def __init__(self):
+            self.nlons = (self.maxdeg) * 2 
+            self.nlats = (self.maxdeg)
+            x,w=pysh.expand.SHGLQ(self.maxdeg-1)
+            x_GL = np.arccos(x[::-1])*180/math.pi - 90
+            lon_GL = np.linspace(0,360,2*self.maxdeg+1)
+            lon_GL = lon_GL[:-1]
+            self.lats=x_GL
+            self.elons=lon_GL
+            self.colats = 90 - self.lats
+            #self.elons,self.lats=np.meshgrid(self.elons,self.lats)
+        
+        # def add_time(self,time_step):
+        #     '''
+            
+        #     This function add time field to the object.
+        
+        # Parameters :  
+        #     time_step (np.array): a vector array of length number of time step.
+             
+        # See the documentation of the cited class object for more information on different parameters used in the function.
+        
+        # Returns :
+            
+        # Added fields : 
+        #     time_step (np.array): an array of each time step of length number of time step.
+        
+        #     '''
+        #     self.time_step=time_step # à ajouter dans ice grid definition
+            
+        def interp_on(self,grd,lon,lat,smoothing=False,grid_type='global',error=False):
+            '''
+            The method _`interp_on` interpolate a grid of data on the grid of the model calculated in the init function of `GRID`_. This function is using stripy library to pursue the interpolation (`Stripy library <https://underworldcode.github.io/stripy/2.0.5b2/FrontPage.html>`_).
+        
+            Attribute
+            --------- 
+                grd : np.array([m,n])
+                    The grid data over space.
+                lon : np.array([m,])
+                    The longitude of the data.
+                lat : np.array([n,])
+                    The latitude of the data.   
+                smoothing : bool
+                    If a smoothing is applied to the grid before the interpolation, see `smooth_on`_.
+                grid_type : str
+                    grid type define if it's a grid over the whole world or over a small area. This is used to avoid long computation for the interpolation in the case of interpolating small areas over the world. There is two possible 'global' and 'local'. The global interpolation is using `stripy.sTriangulaion <https://underworldcode.github.io/stripy/2.0.5b2/SphericalMeshing/SphericalTriangulations/Ex3-Interpolation.html>`_. The local interpolation is using `stripyt.Triangulation <https://underworldcode.github.io/stripy/2.0.5b2/SphericalMeshing/CartesianTriangulations/Ex3-Interpolation.html>`_.        
+                error : bool
+                    If true, the method return the error of the interpolation calculated by stripy.
+                
+            Return
+            ------
+                grd : np.array([maxdeg*2,maxdeg])
+                    The grid interpolated on the model grid.
+            '''
+            if grid_type=='global':
+                lon,lat=np.meshgrid(lon,lat)
+                vertices_lat=np.radians(lat.flatten())
+                vertices_lon=np.radians(lon.flatten())
+                spherical_triangulation = stripy.sTriangulation(lons=vertices_lon, lats=vertices_lat,refinement_levels=0,permute=True)
+                if smoothing :
+                    grd,dds,err=spherical_triangulation.smoothing(grd.flatten(),np.ones_like(grd.flatten()),0.1,0.1,0.01)
+                elons,lats=np.meshgrid(self.elons,self.lats)
+                vertices_lats=np.radians(lats.flatten())
+                vertices_elons=np.radians(elons.flatten())
+                grd,err=spherical_triangulation.interpolate_nearest(vertices_elons,vertices_lats,data=grd.flatten())
+                grd[np.isnan(grd)]=0
+            elif grid_type=='local':
+                # Select the points inside the local studied zone.
+                spherical_triangulation = stripy.Triangulation(x=lon, y=lat,permute=True)
+                if smoothing :
+                    grd,dds,err=spherical_triangulation.smoothing(grd,np.ones_like(grd),0.1,0.1,0.01)
+                elons,lats=np.meshgrid(self.elons,self.lats)
+                lats=lats.flatten()
+                elons=elons.flatten()
+                point_in=((elons>lon.min())*(elons<lon.max()))*((lats>lat.min())*(lats<lat.max()))
+                elons_in=elons[point_in]
+                lats_in=lats[point_in]
+                grd_in,err=spherical_triangulation.interpolate_nearest(elons_in,lats_in,grd)
+                # I need to complete the grid where the is no data
+                grd=np.zeros(elons.shape)
+                grd[point_in]=grd_in
+            else:
+                print('No such grid type, please select one between : regular or samples')
+            if error : 
+                return grd.reshape((self.nlats,self.nlons)), err.reshape((self.nlats,self.nlons))
+            return grd.reshape((self.nlats,self.nlons))
+        
+        def smooth_on(self,grd,lon,lat):
+
+            '''
+            The method _`smooth_on` is smoothing the grid over the area whith `smoothing <https://underworldcode.github.io/stripy/2.0.5b2/SphericalMeshing/CartesianTriangulations/Ex5-Smoothing.html>`_. This function can be used to correct values before the interpolation over time and space. This way, you can have better results on topographic convergence.
+
+            Attribute
+            ---------
+                grd : np.array([m,n])
+                    Array containig the grid values over the space.
+                lat : nparray([n,])
+                    latitude.
+                lon : nparray([m,])
+                    longitude.
+            
+            Return
+            ------
+                grd : np.array([m,n])
+                    smoothed array with the same shape then the initial grid.
+            '''
+
+            lon,lat=np.meshgrid(lon,lat)
+            vertices_lat=np.radians(lat.ravel())
+            vertices_lon=np.radians(lon.ravel())
+            spherical_triangulation = stripy.sTriangulation(lons=vertices_lon, lats=vertices_lat,refinement_levels=0)
+            grd,dds,err=spherical_triangulation.smoothing(grd.flatten(),np.ones_like(grd.flatten()),10,0.1,0.01)
+            elons,lats=np.meshgrid(self.elons,self.lats)
+            vertices_lats=np.radians(lats.ravel())
+            vertices_elons=np.radians(elons.ravel())
+            grd,err=spherical_triangulation.interpolate_nearest(vertices_elons,vertices_lats,data=grd.flatten())
+            grd[np.isnan(grd)]=0
+            grd=grd.reshape(elons.shape)
+            return grd
+
+        def disk(self,lat,lon,radius,high,tx=1):
+            '''
+            _`disk` is a method used to create a thickness grid. This grid can be used to test different parameters.
+
+            Attribute
+            ---------
+                lat : nparray([1,])
+                    Array contaning the latitudinal coordinate in degree of the center of the disk.
+                lon : nparray(1,[])
+                    Array containing the longitudinal coordinate in degree of the center of the disk.
+                radius : double
+                    The radius in degree of the disk in degree.
+                high : double
+                    The thickness in meter of the disk over the considered area.
+            
+            Return
+            ------
+                grd : np.array([maxdeg*2,maxdeg])
+                    The grid as defined by the `GRID`_ class with a disk of thikness high at lon,lat position with the size of radius.
+        
+            '''
+
+            grd=np.zeros((tx,self.lats.size,self.elons.size))
+            lon_g,lat_g=np.meshgrid(self.elons,self.lats)
+            grd[:,((lon-lon_g)**2+(lat-lat_g)**2)<radius]=high
+            grd[:,:2,:]=grd[:,:2,:]*0
+            return grd
+
+        def zeros(self,tx=1):
+            '''
+            _`zeros` is a method used to generate a zero array with the caracteristics of the grid. 
+            
+            Attribute : 
+            -----------
+                tx : int
+                    times the thickness is repeated
+
+            Return :
+            --------
+                np.zeros((tx,self.lats.size,self.elons.size))
+                    An array containing only zeros 
+            '''
+            return np.zeros((tx,self.lats.size,self.elons.size))
+        
+        def along_transect(self,coord=('lat_start','lon_start','lat_stop','lon_stop'),point_density=None,point_distance=None):
+            if not(point_density is None):
+                theta=np.linspace(coord[0],coord[2],point_density)
+                phi=np.linspace(coord[1],coord[3],point_density)
+            if not(point_distance is None):
+                theta=np.arange(coord[0],coord[2],point_distance)
+                phi=np.arange(coord[1],coord[3],point_distance)
+            i=0
+            Y_lm=np.expand_dims(pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[0]+pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[1]*1j,axis=1)
+            
+            for i in range(1,len(phi)):
+                Y_lm=np.concatenate((Y_lm,np.expand_dims((pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[0]+pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[1]*1j),axis=1)),axis=1)
+            return (Y_lm*np.repeat(np.expand_dims(self.coeff,axis=1),point_density,axis=1)).sum(0)
+
+class TIME_GRID(GRID,sphericalobject):
+    """
+    The _`TIME_GRID` class is used to manage the mass grids. These grids have a time dimenssion this way wa can manage the time variation of the mass. We can define the mass grid by it's mass directly or by coupling a height with a density. If needed you can load spherical harmonics coefficient.Tis class is inheriting the methods from :ref:`sphericalobject <sphericalobject>` and :ref:`GRID <GRID>`. 
+
+    Attributes
+    ----------
+        time_step : np.array([time_step_number,])
+            This array contains the time step of the data you are importing. They will be use for temporal interpolation.
+        maxdeg : int
+            Maximum harmonic coefficient degree of the data. this define the chape of the grid and coefficient arrays
+        height_time_grid : np.array([maxedg*2,maxdeg])
+            This array is the height grid at each time steps defined in grid_time_step
+        mass_time_grid : np.array([maxedg*2,maxdeg])
+            This array is the mass grid at each time steps defined in grid_time_step
+        height_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
+            This array is the height spherical harmonic coefficient at each time steps defined in grid_time_step
+        mass_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
+            This array is the mass spherical harmonic coefficient at each time steps defined in grid_time_step
+        rho : float
+            The density of the considered layer. 
+        
+        .. note::
+
+            In future development the density may vary threw space and time. We'll have to make a variable object more then a constant density. 
+
+        grid_name : str
+            The name of the grid. We recommand you to choose a specific name for each grid you create. This name is used to save the grid in an nc file with `save`_. 
+        from_file : (bool,way)
+            This parameter define if the data are new or loaded from a previously saved model in a nc file. If the first element is False, the code will create a blank object, based on provided datas. If the first element is True, the method will get the data from the file way specified in the second element of this attribute.
+        superinit : bool
+            This parameter is used to specify if the object is used as herited method in an initialisation of a child class object.
+    
+    Methods
+    -------
+        `interp_on_time`_ 
+            Interpolate a grid over the time considered in the model  
+        `interp_on_time_and_space`_ :
+            Interpolate the grid over time and space as in the defined Grid during the initialisation of the class
+        `grid_from_step`_ :
+            Get the grid for a defined time iteration
+        `coeff_from_step`_ :
+            Get the spherical harmonics coefficient for a defined time iteration
+        `timegrdtotimecoeff`_ :
+            Convert the grid into spherical harmonics coefficient for all time steps
+        `timecoefftotimegrd`_ :
+            Convert the spherical harmonics coefficient into grid for all time steps
+        `zeros_time`_ :
+            Generate a zero grid for all time steps
+        `disk_time`_ :
+            Generate a disk of a specified thickness at a specified location over all time steps
+        `update_0`_ :
+            Update the 0 time step data of the grid
+        `save`_ :
+            Save the grid in a specified nc file with the name of the grid
+
+    """
+
+    def __init__(self,time_step=np.array([1,2]),maxdeg=64,height_time_grid=None,mass_time_grid=None,mass_time_coeff=None,height_time_coeff=None,rho=0,grid_name='time_grid',from_file=(False,),superinit=False):
+        if not(from_file[0]) :
+            self.maxdeg=maxdeg
+            super().__init__()
+            self.isgrd=False
+            self.iscoeff=False
+
+
+            self.time_grid_name=grid_name
+
+            self.saved=np.array([]) # initialize the save of the spherical harmonic object
+
+            self.rho=rho
+
+            self.time_step=time_step
+            self.time_step_number=len(time_step)
+
+            self.height_time_grid=np.zeros((self.time_step_number-1,self.nlats,self.nlons))
+            self.mass_time_grid=np.zeros((self.time_step_number-1,self.nlats,self.nlons))
+            self.height_time_coeff=np.zeros((self.time_step_number-1,int(maxdeg*(maxdeg+1)/2)))+0j
+            self.mass_time_coeff=np.zeros((self.time_step_number-1,int(maxdeg*(maxdeg+1)/2)))+0j
+
+            if not(height_time_grid is None):
+                self.height_time_grid=height_time_grid
+                self.mass_time_grid=height_time_grid*rho
+                self.grd_0=self.mass_time_grid[0,:,:]
+            elif not(mass_time_grid is None):
+                self.mass_time_grid=mass_time_grid
+                self.grd_0=self.mass_time_grid[0,:,:]
+            elif not(height_time_coeff is None):
+                self.height_time_coeff=height_time_coeff
+                self.mass_time_coeff=height_time_coeff*rho
+                self.coeff_0=self.mass_time_coeff[0,:]
+            elif not(mass_time_coeff is None):
+                self.mass_time_coeff=mass_time_coeff
+                self.coeff_0=self.mass_time_coeff[0,:]
+
+        elif from_file[0] :
+            self.ncgrid = Dataset(from_file[1]+'.nc',mode='r',format='NETCDF4_CLASSIC') 
+            self.time_grid_name=self.ncgrid.title
+            self.maxdeg=len(self.ncgrid['lat'][:].data)
+            super().__init__()
+
+            self.time_step=self.ncgrid['time'][:].data
+            self.time_step_number=len(self.time_step)
+            self.maxdeg=self.ncgrid.dimensions['maxdeg'].size
+
+            self.rho=self.ncgrid['rho'][:].data
+
+            self.height_time_grid=self.ncgrid['thickness'][:].data
+            self.mass_time_grid=np.zeros((self.time_step_number,self.nlats,self.nlons))
+            self.height_time_coeff=self.ncgrid['coeff_real'][:].data+self.ncgrid['coeff_imag'][:].data*1j
+            self.mass_time_coeff=np.zeros((self.time_step_number,int(self.maxdeg*(self.maxdeg+1)/2)))+0j
+
+            self.mass_time_grid=self.height_time_grid*rho
+
+            if not(superinit):
+                self.ncgrid.close()
+
+    def interp_on_time(self,grid_to_interp,grid_time_step,model_time_step,interp_type='Thickness_divide',backend='False',grid_type='regular'):
+        """
+        The function _`interp_on_time` is used for interpolation upon time and space it call the interpolation function of the :ref:`GRID <GRID>` parameter. This function adapt the order of time and space interpolation to reduce computation time. The temporal interpolation try to preserve the thickness of the overall time. Tis is down by cutting and merging time steps of the original grid to match the model time_step. 
+
+        Attributes
+        ----------
+            grid_to_interp : np.array([k,n,m])
+                The grid to be interpreted.
+            grid_time_step : np.array([k,])
+                The time value of each time step of the grid model.
+            model_time_step ; np.array([time_step_number,])
+                The time values of the model.
+            interp_type : str
+                No use of this parameter anymore
+            backend : bool 
+                Define if the function retur, backends. True it will return the backends, False (default value) don't give any backend. 
+        
+        Return :
+        --------
+            grid_interpolated : np.array([time_step_number,n,m])
+                The interpolated grid over time. Depending of the model parameters. 
+        """
+
+        if interp_type=="Thickness_divide":
+            grid_time_step=grid_time_step[::-1]
+            model_time_step=model_time_step[::-1]
+            if grid_type=='global':
+                grid_to_interp=grid_to_interp[::-1,:,:]
+                d_grid_time_step=np.diff(grid_time_step)
+                d_grid_to_interp=grid_to_interp/d_grid_time_step[:,np.newaxis,np.newaxis]
+
+                Merge_time_step=np.unique(np.concatenate((grid_time_step,model_time_step)), return_index=True)
+                Merge_time_step=(Merge_time_step[0],Merge_time_step[1]+1)
+                Merge_time_step[1][Merge_time_step[1]>len(grid_time_step)]=0
+
+                out=len(model_time_step[model_time_step>grid_time_step.max()])
+
+                count=np.diff(np.nonzero(Merge_time_step[1])).squeeze()
+                to_merge=np.searchsorted(Merge_time_step[0],grid_time_step[np.isin(grid_time_step,model_time_step,invert=True)].squeeze())-1
+                grd_interpolated=np.zeros((len(Merge_time_step[0])-1,d_grid_to_interp.shape[1],d_grid_to_interp.shape[2]))
+                #print(np.concatenate((d_grid_to_interp.repeat(count,axis=0),np.zeros((out,d_grid_to_interp.shape[1],d_grid_to_interp.shape[2])))).shape)
+                grd_interpolated=np.array(np.concatenate((d_grid_to_interp.repeat(count,axis=0),np.zeros((out,d_grid_to_interp.shape[1],d_grid_to_interp.shape[2]))))*np.diff(Merge_time_step[0])[:,np.newaxis,np.newaxis])
+
+                for i in range(len(to_merge)):
+                    if backend :
+                        print('time slicing : ' + str(i))
+                    grd_interpolated[to_merge[i]-1,:,:]+=grd_interpolated[to_merge[i],:,:]
+                    grd_interpolated=np.delete(grd_interpolated,to_merge[i],0)
+                    to_merge-=1
+                return grd_interpolated[::-1,:,:]
+            elif grid_type=='local':
+                grid_to_interp=grid_to_interp[::-1,:]
+                d_grid_time_step=np.diff(grid_time_step)
+                d_grid_to_interp=grid_to_interp/d_grid_time_step[:,np.newaxis]
+
+                Merge_time_step=np.unique(np.concatenate((grid_time_step,model_time_step)), return_index=True)
+                Merge_time_step=(Merge_time_step[0],Merge_time_step[1]+1)
+                Merge_time_step[1][Merge_time_step[1]>len(grid_time_step)]=0
+
+                out=len(model_time_step[model_time_step>grid_time_step.max()])
+
+
+                count=np.diff(np.nonzero(Merge_time_step[1])).squeeze()
+                to_merge=np.searchsorted(Merge_time_step[0],grid_time_step[np.isin(grid_time_step,model_time_step,invert=True)].squeeze())-1
+                grd_interpolated=np.zeros((len(Merge_time_step[0])-1,d_grid_to_interp.shape[1]))
+                grd_interpolated=np.array(np.concatenate((d_grid_to_interp.repeat(count,axis=0),np.zeros((out,d_grid_to_interp.shape[1]))))*np.diff(Merge_time_step[0])[:,np.newaxis])
+                print(type(to_merge))
+                if type(to_merge) is 'np.array' :
+                    for i in range(len(to_merge)):
+                        if backend :
+                            print('time slicing : ' + str(i))
+                        grd_interpolated[to_merge[i]-1,:]+=grd_interpolated[to_merge[i],:]
+                        grd_interpolated=np.delete(grd_interpolated,to_merge[i],0)
+                        to_merge-=1
+                else :
+                    if backend :
+                        print('time slicing : ' + str(0))
+                    grd_interpolated[to_merge-1,:]+=grd_interpolated[to_merge,:]
+                    grd_interpolated=np.delete(grd_interpolated,to_merge,0)
+                    to_merge-=1
+                return grd_interpolated[::-1,:]
+            else :
+                print('no such grid type avaiable. try local or global')
+
+    def interp_on_time_and_space(self,grid_to_interp,grid_time_step,grid_lon,grid_lat,interp_type='Thickness_divide',backend=False,grid_type='global'):
+        """
+        The _`interp_on_time_and_space` function is used for interpolation upon time and space it call the interpolation function of the :ref:`GRID <GRID>` parameter. This function perform the temporal and spatial interpolation in different order to ameliorate the computation time. If the temporal resolution of the input grid is higher than the model time resolution the temporal resolution will be perform first. The spatial resolution is performed first in the other case.
+
+        Attributes
+        ----------
+            grid_to_interp : np.array([k,n,m])
+                The grid to be interpreted.
+            grid_time_step : np.array([k,])
+                The time value of each time step of the grid_to_interp.
+            grid_lon : np.array([n])
+                The longitudinal coordinates of the grid_to_interp.
+            grid_lat : np.array([m])
+                The latitudinal coordinate of the grid_to_interp.
+            interp_type : str
+                No use of this parameter anymore
+            backend : bool 
+                Define if the function retur, backends. True it will return the backends, False (default value) don't give any backend. 
+        
+        Return :
+        --------
+            grid_interpolated : np.array([time_step_number,maxdeg*2,maxdeg])
+                The interpolated grid over time. Depending of the model parameters. 
+        """
+        if len(grid_time_step)<self.time_step_number:
+            time_grid_pre_interp=np.zeros((len(grid_time_step)-1,self.nlats,self.nlons))
+            for i in range(len(grid_time_step)-1):
+                if backend :
+                    print('interpolation number : ' + str(i))
+
+                time_grid_pre_interp[i,:,:]=self.interp_on(grid_to_interp[i],grid_lon,grid_lat,grid_type=grid_type)
+            grid_type='global'
+            self.height_time_grid=self.interp_on_time(time_grid_pre_interp,grid_time_step,self.time_step,interp_type,backend=backend,grid_type=grid_type)
+        else :
+            grd_to_interpolate=self.interp_on_time(grid_to_interp,grid_time_step,self.time_step,interp_type,backend=backend,grid_type=grid_type)
+            for i in range(self.time_step_number-1):
+                if backend :
+                    print('interpolation number : ' + str(i))
+                self.height_time_grid[i,:,:]=self.interp_on(grd_to_interpolate[i,:],grid_lon,grid_lat,grid_type=grid_type)
+
+    
+    def grid_from_step(self,t_it):
+        """
+        The _`grid_from_step` method is used to get the value of the grid at the defined time step.
+        
+        Attributes :
+        ------------
+            t_it : int
+                This is the value of the time step iteration on wich you are trying to retreave the grid. It must inside the time_step interpolation you have used during the initialisation of the time grid. 
+        
+        Return :
+        --------
+            None
+        """
+        # if not(self.mass_time_grid is None) :
+        #     self.grd=self.mass_time_grid[t_it,:,:]
+        # elif not(self.height_time_grid is None):
+        self.grd=self.height_time_grid[t_it,:,:].copy()
+        return self
+
+    def coeff_from_step(self,t_it):
+        """
+        The _`coeff_from_step` method is used to get the value of the coefficient at the requested time iteration.
+        
+        Attributes :
+        ------------
+            t_it : double
+                This is the value of the time step iteration on wich you are trying to retreave the coefficient. It must be inside the time_step interpolation you have used during the initialisation of the time grid.
+
+        Return :
+        --------
+            None
+        """
+        # if not(self.mass_time_coeff is None) :
+        #     self.coeff=self.mass_time_coeff[t_it,:]
+        # elif not(self.height_time_coeff is None):
+        self.coeff=self.height_time_coeff[t_it,:].copy()
+        return self
+    
+    def timegrdtotimecoeff(self):
+        """
+        The _`timegrdtotimecoeff` method transform for each time step the grid into spherical harmonics coefficient. 
+
+        Attribute :
+        -----------
+            None
+        
+        Result :
+        --------
+            None
+
+        """
+        for i in range(self.time_step_number-1):
+            self.grd=self.height_time_grid[i,:,:]
+            self.height_time_coeff[i,:]=self.grdtocoeff().coeff
+        return self
+    
+    def timecoefftotimegrd(self):
+        """
+        The _`timecoefftotimegrd` method transform for each time step the spherical harmonic coefficient into a grid. 
+
+        Attribute :
+        -----------
+            None
+        
+        Result :
+        --------
+            None
+        """
+        for i in range(self.time_step_number-1):
+            self.coeff=self.height_time_coeff[i,:]
+            self.height_time_grid[i,:,:]=self.coefftogrd().grd
+        return self
+    
+    def zeros_time(self,time_step_number):
+        """
+        The _`zeros_time` method is used to define a grid over time with only 0 value. It is based on :ref:`GRID.zeros <zeros>`. 
+
+        Attribute :
+        -----------
+            time_step_number : int
+                The number of time step on wich we apply the zeros grid.
+        
+        Return :
+        --------
+            None
+        """
+        self.height_time_grid=self.zeros(time_step_number)
+    
+    def disk_time(self,time_step_number,lat,lon,radius,high):
+        """
+        The _`disk_time` method is used to define a grid over time with a disk defined with it's center coordinate and the height. This function is based on :ref:`GRID.disk <disk>`.
+
+        Attribute :
+        -----------
+            time_step_number : int
+                The number of time step on wich the disk load will be applyed.
+            lat : double
+                The latitude of the center of the disk (°).
+            lon : double
+                The longitude of the center of the disk (°).
+            radius : double
+                The radius of the disk (°).
+            high : double
+                The high of the disk (m).
+        Return :
+        --------
+            None
+        """
+        self.height_time_grid=self.disk(lat,lon,radius,high,time_step_number)
+    
+    def update_0(self):
+        """
+        The _`update_0` function is used to save the first time iteration of the object before it's modification to be called at any moment in the code without alteration.
+
+        Attribute :
+        -----------
+            None
+        Return :
+        --------
+            None
+
+        """
+        if not(self.height_time_grid is None) :
+            self.grd_0=self.height_time_grid[0,:,:].copy()
+        if not(self.height_time_coeff is None) :
+            self.coeff_0=self.height_time_coeff[0,:].copy()
+
+    def plot_step_on_sphere(self,time_step,cmap=cm.inferno,vmin=None,vmax=None,clip=False,inverse=False):
+        colormap=cmap
+        if vmin==None and vmax==None :
+            normaliser = mpl.colors.Normalize(vmin=np.min(self.height_time_grid[time_step,:,:]), vmax=np.max(self.height_time_grid[time_step,:,:]),clip=clip)
+        elif vmax==None and not(vmin==None):
+            normaliser = mpl.colors.Normalize(vmin=vmin, vmax=np.max(self.height_time_grid[time_step,:,:]),clip=clip)
+        elif vmin==None and not(vmax==None):
+            normaliser = mpl.colors.Normalize(vmin=np.min(self.height_time_grid[time_step,:,:]), vmax=vmax,clip=clip)
+        if inverse:
+            normaliser.inverse()
+        
+        elons,lats=np.meshgrid(self.elons,self.lats)
+        
+        u=elons/360*2*math.pi
+        v=(lats+90)/180*math.pi
+        x,y,z=sph2cart(u.flatten(),v.flatten(),np.ones((u.flatten().shape)))
+        fig = plt.figure()
+        ax = fig.add_subplot(111, projection="3d")
+        ax.plot_surface(np.reshape(x,(self.lats.shape[0],self.elons.shape[0])),np.reshape(y,(self.lats.shape[0],self.elons.shape[0])),np.reshape(z,(self.lats.shape[0],self.elons.shape[0])),facecolors=colormap(normaliser(self.height_time_grid[time_step,:,:])),cmap=colormap)
+        ax.set_aspect('equal')
+
+    def scatter_step_on_sphere(self,time_step,cmap=cm.inferno,vmin=None,vmax=None,clip=False,inverse=False,marker='.',s=0.2):
+        colormap=cmap
+        if vmin==None and vmax==None :
+            normaliser = mpl.colors.Normalize(vmin=np.min(self.height_time_grid[time_step,:,:]), vmax=np.max(self.height_time_grid[time_step,:,:]),clip=clip)
+        elif vmax==None and not(vmin==None):
+            normaliser = mpl.colors.Normalize(vmin=vmin, vmax=np.max(self.height_time_grid[time_step,:,:]),clip=clip)
+        elif vmin==None and not(vmax==None):
+            normaliser = mpl.colors.Normalize(vmin=np.min(self.height_time_grid[time_step,:,:]), vmax=vmax,clip=clip)
+        if inverse:
+            normaliser.inverse()
+
+        elons,lats=np.meshgrid(self.elons,self.lats)
+        
+        u=elons/360*2*math.pi
+        v=(lats+90)/180*math.pi
+        x,y,z=sph2cart(u.flatten(),v.flatten(),np.ones((u.flatten().shape)))
+        fig = plt.figure()
+        ax = fig.add_subplot(111, projection="3d")
+        ax.scatter(x,y,z,marker=marker,c=colormap(normaliser(self.height_time_grid[time_step,:,:].flatten())),s=s)
+        ax.set_aspect('equal')
+
+    def plot_step(self,time_step):
+        fig = plt.figure()
+        ax = fig.add_subplot(111)
+        elons,lats=np.meshgrid(self.elons,self.lats)
+        ax.pcolor(elons,lats,self.height_time_grid[time_step,:,:])
+
+    def point_time(self,coords):
+        points=np.zeros((coords.shape[0],self.time_step_number))
+        for t_it in range(self.time_step_number):
+            coeff=(self.height_time_coeff[t_it-2,:]-self.height_time_coeff[t_it-3,:])/(self.time_step[t_it-2]-self.time_step[t_it-3])
+            coeff=np.stack((coeff.real,coeff.imag))
+            coeff=pysh.shio.SHCindexToCilm(coeff)
+            points[:,t_it]=-pysh.expand.MakeGridPoint(coeff,-coords[:,0],coords[:,1])
+        return points
+    
+    def along_transect(self,coord=('lat_start','lon_start','lat_stop','lon_stop'),point_density=None,point_distance=None,backend=False):
+        if not(point_density is None):
+            theta=np.linspace(-coord[0],-coord[2],point_density)
+            phi=np.linspace(coord[1],coord[3],point_density)
+        if not(point_distance is None):
+            theta=np.arange(-coord[0],-coord[2],point_distance)
+            phi=np.arange(coord[1],coord[3],point_distance)
+        coeff=np.stack((self.coeff.real,self.coeff.imag))
+        coeff=pysh.shio.SHCindexToCilm(coeff)
+        transect=pysh.expand.MakeGridPoint(coeff,theta,phi)
+        # Y_lm=np.expand_dims(pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[0]+pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[1]*1j,axis=1)
+        # for i in range(1,len(phi)):
+        #     Y_lm=np.concatenate((Y_lm,np.expand_dims((pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[0]+pysh.expand.spharm(self.maxdeg-1,theta[i],phi[i],packed=True)[1]*1j),axis=1)),axis=1)
+        # self.coeff_from_step(0)
+        # transect=np.expand_dims((Y_lm*np.repeat(np.expand_dims(self.coeff,axis=1),point_density,axis=1)).sum(0),axis=1)
+        # for t_it in range(1,self.height_time_coeff.shape[0]):
+        #     if backend :
+        #         print(t_it)
+        #     self.coeff_from_step(t_it)
+        #     transect=np.concatenate((transect,np.expand_dims((Y_lm*np.repeat(np.expand_dims(self.coeff,axis=1),point_density,axis=1)).sum(0),axis=1)),axis=1)
+        return transect
+
+    def save(self,save_way='',supersave=False):
+
+        """
+        The _`save` function is used to save the grid and all it's parameters inside a nc file. Parameters saved are, longitude, latitude, maximum degree, the time steps of the grid, the thickness of the grid, the harmonic coefficient, grid density. The harmonic coefficient, due to complexe data type management of nc, are saved separately in there complexe and real part. The created file will have the name of the grid. 
+
+        Attribute :
+        -----------
+            save_way : str
+                The filepath where the data will be saved. Default value is the current file
+            supersave : bool
+                Define if the save is called as a super method from an object that inherit the function. This precise if this method has to close the nc file (False) of if the herited class will do it (True). Default value is False.
+        Return :
+        --------
+            None
+
+        """
+
+        self.ncgrid=Dataset(save_way+'/'+self.time_grid_name+'.nc','w','NETCDF4_CLASSIC')
+        self.ncgrid.title=self.time_grid_name
+
+        self.ncgrid.createDimension('maxdeg',self.maxdeg)
+        self.ncgrid.createDimension('maxdeg_order',(self.maxdeg)*(self.maxdeg+1)/2)
+        self.ncgrid.createDimension('lon',self.nlons)
+        self.ncgrid.createDimension('lat',self.nlats)
+        self.ncgrid.createDimension('time_diff',self.time_step_number-1)
+        self.ncgrid.createDimension('time_step',self.time_step_number)
+
+        lat=self.ncgrid.createVariable('lat', np.float32, ('lat',))
+        lat.units = 'degrees_north'
+        lat.long_name = 'latitude'
+        lat[:]=self.lats
+
+        lon=self.ncgrid.createVariable('lon', np.float32, ('lon',))
+        lon.units = 'degrees_east'
+        lon.long_name = 'longitude'
+        lon[:]=self.elons
+
+        time=self.ncgrid.createVariable('time', np.float32, ('time_step',))
+        time.units = 'kyr'
+        time.long_name = 'time'
+        time[:]=self.time_step
+
+        thickness=self.ncgrid.createVariable('thickness',np.float32,('time_diff','lat','lon'))
+        thickness.units='m'
+        thickness.long_name='layer_thickness'
+        thickness[:,:,:]=self.height_time_grid
+
+        coeff_real=self.ncgrid.createVariable('coeff_real',np.float32,('time_diff','maxdeg_order'))
+        coeff_real.units='m'
+        coeff_real.long_name='layer thickness in spherical harmonics'
+        coeff_real[:,:]=np.real(self.height_time_coeff)
+
+        coeff_imag=self.ncgrid.createVariable('coeff_imag',np.float32,('time_diff','maxdeg_order'))
+        coeff_imag.units='m'
+        coeff_imag.long_name='layer thickness in spherical harmonics'
+        coeff_imag[:,:]=np.imag(self.height_time_coeff)
+
+        rho=self.ncgrid.createVariable('rho',np.float32)
+        rho.units='kg/m3'
+        rho.long_name='density of the considered grid'
+        rho[:]=self.rho
+        
+        if not(supersave) :
+            self.ncgrid.close()
+
+class SEDIMENT_TIME_GRID(TIME_GRID):
+    """
+    The _`SEDIMENT_TIME_GRID` class is used to represent sediment deposited thickness and time over time. It inherit from :ref:`TIME_GRID <TIME_GRID>` and just add a default value of sediment density at 2600 kg/m3. 
+
+    .. note::
+        This class must include the developement of :cite:`ferrier_2017` on sediment compaction and it's effect on water redistriution. 
+
+    Attributes
+    ----------
+        time_step : np.array([time_step_number,])
+            This array contains the time step of the data you are importing. They will be use for temporal interpolation.
+        maxdeg : int
+            Maximum harmonic coefficient degree of the data. this define the chape of the grid and coefficient arrays
+        height_time_grid : np.array([maxedg*2,maxdeg])
+            This array is the height grid at each time steps defined in grid_time_step
+        mass_time_grid : np.array([maxedg*2,maxdeg])
+            This array is the mass grid at each time steps defined in grid_time_step
+        height_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
+            This array is the height spherical harmonic coefficient at each time steps defined in grid_time_step
+        mass_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
+            This array is the mass spherical harmonic coefficient at each time steps defined in grid_time_step
+        rho : float
+            The density of the considered layer. Default value is 2600.
+        
+        .. note::
+
+            In future development the density may vary threw space and time. We'll have to make a variable object more then a constant density. 
+
+        grid_name : str
+            The name of the grid. We recommand you to choose a specific name for each grid you create. This name is used to save the grid in an nc file with `save`_. 
+        from_file : (bool,way)
+            This parameter define if the data are new or loaded from a previously saved model in a nc file. If the first element is False, the code will create a blank object, based on provided datas. If the first element is True, the method will get the data from the file way specified in the second element of this attribute.
+
+    Method
+    ------
+        :ref:`save <sed_save>` 
+            used to save data
+
+    """
+    def __init__(self,time_step=np.array([1,2]),maxdeg=64,height_time_grid=None,mass_time_grid=None,mass_time_coeff=None,height_time_coeff=None,rho=2600,grid_name='time_grid',from_file=(False,)) : 
+        """
+        Parameters
+        ----------
+        """
+        # preset the grid and coefficient to none. The sediment density is set to 2300 
+        super().__init__(time_step,maxdeg,height_time_grid,mass_time_grid,height_time_coeff,mass_time_coeff,rho,grid_name,from_file,superinit=True)
+        self.isgrd=False
+        self.iscoeff=False
+        self.saved=np.array([])
+        if from_file[0] :
+            self.ncgrid.close()
+
+    def save(self,save_way=''):
+        """
+        .. _sed_save:
+
+        The save method is used to save the grid data to a file. It call the super method :ref:`save <save>` method with no additional saved parameters.   
+
+        .. note::
+            Because we need to include :cite:`ferrier_2017` works, this save function will be modified to include data about the sediment compaction.  
+
+        Attributes
+        ----------
+            rho : float
+                Density value of the sediment as a constant, default value is 2600.
+
+        Return
+        ------
+            None
+
+        """
+        super().save(save_way,supersave=True)
+        self.ncgrid.close()
+
+class ICE_TIME_GRID(TIME_GRID):
+    """
+    The _`ICE_TIME_GRID` class is used to represent the ice thickness evolution threw time. This class inherit of :ref:`TIME_GRID <TIME_GRID>`. 
+
+    ...
+
+    Attributes
+    ----------
+        time_step : np.array([time_step_number,])
+            This array contains the time step of the data you are importing. They will be use for temporal interpolation.
+        maxdeg : int
+            Maximum harmonic coefficient degree of the data. this define the chape of the grid and coefficient arrays
+        height_time_grid : np.array([maxedg*2,maxdeg])
+            This array is the height grid at each time steps defined in grid_time_step
+        mass_time_grid : np.array([maxedg*2,maxdeg])
+            This array is the mass grid at each time steps defined in grid_time_step
+        height_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
+            This array is the height spherical harmonic coefficient at each time steps defined in grid_time_step
+        mass_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
+            This array is the mass spherical harmonic coefficient at each time steps defined in grid_time_step
+        rho : float
+            The density of the considered layer. Default is 916.7 kg/m3.
+        
+        .. note::
+
+            In future development the density may vary threw space and time. We'll have to make a variable object more then a constant density. 
+
+        grid_name : str
+            The name of the grid. We recommand you to choose a specific name for each grid you create. This name is used to save the grid in an nc file with `save`_. 
+        from_file : (bool,way)
+            This parameter define if the data are new or loaded from a previously saved model in a nc file. If the first element is False, the code will create a blank object, based on provided datas. If the first element is True, the method will get the data from the file way specified in the second element of this attribute.
+        
+        
+    Methods
+    -------
+        `ice_correction`_ 
+            correct the grounded ice thickness from the created floating ice by ground vertical mouvement
+        :ref:`save <ice_save>` 
+            used to save data
+        
+    """
+    def __init__(self,time_step=np.array([1,2]),maxdeg=64,height_time_grid=None,mass_time_grid=None,mass_time_coeff=None,height_time_coeff=None,rho=916.7,grid_name='time_grid',from_file=(False,)) : 
+        """
+        Parameters
+        ----------
+        """
+        # initialize to false the grid and coefficient (no grid or coefficient pre loaded). The ice volumetric masse is set to 916.7 kg/m3.
+        super().__init__(time_step,maxdeg,height_time_grid,mass_time_grid,height_time_coeff,mass_time_coeff,rho,grid_name,from_file,superinit=True)
+        # self.isgrd=False
+        # self.iscoeff=False
+        self.saved=np.array([])
+        self.sdeli_00=0
+        self.deli_00_prev=0
+
+        if from_file[0] :
+            self.ice=self.ncgrid['ice'][:].data
+            self.ncgrid.close()
+
+    def ice_correction(self,topo,oc):
+        """
+        The _`ice_correction` method is used to correct the grounded ice thickness from the floating ice generted by vertical ground motion. This correction is done for each time step to remove the floating ice.  The correction of grounded ice is based on :ref:`Grounded ice correction <Ice_corr>`.
+
+        Attributes
+        ----------
+            topo : :ref:`TOPOGRAPHIC_TIME_GRID <TOPOGRAPHIC_TIME_GRID>` class object
+                A topogrphic grid object, used to check if grounded ice become floating ice. The topography is then modified to by this function. 
+            oc : :ref:`OCEAN_TIME_GRID <OCEAN_TIME_GRID>` class object
+                An oceanic time grid object used only to get the density of ocean set for the model. 
+
+            .. note::
+                To avoid memory consumption the oc parameter should be replace simply by oc_rho the ocean density. 
+                 
+
+        Return
+        ------
+            None
+
+        """
+        for t_it in range(self.time_step_number-1):
+            if t_it==0 :
+                topo.height_time_grid[t_it,:,:]=topo.height_time_grid[t_it,:,:]-self.height_time_grid[t_it,:,:]+self.ice[t_it,:,:]
+            else :
+                topo.height_time_grid[t_it,:,:]=topo.height_time_grid[t_it,:,:]-self.height_time_grid[:t_it+1,:,:].sum(0)+self.ice[:t_it+1,:,:].sum(0)
+        for t_it in range(self.time_step_number-1): 
+            if t_it==0:
+                check1 = OCEAN_TIME_GRID().evaluate_ocean(-topo.height_time_grid[t_it,:,:]+self.ice[t_it,:,:]) # generate the ocean function for ice-topo
+                check2 = OCEAN_TIME_GRID().evaluate_ocean(topo.height_time_grid[t_it,:,:]-self.ice[t_it,:,:]).grd*(OCEAN_TIME_GRID().evaluate_ocean(-self.ice[t_it,:,:]*self.rho-(topo.height_time_grid[t_it,:,:]-self.ice[t_it,:,:])*oc.rho).grd)
+                self.height_time_grid[t_it,:,:] = check1.grd*self.ice[t_it,:,:]+check2*self.ice[t_it,:,:] # add the two part of ice over the check1 nd check2 positive area.
+            else :
+                check1 = OCEAN_TIME_GRID().evaluate_ocean(-topo.height_time_grid[t_it,:,:]+self.ice[:t_it+1,:,:].sum(0)) # generate the ocean function for ice-topo
+                check2 = OCEAN_TIME_GRID().evaluate_ocean(topo.height_time_grid[t_it,:,:]-self.ice[:t_it+1,:,:].sum(0)).grd*(OCEAN_TIME_GRID().evaluate_ocean(-self.ice[:t_it+1,:,:].sum(0)*self.rho-(topo.height_time_grid[t_it,:,:]-self.ice[:t_it+1,:,:].sum(0))*oc.rho).grd)
+                self.height_time_grid[t_it,:,:] = check1.grd*self.ice[:t_it+1,:,:].sum(0)+check2*self.ice[:t_it+1,:,:].sum(0)-self.height_time_grid[:t_it,:,:].sum(0) # add the two part of ice over the check1 nd check2 positive area.
+        for t_it in range(self.time_step_number-1):    
+            if t_it==0 :
+                topo.height_time_grid[t_it,:,:]=topo.height_time_grid[t_it,:,:]+self.height_time_grid[t_it,:,:]-self.ice[t_it,:,:]
+            else :
+                topo.height_time_grid[t_it,:,:]=topo.height_time_grid[t_it,:,:]+self.height_time_grid[:t_it+1,:,:].sum(0)-self.ice[:t_it+1,:,:].sum(0)
+
+    def save(self,save_way=''):
+
+        """
+        .. _ice_save:
+
+        The save method is used to save the data of the ice grid. Because of the `ice_correction`_ method that update the grid we choosed to preserve the original ice thickness data in a ice parameter that is saved inside the nc file. Otherwise this method use the super method :ref:`save` to save the rest of the data.  
+
+        Attributes
+        ----------
+            save_way :str
+                The way where the nc file is saved. Default value is the current file (an empty str).              
+
+        Return
+        ------
+            None
+
+        """
+
+        super().save(save_way,supersave=True)
+        ice=self.ncgrid.createVariable('ice',np.float32,('time_diff','lat','lon'))
+        ice.units='m'
+        ice.long_name='initial_ice_thickness'
+
+        if self.__dict__.keys().__contains__('ice'):
+            ice[:,:,:]=self.ice
+        else :
+            ice[:,:,:]=self.height_time_grid.copy()
+
+        self.ncgrid.close()
+
+class OCEAN_TIME_GRID(TIME_GRID):
+    """
+    The _`OCEAN_TIME_GRID` class is used to represent the ocean thickness variation and contains the method to resolve the sea level equation. This method inherit from :ref:`TIME_GRID <TIME_GRID>`.
+
+    ...
+
+    Attributes
+    ----------
+        time_step : np.array([time_step_number,])
+            This array contains the time step of the data you are importing. They will be use for temporal interpolation.
+        maxdeg : int
+            Maximum harmonic coefficient degree of the data. this define the chape of the grid and coefficient arrays
+        height_time_grid : np.array([maxedg*2,maxdeg])
+            This array is the height grid at each time steps defined in grid_time_step
+        mass_time_grid : np.array([maxedg*2,maxdeg])
+            This array is the mass grid at each time steps defined in grid_time_step
+        height_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
+            This array is the height spherical harmonic coefficient at each time steps defined in grid_time_step
+        mass_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
+            This array is the mass spherical harmonic coefficient at each time steps defined in grid_time_step
+        rho : float
+            The density of the considered layer. Default is 1000 kg/m3.
+        
+        .. note::
+
+            In future development the density may vary threw space and time. We'll have to make a variable object more then a constant density. 
+
+        grid_name : str
+            The name of the grid. We recommand you to choose a specific name for each grid you create. This name is used to save the grid in an nc file with `save`_. 
+        from_file : (bool,way)
+            This parameter define if the data are new or loaded from a previously saved model in a nc file. If the first element is False, the code will create a blank object, based on provided datas. If the first element is True, the method will get the data from the file way specified in the second element of this attribute.
+           
+    Methods
+    -------
+        :ref:`update_0 <update_0_oce>`
+            set the grd_0 from the actual grd loaded in the grid
+        `evaluate_ocean`_
+            evaluate the ocean function based on the Gaussian grid of the topography 
+
+    """
+    def __init__(self,time_step=np.array([1,2]),maxdeg=64,height_time_grid=None,mass_time_grid=None,mass_time_coeff=None,height_time_coeff=None,rho=1000,grid_name='time_grid',from_file=(False,)) :
+        """
+        Parameters
+        ----------
+        """
+        # initialize the ocean with no grid and no coefficient. The saved is also initialized. The volumetric mass of water is set to 1000 
+
+        super().__init__(time_step,maxdeg,height_time_grid,mass_time_grid,height_time_coeff,mass_time_coeff,rho,grid_name,from_file,superinit=True)
+        self.saved=np.array([])
+        if from_file[0] :
+            self.ncgrid.close()
+        
+    def update_0(self):
+        """
+        .. _update_0_oce:
+
+        The update_0 method update the grd_0 parameter of the object to the currend loaded grd. 
+
+        Attributes
+        ----------
+            None
+            
+        Return
+        -------
+            None
+
+        """
+        self.grd_0=self.grd.copy()
+        
+    def evaluate_ocean(self,topo) :
+        '''
+        The _`evaluate_ocean` method evaluate the ocean function using the topography. It create a 0-1 matrix wich is 1 where topo<0 and 0 where topo>0.  The ocean function is described in :ref:`ocean function <oc_func>`.
+    
+        Attribute
+        ---------
+            topo : np.array(maxdeg,maxdegx2)
+                topographic gaussian grid.
+        
+        Returns :
+            None
+
+        '''
+        # use sign function to optimize the conversion from positive negative value to boolean value.
+        out = -0.5*np.sign(topo)+0.5
+        out = 0.5*np.sign(out-0.6)+0.5
+        # set the grd to the output of the previous computation.
+        self.grd=out
+        return self
+    
+    def sea_level_solver(self,load,ice_time_grid,sed_time_grid,love_number,TO,t_it,conv_it,conv_lim):
+        '''
+        The _`sea_level_solver` method solve the sea level equation until. Beacause of the iterative type of the resolution of the SLE, this method define also a first guess of the Sea level at the first iteration and the first time step. This function is based on the convergence iteration for the estimation of the variability defined in :ref:`Convergence parameter <conv>`.
+
+        Attribute
+        ---------
+            load : :ref:`LOAD_TIME_GRID <LOAD_TIME_GRID>` class object
+                The load time grid as specified in the class object. This grid needs to be of the same shape (maxdeg) then the one of the current object. 
+            ice_time_grid : :ref:`ICE_TIME_GRID <ICE_TIME_GRID>` class object
+                The ice time grid as specified in the class object. This grid needs to be of the same shape (maxdeg) then the one of the current object. 
+            sed_time_grid : :ref:`SEDIMENT_TIME_GRID <SEDIMENT_TIME_GRID>` class object
+                The sediment time grid as specified in the class object. This grid needs to be of the same shape (maxdeg) then the one of the current object. 
+            love_number : :ref:`LOVE <LOVE>` class object 
+                The love numbers as specified in the class object. The love numbers must have been set up with the same maximm degree thne the currend object.
+            TO : :ref:`sphericalobject <sphericalobject>` class object
+                The ocean contours variability area computed as a sphericalobject class computed for the previous iteration. !Trouver où définir ce calcul!. 
+            t_it : int
+                The time iteration of the current computation on wich apply the resolution of the SLE.
+            conv_it : int
+                convergence iteration set to 0 if it's for a simple resolution of the SLE on one time step. This is used when you are working on a topographic convergence. In the code, the first guess for the SLE will be if it's not the first topographic convergence iteration, the guess of the previuous one.
+            conv_lim : float
+                To stop the convergence of the solution, the conv_lim is usually set to 10^-3. The number of required step is then between 13 and 7. 
+        Return 
+        ------
+            None 
+
+        '''
+        if conv_it==0 :
+            if t_it==0:
+                self.height_time_coeff[t_it,:]=self.prev/self.prev[0]*(TO.coeff[0]-TO.prev[0])-TO.coeff-TO.prev
+            else :
+                self.height_time_coeff[t_it,:]=self.prev/self.prev[0]*(-ice_time_grid.rho/self.rho*ice_time_grid.height_time_coeff[:t_it+1,:].sum(0) + TO.coeff[0]-TO.prev[0])-TO.coeff-TO.prev
+        chi=np.inf
+        while chi>conv_lim:
+            chi=self.sea_level_equation(load,ice_time_grid,sed_time_grid,love_number,TO,t_it)
+            conv_it+=1
+        #if t_it >1 :
+            #print(load.rot_pot[t_it-1,:],sed_time_grid.height_time_coeff[t_it,:].max())
+        return conv_it
+    
+    def sea_level_equation(self,load,ice_time_grid,sed_time_grid,love_number,TO,t_it):
+        '''
+        The _`sea_level_equation` method calculate the Sea level variation following the SLE. Tis function is resolving both the conservation of mass equation and the SL variation. This follows the method described in :ref:`Resolution of SLE including the deconvolution<spec_sol>`.
+
+        Attribute
+        ---------
+            load : :ref:`LOAD_TIME_GRID <LOAD_TIME_GRID>` class object
+                The load time grid as specified in the class object. This grid needs to be of the same shape (maxdeg) then the one of the current object. 
+            ice_time_grid : :ref:`ICE_TIME_GRID <ICE_TIME_GRID>` class object
+                The ice time grid as specified in the class object. This grid needs to be of the same shape (maxdeg) then the one of the current object. 
+            sed_time_grid : :ref:`SEDIMENT_TIME_GRID <SEDIMENT_TIME_GRID>` class object
+                The sediment time grid as specified in the class object. This grid needs to be of the same shape (maxdeg) then the one of the current object. 
+            love_number : :ref:`LOVE <LOVE>` class object 
+                The love numbers as specified in the class object. The love numbers must have been set up with the same maximm degree thne the currend object.
+            TO : :ref:`sphericalobject <sphericalobject>` class object
+                The ocean contours variability area computed as a sphericalobject class computed for the previous iteration. !Trouver où définir ce calcul!. 
+            t_it : int
+                The time iteration of the current computation on wich apply the resolution of the SLE.
+        Return 
+        ------
+            None 
+            
+        '''
+        if t_it==0 :
+            delSLcurl_fl=love_number.E* love_number.T.coeff *(ice_time_grid.height_time_coeff[0,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[0,:]*sed_time_grid.rho+self.height_time_coeff[0,:]*self.rho)
+            self.delSLcurl=sphericalobject(coeff=delSLcurl_fl - ice_time_grid.height_time_coeff[0,:]- sed_time_grid.height_time_coeff[0,:]).coefftogrd()
+            load.calc_rot_visc(ice_time_grid.height_time_coeff[1:t_it,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[1:t_it,:]*sed_time_grid.rho+self.height_time_coeff[1:t_it,:]*self.rho,0,love_number)
+            RO=sphericalobject(grd=self.delSLcurl.grd*self.grd).grdtocoeff()
+            self.delPhi_g=np.real(1/self.coeff[0] * (- ice_time_grid.rho/self.rho*ice_time_grid.coeff[0] - RO.coeff[0] + TO.coeff[0]))
+            chi = np.abs( (np.sum(np.abs(RO.coeff + self.delPhi_g*self.coeff -  TO.coeff)) - np.sum(np.abs(self.height_time_coeff[t_it,:]))) / np.sum(np.abs(self.height_time_coeff[t_it,:])))
+            self.height_time_coeff[t_it,:]=RO.coeff + self.delPhi_g*self.coeff -  TO.coeff
+        else :
+            
+            if t_it == 1 : 
+                #load.calc_viscuous_load(ice_time_grid.height_time_coeff[0,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[0,:]*sed_time_grid.rho+self.height_time_coeff[0,:]*self.rho,love_number.beta_l,0)
+                load.calc_rot_visc(ice_time_grid.height_time_coeff[1,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[1,:]*sed_time_grid.rho+self.height_time_coeff[1,:]*self.rho,t_it,love_number)
+                load.rot_pot[t_it,:]=load.rot_pot[t_it,:]
+                load.calc_rotational_viscuous(np.zeros(6),love_number.beta_l_tide,0)
+                load.calc_viscuous(np.zeros(ice_time_grid.height_time_coeff[0,:].shape),love_number.beta_l,0)
+
+            else : 
+                load.calc_rot_visc(ice_time_grid.height_time_coeff[1:t_it,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[1:t_it,:]*sed_time_grid.rho+self.height_time_coeff[1:t_it,:]*self.rho,t_it,love_number)
+                load.rot_pot[t_it,:]=load.rot_pot[t_it,:]-load.rot_pot[:t_it,:].sum(0) # calc small variation
+                load.calc_viscuous(ice_time_grid.height_time_coeff[1:t_it,:]*ice_time_grid.rho+sed_time_grid.height_time_coeff[1:t_it,:]*sed_time_grid.rho+self.height_time_coeff[1:t_it,:]*self.rho,love_number.beta_l,t_it)
+                load.calc_rotational_viscuous(load.rot_pot[1:t_it,:],love_number.beta_l_tide,t_it)
+            # print(t_it)
+            # print('rot_pot : ',load.rot_pot[:t_it])
+            # print('m : ',load.sdelm[:t_it])
+            # print('I : ', load.sdelI[:t_it])
+            # print('V_lm_T : ', load.V_lm_tide.coeff)
+            delSLcurl_tide_fl=1/load.g*load.V_lm_tide.coeff+1/load.g*love_number.E_T[:6]*load.rot_pot[:t_it,:].sum(0)
+            
+            delSLcurl_fl=love_number.E* love_number.T.coeff *(ice_time_grid.height_time_coeff[1:t_it+1,:].sum(0)*ice_time_grid.rho+sed_time_grid.height_time_coeff[1:t_it+1,:].sum(0)*sed_time_grid.rho+self.height_time_coeff[1:t_it+1,:].sum(0)*self.rho)+love_number.T.coeff*load.V_lm.coeff
+
+            #print(load.V_lm_tide.coeff.shape,load.V_lm.coeff.shape)
+
+            delSLcurl_tide_fl=np.concatenate((delSLcurl_tide_fl,np.zeros(delSLcurl_fl.shape[0]-delSLcurl_tide_fl.shape[0])))
+
+            self.delSLcurl=sphericalobject(coeff=delSLcurl_fl + delSLcurl_tide_fl - ice_time_grid.height_time_coeff[1:t_it+1,:].sum(0)- sed_time_grid.height_time_coeff[1:t_it+1,:].sum(0)).coefftogrd()
+            RO=sphericalobject(grd=self.delSLcurl.grd*self.grd).grdtocoeff()
+            self.delPhi_g=np.real(1/self.coeff[0] * (- ice_time_grid.rho/self.rho*ice_time_grid.height_time_coeff[1:t_it+1,0].sum() - RO.coeff[0] + TO.coeff[0]))
+            #print(t_it,':',self.coeff[0])
+            if t_it==1:
+                chi = np.abs((np.sum(np.abs(RO.coeff + self.delPhi_g*self.coeff -  TO.coeff - self.height_time_coeff[0,:])) - np.sum(np.abs(self.height_time_coeff[t_it,:]))) / np.sum(np.abs(self.height_time_coeff[t_it,:])))
+                self.height_time_coeff[t_it,:]=RO.coeff + self.delPhi_g*self.coeff -  TO.coeff - self.height_time_coeff[0,:]
+            else :
+                chi = np.abs((np.sum(np.abs(RO.coeff + self.delPhi_g*self.coeff -  TO.coeff - self.height_time_coeff[:t_it,:].sum(0))) - np.sum(np.abs(self.height_time_coeff[t_it,:]))) / np.sum(np.abs(self.height_time_coeff[t_it,:])))
+                self.height_time_coeff[t_it,:]=RO.coeff + self.delPhi_g*self.coeff -  TO.coeff - self.height_time_coeff[:t_it,:].sum(0)
+            # print('chi : ',chi)
+        return chi
+
+class TOPOGRAPHIC_TIME_GRID(TIME_GRID):
+    """
+    The _`TOPOGRAPHIC_TIME_GRID` class is used to save and include all the topographic variations. This class inherits of :ref:`TIME_GRID <TIME_GRID>`. This class main difference with TIME_GRID is the presence of a parameter called topo_pres wich is the present topography. It is created using :ref:`Precomputation <Precomputation>`.
+
+    Attributes
+    ----------
+        time_step : np.array([time_step_number,])
+            This array contains the time step of the data you are importing. They will be use for temporal interpolation.
+        maxdeg : int
+            Maximum harmonic coefficient degree of the data. this define the chape of the grid and coefficient arrays
+        height_time_grid : np.array([maxedg*2,maxdeg])
+            This array is the height grid at each time steps defined in grid_time_step
+        mass_time_grid : np.array([maxedg*2,maxdeg])
+            This array is the mass grid at each time steps defined in grid_time_step
+        height_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
+            This array is the height spherical harmonic coefficient at each time steps defined in grid_time_step
+        mass_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
+            This array is the mass spherical harmonic coefficient at each time steps defined in grid_time_step
+        rho : float
+            The density of the considered layer.
+        
+        .. note::
+
+            In future development the density may vary threw space and time. We'll have to make a variable object more then a constant density. 
+
+        grid_name : str
+            The name of the grid. We recommand you to choose a specific name for each grid you create. This name is used to save the grid in an nc file with `save`_. 
+        from_file : (bool,way)
+            This parameter define if the data are new or loaded from a previously saved model in a nc file. If the first element is False, the code will create a blank object, based on provided datas. If the first element is True, the method will get the data from the file way specified in the second element of this attribute.
+
+    Methods
+    -------
+        :ref:`save <topo_save>` 
+            Method to save the topographic datas   
+
+    """
+    def __init__(self,time_step=np.array([1,2]),maxdeg=64,height_time_grid=None,mass_time_grid=None,mass_time_coeff=None,height_time_coeff=None,rho=0,grid_name='time_grid',from_file=(False,)) : 
+        """
+        Parameters
+        ----------
+        """
+        super().__init__(time_step,maxdeg,height_time_grid,mass_time_grid,height_time_coeff,mass_time_coeff,rho,grid_name,from_file,superinit=True)
+        if from_file[0] :
+            self.topo_pres=self.ncgrid['topo_pres'][:].data
+            self.ncgrid.close()
+        
+        # initialize coefficient and grid to 0 because no grid or coefficient has been created
+        # self.isgrd=False
+        # self.iscoeff=False
+        #self.saved=np.array([])
+
+    def save(self,save_way=''):
+        """
+        .. _topo_save:
+
+        The save method is used to save the data of the topographic grid. Particularity of the topography is the present day topography used in the code to converge toward it. The function save is. Otherwise this method use the super method :ref:`save` to save the rest of the data.  
+
+        Attributes
+        ----------
+            save_way :str
+                The way where the nc file is saved. Default value is the current file (an empty str).              
+
+        Return
+        ------
+            None
+
+        """
+        super().save(save_way,supersave=True)
+        topo_pres=self.ncgrid.createVariable('topo_pres',np.float32,('lat','lon'))
+        topo_pres.units='m'
+        topo_pres.long_name='present topography'
+
+        if self.__dict__.keys().__contains__('topo_pres'):
+            topo_pres[:,:]=self.topo_pres
+
+        self.ncgrid.close()
+
+
+from .love import get_tlm
+
+class LOAD_TIME_GRID(TIME_GRID) :
+    """
+    The _`LOAD_TIME_GRID` class is used to save and include all the topographic variations. This class inherits of :ref:`TIME_GRID <TIME_GRID>` and :ref:`LOAD <LOAD>`.
+
+    Attributes
+    ---------- 
+        sdelL : np.array([time_step_number,maxdeg,maxdegx2])
+            The load variation grid used to compute earth vertical motion.
+        betal : np.array([time_step_number,time_step_number,maxdeg])
+            The beta love number as described in :ref:`Variation of geoïd and ground Equations <geoid_ground_variation_theory>` section. There calculated in the :ref:`LOVE <LOVE>` class.
+        E : np.array([(maxdeg+1)(maxdeg+2)/2,])
+            The elastic component of the earth as love numbers computed form :ref:`LOVE <LOVE>` class.
+        a : float
+            The earth radius in meter, set by default to 7371000 meters.
+        Me : float
+            The earth mass in set by default to 5000. 
+        time_step : np.array([time_step_number,])
+            This array contains the time step of the data you are importing. They will be use for temporal interpolation.
+        maxdeg : int
+            Maximum harmonic coefficient degree of the data. this define the chape of the grid and coefficient arrays
+        height_time_grid : np.array([maxedg*2,maxdeg])
+            This array is the height grid at each time steps defined in grid_time_step
+        mass_time_grid : np.array([maxedg*2,maxdeg])
+            This array is the mass grid at each time steps defined in grid_time_step
+        height_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
+            This array is the height spherical harmonic coefficient at each time steps defined in grid_time_step
+        mass_time_coeff : np.array([(maxdeg+1)(maxedg+2)/2,])
+            This array is the mass spherical harmonic coefficient at each time steps defined in grid_time_step
+        rho : float
+            The density of the considered layer.
+        grid_name : str
+            The name of the grid. We recommand you to choose a specific name for each grid you create. This name is used to save the grid in an nc file with `save`_. 
+        from_file : (bool,way)
+            This parameter define if the data are new or loaded from a previously saved model in a nc file. If the first element is False, the code will create a blank object, based on provided datas. If the first element is True, the method will get the data from the file way specified in the second element of this attribute.
+
+    Methods
+    -------
+        `calc_viscuous`_:
+            Compute the viscous motion of the geoïd and ground for one time step.
+        `calc_viscuous_time`_ :
+            Compute the viscous ground motion of the earth on all time steps.    
+        `calc_elastic_time`_ :
+            Compute the elastic ground motion of the earth on all time steps.
+        :ref:`save <load_save>` :
+            Save the load data
+
+    """
+    def __init__(self,sdelL=np.array([]),beta_l=np.array([]),E=np.array([]),E_T=np.array([]),a=7371000,Me=5000,time_step=np.array([1,2]),maxdeg=64,height_time_grid=None,mass_time_grid=None,mass_time_coeff=None,height_time_coeff=None,rho=0,grid_name='time_grid',from_file=(False,),g=9.80665):
+        TIME_GRID.__init__(self,time_step,maxdeg,height_time_grid,mass_time_grid,height_time_coeff,mass_time_coeff,rho,grid_name,from_file,superinit=True)
+        #LOAD.__init__(self,maxdeg,time_step)
+        self.beta_counter=np.repeat(np.arange(0,self.maxdeg),np.arange(1,self.maxdeg+1))
+        if from_file[0]:
+            self.a=self.ncgrid['a'][:].data
+            self.Me=self.ncgrid['Me'][:].data
+            self.viscuous_deformation=self.ncgrid['viscuous_deformation_real'][:].data+self.ncgrid['viscuous_deformation_imag'][:].data*1j
+            self.elastic_deformation=self.ncgrid['elastic_deformation_real'][:].data+self.ncgrid['elastic_deformation_imag'][:].data*1j
+            #self.beta_l=self.ncgrid['beta_l'][:].data
+            self.elastic_love=self.ncgrid['elastic_love'][:].data
+            self.load=self.ncgrid['load_real'][:].data+self.ncgrid['load_imag'][:].data*1j
+        else :
+            self.g=g
+            self.viscuous_deformation=np.zeros((self.time_step_number-2,int(maxdeg*(maxdeg+1)/2)))+0j
+            self.elastic_deformation=np.zeros((self.time_step_number-2,int(maxdeg*(maxdeg+1)/2)))+0j
+            self.load=sdelL[1:,:]
+            self.elastic_love=E[self.beta_counter.astype(int)]
+            self.elastic_tidal_love=E_T
+            self.a=a
+            self.Me=Me
+            self.beta_l=beta_l
+            self.viscuous_love=self.beta_l[:,:,self.beta_counter.astype(int)]
+            self.V_lm=sphericalobject(coeff=np.zeros((int(maxdeg*(maxdeg+1)/2)))+0j)
+            self.V_lm_tide=sphericalobject(coeff=np.zeros((6,))+0j)
+            self.rot_pot=np.zeros((self.time_step_number-1,6))+0j
+            self.sdelI=np.zeros((self.time_step_number-2,3))+0j
+            self.sdelm=np.zeros((self.time_step_number-2,3))+0j
+        self.T = sphericalobject(coeff=get_tlm(self.maxdeg-1,self.a,self.Me))
+
+    def calc_viscuous(self,sdelL,beta,t_it):
+        '''
+        The _`calc_viscuous` method is used to calculate the ground and geoïd deformation based on viscuous love numbers.
+
+        Attribute
+        ---------
+            sdelL : np.array([t_it,(maxdeg+1)(maxdeg+20/2)])
+                The load grid used to estimate the ground vertical mouvement. This include all previous loading history because of the viscous comportment of earth. 
+            beta : np.array([time_step_number,time_step_number,(maxdeg+1)(maxdeg+2)/2])
+                The beta love numbers used to compute the earth deformation to include the viscous part. These love numbers are particularly heavy in the memory due to the representation of the time. 
+            t_it : int
+                The time iteration at wich the computation is performed.
+            
+        '''
+        if t_it==1 :
+            self.V_lm.coeff=np.zeros(beta.shape[2])
+        else :
+            self.V_lm.coeff=(beta[t_it-1,:t_it-1]*sdelL).sum(0)
+
+    def calc_rotational_viscuous(self,rot_pot,beta_tide,t_it):
+        if t_it==1 :
+            self.V_lm_tide.coeff=np.zeros(6)
+        else :
+            self.V_lm_tide.coeff=(beta_tide[t_it-1,:t_it-1]*rot_pot).sum(0)
+
+    def calc_viscuous_time(self,backend=False) :
+        '''
+        The _`calc_viscuous_time` method compute the vicuous vertical ground motion. This method call the :ref:`LOAD <LOAD>` method for this. 
+
+        Attribute
+        ---------
+            backend : bool
+                Specifie if the method give backend (True) or not (False). Default is False.
+
+        Return
+        ------
+            None
+
+        '''
+        for t_it in range(1,self.time_step_number-1):
+            if t_it+1==1 :
+                self.calc_viscuous(np.zeros(self.height_time_coeff[0,:].shape),self.viscuous_love,0)
+            else :
+                self.calc_viscuous(self.load[1:t_it,:],self.viscuous_love,t_it)
+            self.viscuous_deformation[t_it-1,:]=self.T.coeff*np.squeeze(self.V_lm.coeff.T)
+            if backend:
+                print(f'viscuous calculation at {self.time_step[t_it]} kyr done')
+    
+    def calc_elastic_time(self):
+        '''
+        The _`calc_elastic_time` method compute the elactic vertical ground motion. This method call the :ref:`LOAD <LOAD>` method for this. 
+
+        Attribute
+        ---------
+            None
+
+        Return
+        ------
+            None
+             
+        '''
+        self.elastic_deformation=np.repeat(np.expand_dims(self.T.coeff,axis=0),self.time_step_number-2,axis=0)*np.repeat(np.expand_dims(self.elastic_love,axis=0),self.time_step_number-2,axis=0)*self.load
+
+    def save(self,save_way=''):
+        '''
+        .. _load_save:
+
+        The save method is used to save the data from the class. It is based on the inherited :ref:`save <save>` method. Because of the particularity of this TIME_GRID, we had to save the new parameters, and calculated data. This function save for each data the real and complex part of the data due to the nc file particularity. The saved data are, The load (load), the viscuous groud motion (viscous_deformation), the elastic ground motion (elastic_deformation), the elastic love numbers (elastic_love), earth radius (a), earth mass (Me). 
+
+        Attribute
+        ---------
+            save_way : str
+                file path to where the grid will be saved. 
+
+        Return
+        ------
+            None
+             
+        '''
+        super().save(save_way,supersave=True)
+
+        self.ncgrid.createDimension('time_no_init',self.time_step_number-2)
+
+        load_real=self.ncgrid.createVariable('load_real',np.float32,('time_no_init','maxdeg_order'))
+        load_real.units='kg'
+        load_real.long_name='load grid used to compute the earth deformation.'
+        load_real[:,:]=np.real(self.load)
+
+        load_imag=self.ncgrid.createVariable('load_imag',np.float32,('time_no_init','maxdeg_order'))
+        load_imag.units='kg'
+        load_imag.long_name='load grid used to compute the earth deformation.'
+        load_imag[:,:]=np.imag(self.load)
+
+        viscuous_deformation_real=self.ncgrid.createVariable('viscuous_deformation_real',np.float32,('time_no_init','maxdeg_order'))
+        viscuous_deformation_real.units='mm/yr'
+        viscuous_deformation_real.long_name='viscuous component of the earth deformation due to load.'
+        viscuous_deformation_real[:,:]=np.real(self.viscuous_deformation)
+
+        viscuous_deformation_imag=self.ncgrid.createVariable('viscuous_deformation_imag',np.float32,('time_no_init','maxdeg_order'))
+        viscuous_deformation_imag.units='mm/yr'
+        viscuous_deformation_imag.long_name='viscuous component of the earth deformation due to load.'
+        viscuous_deformation_imag[:,:]=np.imag(self.viscuous_deformation)
+
+        elastic_deformation_real=self.ncgrid.createVariable('elastic_deformation_real',np.float32,('time_no_init','maxdeg_order'))
+        elastic_deformation_real.units='mm/yr'
+        elastic_deformation_real.long_name='elastic component of the earth deformation due to load.'
+        elastic_deformation_real[:,:]=np.real(self.elastic_deformation)
+
+        elastic_deformation_imag=self.ncgrid.createVariable('elastic_deformation_imag',np.float32,('time_no_init','maxdeg_order'))
+        elastic_deformation_imag.units='mm/yr'
+        elastic_deformation_imag.long_name='elastic component of the earth deformation due to load.'
+        elastic_deformation_imag[:,:]=np.imag(self.elastic_deformation)
+
+        elastic_love=self.ncgrid.createVariable('elastic_love',np.float32,('maxdeg_order'))
+        elastic_love.units='none'
+        elastic_love.long_name='elastic load love numbers used to compute the earth deformation'
+        elastic_love[:]=self.elastic_love
+
+        # beta_l=self.ncgrid.createVariable('beta_l',np.float32,('time_diff','time_diff','maxdeg'))
+        # beta_l.units='none'
+        # beta_l.long_name='viscuous load love numbers used to compute the earth deformation'
+        # beta_l[:,:]=self.beta_l
+
+        a=self.ncgrid.createVariable('a',np.float32)
+        a.units='m'
+        a.long_name='earth radius'
+        a=self.a
+
+        Me=self.ncgrid.createVariable('Me',np.float32)
+        Me.units='kg'
+        Me.long_name='earth mass'
+        Me=self.Me
+
+        self.ncgrid.close()
+
+    def clean_memory(self):
+        '''
+        This method is used to clean the memory to avoïd over charging RAM. 
+        '''
+        self.viscuous_love=0
+
+    def calc_rot_visc(self,sdelL,t_it,love_number,G=6.67408E-11,a=6371000,C=8.034e37,k_f=0.942,omega=7.292E-5):
+        '''
+        .. note::
+            This function must be updated to work with the new versions of the code.
+
+        '''
+        # extract degree 2 coefficient from the load
+        CminA = (k_f*(a**5)*(omega)**2)/(3*G)
+
+        if t_it==1 :
+            L00 = sdelL[0]
+            L20 = sdelL[3]
+            L21 = sdelL[4]
+        else :
+            L00 = sdelL[:,0].sum(0)
+            L20 = sdelL[:,3].sum(0)
+            L21 = sdelL[:,4].sum(0)
+
+        # calculate the load effect constant 
+        I1=math.sqrt(32/15)*math.pi*a**4*np.real(L21)
+        I2=math.sqrt(32/15)*math.pi*a**4*np.imag(L21)   
+        I3=8/3*math.pi*a**4*(L00-L20/math.sqrt(5))
+        I=np.array([I1,I2,I3])
+        if t_it==1 :
+            V_lm=np.zeros(3)
+            V_lm_T=np.zeros(3)
+        if t_it==2 :
+            V_lm = love_number.beta_konly_l[t_it-2,:t_it-1]*self.sdelI[:t_it-1,:].squeeze()
+            V_lm_T = love_number.beta_konly_l_tide[t_it-2,:t_it-1]*self.sdelm[:t_it-1,:].squeeze()
+        else : #apply the visco elastic properties of the earth on the rotation using the load.
+            V_lm = np.dot(love_number.beta_konly_l[t_it-2,:t_it-1],self.sdelI[:t_it-1,:].squeeze())
+            V_lm_T = np.dot(love_number.beta_konly_l_tide[t_it-2,:t_it-1],self.sdelm[:t_it-1,:].squeeze())
+        
+        temp = 1/(1-love_number.k_tide_e[1]/k_f)*(1/CminA * ((1+love_number.k_e[1])*I + V_lm.squeeze()) + V_lm_T.squeeze()/k_f)
+        # calculate the perturbation to the rotational potential from Milne 1998
+        m1=temp[0]
+        m2=temp[1]
+        temp = -1/(1-love_number.k_tide_e[1]/k_f)*(1/C * ((1+love_number.k_e[1])*I + V_lm.squeeze()))
+        m3=temp[2]
+
+        m=np.array([m1,m2,m3])
+        # print(t_it)
+        # print('L : ', sdelL)
+        # print('L : ', L00,L20,L21)
+        # print('temp : ',(1/CminA * ((1+love_number.k_e[1])*I + V_lm.squeeze()) + V_lm_T.squeeze()/k_f))
+        # print('CminA : ',CminA)
+        # print(t_it)
+        # print('V_lm : ',V_lm)
+        # print('V_lm_T : ', V_lm_T)
+        # print('I : ',I)
+        # print('m : ',m)
+        #update the rotational load using.
+        #print(self.sdelI[:t_it-1,:].sum(0),self.sdelI[:t_it-1,:].sum(0).shape,I.T.squeeze(),I.T.squeeze().shape,self.sdelI[t_it-1,:],self.sdelI[t_it-1,:].shape)
+        self.sdelI[t_it-1,:] = I.T.squeeze() - self.sdelI[:t_it-2,:].sum(0)
+        self.sdelm[t_it-1,:] = m.T.squeeze() - self.sdelm[:t_it-2,:].sum(0)
+
+        #print('m : ',self.sdelm[t_it-1,:])
+        # calculate the rotational perturbation of the earth potential, just for the 6 first coefficient (no use to calculate further)
+        self.rot_pot[t_it-1,0] = a**2 * omega**2/3 * (np.sum(m**2) + 2*m3)+0j
+        self.rot_pot[t_it-1,3] = a**2 * omega**2/(6*np.sqrt(5)) * (m1**2 + m2**2 - 2*m3**2 - 4*m3)+1j*0
+        self.rot_pot[t_it-1,4] = a**2 * omega**2/np.sqrt(30) * (m1*(1+m3) - 1j*m2*(1+m3))+1j*0
+        self.rot_pot[t_it-1,5] = a**2 * omega**2/(np.sqrt(5) * np.sqrt(24)) * ( (m2**2-m1**2) + 1j*2*m1*m2 )+1j*0
+        
         #print('rot_pot : ',self.rot_pot[t_it-1])
```

### Comparing `slcode-0.4.1/src/SL_C0de/love.py` & `slcode-1.0.0/slcode/love.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,348 +1,378 @@
-import numpy as np
-from numpy.matlib import repmat #used to add repmat 
-from .spharm import sphericalobject
-import math
-from scipy import io
-
-
-
-def love_lm(num,maxdeg):
-    '''
-    the _`love_lm` funtion get from love numbers the h_lm spherical coefficient. 
-
-    Attribute 
-    ---------
-        num : np.array([n,]) 
-            Love number coefficient of the size of the entry file
-        maxdeg : int
-            The maximum harmonic coefficient degree. 
-
-    Returns
-    -------
-        h_lm : np.array([(maxdeg+1)(maxdeg+2)/2,])
-            Array of the love number repeated on harmonic degree orders. 
-
-    '''
-    num=np.concatenate((np.zeros((1,1)),num)) 
-    h_lm=np.repeat(num,np.arange(1,maxdeg+2,1))
-    return h_lm 
-
-def get_tlm(maxdeg,a,Me):
-    '''
-    The _`get_lm` function generate the T spherical harmonic coefficient as defined in :ref:`Theory <T_definition>`.
-
-    Attribute
-    --------- 
-        maxdeg : int
-            maximum degree of spherical harmonic defined in the model parameters. 
-        a : float
-            The earth radius in meters. 
-        Me : float
-            The earth mass.
-
-    Returns
-    ------- 
-        T_lm : np.array([(maxdeg+1)(maxdeg+2)/2])
-            The T harmonic coefficient 
-
-    '''
-    T_lm=np.array([]) # preset the output
-    T = np.zeros(maxdeg+1) # preset an array of the size maxdeg who will obtaine the coefficient and then be added to T_lm
-    const = 4*np.pi*a**3/Me # setting the tide constant for earth !!!! CHECK !!!!
-    for n in range(maxdeg+1) :
-            T[n]=const/(2*n+1) # for each nth add to T the earth constant moduladed by the nth step
-            T_add=repmat(T[n],1,n+1) # prepare T_add as the repetition of T
-            if n==0 :
-                T_lm=T_add # if there is nothing in T_lm preset T_lm as T_add
-            else :
-                T_lm=np.concatenate((T_lm,T_add),1) # else add T_add to T_lm
-    return np.squeeze(T_lm) # we have to squeeze the array so that the requested indices are directly on the good axis
-
-def calc_beta_counter(self,maxdeg):
-    '''
-    The _`calc_beta_counter` define the degree of the spherical harmonic for each beta coefficient 
-    
-    Attribute
-    ---------
-        self : :ref:`LOVE <LOVE>` class object
-            The LOVE class object on wich the betacounter is calculated
-        maxdeg : int
-            maximum spherical harmonic coefficient
-    
-    Returns
-    -------
-        None
-
-    '''
-    # self.beta_counter = np.ones((self.h.shape[0]-1,))
-    self.beta_counter=np.repeat(np.arange(0,maxdeg),np.arange(1,maxdeg+1))
-    # l_it = 1
-    # for lm_it in range(1,len(self.h)-1):
-    #     # for each time step if the coefficient indices is one degree then , all the next values in beta_counter will have the previous of this one +1. litteraly the degree associated to there indices.
-    #     if lm_it == l_it*(l_it+1)/2:
-    #         self.beta_counter[lm_it] = self.beta_counter[lm_it-1]+1
-    #         l_it = l_it+1
-    #     else:
-    #         self.beta_counter[lm_it] = self.beta_counter[lm_it-1]
-    return
-
-class LOVE(object):
-    """
-    The _`LOVE` class is used to keep the love numbers values and prepare them for the computation of geoïd and ground vertical motion. The love number are calculted and loaded from a file as described in :ref:`Implementation of Love numbers <love>`. This function also include the possibility to compute the love numbers from normal modes love numbers parameters. 
-
-    Attributes
-    ----------
-        maxedeg : int
-            The spherical harmonic maximum degree.
-        way : str
-            The file path to the ALMA output file. This file must follow the described pattern in ...
-        time_step : np.array([time_step_number,])
-            The time step of the model, used to prepare the viscuous love numbers.
-        a : float
-            The earth radius in meter.
-        Me : float
-            The earth mass.
-        type : str
-            The type of love number in input. could be 'time' or 'normal, where 'time' is for love numbers from ALMA3 code and 'normal' is for love number in normale mode from MIT serveur. Default is 'time'.
-    
-    Methods
-    -------
-        `dev_beta`_ :
-            This method is used to calculate the beta love numbers.
-        `dev_beta_tide`_ :
-            This method is used to calculate the beta tidal love numbers.
-        `clean_memory`_ :
-            This method is used to clean the memory of your computer. 
-
-    """
-    def __init__(self,maxdeg,way,time_step,a,Me,type='time'):
-        """
-    Parameters
-    ----------
-    grid : object (from class GRID)
-    way : !!!! A corriger !!!! 
-        """
-        self.type=type
-        self.time_step=time_step
-        self.maxdeg=maxdeg
-        self.time_step_number=len(time_step)
-        # Load the Load Love Numbers
-        if type is 'time': 
-            self.h_e=np.loadtxt(way+'/h_e.dat',unpack=True)[1,:maxdeg]#/(4*math.pi)
-            self.k_e=np.loadtxt(way+'/k_e.dat',unpack=True)[1,:maxdeg]#/(4*math.pi)
-            self.k_e[0]=0
-            self.h=np.repeat(self.h_e,np.arange(1,maxdeg+1,1))
-            self.k=np.repeat(self.k_e,np.arange(1,maxdeg+1,1))
-            self.k_ve=np.loadtxt(way+'/k_ve.dat',unpack=True)[1:,:]#/(4*math.pi)
-            self.h_ve=np.loadtxt(way+'/h_ve.dat',unpack=True)[1:,:]#/(4*math.pi)
-
-            self.love_time=np.loadtxt(way+'/time.dat',unpack=True)
-
-
-            time_step_diff=-(time_step.reshape(-1,1)-time_step)
-            time_step_diff[time_step_diff<=0]=0
-            data=np.arange(0,len(self.love_time),1)
-            data=np.repeat(repmat(data,len(time_step_diff),1)[np.newaxis,:,:],len(time_step_diff),axis=0)
-            time_interval=(np.repeat(time_step_diff[:,:,np.newaxis],len(self.love_time),axis=2)-np.repeat(repmat(self.love_time,len(time_step_diff),1)[np.newaxis,:,:],len(time_step_diff),axis=0))==0
-            data[time_interval==False]=0
-            data=data.sum(2)
-
-            # time_step_diff=time_step_diff.flatten()
-            # time_step_diff=time_step_diff[time_step_diff>0]
-
-
-            # time_interval=np.where((repmat(time_step_diff,len(self.love_time),1).transpose()-repmat(self.love_time,len(time_step_diff),1))==0)[1]
-            # time_interval_tri=np.zeros((self.time_step_number,self.time_step_number))
-            # time_interval_tri[np.triu_indices(self.time_step_number,1)]=time_interval
-            # time_interval_tri=time_interval_tri.transpose().astype(int)
-
-            k_ve=np.concatenate((np.zeros((self.k_ve.shape[0],1)),self.k_ve),axis=1)
-            h_ve=np.concatenate((np.zeros((self.h_ve.shape[0],1)),self.h_ve),axis=1)
-            k_e=np.concatenate((np.zeros((1,)),self.k_e))
-            h_e=np.concatenate((np.zeros((1,)),self.h_e))
-            self.beta_G_l=k_ve[data,:maxdeg].squeeze()+np.repeat(self.k_e[:maxdeg,np.newaxis],self.time_step_number,1).T
-            self.beta_G_l[0,:,0]=0
-            self.beta_G_l[0,0,:]=0
-            #self.beta_G_l=k_ve[time_interval_tri+1,:maxdeg].squeeze()-k_ve[time_interval_tri,:maxdeg].squeeze()
-            self.beta_G_l[data<=0]=self.beta_G_l[data<=0]*0
-            self.beta_R_l=h_ve[:,:maxdeg]+np.repeat(self.h_e[:maxdeg,np.newaxis],h_ve.shape[0],1).T
-            self.beta_R_l=self.beta_R_l[data,:maxdeg].squeeze()#-h_e[:maxdeg]
-            #self.beta_R_l=h_ve[time_interval_tri+1,:maxdeg].squeeze()-h_ve[time_interval_tri,:maxdeg].squeeze()
-            self.beta_R_l[data<=0]=self.beta_R_l[data<=0]*0
-            self.beta_l=self.beta_G_l-self.beta_R_l
-            self.beta_konly_l=self.k_ve[data,1]-self.k_e[0]#-(self.h_ve[data,1]-self.h_e[0])
-
-
-            # Load the Tide Love Numbers
-            self.h_tide_e=np.loadtxt(way+'/h_e_T.dat',unpack=True)[1,1:7]
-            self.k_tide_e=np.loadtxt(way+'/k_e_T.dat',unpack=True)[1,1:7]
-            self.h_tide=np.repeat(self.h_tide_e,np.arange(1,7,1))
-            self.k_tide=np.repeat(self.k_tide_e,np.arange(1,7,1))
-            self.k_tide_ve=np.loadtxt(way+'/k_ve_T.dat',unpack=True)[1:,1:7]
-            self.h_tide_ve=np.loadtxt(way+'/h_ve_T.dat',unpack=True)[1:,1:7]
-            #print(self.h_tide_e.shape,self.k_tide_e.shape,self.h_tide.shape,self.k_tide.shape,self.k_tide_ve.shape,self.h_tide_ve.shape)
-
-            k_tide_ve=np.concatenate((np.zeros((self.k_tide_ve.shape[0],1)),self.k_tide_ve),axis=1)
-            h_tide_ve=np.concatenate((np.zeros((self.h_tide_ve.shape[0],1)),self.h_tide_ve),axis=1)
-            k_tide_e=np.concatenate((np.zeros((1,)),self.k_tide_e))
-            h_tide_e=np.concatenate((np.zeros((1,)),self.h_tide_e))
-
-            self.beta_G_l_tide=k_tide_ve[data,:6].squeeze()+np.repeat(self.k_tide_e[:6,np.newaxis],self.time_step_number,1).T
-            self.beta_G_l_tide[0,:,0]=0
-            self.beta_G_l_tide[0,0,:]=0
-            #self.beta_G_l=k_ve[time_interval_tri+1,:maxdeg].squeeze()-k_ve[time_interval_tri,:maxdeg].squeeze()
-            self.beta_G_l_tide[data<=0]=self.beta_G_l_tide[data<=0]*0
-            self.beta_R_l_tide=h_tide_ve[:,:6]+np.repeat(self.h_tide_e[:6,np.newaxis],h_tide_ve.shape[0],1).T
-            self.beta_R_l_tide=self.beta_R_l_tide[data,:7].squeeze()#-h_e[:maxdeg]
-            #self.beta_R_l=h_ve[time_interval_tri+1,:maxdeg].squeeze()-h_ve[time_interval_tri,:maxdeg].squeeze()
-            self.beta_R_l_tide[data<=0]=self.beta_R_l_tide[data<=0]*0
-            self.beta_l_tide=self.beta_G_l_tide-self.beta_R_l_tide
-            self.beta_konly_l_tide=self.k_tide_ve[data,1]-self.k_tide_e[0]#-(self.h_tide_ve[data,1]-self.h_tide_e[0])
-
-            
-            # self.beta_tide=k_tide_ve[time_interval_tri,:maxdeg+1].squeeze()-k_tide_e[:maxdeg+1]-(h_tide_ve[time_interval_tri,:maxdeg+1].squeeze()-h_tide_e[:maxdeg+1])
-            # self.beta_konly_tide=self.k_tide_ve[time_interval_tri,1]-self.k_tide_e[0]-(self.h_tide_ve[time_interval_tri,1]-self.h_tide_e[0])
-            
-            self.E = 1+self.k - self.h
-            self.E_T = 1 + self.k_tide - self.h_tide
-            self.T = sphericalobject(coeff=get_tlm(maxdeg-1,a,Me))
-
-            calc_beta_counter(self,maxdeg)
-            #self.beta_G_l=np.array(self.beta_G_l)[:,:,self.beta_counter.astype(int)]
-            #self.beta_R_l=np.array(self.beta_R_l)[:,:,self.beta_counter.astype(int)]
-            self.beta_konly_l=np.array(self.beta_konly_l)
-            #self.beta_tide=np.array(self.beta_tide)[:,:,self.beta_counter.astype(int)]
-            self.beta_konly_l_tide=np.array(self.beta_konly_l_tide)
-        elif type is 'normal':
-            a=0
-            #retrouver comment on charge les love numbers. 
-            love = io.loadmat(way)
-            self.mode_found=love['mode_found']
-            self.k_amp=love['k_amp']
-            self.h_amp=love['h_amp']
-            self.k_amp_tide=love['k_amp_tide']
-            self.h_amp_tide=love['h_amp_tide']
-            self.spoles=love['spoles']     
-            self.k_el=love['k_el']
-            self.k_el_tide=love['k_el_tide']
-            self.h = love_lm(love['h_el'],maxdeg)
-            self.k = love_lm(love['k_el'],maxdeg)
-            self.h_tide = love_lm(love['h_el_tide'],maxdeg)
-            self.k_tide = love_lm(love['k_el_tide'],maxdeg)
-            self.E = 1 + self.k - self.h
-            self.T = sphericalobject(coeff=get_tlm(maxdeg-1,a,Me))
-            self.beta_l = np.zeros((self.time_step_number-1,self.time_step_number-1,maxdeg+1))
-            self.beta_G_l = np.zeros((self.time_step_number-1,self.time_step_number-1,maxdeg+1))
-            self.beta_R_l = np.zeros((self.time_step_number-1,self.time_step_number-1,maxdeg+1))
-            self.beta_konly_l = np.zeros((self.time_step_number-1,self.time_step_number-1))
-            self.beta_G_konly_l = np.zeros((self.time_step_number-1,self.time_step_number-1))
-            self.beta_R_konly_l = np.zeros((self.time_step_number-1,self.time_step_number-1))
-            for t_it in range(1,self.time_step_number):  # loop on the time step
-                #initialise the temporary variable for calculation use
-                beta_l_int=self.beta_l[t_it-1]
-                beta_konly_l_int=self.beta_konly_l[t_it-1]
-                beta_G_l_int=self.beta_l[t_it-1]
-                beta_G_konly_l_int=self.beta_konly_l[t_it-1]
-                beta_R_l_int=self.beta_l[t_it-1]
-                beta_R_konly_l_int=self.beta_konly_l[t_it-1]
-                for n in range(1,t_it):
-                    # initialize the beta for each time step
-                    beta = np.zeros((maxdeg,)) 
-                    beta_G = np.zeros((maxdeg,)) 
-                    beta_R = np.zeros((maxdeg,)) 
-                    for lm in range(maxdeg):
-                        # num_mod is the number of love number needed for each degree-order
-                        num_mod = self.mode_found[lm][0] 
-                        # calculate the beta coefficient for each time step and degree-order
-                        beta[lm] = np.sum((self.k_amp[lm,:num_mod] - self.h_amp[lm,:num_mod])/self.spoles[lm,:num_mod] * (1 - np.exp(- self.spoles[lm,:num_mod]* (-time_step[t_it] + time_step[n]))))
-                        beta_G[lm]=np.sum((self.k_amp[lm,:num_mod])/self.spoles[lm,:num_mod] * (1 - np.exp(- self.spoles[lm,:num_mod]* (-time_step[t_it] + time_step[n]))))
-                        beta_R[lm]=np.sum((self.h_amp[lm,:num_mod])/self.spoles[lm,:num_mod] * (1 - np.exp(- self.spoles[lm,:num_mod]* (-time_step[t_it] + time_step[n]))))
-                    # add to the beta a coefficient of value 0 !!!!
-                    beta_l_int[n-1,:]=np.concatenate((np.array([0]),beta))
-                    beta_G_l_int[n-1,:]=np.concatenate((np.array([0]),beta_G))
-                    beta_R_l_int[n-1,:]=np.concatenate((np.array([0]),beta_R))
-                    # for rotation only needed for degree 2
-                    lm=1
-                    num_mod=self.mode_found[lm][0]
-                    # calculate the beta konly 
-                    beta_konly_l_int[n-1] = np.sum((self.k_amp[lm,:num_mod]-self.h_amp[lm,:num_mod])/self.spoles[lm,:num_mod] * (1 - np.exp(- self.spoles[lm,:num_mod] * (-time_step[t_it] + time_step[n]))))
-                    beta_G_konly_l_int[n-1] = np.sum((self.k_amp[lm,:num_mod])/self.spoles[lm,:num_mod] * (1 - np.exp(- self.spoles[lm,:num_mod] * (-time_step[t_it] + time_step[n]))))
-                    beta_R_konly_l_int[n-1] = np.sum((self.h_amp[lm,:num_mod])/self.spoles[lm,:num_mod] * (1 - np.exp(- self.spoles[lm,:num_mod] * (-time_step[t_it] + time_step[n]))))
-                #for each time step update the beta coeffcient
-                self.beta_l[t_it-1]=beta_l_int
-                self.beta_R_l[t_it-1]=beta_R_l_int
-                self.beta_G_l[t_it-1]=beta_G_l_int
-            self.beta_konly_l[t_it-1]=beta_konly_l_int
-            self.beta_G_konly_l[t_it-1]=beta_G_konly_l_int
-            self.beta_R_konly_l[t_it-1]=beta_R_konly_l_int
-
-    def dev_beta(self,applied='beta'):
-        '''
-        The _`dev_beta` method can be used to rise the love numbers to their full shape to fit the computation method. This is required before using the beta in the methods from :ref:`LOAD <LOAD>`.
-
-        Attribute
-        ---------
-            applied : str
-                The kinf of beta you are calculating. Three values are possible : beta, beta_R et beta_G. 'beta' define the love numbers used to caculate the variation of ocean thickness. 'beta_R' define the love numbers used to calculate the variation of groud. 'beta_G' define the love numbers used to calculate the variation of geoïd. 
-        Return
-        ------
-            None
-
-        '''
-        if applied is 'beta':
-            self.beta_G=0
-            self.beta_R=0
-            self.beta_l=self.beta_G_l-self.beta_R_l
-            self.beta_l=np.array(self.beta_l)[:,:,self.beta_counter.astype(int)]
-        elif applied is 'beta_R':
-            self.beta_l=0
-            self.beta_G=0
-            self.beta_R=np.array(self.beta_R_l)[:,:,self.beta_counter.astype(int)]
-        elif applied is 'beta_G':
-            self.beta_l=0
-            self.beta_R=0
-            self.beta_G=np.array(self.beta_G_l)[:,:,self.beta_counter.astype(int)]
-
-    def dev_beta_tide(self,applied='beta'):
-        '''
-        The _`dev_beta_tide` method can be used to rise the love numbers to their full shape to fit the computation method. This is required before using the beta in the methods from :ref:`LOAD <LOAD>`.
-
-        Attribute
-        ---------
-            applied : str
-                The kinf of beta you are calculating. Three values are possible : beta, beta_R et beta_G. 'beta' define the love numbers used to caculate the variation of ocean thickness. 'beta_R' define the love numbers used to calculate the variation of groud. 'beta_G' define the love numbers used to calculate the variation of geoïd. 
-        Return
-        ------
-            None
-
-        '''
-        if applied is 'beta':
-            self.beta_G_tide=0
-            self.beta_R_tide=0
-            self.beta_l_tide=self.beta_G_l_tide-self.beta_R_l_tide
-            self._tide=np.array(self.beta_l)[:,:,self.beta_counter.astype(int)[:6]]
-        elif applied is 'beta_R':
-            self.beta_l_tide=0
-            self.beta_G_tide=0
-            self.beta_R_tide=np.array(self.beta_R_l_tide)[:,:,self.beta_counter.astype(int)[:6]]
-        elif applied is 'beta_G':
-            self.beta_l_tide=0
-            self.beta_R_tide=0
-            self.beta_G_tide=np.array(self.beta_G_l_tide)[:,:,self.beta_counter.astype(int)[:6]]
-    
-    def clean_memory(self):
-        '''
-        The _`clean_memory` method can be used to araise the beta_l, beta_R and beta_G to avoid memory issues. 
-
-        Attribute
-        ---------
-            None
-
-        Return
-        ------
-            None
-
-        '''
-        self.beta_l=0
-        self.beta_R=0
-        self.beta_G=0
+import numpy as np
+from numpy.matlib import repmat #used to add repmat 
+from .spharm import sphericalobject
+import math
+from scipy import io
+
+
+
+def love_lm(num,maxdeg):
+    '''
+    the _`love_lm` funtion get from love numbers the h_lm spherical coefficient. 
+
+    Attribute 
+    ---------
+        num : np.array([n,]) 
+            Love number coefficient of the size of the entry file
+        maxdeg : int
+            The maximum harmonic coefficient degree. 
+
+    Returns
+    -------
+        h_lm : np.array([(maxdeg+1)(maxdeg+2)/2,])
+            Array of the love number repeated on harmonic degree orders. 
+
+    '''
+    num=np.concatenate((np.zeros((1,1)),num)) 
+    h_lm=np.repeat(num,np.arange(1,maxdeg+2,1))
+    return h_lm 
+
+def get_tlm(maxdeg,a,Me):
+    '''
+    The _`get_lm` function generate the T spherical harmonic coefficient as defined in :ref:`Theory <T_definition>`.
+
+    Attribute
+    --------- 
+        maxdeg : int
+            maximum degree of spherical harmonic defined in the model parameters. 
+        a : float
+            The earth radius in meters. 
+        Me : float
+            The earth mass.
+
+    Returns
+    ------- 
+        T_lm : np.array([(maxdeg+1)(maxdeg+2)/2])
+            The T harmonic coefficient 
+
+    '''
+    T_lm=np.array([]) # preset the output
+    T = np.zeros(maxdeg+1) # preset an array of the size maxdeg who will obtaine the coefficient and then be added to T_lm
+    const = 4*np.pi*a**3/Me # setting the tide constant for earth !!!! CHECK !!!!
+    for n in range(maxdeg+1) :
+            T[n]=const/(2*n+1) # for each nth add to T the earth constant moduladed by the nth step
+            T_add=repmat(T[n],1,n+1) # prepare T_add as the repetition of T
+            if n==0 :
+                T_lm=T_add # if there is nothing in T_lm preset T_lm as T_add
+            else :
+                T_lm=np.concatenate((T_lm,T_add),1) # else add T_add to T_lm
+    return np.squeeze(T_lm) # we have to squeeze the array so that the requested indices are directly on the good axis
+
+def calc_beta_counter(self,maxdeg):
+    '''
+    The _`calc_beta_counter` define the degree of the spherical harmonic for each beta coefficient 
+    
+    Attribute
+    ---------
+        self : :ref:`LOVE <LOVE>` class object
+            The LOVE class object on wich the betacounter is calculated
+        maxdeg : int
+            maximum spherical harmonic coefficient
+    
+    Returns
+    -------
+        None
+
+    '''
+    # self.beta_counter = np.ones((self.h.shape[0]-1,))
+    self.beta_counter=np.repeat(np.arange(0,maxdeg),np.arange(1,maxdeg+1))
+    # l_it = 1
+    # for lm_it in range(1,len(self.h)-1):
+    #     # for each time step if the coefficient indices is one degree then , all the next values in beta_counter will have the previous of this one +1. litteraly the degree associated to there indices.
+    #     if lm_it == l_it*(l_it+1)/2:
+    #         self.beta_counter[lm_it] = self.beta_counter[lm_it-1]+1
+    #         l_it = l_it+1
+    #     else:
+    #         self.beta_counter[lm_it] = self.beta_counter[lm_it-1]
+    return
+
+class LOVE(object):
+    """
+    The _`LOVE` class is used to keep the love numbers values and prepare them for the computation of geoïd and ground vertical motion. The love number are calculted and loaded from a file as described in :ref:`Implementation of Love numbers <love>`. This function also include the possibility to compute the love numbers from normal modes love numbers parameters. 
+
+    Attributes
+    ----------
+        maxedeg : int
+            The spherical harmonic maximum degree.
+        way : str
+            The file path to the ALMA output file. This file must follow the described pattern in ...
+        time_step : np.array([time_step_number,])
+            The time step of the model, used to prepare the viscuous love numbers.
+        a : float
+            The earth radius in meter.
+        Me : float
+            The earth mass.
+        type : str
+            The type of love number in input. could be 'time', 'normal' or 'spectral', where 'time' is for love numbers from ALMA3 code, 'normal' is for love number in normale mode from MIT server and 'spectral' is the frequential decomposition of the Love numbers available in ALMA3. Default is 'time'.
+    
+    Methods
+    -------
+        `dev_beta`_ :
+            This method is used to calculate the beta love numbers.
+        `dev_beta_tide`_ :
+            This method is used to calculate the beta tidal love numbers.
+        `clean_memory`_ :
+            This method is used to clean the memory of your computer. 
+
+    """
+    def __init__(self,maxdeg,way,time_step,a,Me,type='time',T=None):
+        """
+    Parameters
+    ----------
+    grid : object (from class GRID)
+    way : !!!! A corriger !!!! 
+        """
+        self.type=type
+        self.time_step=time_step
+        self.maxdeg=maxdeg
+        self.time_step_number=len(time_step)
+        # Load the Load Love Numbers
+        if type is 'time': 
+            self.h_e=np.loadtxt(way+'/h_e.dat',unpack=True)[1,:maxdeg]#/(4*math.pi)
+            self.k_e=np.loadtxt(way+'/k_e.dat',unpack=True)[1,:maxdeg]#/(4*math.pi)
+            self.k_e[0]=0
+            self.h=np.repeat(self.h_e,np.arange(1,maxdeg+1,1))
+            self.k=np.repeat(self.k_e,np.arange(1,maxdeg+1,1))
+            self.k_ve=np.loadtxt(way+'/k_ve.dat',unpack=True)[1:,:]#/(4*math.pi)
+            self.h_ve=np.loadtxt(way+'/h_ve.dat',unpack=True)[1:,:]#/(4*math.pi)
+
+            self.love_time=np.loadtxt(way+'/time.dat',unpack=True)
+
+
+            time_step_diff=-(time_step.reshape(-1,1)-time_step)
+            time_step_diff[time_step_diff<=0]=0
+            data=np.arange(0,len(self.love_time),1)
+            data=np.repeat(repmat(data,len(time_step_diff),1)[np.newaxis,:,:],len(time_step_diff),axis=0)
+            time_interval=(np.repeat(time_step_diff[:,:,np.newaxis],len(self.love_time),axis=2)-np.repeat(repmat(self.love_time,len(time_step_diff),1)[np.newaxis,:,:],len(time_step_diff),axis=0))==0
+            data[time_interval==False]=0
+            data=data.sum(2)
+
+            # time_step_diff=time_step_diff.flatten()
+            # time_step_diff=time_step_diff[time_step_diff>0]
+
+
+            # time_interval=np.where((repmat(time_step_diff,len(self.love_time),1).transpose()-repmat(self.love_time,len(time_step_diff),1))==0)[1]
+            # time_interval_tri=np.zeros((self.time_step_number,self.time_step_number))
+            # time_interval_tri[np.triu_indices(self.time_step_number,1)]=time_interval
+            # time_interval_tri=time_interval_tri.transpose().astype(int)
+
+            k_ve=np.concatenate((np.zeros((self.k_ve.shape[0],1)),self.k_ve),axis=1)
+            h_ve=np.concatenate((np.zeros((self.h_ve.shape[0],1)),self.h_ve),axis=1)
+            k_e=np.concatenate((np.zeros((1,)),self.k_e))
+            h_e=np.concatenate((np.zeros((1,)),self.h_e))
+            self.beta_G_l=k_ve[data,:maxdeg].squeeze()+np.repeat(self.k_e[:maxdeg,np.newaxis],self.time_step_number,1).T
+            self.beta_G_l[0,:,0]=0
+            self.beta_G_l[0,0,:]=0
+            #self.beta_G_l=k_ve[time_interval_tri+1,:maxdeg].squeeze()-k_ve[time_interval_tri,:maxdeg].squeeze()
+            self.beta_G_l[data<=0]=self.beta_G_l[data<=0]*0
+            self.beta_R_l=h_ve[:,:maxdeg]+np.repeat(self.h_e[:maxdeg,np.newaxis],h_ve.shape[0],1).T
+            self.beta_R_l=self.beta_R_l[data,:maxdeg].squeeze()#-h_e[:maxdeg]
+            #self.beta_R_l=h_ve[time_interval_tri+1,:maxdeg].squeeze()-h_ve[time_interval_tri,:maxdeg].squeeze()
+            self.beta_R_l[data<=0]=self.beta_R_l[data<=0]*0
+            self.beta_l=self.beta_G_l-self.beta_R_l
+            self.beta_konly_l=self.k_ve[data,1]-self.k_e[0]#-(self.h_ve[data,1]-self.h_e[0])
+
+
+            # Load the Tide Love Numbers
+            self.h_tide_e=np.loadtxt(way+'/h_e_T.dat',unpack=True)[1,1:7]
+            self.k_tide_e=np.loadtxt(way+'/k_e_T.dat',unpack=True)[1,1:7]
+            self.h_tide=np.repeat(self.h_tide_e,np.arange(1,7,1))
+            self.k_tide=np.repeat(self.k_tide_e,np.arange(1,7,1))
+            self.k_tide_ve=np.loadtxt(way+'/k_ve_T.dat',unpack=True)[1:,1:7]
+            self.h_tide_ve=np.loadtxt(way+'/h_ve_T.dat',unpack=True)[1:,1:7]
+            #print(self.h_tide_e.shape,self.k_tide_e.shape,self.h_tide.shape,self.k_tide.shape,self.k_tide_ve.shape,self.h_tide_ve.shape)
+
+            k_tide_ve=np.concatenate((np.zeros((self.k_tide_ve.shape[0],1)),self.k_tide_ve),axis=1)
+            h_tide_ve=np.concatenate((np.zeros((self.h_tide_ve.shape[0],1)),self.h_tide_ve),axis=1)
+            k_tide_e=np.concatenate((np.zeros((1,)),self.k_tide_e))
+            h_tide_e=np.concatenate((np.zeros((1,)),self.h_tide_e))
+
+            self.beta_G_l_tide=k_tide_ve[data,:6].squeeze()+np.repeat(self.k_tide_e[:6,np.newaxis],self.time_step_number,1).T
+            self.beta_G_l_tide[0,:,0]=0
+            self.beta_G_l_tide[0,0,:]=0
+            #self.beta_G_l=k_ve[time_interval_tri+1,:maxdeg].squeeze()-k_ve[time_interval_tri,:maxdeg].squeeze()
+            self.beta_G_l_tide[data<=0]=self.beta_G_l_tide[data<=0]*0
+            self.beta_R_l_tide=h_tide_ve[:,:6]+np.repeat(self.h_tide_e[:6,np.newaxis],h_tide_ve.shape[0],1).T
+            self.beta_R_l_tide=self.beta_R_l_tide[data,:7].squeeze()#-h_e[:maxdeg]
+            #self.beta_R_l=h_ve[time_interval_tri+1,:maxdeg].squeeze()-h_ve[time_interval_tri,:maxdeg].squeeze()
+            self.beta_R_l_tide[data<=0]=self.beta_R_l_tide[data<=0]*0
+            self.beta_l_tide=self.beta_G_l_tide-self.beta_R_l_tide
+            self.beta_konly_l_tide=self.k_tide_ve[data,1]-self.k_tide_e[0]#-(self.h_tide_ve[data,1]-self.h_tide_e[0])
+
+            
+            # self.beta_tide=k_tide_ve[time_interval_tri,:maxdeg+1].squeeze()-k_tide_e[:maxdeg+1]-(h_tide_ve[time_interval_tri,:maxdeg+1].squeeze()-h_tide_e[:maxdeg+1])
+            # self.beta_konly_tide=self.k_tide_ve[time_interval_tri,1]-self.k_tide_e[0]-(self.h_tide_ve[time_interval_tri,1]-self.h_tide_e[0])
+            
+            self.E = 1+self.k - self.h
+            self.E_T = 1 + self.k_tide - self.h_tide
+            self.T = sphericalobject(coeff=get_tlm(maxdeg-1,a,Me))
+
+            calc_beta_counter(self,maxdeg)
+            #self.beta_G_l=np.array(self.beta_G_l)[:,:,self.beta_counter.astype(int)]
+            #self.beta_R_l=np.array(self.beta_R_l)[:,:,self.beta_counter.astype(int)]
+            self.beta_konly_l=np.array(self.beta_konly_l)
+            #self.beta_tide=np.array(self.beta_tide)[:,:,self.beta_counter.astype(int)]
+            self.beta_konly_l_tide=np.array(self.beta_konly_l_tide)
+        elif type is 'normal':
+            a=0
+            #retrouver comment on charge les love numbers. 
+            love = io.loadmat(way)
+            self.mode_found=love['mode_found']
+            self.k_amp=love['k_amp']
+            self.h_amp=love['h_amp']
+            self.k_amp_tide=love['k_amp_tide']
+            self.h_amp_tide=love['h_amp_tide']
+            self.spoles=love['spoles']     
+            self.k_el=love['k_el']
+            self.k_el_tide=love['k_el_tide']
+            self.h = love_lm(love['h_el'],maxdeg)
+            self.k = love_lm(love['k_el'],maxdeg)
+            self.h_tide = love_lm(love['h_el_tide'],maxdeg)
+            self.k_tide = love_lm(love['k_el_tide'],maxdeg)
+            self.E = 1 + self.k - self.h
+            self.T = sphericalobject(coeff=get_tlm(maxdeg-1,a,Me))
+            self.beta_l = np.zeros((self.time_step_number-1,self.time_step_number-1,maxdeg+1))
+            self.beta_G_l = np.zeros((self.time_step_number-1,self.time_step_number-1,maxdeg+1))
+            self.beta_R_l = np.zeros((self.time_step_number-1,self.time_step_number-1,maxdeg+1))
+            self.beta_konly_l = np.zeros((self.time_step_number-1,self.time_step_number-1))
+            self.beta_G_konly_l = np.zeros((self.time_step_number-1,self.time_step_number-1))
+            self.beta_R_konly_l = np.zeros((self.time_step_number-1,self.time_step_number-1))
+            for t_it in range(1,self.time_step_number):  # loop on the time step
+                #initialise the temporary variable for calculation use
+                beta_l_int=self.beta_l[t_it-1]
+                beta_konly_l_int=self.beta_konly_l[t_it-1]
+                beta_G_l_int=self.beta_l[t_it-1]
+                beta_G_konly_l_int=self.beta_konly_l[t_it-1]
+                beta_R_l_int=self.beta_l[t_it-1]
+                beta_R_konly_l_int=self.beta_konly_l[t_it-1]
+                for n in range(1,t_it):
+                    # initialize the beta for each time step
+                    beta = np.zeros((maxdeg,)) 
+                    beta_G = np.zeros((maxdeg,)) 
+                    beta_R = np.zeros((maxdeg,)) 
+                    for lm in range(maxdeg):
+                        # num_mod is the number of love number needed for each degree-order
+                        num_mod = self.mode_found[lm][0] 
+                        # calculate the beta coefficient for each time step and degree-order
+                        beta[lm] = np.sum((self.k_amp[lm,:num_mod] - self.h_amp[lm,:num_mod])/self.spoles[lm,:num_mod] * (1 - np.exp(- self.spoles[lm,:num_mod]* (-time_step[t_it] + time_step[n]))))
+                        beta_G[lm]=np.sum((self.k_amp[lm,:num_mod])/self.spoles[lm,:num_mod] * (1 - np.exp(- self.spoles[lm,:num_mod]* (-time_step[t_it] + time_step[n]))))
+                        beta_R[lm]=np.sum((self.h_amp[lm,:num_mod])/self.spoles[lm,:num_mod] * (1 - np.exp(- self.spoles[lm,:num_mod]* (-time_step[t_it] + time_step[n]))))
+                    # add to the beta a coefficient of value 0 !!!!
+                    beta_l_int[n-1,:]=np.concatenate((np.array([0]),beta))
+                    beta_G_l_int[n-1,:]=np.concatenate((np.array([0]),beta_G))
+                    beta_R_l_int[n-1,:]=np.concatenate((np.array([0]),beta_R))
+                    # for rotation only needed for degree 2
+                    lm=1
+                    num_mod=self.mode_found[lm][0]
+                    # calculate the beta konly 
+                    beta_konly_l_int[n-1] = np.sum((self.k_amp[lm,:num_mod]-self.h_amp[lm,:num_mod])/self.spoles[lm,:num_mod] * (1 - np.exp(- self.spoles[lm,:num_mod] * (-time_step[t_it] + time_step[n]))))
+                    beta_G_konly_l_int[n-1] = np.sum((self.k_amp[lm,:num_mod])/self.spoles[lm,:num_mod] * (1 - np.exp(- self.spoles[lm,:num_mod] * (-time_step[t_it] + time_step[n]))))
+                    beta_R_konly_l_int[n-1] = np.sum((self.h_amp[lm,:num_mod])/self.spoles[lm,:num_mod] * (1 - np.exp(- self.spoles[lm,:num_mod] * (-time_step[t_it] + time_step[n]))))
+                #for each time step update the beta coeffcient
+                self.beta_l[t_it-1]=beta_l_int
+                self.beta_R_l[t_it-1]=beta_R_l_int
+                self.beta_G_l[t_it-1]=beta_G_l_int
+            self.beta_konly_l[t_it-1]=beta_konly_l_int
+            self.beta_G_konly_l[t_it-1]=beta_G_konly_l_int
+            self.beta_R_konly_l[t_it-1]=beta_R_konly_l_int
+        elif type is 'spectral':
+            self.h=np.loadtxt(way+'/h_ve.dat',unpack=True)[:,:maxdeg]
+            self.h=self.h[1,:]+self.h[2,:]*1j
+            self.k=np.loadtxt(way+'/k_ve.dat',unpack=True)[:,:maxdeg]
+            self.k=self.k[1,:]+self.k[2,:]*1j
+            self.h_e=np.loadtxt(way+'/h_e.dat',unpack=True)[1,:maxdeg]
+            self.k_e=np.loadtxt(way+'/k_e.dat',unpack=True)[1,:maxdeg]
+            self.h_e[0]=0
+            self.k_e[0]=0
+            # self.h_e=np.abs(self.h)*np.exp(np.imag(self.h)/np.real(self.h))#-np.loadtxt(way+'/k_e.dat',unpack=True)[1,:maxdeg]
+            # self.k_e=np.abs(self.k)*np.exp(np.imag(self.k)/np.real(self.k))#-np.loadtxt(way+'/k_e.dat',unpack=True)[1,:maxdeg]
+            time_diff=np.repeat(self.time_step[::-1,np.newaxis],self.time_step_number,axis=1)-np.repeat(self.time_step[::-1,np.newaxis],self.time_step_number,axis=1).T
+            time_diff[time_diff<0]=0
+            # self.beta_R_l=np.repeat(np.repeat(self.h[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0)*np.exp(1j*2*np.pi/T*np.repeat(time_diff[:,:,np.newaxis],self.h.shape[0],axis=2))#-np.repeat(np.repeat(self.h_e[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0)
+            # self.beta_G_l=np.repeat(np.repeat(self.k[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0)*np.exp(1j*2*np.pi/T*np.repeat(time_diff[:,:,np.newaxis],self.k.shape[0],axis=2))#-np.repeat(np.repeat(self.k_e[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0)
+            # self.beta_R_l=np.real(np.repeat(np.repeat(self.h[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0)*np.exp(1j*2*np.pi/T*np.repeat(time_diff[:,:,np.newaxis],self.h.shape[0],axis=2)))#-np.repeat(np.repeat(self.h_e[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0)
+            # self.beta_G_l=np.real(np.repeat(np.repeat(self.k[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0)*np.exp(1j*2*np.pi/T*np.repeat(time_diff[:,:,np.newaxis],self.k.shape[0],axis=2)))#-np.repeat(np.repeat(self.k_e[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0)
+
+            Phi=np.imag(np.repeat(np.repeat(self.h[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0))/np.real(np.repeat(np.repeat(self.h[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0))
+
+
+            self.beta_R_l=np.real(np.abs(np.repeat(np.repeat(self.h[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0))*np.exp(1j*2*np.pi/T*np.repeat(time_diff[:,:,np.newaxis],self.h.shape[0],axis=2)+Phi))-np.repeat(np.repeat(self.h_e[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0)-np.abs(self.h)*np.exp(np.imag(self.h)/np.real(self.h))
+
+            self.beta_G_l=np.real(np.repeat(np.repeat(self.k[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0)*np.exp(1j*2*np.pi/T*np.repeat(time_diff[:,:,np.newaxis],self.k.shape[0],axis=2)+Phi))-np.repeat(np.repeat(self.k_e[np.newaxis,:],self.time_step_number,axis=0)[np.newaxis,:,:],self.time_step_number,axis=0)-np.abs(self.k)*np.exp(np.imag(self.k)/np.real(self.k))
+
+            self.beta_G_l[0,:,0]=0
+            self.beta_G_l[0,0,:]=0
+            self.beta_l=self.beta_G_l-self.beta_R_l
+            calc_beta_counter(self,maxdeg)
+
+
+    def dev_beta(self,applied='beta'):
+        '''
+        The _`dev_beta` method can be used to rise the love numbers to their full shape to fit the computation method. This is required before using the beta in the methods from :ref:`LOAD <LOAD>`.
+
+        Attribute
+        ---------
+            applied : str
+                The kinf of beta you are calculating. Three values are possible : beta, beta_R et beta_G. 'beta' define the love numbers used to caculate the variation of ocean thickness. 'beta_R' define the love numbers used to calculate the variation of groud. 'beta_G' define the love numbers used to calculate the variation of geoïd. 
+        Return
+        ------
+            None
+
+        '''
+        if applied is 'beta':
+            self.beta_G=0
+            self.beta_R=0
+            self.beta_l=self.beta_G_l-self.beta_R_l
+            self.beta_l=np.array(self.beta_l)[:,:,self.beta_counter.astype(int)]
+        elif applied is 'beta_R':
+            self.beta_l=0
+            self.beta_G=0
+            self.beta_R=np.array(self.beta_R_l)[:,:,self.beta_counter.astype(int)]
+        elif applied is 'beta_G':
+            self.beta_l=0
+            self.beta_R=0
+            self.beta_G=np.array(self.beta_G_l)[:,:,self.beta_counter.astype(int)]
+
+    def dev_beta_tide(self,applied='beta'):
+        '''
+        The _`dev_beta_tide` method can be used to rise the love numbers to their full shape to fit the computation method. This is required before using the beta in the methods from :ref:`LOAD <LOAD>`.
+
+        Attribute
+        ---------
+            applied : str
+                The kinf of beta you are calculating. Three values are possible : beta, beta_R et beta_G. 'beta' define the love numbers used to caculate the variation of ocean thickness. 'beta_R' define the love numbers used to calculate the variation of groud. 'beta_G' define the love numbers used to calculate the variation of geoïd. 
+        Return
+        ------
+            None
+
+        '''
+        if applied is 'beta':
+            self.beta_G_tide=0
+            self.beta_R_tide=0
+            self.beta_l_tide=self.beta_G_l_tide-self.beta_R_l_tide
+            self._tide=np.array(self.beta_l)[:,:,self.beta_counter.astype(int)[:6]]
+        elif applied is 'beta_R':
+            self.beta_l_tide=0
+            self.beta_G_tide=0
+            self.beta_R_tide=np.array(self.beta_R_l_tide)[:,:,self.beta_counter.astype(int)[:6]]
+        elif applied is 'beta_G':
+            self.beta_l_tide=0
+            self.beta_R_tide=0
+            self.beta_G_tide=np.array(self.beta_G_l_tide)[:,:,self.beta_counter.astype(int)[:6]]
+    
+    def clean_memory(self):
+        '''
+        The _`clean_memory` method can be used to araise the beta_l, beta_R and beta_G to avoid memory issues. 
+
+        Attribute
+        ---------
+            None
+
+        Return
+        ------
+            None
+
+        '''
+        self.beta_l=0
+        self.beta_R=0
+        self.beta_G=0
```

### Comparing `slcode-0.4.1/src/SL_C0de/spharm.py` & `slcode-1.0.0/slcode/spharm.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-import numpy as np
-import math
-#import pyshtools as pysh #pyshtools is still necessary, even if i don't use the expend function (still need the legendre  polynome function)
-import sys
-import logging
-import pyshtools as pysh
-import pyshtools.expand as expand
-    
-def get_coeffs(a_lm,n):
-    '''
-    The _`get_coeffs` function get the spherical harmonics coefficients of the nth order from a linearly Spharm array.
-
-    Attribute : 
-    -----------
-        a_lm : np.array([maxdeg*(maxdeg+1)/2,])
-            An array containing the spherical coefficient in a linear form
-        n : int
-            The order of the spherical harmonics coefficient you are trying to retrive
-
-    Returns :
-    ---------  
-        a_n : np.array([n,])
-            The spherical harmonic coefficient of the order n.
-    '''
-    if n == 0 :
-        a_n = a_lm[0]
-    else :
-        gauss_sum = int(n*(n+1)/2)
-        # position of current order in a_lm vector
-        a_n = a_lm[gauss_sum:gauss_sum+n+1]
-    return a_n
-
-class sphericalobject(object):
-    """
-    The _`sphericalobject` class include any spherical object. This class is working with pyshtools (`pyshtools <https://shtools.github.io/SHTOOLS/>`_).
-
-    Attributes
-    ----------
-        grd : np.array[(maxdeg,maxdeg x2)]
-           Value of the spherical object on a Gaussian Grid. 
-        isgrd : Bool
-           A boolean to define if a Gaussian grid have been defined for this object. 
-        coeff : np.array[(maxdeg,maxdeg)]
-           Spherical harmonic coefficient array. 
-        iscoeff : Bool
-           A boolean to define if a spherical harmonic coefficient have been defined for this object.
-        saved : np.array[(n, maxdeg, maxdeg)]
-           An array wich contain the spherical harmonic coefficient each time th save method is applied.
-        prev : np.array[(maxedg, maxdeg)] 
-           save the spherical coefficient using save_prev. 
-
-    Methods
-    -------
-        `grdtocoeff`_ : 
-           Convert the Gaussian grid to spherical harmonic coefficient
-        `coefftogrd`_ : 
-           Convert spherical harmonic coefficient to Gaussian grid
-        `coefftogrdhd`_ :
-           Convert spherical harmonic coefficient to a Gaussian grid with a higher resolution then maxdeg
-        `save_prev`_ :
-           Save the spherical harmonic coefficient to the attribute prev
-        
-           
-    """
-    
-    def __init__(self,grd=None,coeff=None,maxdeg=None):
-        
-        if coeff is None : # initialize the grid if the entry is a grid
-            self.grd=grd.copy()
-            self.maxdeg=grd.shape[0]
-        elif grd is None: # initialize the coefficient if the entry is a coefficient
-            self.coeff=coeff.copy()
-            self.maxdeg=int(abs((-1+math.sqrt(1+8*len(coeff)))/2))
-        else :
-            self.maxdeg=maxdeg
-        
-    def grdtocoeff(self):
-        '''
-        The _`grdtocoeff` method convert a Gaussian grid into spherical harmonic coefficient array using a numerical method to create spherical harmonic coefficient
-        self.coeff is updated usig these output.
-        self.iscoeff defining if a coefficient have been created for this object. 
-        If there is no grid created (self.isgrid == 0) then it returns an error.
-    
-        Attribute :
-        ----------- 
-            None 
-        
-        Returns :
-        ---------
-            None        
-        '''
-        zero , w = expand.SHGLQ(self.maxdeg)
-        self.coeff=expand.SHExpandGLQ(self.grd,w,zero)
-        self.coeff=pysh.shio.SHCilmToCindex(self.coeff)
-        self.coeff=self.coeff[0]+self.coeff[1]*1j
-        self.iscoeff=True
-        return self
-                                                                                  
-    def coefftogrd(self):
-        '''
-        The _`coefftogrd` method convert spherical harmonic coefficient into a gird array using shtools.
-        The output of pysh.SHCoeff are converted to real.
-        self.grd is updated usig these output.
-        self.isgrd defining if a grid have been created for this object. 
-        If there is no grid created (self.iscoeff == 0) then it returns an error.
-        A modifier pour pouvoir modifier les entrées de la fonction.
-    
-        Parameters : 
-            
-        See the documentation of the cited class object for more information on different parameters used in the function.
-        
-        Returns : 
-        
-        Added fields : 
-
-        '''       
-        zero , w = expand.SHGLQ(self.maxdeg)
-        coeff=np.stack((self.coeff.real,self.coeff.imag))
-        coeff=pysh.shio.SHCindexToCilm(coeff)
-        self.grd=expand.MakeGridGLQ(coeff,zero,extend=1)
-        self.isgrd=True
-
-        return self
-    
-    def coefftogrdhd(self,max_calc_deg):
-        '''
-        The _`coefftogrdhd` convert spherical harmonic coefficient into a gird array using shtools.
-        The output of pysh.SHCoeff are converted to real.
-        self.grd is updated usig these output.
-        self.isgrd defining if a grid have been created for this object. 
-        If there is no grid created (self.iscoeff == 0) then it returns an error.
-        A modifier pour pouvoir modifier les entrées de la fonction.
-    
-        Attribute :
-        -----------
-            max_calc_deg : int
-                The maximum spherical harmonic degree to calculate the grid. This function can be used to have a better rendering in output.
-        
-        Returns :
-        ---------
-            None 
-        '''
-        
-        zero , w = expand.SHGLQ(max_calc_deg-1)
-        x_GL = np.arccos(zero[::-1])*180/math.pi - 90
-        lon_GL = np.linspace(0,360,2*(max_calc_deg)+1)
-        lon_GL = lon_GL[:-1]
-        lat_hd=x_GL
-        lon_hd=lon_GL
-        self.colats = 90 - self.lats
-        coeff=np.stack((self.coeff.real,self.coeff.imag))
-        coeff=pysh.shio.SHCindexToCilm(coeff)
-        return expand.MakeGridGLQ(coeff,zero,lmax=max_calc_deg-1,extend=1),lon_hd,lat_hd[::-1]
-    
-    # def multiply(self,coeff2):
-    #     '''
-    #     This function is no longer used !!!!    
-        
-    #     Multiply the spherical coefficient of a gird with the others. It could be done using the pysh.SHcoeffs.Multiply.
-    #     I choose to do it manually but i could test the efficiency of the pysh tool function. 
-    
-    #     Parameters : 
-    #         flm2 (np.array): the harmonic coefficient matrix of size maxdeg, maxdeg !!!! A vérifier !!!!!
-             
-    #     See the documentation of the cited class object for more information on different parameters used in the function.
-        
-    #     Returns : 
-    #         flm[0,:,:]+1j*flm[1,:,:] (np.array): the harmonic coefficient matrix resulting of the multiplication of the two grids. 
-    #         size maxdeg, maxdeg !!!! A vérifier !!!!
-            
-    #     Added fields : 
-
-    #     '''
-    #     # convert two spherical coefficient into gaussian grid.
-    #     coeff1=np.stack((self.coeff.real,self.coeff.imag))
-    #     coeff1=pysh.shio.SHCindexToCilm(coeff1)
-    #     coeff2=np.stack((coeff2.real,coeff2.imag))
-    #     coeff2=pysh.shio.SHCindexToCilm(coeff2)
-    #     coeff=pysh.expand.SHMultiply(coeff1,coeff2)
-    #     coeff=pysh.shio.SHCilmToCindex(coeff)
-    #     coeff=coeff[0]+coeff[1]*1j
-    #     return coeff[:int((self.maxdeg*(self.maxdeg+1))/2)]
-    
-    # def calculate_value_at_point(self,phi,theta):
-    #     Y_lm=(pysh.expand.spharm(self.maxdeg,theta,phi,packed=True)[0]+pysh.expand.spharm(self.maxdeg,theta,phi,packed=True)[1]*1j)
-    #     return np.dot(self.coeff,Y_lm)
-    
-    def save_prev(self):
-        '''
-        The _`save_prev` create a new field for the object to save the spherical coefficient at the moment of the applied function. 
-        This function make a clean copy of the array to avoid modification. 
-    
-        Attribute :
-        -----------
-            None 
-        
-        Returns :
-        --------- 
-            None
-        '''
-        if not(self.coeff is None) : # if there is spherical coefficient for this object copy these coefficient to self.prev
-            self.prev=self.coeff.copy()
-        else : # else retrun an error
-            logging.error('error: ', "No coeff created for this spherical object. Check if you have created the object with coeff or haven't run the grdtocoeff() method")
-            sys.exit(1)
-        return self
+import numpy as np
+import math
+#import pyshtools as pysh #pyshtools is still necessary, even if i don't use the expend function (still need the legendre  polynome function)
+import sys
+import logging
+import pyshtools as pysh
+import pyshtools.expand as expand
+    
+def get_coeffs(a_lm,n):
+    '''
+    The _`get_coeffs` function get the spherical harmonics coefficients of the nth order from a linearly Spharm array.
+
+    Attribute : 
+    -----------
+        a_lm : np.array([maxdeg*(maxdeg+1)/2,])
+            An array containing the spherical coefficient in a linear form
+        n : int
+            The order of the spherical harmonics coefficient you are trying to retrive
+
+    Returns :
+    ---------  
+        a_n : np.array([n,])
+            The spherical harmonic coefficient of the order n.
+    '''
+    if n == 0 :
+        a_n = a_lm[0]
+    else :
+        gauss_sum = int(n*(n+1)/2)
+        # position of current order in a_lm vector
+        a_n = a_lm[gauss_sum:gauss_sum+n+1]
+    return a_n
+
+class sphericalobject(object):
+    """
+    The _`sphericalobject` class include any spherical object. This class is working with pyshtools (`pyshtools <https://shtools.github.io/SHTOOLS/>`_).
+
+    Attributes
+    ----------
+        grd : np.array[(maxdeg,maxdeg x2)]
+           Value of the spherical object on a Gaussian Grid. 
+        isgrd : Bool
+           A boolean to define if a Gaussian grid have been defined for this object. 
+        coeff : np.array[(maxdeg,maxdeg)]
+           Spherical harmonic coefficient array. 
+        iscoeff : Bool
+           A boolean to define if a spherical harmonic coefficient have been defined for this object.
+        saved : np.array[(n, maxdeg, maxdeg)]
+           An array wich contain the spherical harmonic coefficient each time th save method is applied.
+        prev : np.array[(maxedg, maxdeg)] 
+           save the spherical coefficient using save_prev. 
+
+    Methods
+    -------
+        `grdtocoeff`_ : 
+           Convert the Gaussian grid to spherical harmonic coefficient
+        `coefftogrd`_ : 
+           Convert spherical harmonic coefficient to Gaussian grid
+        `coefftogrdhd`_ :
+           Convert spherical harmonic coefficient to a Gaussian grid with a higher resolution then maxdeg
+        `save_prev`_ :
+           Save the spherical harmonic coefficient to the attribute prev
+        
+           
+    """
+    
+    def __init__(self,grd=None,coeff=None,maxdeg=None):
+        
+        if coeff is None : # initialize the grid if the entry is a grid
+            self.grd=grd.copy()
+            self.maxdeg=grd.shape[0]
+        elif grd is None: # initialize the coefficient if the entry is a coefficient
+            self.coeff=coeff.copy()
+            self.maxdeg=int(abs((-1+math.sqrt(1+8*len(coeff)))/2))
+        else :
+            self.maxdeg=maxdeg
+        
+    def grdtocoeff(self):
+        '''
+        The _`grdtocoeff` method convert a Gaussian grid into spherical harmonic coefficient array using a numerical method to create spherical harmonic coefficient
+        self.coeff is updated usig these output.
+        self.iscoeff defining if a coefficient have been created for this object. 
+        If there is no grid created (self.isgrid == 0) then it returns an error.
+    
+        Attribute :
+        ----------- 
+            None 
+        
+        Returns :
+        ---------
+            None        
+        '''
+        zero , w = expand.SHGLQ(self.maxdeg)
+        self.coeff=expand.SHExpandGLQ(self.grd,w,zero)
+        self.coeff=pysh.shio.SHCilmToCindex(self.coeff)
+        self.coeff=self.coeff[0]+self.coeff[1]*1j
+        self.iscoeff=True
+        return self
+                                                                                  
+    def coefftogrd(self):
+        '''
+        The _`coefftogrd` method convert spherical harmonic coefficient into a gird array using shtools.
+        The output of pysh.SHCoeff are converted to real.
+        self.grd is updated usig these output.
+        self.isgrd defining if a grid have been created for this object. 
+        If there is no grid created (self.iscoeff == 0) then it returns an error.
+        A modifier pour pouvoir modifier les entrées de la fonction.
+    
+        Parameters : 
+            
+        See the documentation of the cited class object for more information on different parameters used in the function.
+        
+        Returns : 
+        
+        Added fields : 
+
+        '''       
+        zero , w = expand.SHGLQ(self.maxdeg)
+        coeff=np.stack((self.coeff.real,self.coeff.imag))
+        coeff=pysh.shio.SHCindexToCilm(coeff)
+        self.grd=expand.MakeGridGLQ(coeff,zero,extend=1)
+        self.isgrd=True
+
+        return self
+    
+    def coefftogrdhd(self,max_calc_deg):
+        '''
+        The _`coefftogrdhd` convert spherical harmonic coefficient into a gird array using shtools.
+        The output of pysh.SHCoeff are converted to real.
+        self.grd is updated usig these output.
+        self.isgrd defining if a grid have been created for this object. 
+        If there is no grid created (self.iscoeff == 0) then it returns an error.
+        A modifier pour pouvoir modifier les entrées de la fonction.
+    
+        Attribute :
+        -----------
+            max_calc_deg : int
+                The maximum spherical harmonic degree to calculate the grid. This function can be used to have a better rendering in output.
+        
+        Returns :
+        ---------
+            None 
+        '''
+        
+        zero , w = expand.SHGLQ(max_calc_deg-1)
+        x_GL = np.arccos(zero[::-1])*180/math.pi - 90
+        lon_GL = np.linspace(0,360,2*(max_calc_deg)+1)
+        lon_GL = lon_GL[:-1]
+        lat_hd=x_GL
+        lon_hd=lon_GL
+        self.colats = 90 - self.lats
+        coeff=np.stack((self.coeff.real,self.coeff.imag))
+        coeff=pysh.shio.SHCindexToCilm(coeff)
+        return expand.MakeGridGLQ(coeff,zero,lmax=max_calc_deg-1,extend=1),lon_hd,lat_hd[::-1]
+    
+    # def multiply(self,coeff2):
+    #     '''
+    #     This function is no longer used !!!!    
+        
+    #     Multiply the spherical coefficient of a gird with the others. It could be done using the pysh.SHcoeffs.Multiply.
+    #     I choose to do it manually but i could test the efficiency of the pysh tool function. 
+    
+    #     Parameters : 
+    #         flm2 (np.array): the harmonic coefficient matrix of size maxdeg, maxdeg !!!! A vérifier !!!!!
+             
+    #     See the documentation of the cited class object for more information on different parameters used in the function.
+        
+    #     Returns : 
+    #         flm[0,:,:]+1j*flm[1,:,:] (np.array): the harmonic coefficient matrix resulting of the multiplication of the two grids. 
+    #         size maxdeg, maxdeg !!!! A vérifier !!!!
+            
+    #     Added fields : 
+
+    #     '''
+    #     # convert two spherical coefficient into gaussian grid.
+    #     coeff1=np.stack((self.coeff.real,self.coeff.imag))
+    #     coeff1=pysh.shio.SHCindexToCilm(coeff1)
+    #     coeff2=np.stack((coeff2.real,coeff2.imag))
+    #     coeff2=pysh.shio.SHCindexToCilm(coeff2)
+    #     coeff=pysh.expand.SHMultiply(coeff1,coeff2)
+    #     coeff=pysh.shio.SHCilmToCindex(coeff)
+    #     coeff=coeff[0]+coeff[1]*1j
+    #     return coeff[:int((self.maxdeg*(self.maxdeg+1))/2)]
+    
+    # def calculate_value_at_point(self,phi,theta):
+    #     Y_lm=(pysh.expand.spharm(self.maxdeg,theta,phi,packed=True)[0]+pysh.expand.spharm(self.maxdeg,theta,phi,packed=True)[1]*1j)
+    #     return np.dot(self.coeff,Y_lm)
+    
+    def save_prev(self):
+        '''
+        The _`save_prev` create a new field for the object to save the spherical coefficient at the moment of the applied function. 
+        This function make a clean copy of the array to avoid modification. 
+    
+        Attribute :
+        -----------
+            None 
+        
+        Returns :
+        --------- 
+            None
+        '''
+        if not(self.coeff is None) : # if there is spherical coefficient for this object copy these coefficient to self.prev
+            self.prev=self.coeff.copy()
+        else : # else retrun an error
+            logging.error('error: ', "No coeff created for this spherical object. Check if you have created the object with coeff or haven't run the grdtocoeff() method")
+            sys.exit(1)
+        return self
```

### Comparing `slcode-0.4.1/src/slcode.egg-info/PKG-INFO` & `slcode-1.0.0/slcode.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,33 @@
-Metadata-Version: 2.1
-Name: slcode
-Version: 0.4.1
-Summary: SL_C0de is a python library based on the matlab code SL_code. This module is used to calculate GIA over the world but alse the sediment isostasy. It include function to calculate radial symetric auto gravitational earth visco-elastic response. This module also include the possibility to resolve the Sea level equation based on the publication of Mitrovica and Austermann ... ajouter des refs. The aim of this library is to be easy to include new sources of load and link to other python library.
-Author-email: HENRY-LARROZE Adrien <adrien.henry@univ-lr.fr>
-Project-URL: Homepage, https://github.com/AHenryLarroze/Py_SL_C0de
-Project-URL: Bug Tracker, https://github.com/AHenryLarroze/Py_SL_C0de/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENCE.md
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: pyshtools
-Requires-Dist: matplotlib
-
-version 0.1.0 First realise of the library. 
-version 0.2.0 Paralelisation of several functions in the code. 
-version 0.3.0 Modification of the code to decompose the perturbation of the Sea level.
-version 0.3.1 New love number importation based on love numbers calculated by ALMA3
-version 0.3.2 Output function added as a csv writer for using in other application
-version 0.3.3 Add of the sediment import as in the matlab code
-version 0.3.4 Revision of the code to calculate the ground motion at the end of the computation
-version 0.3.5 Integration of saving and loading data from previous run
+Metadata-Version: 2.1
+Name: slcode
+Version: 1.0.0
+Summary: SL_C0de is a python library based on the matlab code SL_code. This module is used to calculate GIA over the world but alse the sediment isostasy. It include function to calculate radial symetric auto gravitational earth visco-elastic response. This module also include the possibility to resolve the Sea level equation based on the publication of Mitrovica and Austermann ... ajouter des refs. The aim of this library is to be easy to include new sources of load and link to other python library.
+Home-page: https://github.com/AHenryLarroze/Py_SL_C0de
+Author: Adrien Henry-Larroze
+Author-email: adrien_henry@orange.fr
+License: GPL-3.0
+Project-URL: Homepage, https://py-sl-c0de.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/AHenryLarroze/Py_SL_C0de
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENCE.md
+Requires-Dist: joblib==1.2.0
+Requires-Dist: matplotlib==3.7.0
+Requires-Dist: numpy==1.24.2
+Requires-Dist: plotly==5.13.0
+Requires-Dist: pyshtools==4.10.1
+Requires-Dist: scipy==1.10.0
+Requires-Dist: sphinx_rtd_theme==1.2.0
+Requires-Dist: tomli==2.0.1
+Requires-Dist: stripy==2.2
+Requires-Dist: netcdf4==1.6.2
+Requires-Dist: jupyter==1.0.0
+
+SL_C0de
+=======
+
+**SL_C0de** (/lu'make/) is a python library based on the matlab code SL_code. This module allows to calculate GIA over the world but also the sediment isostasy. It includes function to calculate radial symetric auto gravitational earth visco-elastic response. This module also includes the option to resolve the Sea level equation. This library has been benchmarked with the following Matlab code (jaustermann/SLcode/tree/master/GRL_2022_proglacial_lakes).The aim of this library is to be easy to include new sources of load and can be linked to other python library.
+
+documentation :
```

