# Comparing `tmp/pytexmk-0.5.1.240426.tar.gz` & `tmp/pytexmk-0.5.4.240427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytexmk-0.5.1.240426.tar", last modified: Fri Apr 26 15:20:15 2024, max compression
+gzip compressed data, was "pytexmk-0.5.4.240427.tar", last modified: Sat Apr 27 03:11:24 2024, max compression
```

## Comparing `pytexmk-0.5.1.240426.tar` & `pytexmk-0.5.4.240427.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 15:20:15.165012 pytexmk-0.5.1.240426/
--rw-rw-r--   0 yanming   (1000) yanming   (1000)    35149 2024-02-28 15:10:35.000000 pytexmk-0.5.1.240426/LICENSE
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       30 2024-03-06 03:27:48.000000 pytexmk-0.5.1.240426/MANIFEST.in
--rw-rw-r--   0 yanming   (1000) yanming   (1000)      466 2024-03-06 03:27:48.000000 pytexmk-0.5.1.240426/Makefile
--rw-r--r--   0 yanming   (1000) yanming   (1000)     9034 2024-04-26 15:20:15.165012 pytexmk-0.5.1.240426/PKG-INFO
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     7988 2024-04-26 14:37:00.000000 pytexmk-0.5.1.240426/README.md
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     1195 2024-03-21 15:51:11.000000 pytexmk-0.5.1.240426/pyproject.toml
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       38 2024-04-26 15:20:15.165012 pytexmk-0.5.1.240426/setup.cfg
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 15:20:15.161012 pytexmk-0.5.1.240426/src/
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 15:20:15.161012 pytexmk-0.5.1.240426/src/pytexmk/
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     1940 2024-02-29 11:40:30.000000 pytexmk-0.5.1.240426/src/pytexmk/__init__.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)    11497 2024-04-26 15:19:03.000000 pytexmk-0.5.1.240426/src/pytexmk/__main__.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)    10250 2024-04-26 15:10:42.000000 pytexmk-0.5.1.240426/src/pytexmk/additional_operation.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     9922 2024-03-22 06:51:11.000000 pytexmk-0.5.1.240426/src/pytexmk/compile_model.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     5896 2024-03-22 06:50:52.000000 pytexmk-0.5.1.240426/src/pytexmk/info_print.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     1922 2024-04-26 15:19:26.000000 pytexmk-0.5.1.240426/src/pytexmk/version.py
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 15:20:15.165012 pytexmk-0.5.1.240426/src/pytexmk.egg-info/
--rw-r--r--   0 yanming   (1000) yanming   (1000)     9034 2024-04-26 15:20:15.000000 pytexmk-0.5.1.240426/src/pytexmk.egg-info/PKG-INFO
--rw-rw-r--   0 yanming   (1000) yanming   (1000)      441 2024-04-26 15:20:15.000000 pytexmk-0.5.1.240426/src/pytexmk.egg-info/SOURCES.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)        1 2024-04-26 15:20:15.000000 pytexmk-0.5.1.240426/src/pytexmk.egg-info/dependency_links.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       41 2024-04-26 15:20:15.000000 pytexmk-0.5.1.240426/src/pytexmk.egg-info/entry_points.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       13 2024-04-26 15:20:15.000000 pytexmk-0.5.1.240426/src/pytexmk.egg-info/requires.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)        8 2024-04-26 15:20:15.000000 pytexmk-0.5.1.240426/src/pytexmk.egg-info/top_level.txt
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 15:20:15.165012 pytexmk-0.5.1.240426/tests/
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     9643 2024-03-22 06:30:29.000000 pytexmk-0.5.1.240426/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:11:24.246015 pytexmk-0.5.4.240427/
+-rw-rw-rw-   0        0        0    35823 2024-03-01 02:38:22.000000 pytexmk-0.5.4.240427/LICENSE
+-rw-rw-rw-   0        0        0       31 2024-03-04 05:22:02.000000 pytexmk-0.5.4.240427/MANIFEST.in
+-rw-rw-rw-   0        0        0      945 2024-04-27 03:10:22.000000 pytexmk-0.5.4.240427/Makefile
+-rw-rw-rw-   0        0        0     9479 2024-04-27 03:11:24.243019 pytexmk-0.5.4.240427/PKG-INFO
+-rw-rw-rw-   0        0        0     8407 2024-04-27 02:11:09.000000 pytexmk-0.5.4.240427/README.md
+-rw-rw-rw-   0        0        0     1232 2024-04-04 02:04:13.000000 pytexmk-0.5.4.240427/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 03:11:24.247073 pytexmk-0.5.4.240427/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 03:11:24.163851 pytexmk-0.5.4.240427/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 03:11:24.208014 pytexmk-0.5.4.240427/src/pytexmk/
+-rw-rw-rw-   0        0        0     1975 2024-03-01 02:38:22.000000 pytexmk-0.5.4.240427/src/pytexmk/__init__.py
+-rw-rw-rw-   0        0        0    11676 2024-04-27 02:17:13.000000 pytexmk-0.5.4.240427/src/pytexmk/__main__.py
+-rw-rw-rw-   0        0        0    10693 2024-04-27 02:17:54.000000 pytexmk-0.5.4.240427/src/pytexmk/additional_operation.py
+-rw-rw-rw-   0        0        0    10114 2024-04-04 02:04:13.000000 pytexmk-0.5.4.240427/src/pytexmk/compile_model.py
+-rw-rw-rw-   0        0        0     6013 2024-04-04 02:04:13.000000 pytexmk-0.5.4.240427/src/pytexmk/info_print.py
+-rw-rw-rw-   0        0        0     1951 2024-04-27 02:11:19.000000 pytexmk-0.5.4.240427/src/pytexmk/version.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:11:24.240015 pytexmk-0.5.4.240427/src/pytexmk.egg-info/
+-rw-rw-rw-   0        0        0     9479 2024-04-27 03:11:24.000000 pytexmk-0.5.4.240427/src/pytexmk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2024-04-27 03:11:24.000000 pytexmk-0.5.4.240427/src/pytexmk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 03:11:24.000000 pytexmk-0.5.4.240427/src/pytexmk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-27 03:11:24.000000 pytexmk-0.5.4.240427/src/pytexmk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2024-04-27 03:11:24.000000 pytexmk-0.5.4.240427/src/pytexmk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 03:11:24.000000 pytexmk-0.5.4.240427/src/pytexmk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 03:11:24.236027 pytexmk-0.5.4.240427/tests/
+-rw-rw-rw-   0        0        0     9852 2024-04-04 02:04:13.000000 pytexmk-0.5.4.240427/tests/test.py
```

### Comparing `pytexmk-0.5.1.240426/LICENSE` & `pytexmk-0.5.4.240427/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
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
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
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
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `pytexmk-0.5.1.240426/PKG-INFO` & `pytexmk-0.5.4.240427/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,152 +1,158 @@
-Metadata-Version: 2.1
-Name: pytexmk
-Version: 0.5.1.240426
-Summary: LaTeX 辅助编译命令行工具 LaTeX Auxiliary Compilation Command Line Tool
-Author-email: 焱铭 <lxb-yanming@foxmail.com>
-Project-URL: Homepage, https://github.com/YanMing-lxb/PyTeXMK
-Project-URL: Bug Tracker, https://github.com/YanMing-lxb/PyTeXMK/issues
-Keywords: LaTeX,build,latexmk
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers 
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: rich
-Requires-Dist: pymupdf
-
-<!--
- *  =======================================================================
- *  ····Y88b···d88P················888b·····d888·d8b·······················
- *  ·····Y88b·d88P·················8888b···d8888·Y8P·······················
- *  ······Y88o88P··················88888b·d88888···························
- *  ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
- *  ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
- *  ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
- *  ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
- *  ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
- *  ·······························································888·····
- *  ··························································Y8b·d88P·····
- *  ···························································"Y88P"······
- *  =======================================================================
- * 
- *  -----------------------------------------------------------------------
- * Author       : 焱铭
- * Date         : 2024-02-29 10:23:19 +0800
- * LastEditTime : 2024-04-26 22:37:00 +0800
- * Github       : https://github.com/YanMing-lxb/
- * FilePath     : /PyTeXMK/README.md
- * Description  : 
- *  -----------------------------------------------------------------------
- -->
-
-# PyTeXMK
-
-[![GitHub](https://img.shields.io/badge/Github-PyTeXMK-000000.svg)](https://github.com/YanMing-lxb/PyTeXMK) [![License](https://img.shields.io/badge/license-GPLv3-aff)](https://www.latex-project.org/lppl/) ![OS](https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg) [![GitHub release](https://img.shields.io/github/release/YanMing-lxb/PyTeXMK.svg?color=blueviolet&label=version&style=popout)](https://github.com/YanMing-lxb/PyTeXMK/releases/latest) [![Last Commit](https://img.shields.io/github/last-commit/YanMing-lxb/PyTeXMK)](https://github.com/YanMing-lxb/PyTeXMK/zipball/master) [![Issues](https://img.shields.io/github/issues/YanMing-lxb/PyTeXMK)](https://github.com/YanMing-lxb/PyTeXMK/issues) [![Github Action](https://github.com/YanMing-lxb/PyTeXMK/workflows/Test/badge.svg)](https://github.com/YanMing-lxb/PyTeXMK/actions) [![PyPI version](https://img.shields.io/pypi/v/pytexmk.svg)](https://pypi.python.org/pypi/pytexmk/) [![PyPI Downloads](https://img.shields.io/pypi/dm/pytexmk.svg?label=PyPI%20downloads)](https://pypi.org/project/pytexmk/) ![GitHub repo size](https://img.shields.io/github/repo-size/YanMing-lxb/PyTeXMK)
-
-LaTeX 辅助编译命令行程序 LaTeX Auxiliary Compilation Command Line Tool
-
----
-
-## 安装
-
-官方版本 PyTeXMK 发布在 [PyPI](https://pypi.org/project/pytexmk/) 上，并且可以通过 pip 包管理器从 PyPI 镜像轻松安装。
-
-请注意，您必须使用 Python 3 版本pip：
-
-```
-pip3 install pytexmk
-```
-
-## 升级
-
-```
-pip3 install --upgrade pytexmk
-```
-
-## 使用入门
-
-PyTeXMK 默认参数：`xelatex` 编译、主文件名 main、batch 模式（编译过程信息不显，如需显示编译过程信息请使用 `-nq` 参数）、编译结果存放在 LaTeX 项目的 Build 文件夹下 ( VSCode 用户则需要在 `settings.json` 中注意设置 `"latex-workshop.latex.outDir": "./Build",` 使得latex workshop 能够找到pdf )。
-
-请仔细阅读：[主文件及编译类型选定逻辑](#主文件及编译类型选定逻辑)
-
-### 编译命令
-PyTeXMK 支持：
-
-- 编译命令：`xelatex` `pdflatex` `lualatex`
-- 参考文献：`bibtex` `biblatex` `thebibliography`
-- 符号索引：`glossaries` `nomencl` `mkeidx`
-
-位置参数:
-| Option              | Description                    |
-|---------------------|-------------------------------|
-| document          | 要被编译的文件名                   |
-
-选项:
-| Option           | Description                                |
-|------------------|--------------------------------------------|
-| -h, --help       | 显示帮助信息                                 |
-| -v, --version    | 显示程序版本号                               |
-| -p, --pdflatex   | pdflatex 进行编译                           |
-| -x, --xelatex    | xelatex 进行编译                            |
-| -l, --lualatex   | lualatex 进行编译                           |
-| -c, --clean      | 清除所有辅助文件                              |
-| -C, --Clean      | 清除所有辅助文件和 pdf 文件                    |
-| -nq, --no-quiet  | 非安静模式运行，此模式下显示编译过程             |
-| -cp, --clean-pdf  | 清理所有 pdf 文件             |
-
-**说明：**
-`-cp` 参数的功能是 "当 LaTeX 编译过程中报类似 `invalid X X R object at offset XXXXX` 的警告时，可使用此参数清理所有 pdf 文件"
-
-### 魔法注释
-
-PyTeXMK 支持使用魔法注释来自定义编译命令、编译类型、编译结果存放位置等。    
-
-| Magic Comment | Description                                |
-|---------------|----------|
-| `% !TEX program = xelatex` | 指定编译类型，可选 `xelatex` `pdflatex` `lualatex` |
-| `% !TEX root = file.tex` | 指定主 LaTeX 文件名，仅支持主文件在项目根目录下的情况 |
-| `% !TEX outdir = PDFfile` | 指定编译结果存放位置，仅支持文件夹名称，如果使用 LaTeX-Workshop，则需要在 `settings.json` 中设置 `"latex-workshop.latex.outDir": "./PDFfile",` |
-
-### 主文件及编译类型选定逻辑
-- PyTeXMK 优先使用终端输入命令 `-p` `-x` `-l` 参数指定的编译类型，如果没有指定，则会使用 `% !TEX program = xelatex` 指定的编译类型，如果没有指定，则会使用默认的编译类型 `xelatex`
-- PyTeXMK 主文件选定逻辑顺序：
-    1. 使用终端输入的文件名
-    2. 使用 `% !TEX root = file.tex` 指定的主 LaTeX 文件名
-    3. 使用默认的主文件名 `main`
-    4. 检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
-    5. 根目录下 TeX 文件中只有一个文件，则选择该文件作为主文件
-        
-- PyTeXMK 会优先使用 `% !TEX outdir = PDFfile` 指定的编译结果存放位置，如果没有指定，则会使用默认的编译结果存放位置 `Build`
-
-# 更新日志
-
-- 2024-03-22 完善编译过程出错后的中断处理机制：在编译过程中出现错误时，程序会自动中断，并提示 `请用 -nq 模式运行以显示错误信息！`,使用 `-nq` 参数运行时，则会显示错误信息。
-- 2024-04-26 增加：
-    1. 魔法注释功能，使得用户可以自定义编译命令、编译类型、编译结果存放位置等
-    2. 完善主文件及编译类型选定逻辑
-
-
-# 未来工作方向
-
-- [X] 完善编译过程出错后的中断处理机制
-- [ ] 完善检索主 LaTeX 文件的功能：
-    - [X] 根据魔法注释 `% !TEX root = file.tex` 找到主 LaTeX 文件
-    - [ ] 通过检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
-- [ ] 完善自动判断编译类型：
-    - [X] 根据魔法注释 `% !TEX program = xelatex` 设置需要编译的类型
-- [x] 通过魔法注释设置编译结果存放位置
-- [X] 通过魔法注释实现编译命令的自定义
-- [ ] 增加配置文件功能，用于改变默认设置
-    - [ ] 指定生成的结果文件存放位置（目前默认存放在 `Build` 子文件夹下）
-    - [ ] 默认的编译命令（目前默认编译命令是 `xelatex`）
-- [ ] texlive 宏包检缺失并自动安装
-- [ ] 多主文件编译功能
+Metadata-Version: 2.1
+Name: pytexmk
+Version: 0.5.4.240427
+Summary: LaTeX 辅助编译命令行工具 LaTeX Auxiliary Compilation Command Line Tool
+Author-email: 焱铭 <lxb-yanming@foxmail.com>
+Project-URL: Homepage, https://github.com/YanMing-lxb/PyTeXMK
+Project-URL: Bug Tracker, https://github.com/YanMing-lxb/PyTeXMK/issues
+Keywords: LaTeX,build,latexmk
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers 
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: rich
+Requires-Dist: pymupdf
+
+<!--
+ *  =======================================================================
+ *  ····Y88b···d88P················888b·····d888·d8b·······················
+ *  ·····Y88b·d88P·················8888b···d8888·Y8P·······················
+ *  ······Y88o88P··················88888b·d88888···························
+ *  ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
+ *  ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
+ *  ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
+ *  ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
+ *  ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
+ *  ·······························································888·····
+ *  ··························································Y8b·d88P·····
+ *  ···························································"Y88P"······
+ *  =======================================================================
+ * 
+ *  -----------------------------------------------------------------------
+ * Author       : 焱铭
+ * Date         : 2024-02-29 10:23:19 +0800
+ * LastEditTime : 2024-04-27 10:10:51 +0800
+ * Github       : https://github.com/YanMing-lxb/
+ * FilePath     : \PyTeXMK\README.md
+ * Description  : 
+ *  -----------------------------------------------------------------------
+ -->
+
+# PyTeXMK
+
+[![GitHub](https://img.shields.io/badge/Github-PyTeXMK-000000.svg)](https://github.com/YanMing-lxb/PyTeXMK) [![License](https://img.shields.io/badge/license-GPLv3-aff)](https://www.latex-project.org/lppl/) ![OS](https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg) [![GitHub release](https://img.shields.io/github/release/YanMing-lxb/PyTeXMK.svg?color=blueviolet&label=version&style=popout)](https://github.com/YanMing-lxb/PyTeXMK/releases/latest) [![Last Commit](https://img.shields.io/github/last-commit/YanMing-lxb/PyTeXMK)](https://github.com/YanMing-lxb/PyTeXMK/zipball/master) [![Issues](https://img.shields.io/github/issues/YanMing-lxb/PyTeXMK)](https://github.com/YanMing-lxb/PyTeXMK/issues) [![Github Action](https://github.com/YanMing-lxb/PyTeXMK/workflows/Test/badge.svg)](https://github.com/YanMing-lxb/PyTeXMK/actions) [![PyPI version](https://img.shields.io/pypi/v/pytexmk.svg)](https://pypi.python.org/pypi/pytexmk/) [![PyPI Downloads](https://img.shields.io/pypi/dm/pytexmk.svg?label=PyPI%20downloads)](https://pypi.org/project/pytexmk/) ![GitHub repo size](https://img.shields.io/github/repo-size/YanMing-lxb/PyTeXMK)
+
+LaTeX 辅助编译命令行程序 LaTeX Auxiliary Compilation Command Line Tool
+
+---
+
+## 安装
+
+官方版本 PyTeXMK 发布在 [PyPI](https://pypi.org/project/pytexmk/) 上，并且可以通过 pip 包管理器从 PyPI 镜像轻松安装。
+
+请注意，您必须使用 Python 3 版本pip：
+
+```
+pip3 install pytexmk
+```
+
+## 升级
+
+```
+pip3 install --upgrade pytexmk
+```
+
+## 使用入门
+
+PyTeXMK 默认参数：`xelatex` 编译、主文件名 main.tex、batch 模式（编译过程信息不显，如需显示编译过程信息请使用 `-nq` 参数）、编译结果存放在 LaTeX 项目的 Build 文件夹下 ( VSCode 用户则需要在 `settings.json` 中注意设置 `"latex-workshop.latex.outDir": "./Build",` 使得 LaTeX-Workshop 能够找到 pdf )。
+
+请仔细阅读：[主文件及编译类型选定逻辑](#主文件及编译类型选定逻辑)
+
+> PyTeXMK，仅支持 utf-8 编码的 TeX 文件。
+
+### 编译命令
+PyTeXMK 支持：
+
+- 编译命令：`xelatex` `pdflatex` `lualatex`
+- 参考文献：`bibtex` `biblatex` `thebibliography`
+- 符号索引：`glossaries` `nomencl` `mkeidx`
+
+位置参数:
+| Option              | Description                    |
+|---------------------|-------------------------------|
+| document          | 要被编译的文件名                   |
+
+选项:
+| Option           | Description                                |
+|------------------|--------------------------------------------|
+| -h, --help       | 显示帮助信息                                 |
+| -v, --version    | 显示程序版本号                               |
+| -p, --pdflatex   | pdflatex 进行编译                           |
+| -x, --xelatex    | xelatex 进行编译                            |
+| -l, --lualatex   | lualatex 进行编译                           |
+| -c, --clean      | 清除所有辅助文件                              |
+| -C, --Clean      | 清除所有辅助文件和 pdf 文件                    |
+| -nq, --no-quiet  | 非安静模式运行，此模式下显示编译过程             |
+| -cp, --clean-pdf  | 清理所有 pdf 文件                          |
+
+**说明：**
+`-cp` 参数的功能是 "当 LaTeX 编译过程中报类似 `invalid X X R object at offset XXXXX` 的警告时，可使用此参数清理所有 pdf 文件"
+
+### 魔法注释
+
+PyTeXMK 支持使用魔法注释来自定义编译命令、编译类型、编译结果存放位置等（仅支持检索文档前 50 行）。    
+
+| Magic Comment | Description                                |
+|---------------|----------|
+| `% !TEX program = xelatex` | 指定编译类型，可选 `xelatex` `pdflatex` `lualatex` |
+| `% !TEX root = file.tex` | 指定主 LaTeX 文件名，仅支持主文件在项目根目录下的情况 |
+| `% !TEX outdir = PDFfile` | 指定编译结果存放位置，仅支持文件夹名称，如果使用 LaTeX-Workshop，则需要在 `settings.json` 中设置 `"latex-workshop.latex.outDir": "./PDFfile",` |
+
+### 主文件及编译类型选定逻辑
+
+- PyTeXMK 优先使用终端输入命令 `-p` `-x` `-l` 参数指定的编译类型，如果没有指定，则会使用 `% !TEX program = xelatex` 指定的编译类型，如果没有指定，则会使用默认的编译类型 `xelatex`
+- PyTeXMK 主文件选定逻辑顺序：
+    1. 使用终端输入的文件名
+    2. 使用 `% !TEX root = file.tex` 指定的主 LaTeX 文件名
+    3. 使用默认的主文件名 `main.tex`
+    4. 检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断（仅支持检索文档前 200 行）
+    5. 根目录下 TeX 文件中只有一个文件，则选择该文件作为主文件
+        
+- PyTeXMK 会优先使用 `% !TEX outdir = PDFfile` 指定的编译结果存放位置，如果没有指定，则会使用默认的编译结果存放位置 `Build`
+
+# 更新日志
+
+- 2024-03-22 完善编译过程出错后的中断处理机制：在编译过程中出现错误时，程序会自动中断，并提示 `请用 -nq 模式运行以显示错误信息！`，使用 `-nq` 参数运行时，则会显示错误信息。
+- 2024-04-26 增加：
+    1. 魔法注释功能，使得用户可以自定义编译命令、编译类型、编译结果存放位置等
+    2. 完善主文件及编译类型选定逻辑
+- 2024-04-26 
+    1. 修复边 \documentclass 和 \begin{document} 检索逻辑。
+    2. 解决文档读取编码导致的报错。
+
+
+# 未来工作方向
+
+- [X] 完善编译过程出错后的中断处理机制
+- [ ] 完善检索主 LaTeX 文件的功能：
+    - [X] 根据魔法注释 `% !TEX root = file.tex` 找到主 LaTeX 文件
+    - [X] 通过检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
+- [ ] 完善自动判断编译类型：
+    - [X] 根据魔法注释 `% !TEX program = xelatex` 设置需要编译的类型
+- [x] 通过魔法注释设置编译结果存放位置
+- [X] 通过魔法注释实现编译命令的自定义
+- [ ] 增加配置文件功能，用于改变默认设置
+    - [ ] 指定生成的结果文件存放位置（目前默认存放在 `Build` 子文件夹下）
+    - [ ] 默认的编译命令（目前默认编译命令是 `xelatex`）
+- [ ] texlive 宏包检缺失并自动安装
+- [ ] 多主文件编译功能
```

### Comparing `pytexmk-0.5.1.240426/README.md` & `pytexmk-0.5.4.240427/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,127 +1,133 @@
-<!--
- *  =======================================================================
- *  ····Y88b···d88P················888b·····d888·d8b·······················
- *  ·····Y88b·d88P·················8888b···d8888·Y8P·······················
- *  ······Y88o88P··················88888b·d88888···························
- *  ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
- *  ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
- *  ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
- *  ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
- *  ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
- *  ·······························································888·····
- *  ··························································Y8b·d88P·····
- *  ···························································"Y88P"······
- *  =======================================================================
- * 
- *  -----------------------------------------------------------------------
- * Author       : 焱铭
- * Date         : 2024-02-29 10:23:19 +0800
- * LastEditTime : 2024-04-26 22:37:00 +0800
- * Github       : https://github.com/YanMing-lxb/
- * FilePath     : /PyTeXMK/README.md
- * Description  : 
- *  -----------------------------------------------------------------------
- -->
-
-# PyTeXMK
-
-[![GitHub](https://img.shields.io/badge/Github-PyTeXMK-000000.svg)](https://github.com/YanMing-lxb/PyTeXMK) [![License](https://img.shields.io/badge/license-GPLv3-aff)](https://www.latex-project.org/lppl/) ![OS](https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg) [![GitHub release](https://img.shields.io/github/release/YanMing-lxb/PyTeXMK.svg?color=blueviolet&label=version&style=popout)](https://github.com/YanMing-lxb/PyTeXMK/releases/latest) [![Last Commit](https://img.shields.io/github/last-commit/YanMing-lxb/PyTeXMK)](https://github.com/YanMing-lxb/PyTeXMK/zipball/master) [![Issues](https://img.shields.io/github/issues/YanMing-lxb/PyTeXMK)](https://github.com/YanMing-lxb/PyTeXMK/issues) [![Github Action](https://github.com/YanMing-lxb/PyTeXMK/workflows/Test/badge.svg)](https://github.com/YanMing-lxb/PyTeXMK/actions) [![PyPI version](https://img.shields.io/pypi/v/pytexmk.svg)](https://pypi.python.org/pypi/pytexmk/) [![PyPI Downloads](https://img.shields.io/pypi/dm/pytexmk.svg?label=PyPI%20downloads)](https://pypi.org/project/pytexmk/) ![GitHub repo size](https://img.shields.io/github/repo-size/YanMing-lxb/PyTeXMK)
-
-LaTeX 辅助编译命令行程序 LaTeX Auxiliary Compilation Command Line Tool
-
----
-
-## 安装
-
-官方版本 PyTeXMK 发布在 [PyPI](https://pypi.org/project/pytexmk/) 上，并且可以通过 pip 包管理器从 PyPI 镜像轻松安装。
-
-请注意，您必须使用 Python 3 版本pip：
-
-```
-pip3 install pytexmk
-```
-
-## 升级
-
-```
-pip3 install --upgrade pytexmk
-```
-
-## 使用入门
-
-PyTeXMK 默认参数：`xelatex` 编译、主文件名 main、batch 模式（编译过程信息不显，如需显示编译过程信息请使用 `-nq` 参数）、编译结果存放在 LaTeX 项目的 Build 文件夹下 ( VSCode 用户则需要在 `settings.json` 中注意设置 `"latex-workshop.latex.outDir": "./Build",` 使得latex workshop 能够找到pdf )。
-
-请仔细阅读：[主文件及编译类型选定逻辑](#主文件及编译类型选定逻辑)
-
-### 编译命令
-PyTeXMK 支持：
-
-- 编译命令：`xelatex` `pdflatex` `lualatex`
-- 参考文献：`bibtex` `biblatex` `thebibliography`
-- 符号索引：`glossaries` `nomencl` `mkeidx`
-
-位置参数:
-| Option              | Description                    |
-|---------------------|-------------------------------|
-| document          | 要被编译的文件名                   |
-
-选项:
-| Option           | Description                                |
-|------------------|--------------------------------------------|
-| -h, --help       | 显示帮助信息                                 |
-| -v, --version    | 显示程序版本号                               |
-| -p, --pdflatex   | pdflatex 进行编译                           |
-| -x, --xelatex    | xelatex 进行编译                            |
-| -l, --lualatex   | lualatex 进行编译                           |
-| -c, --clean      | 清除所有辅助文件                              |
-| -C, --Clean      | 清除所有辅助文件和 pdf 文件                    |
-| -nq, --no-quiet  | 非安静模式运行，此模式下显示编译过程             |
-| -cp, --clean-pdf  | 清理所有 pdf 文件             |
-
-**说明：**
-`-cp` 参数的功能是 "当 LaTeX 编译过程中报类似 `invalid X X R object at offset XXXXX` 的警告时，可使用此参数清理所有 pdf 文件"
-
-### 魔法注释
-
-PyTeXMK 支持使用魔法注释来自定义编译命令、编译类型、编译结果存放位置等。    
-
-| Magic Comment | Description                                |
-|---------------|----------|
-| `% !TEX program = xelatex` | 指定编译类型，可选 `xelatex` `pdflatex` `lualatex` |
-| `% !TEX root = file.tex` | 指定主 LaTeX 文件名，仅支持主文件在项目根目录下的情况 |
-| `% !TEX outdir = PDFfile` | 指定编译结果存放位置，仅支持文件夹名称，如果使用 LaTeX-Workshop，则需要在 `settings.json` 中设置 `"latex-workshop.latex.outDir": "./PDFfile",` |
-
-### 主文件及编译类型选定逻辑
-- PyTeXMK 优先使用终端输入命令 `-p` `-x` `-l` 参数指定的编译类型，如果没有指定，则会使用 `% !TEX program = xelatex` 指定的编译类型，如果没有指定，则会使用默认的编译类型 `xelatex`
-- PyTeXMK 主文件选定逻辑顺序：
-    1. 使用终端输入的文件名
-    2. 使用 `% !TEX root = file.tex` 指定的主 LaTeX 文件名
-    3. 使用默认的主文件名 `main`
-    4. 检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
-    5. 根目录下 TeX 文件中只有一个文件，则选择该文件作为主文件
-        
-- PyTeXMK 会优先使用 `% !TEX outdir = PDFfile` 指定的编译结果存放位置，如果没有指定，则会使用默认的编译结果存放位置 `Build`
-
-# 更新日志
-
-- 2024-03-22 完善编译过程出错后的中断处理机制：在编译过程中出现错误时，程序会自动中断，并提示 `请用 -nq 模式运行以显示错误信息！`,使用 `-nq` 参数运行时，则会显示错误信息。
-- 2024-04-26 增加：
-    1. 魔法注释功能，使得用户可以自定义编译命令、编译类型、编译结果存放位置等
-    2. 完善主文件及编译类型选定逻辑
-
-
-# 未来工作方向
-
-- [X] 完善编译过程出错后的中断处理机制
-- [ ] 完善检索主 LaTeX 文件的功能：
-    - [X] 根据魔法注释 `% !TEX root = file.tex` 找到主 LaTeX 文件
-    - [ ] 通过检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
-- [ ] 完善自动判断编译类型：
-    - [X] 根据魔法注释 `% !TEX program = xelatex` 设置需要编译的类型
-- [x] 通过魔法注释设置编译结果存放位置
-- [X] 通过魔法注释实现编译命令的自定义
-- [ ] 增加配置文件功能，用于改变默认设置
-    - [ ] 指定生成的结果文件存放位置（目前默认存放在 `Build` 子文件夹下）
-    - [ ] 默认的编译命令（目前默认编译命令是 `xelatex`）
-- [ ] texlive 宏包检缺失并自动安装
+<!--
+ *  =======================================================================
+ *  ····Y88b···d88P················888b·····d888·d8b·······················
+ *  ·····Y88b·d88P·················8888b···d8888·Y8P·······················
+ *  ······Y88o88P··················88888b·d88888···························
+ *  ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
+ *  ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
+ *  ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
+ *  ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
+ *  ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
+ *  ·······························································888·····
+ *  ··························································Y8b·d88P·····
+ *  ···························································"Y88P"······
+ *  =======================================================================
+ * 
+ *  -----------------------------------------------------------------------
+ * Author       : 焱铭
+ * Date         : 2024-02-29 10:23:19 +0800
+ * LastEditTime : 2024-04-27 10:10:51 +0800
+ * Github       : https://github.com/YanMing-lxb/
+ * FilePath     : \PyTeXMK\README.md
+ * Description  : 
+ *  -----------------------------------------------------------------------
+ -->
+
+# PyTeXMK
+
+[![GitHub](https://img.shields.io/badge/Github-PyTeXMK-000000.svg)](https://github.com/YanMing-lxb/PyTeXMK) [![License](https://img.shields.io/badge/license-GPLv3-aff)](https://www.latex-project.org/lppl/) ![OS](https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg) [![GitHub release](https://img.shields.io/github/release/YanMing-lxb/PyTeXMK.svg?color=blueviolet&label=version&style=popout)](https://github.com/YanMing-lxb/PyTeXMK/releases/latest) [![Last Commit](https://img.shields.io/github/last-commit/YanMing-lxb/PyTeXMK)](https://github.com/YanMing-lxb/PyTeXMK/zipball/master) [![Issues](https://img.shields.io/github/issues/YanMing-lxb/PyTeXMK)](https://github.com/YanMing-lxb/PyTeXMK/issues) [![Github Action](https://github.com/YanMing-lxb/PyTeXMK/workflows/Test/badge.svg)](https://github.com/YanMing-lxb/PyTeXMK/actions) [![PyPI version](https://img.shields.io/pypi/v/pytexmk.svg)](https://pypi.python.org/pypi/pytexmk/) [![PyPI Downloads](https://img.shields.io/pypi/dm/pytexmk.svg?label=PyPI%20downloads)](https://pypi.org/project/pytexmk/) ![GitHub repo size](https://img.shields.io/github/repo-size/YanMing-lxb/PyTeXMK)
+
+LaTeX 辅助编译命令行程序 LaTeX Auxiliary Compilation Command Line Tool
+
+---
+
+## 安装
+
+官方版本 PyTeXMK 发布在 [PyPI](https://pypi.org/project/pytexmk/) 上，并且可以通过 pip 包管理器从 PyPI 镜像轻松安装。
+
+请注意，您必须使用 Python 3 版本pip：
+
+```
+pip3 install pytexmk
+```
+
+## 升级
+
+```
+pip3 install --upgrade pytexmk
+```
+
+## 使用入门
+
+PyTeXMK 默认参数：`xelatex` 编译、主文件名 main.tex、batch 模式（编译过程信息不显，如需显示编译过程信息请使用 `-nq` 参数）、编译结果存放在 LaTeX 项目的 Build 文件夹下 ( VSCode 用户则需要在 `settings.json` 中注意设置 `"latex-workshop.latex.outDir": "./Build",` 使得 LaTeX-Workshop 能够找到 pdf )。
+
+请仔细阅读：[主文件及编译类型选定逻辑](#主文件及编译类型选定逻辑)
+
+> PyTeXMK，仅支持 utf-8 编码的 TeX 文件。
+
+### 编译命令
+PyTeXMK 支持：
+
+- 编译命令：`xelatex` `pdflatex` `lualatex`
+- 参考文献：`bibtex` `biblatex` `thebibliography`
+- 符号索引：`glossaries` `nomencl` `mkeidx`
+
+位置参数:
+| Option              | Description                    |
+|---------------------|-------------------------------|
+| document          | 要被编译的文件名                   |
+
+选项:
+| Option           | Description                                |
+|------------------|--------------------------------------------|
+| -h, --help       | 显示帮助信息                                 |
+| -v, --version    | 显示程序版本号                               |
+| -p, --pdflatex   | pdflatex 进行编译                           |
+| -x, --xelatex    | xelatex 进行编译                            |
+| -l, --lualatex   | lualatex 进行编译                           |
+| -c, --clean      | 清除所有辅助文件                              |
+| -C, --Clean      | 清除所有辅助文件和 pdf 文件                    |
+| -nq, --no-quiet  | 非安静模式运行，此模式下显示编译过程             |
+| -cp, --clean-pdf  | 清理所有 pdf 文件                          |
+
+**说明：**
+`-cp` 参数的功能是 "当 LaTeX 编译过程中报类似 `invalid X X R object at offset XXXXX` 的警告时，可使用此参数清理所有 pdf 文件"
+
+### 魔法注释
+
+PyTeXMK 支持使用魔法注释来自定义编译命令、编译类型、编译结果存放位置等（仅支持检索文档前 50 行）。    
+
+| Magic Comment | Description                                |
+|---------------|----------|
+| `% !TEX program = xelatex` | 指定编译类型，可选 `xelatex` `pdflatex` `lualatex` |
+| `% !TEX root = file.tex` | 指定主 LaTeX 文件名，仅支持主文件在项目根目录下的情况 |
+| `% !TEX outdir = PDFfile` | 指定编译结果存放位置，仅支持文件夹名称，如果使用 LaTeX-Workshop，则需要在 `settings.json` 中设置 `"latex-workshop.latex.outDir": "./PDFfile",` |
+
+### 主文件及编译类型选定逻辑
+
+- PyTeXMK 优先使用终端输入命令 `-p` `-x` `-l` 参数指定的编译类型，如果没有指定，则会使用 `% !TEX program = xelatex` 指定的编译类型，如果没有指定，则会使用默认的编译类型 `xelatex`
+- PyTeXMK 主文件选定逻辑顺序：
+    1. 使用终端输入的文件名
+    2. 使用 `% !TEX root = file.tex` 指定的主 LaTeX 文件名
+    3. 使用默认的主文件名 `main.tex`
+    4. 检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断（仅支持检索文档前 200 行）
+    5. 根目录下 TeX 文件中只有一个文件，则选择该文件作为主文件
+        
+- PyTeXMK 会优先使用 `% !TEX outdir = PDFfile` 指定的编译结果存放位置，如果没有指定，则会使用默认的编译结果存放位置 `Build`
+
+# 更新日志
+
+- 2024-03-22 完善编译过程出错后的中断处理机制：在编译过程中出现错误时，程序会自动中断，并提示 `请用 -nq 模式运行以显示错误信息！`，使用 `-nq` 参数运行时，则会显示错误信息。
+- 2024-04-26 增加：
+    1. 魔法注释功能，使得用户可以自定义编译命令、编译类型、编译结果存放位置等
+    2. 完善主文件及编译类型选定逻辑
+- 2024-04-26 
+    1. 修复边 \documentclass 和 \begin{document} 检索逻辑。
+    2. 解决文档读取编码导致的报错。
+
+
+# 未来工作方向
+
+- [X] 完善编译过程出错后的中断处理机制
+- [ ] 完善检索主 LaTeX 文件的功能：
+    - [X] 根据魔法注释 `% !TEX root = file.tex` 找到主 LaTeX 文件
+    - [X] 通过检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
+- [ ] 完善自动判断编译类型：
+    - [X] 根据魔法注释 `% !TEX program = xelatex` 设置需要编译的类型
+- [x] 通过魔法注释设置编译结果存放位置
+- [X] 通过魔法注释实现编译命令的自定义
+- [ ] 增加配置文件功能，用于改变默认设置
+    - [ ] 指定生成的结果文件存放位置（目前默认存放在 `Build` 子文件夹下）
+    - [ ] 默认的编译命令（目前默认编译命令是 `xelatex`）
+- [ ] texlive 宏包检缺失并自动安装
 - [ ] 多主文件编译功能
```

### Comparing `pytexmk-0.5.1.240426/pyproject.toml` & `pytexmk-0.5.4.240427/pyproject.toml`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "pytexmk"
-dynamic = ["version"]
-authors = [
-  { name = "焱铭", email = "lxb-yanming@foxmail.com" },
-]
-description = "LaTeX 辅助编译命令行工具 LaTeX Auxiliary Compilation Command Line Tool"
-keywords = ["LaTeX", "build", "latexmk"]
-dependencies = ["rich","pymupdf"]
-readme = "README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Environment :: Console",
-    "Intended Audience :: Developers ",
-    "Intended Audience :: End Users/Desktop",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/YanMing-lxb/PyTeXMK"
-"Bug Tracker" = "https://github.com/YanMing-lxb/PyTeXMK/issues"
-
-[project.scripts]
-pytexmk = "pytexmk:main"
-
-[tool.setuptools.dynamic]
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "pytexmk"
+dynamic = ["version"]
+authors = [
+  { name = "焱铭", email = "lxb-yanming@foxmail.com" },
+]
+description = "LaTeX 辅助编译命令行工具 LaTeX Auxiliary Compilation Command Line Tool"
+keywords = ["LaTeX", "build", "latexmk"]
+dependencies = ["rich","pymupdf"]
+readme = "README.md"
+requires-python = ">=3.8"
+classifiers = [
+    "Environment :: Console",
+    "Intended Audience :: Developers ",
+    "Intended Audience :: End Users/Desktop",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/YanMing-lxb/PyTeXMK"
+"Bug Tracker" = "https://github.com/YanMing-lxb/PyTeXMK/issues"
+
+[project.scripts]
+pytexmk = "pytexmk:main"
+
+[tool.setuptools.dynamic]
 version = {attr = "pytexmk.version.__version__"}
```

### Comparing `pytexmk-0.5.1.240426/src/pytexmk/__init__.py` & `pytexmk-0.5.4.240427/src/pytexmk/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-'''
- =======================================================================
- ····Y88b···d88P················888b·····d888·d8b·······················
- ·····Y88b·d88P·················8888b···d8888·Y8P·······················
- ······Y88o88P··················88888b·d88888···························
- ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
- ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
- ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
- ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
- ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
- ·······························································888·····
- ··························································Y8b·d88P·····
- ···························································"Y88P"······
- =======================================================================
-
- -----------------------------------------------------------------------
-Author       : 焱铭
-Date         : 2024-02-29 12:27:07 +0800
-LastEditTime : 2024-02-29 15:45:51 +0800
-Github       : https://github.com/YanMing-lxb/
-FilePath     : /PyTeXMK/src/pytexmk/__init__.py
-Description  : 
- -----------------------------------------------------------------------
-'''
-
-import sys
-
-if sys.version_info[0] == 3:
-
-    from .__main__ import *
-
-else:
-    # Don't import anything.
-    pass
-
+'''
+ =======================================================================
+ ····Y88b···d88P················888b·····d888·d8b·······················
+ ·····Y88b·d88P·················8888b···d8888·Y8P·······················
+ ······Y88o88P··················88888b·d88888···························
+ ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
+ ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
+ ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
+ ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
+ ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
+ ·······························································888·····
+ ··························································Y8b·d88P·····
+ ···························································"Y88P"······
+ =======================================================================
+
+ -----------------------------------------------------------------------
+Author       : 焱铭
+Date         : 2024-02-29 12:27:07 +0800
+LastEditTime : 2024-02-29 15:45:51 +0800
+Github       : https://github.com/YanMing-lxb/
+FilePath     : /PyTeXMK/src/pytexmk/__init__.py
+Description  : 
+ -----------------------------------------------------------------------
+'''
+
+import sys
+
+if sys.version_info[0] == 3:
+
+    from .__main__ import *
+
+else:
+    # Don't import anything.
+    pass
+
```

### Comparing `pytexmk-0.5.1.240426/src/pytexmk/__main__.py` & `pytexmk-0.5.4.240427/src/pytexmk/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-'''
- =======================================================================
- ····Y88b···d88P················888b·····d888·d8b·······················
- ·····Y88b·d88P·················8888b···d8888·Y8P·······················
- ······Y88o88P··················88888b·d88888···························
- ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
- ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
- ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
- ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
- ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
- ·······························································888·····
- ··························································Y8b·d88P·····
- ···························································"Y88P"······
- =======================================================================
-
- -----------------------------------------------------------------------
-Author       : 焱铭
-Date         : 2024-02-28 23:11:52 +0800
-LastEditTime : 2024-04-26 23:19:03 +0800
-Github       : https://github.com/YanMing-lxb/
-FilePath     : /PyTeXMK/src/pytexmk/__main__.py
-Description  : 
- -----------------------------------------------------------------------
-'''
-# -*- coding: utf-8 -*-
-import argparse
-import datetime
-from .version import script_name, __version__
-from .compile_model import compile_tex, compile_bib, compile_index, compile_xdv
-from .additional_operation import *
-from .info_print import time_count, time_print, print_message
-
-# ================================================================================
-# XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX 整体进行编译 XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
-# ================================================================================
-def compile(start_time,tex_name, file_name, quiet, outdir):
-    name_target_list = []
-    time_run_list = []
-
-    time_run_remove_aux, _ = time_count(remove_aux, file_name) # 清除已有辅助文件
-    name_target_list.append("清除旧辅助文件")
-    time_run_list.append(time_run_remove_aux)
-
-    time_run_tex, try_bool_tex = time_count(compile_tex, tex_name, file_name, 1, quiet) # 首次编译 tex 文档
-    if not try_bool_tex: print(f"{tex_name} 1st 编译失败，{'请用 -nq 模式运行以显示错误信息！' if quiet else '请检查上面的错误信息！'}"); return
-    time_run_bib, return_com_bib = time_count(compile_bib, file_name, quiet) # 编译参考文献
-    times_compile_tex_bib, print_bib, name_target_bib, try_bool_bib = return_com_bib # 获取 compile_bib 函数得到的参数
-    if not try_bool_bib: print(f"{name_target_bib} 编译失败，{'请用 -nq 模式运行以显示错误信息！' if quiet else '请检查上面的错误信息！'}"); return
-    time_run_index, return_com_index = time_count(compile_index, file_name) # 编译目录索引
-    times_compile_tex_index, print_index, name_target_index, try_bool_index = return_com_index # 获取 compile_index 函数得到的参数
-    if not try_bool_index: print(f"{name_target_bib} 编译失败，{'请用 -nq 模式运行以显示错误信息！' if quiet else '请检查上面的错误信息！'}"); return
-    
-    times_extra_complie = max(times_compile_tex_bib, times_compile_tex_index) # 计算额外编译 tex 文档次数
-
-    # 将获取到的编译项目名称 添加到对应的列表中
-    name_target_list.append(f'{tex_name} 1st')
-    time_run_list.append(time_run_tex)
-    
-    if times_compile_tex_bib != 0: # 存在参考文献编译过程
-        if name_target_bib:
-            name_target_list.append(name_target_bib)
-            time_run_list.append(time_run_bib)
-    if times_compile_tex_index != 0: # 存在目录索引编译过程
-        if name_target_index:
-            name_target_list.append(name_target_index)
-            time_run_list.append(time_run_index)
-
-    for i in range(times_extra_complie): # 进行额外编译 tex
-        time_run_tex, try_bool_tex = time_count(compile_tex, tex_name, file_name, i + 2, quiet)
-        if i+2 == 2: 
-            if not try_bool_tex: print(f"{tex_name} {i+2}nd 编译失败，{'请用 -nq 模式运行以显示错误信息！' if quiet else '请检查上面的错误信息！'}"); return
-            name_target_list.append(f'{tex_name} {i+2}nd')
-        if i+2 == 3:
-            if not try_bool_tex: print(f"{tex_name} {i+2}rd 编译失败，{'请用 -nq 模式运行以显示错误信息！' if quiet else '请检查上面的错误信息！'}"); return
-            name_target_list.append(f'{tex_name} {i+2}rd')
-            
-        time_run_list.append(time_run_tex)
-
-    if tex_name == "xelatex":  # 判断是否编译 xdv 文件
-        time_run_xdv, try_bool_xdv = time_count(compile_xdv, file_name, quiet) # 编译 xdv 文件
-        if not try_bool_xdv: print("dvipdfmx 编译失败，{'请用 -nq 模式运行以显示错误信息！' if quiet else '请检查上面的错误信息！'}"); return
-        name_target_list.append('dvipdfmx 编译')
-        time_run_list.append(time_run_xdv)
-
-    print("\n\n" + "=" * 80 + "\n" +
-          "▓" * 33 + " 完成所有编译 " + "▓" * 33 + "\n" +
-          "=" * 80 + "\n")
-    print(f"文档整体：{tex_name} 编译 {times_extra_complie+1} 次")
-    print(f"参考文献：{print_bib}")
-    print(f"目录索引：{print_index}")
-    print_message("开始执行编译以外的附加命令！")
-    
-    time_run_remove_res, _ = time_count(remove_result, outdir) # 清除已有结果文件
-    name_target_list.append("清除旧结果文件")
-    time_run_list.append(time_run_remove_res)
-    time_run_move_res, _ = time_count(move_result, file_name, outdir) # 移动生成结果文件
-    name_target_list.append("移动结果文件")
-    time_run_list.append(time_run_move_res)
-    time_run_remove_aux, _ = time_count(remove_aux, file_name) # 清除生成辅助文件
-    name_target_list.append("清除辅助文件")
-    time_run_list.append(time_run_remove_aux)
-
-    time_print(start_time, name_target_list, time_run_list) # 打印编译时长统计
-
-def main():
-    # ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓ 设置默认 ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓
-    tex_name = "xelatex"
-    outdir = "./Build/"
-    magic_comments_keys = ["program", "root", "outdir"]
-    # ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓
-
-    start_time = datetime.datetime.now() # 计算开始时间
-    
-    # --------------------------------------------------------------------------------
-    # 定义命令行参数
-    # --------------------------------------------------------------------------------
-    parser = argparse.ArgumentParser(description="LaTeX 辅助编译程序.")
-    parser.add_argument('-v', '--version', action='version', version=f'{script_name}: {__version__}')
-    parser.add_argument('-p', '--pdflatex', action='store_true', help="pdflatex 进行编译")
-    parser.add_argument('-x', '--xelatex', action='store_true', help="xelatex 进行编译")
-    parser.add_argument('-l', '--lualatex', action='store_true', help="lualatex 进行编译")
-    parser.add_argument('-c', '--clean', action='store_true', help="清除所有辅助文件")
-    parser.add_argument('-C', '--Clean', action='store_true', help="清除所有辅助文件和 pdf 文件")
-    parser.add_argument('-nq', '--no-quiet', action='store_true', help="非安静模式运行，此模式下显示编译过程")
-    parser.add_argument('-cp', '--clean-pdf', action='store_true', help="清理 pdf 文件，当 LaTeX 编译过程中警告 invalid X X R object 时，可使用此参数清理所有 pdf 文件")
-    
-    parser.add_argument('document', nargs='?', help="要被编译的文件名")
-    args = parser.parse_args()
-
-    tex_files = search_tex_file() # 运行 search_tex_file 函数搜索当前目录下所有 tex 文件
-    magic_comments = search_magic_comments(tex_files, magic_comments_keys) # 运行 search_magic_comments 函数搜索 tex_files 列表中是否存在 magic comments
-
-    # --------------------------------------------------------------------------------
-    # 输出文件路径判断
-    # --------------------------------------------------------------------------------
-    if magic_comments.get('outdir'): # 如果存在 magic comments 且 outdir 存在
-        outdir = magic_comments['outdir'] # 使用 magic comments 中的 outdir 作为输出目录
-        print(f"通过魔法注释找到输出目录为 {outdir}！")
-
-    # --------------------------------------------------------------------------------
-    # 主文件逻辑判断
-    # --------------------------------------------------------------------------------
-    if args.document: # pytexmk 指定 latex 文件
-        file_name = check_file_name(args.document) # check_file_name 函数检查 args.document 参数输入的文件名是否正确
-    else: # pytexmk 未指定 latex 文件
-        if magic_comments.get('root'): # 如果存在 magic comments 且 root 存在
-            file_name = check_file_name(magic_comments['root']) # 使用 magic comments 中的 root 作为文件名
-            print(f"通过魔法注释找到 {file_name}.tex 文件！")
-        else: # pytexmk 和魔法注释都不存在，使用search_main_file方法搜索主文件
-            file_name = search_main_file(tex_files)
-    # --------------------------------------------------------------------------------
-    # 编译类型判断
-    # --------------------------------------------------------------------------------
-    if args.xelatex:
-        tex_name = "xelatex"
-    elif args.pdflatex:
-        tex_name = "pdflatex"
-    elif args.lualatex:
-        tex_name = "lualatex"
-    elif magic_comments.get('program'): # 如果存在 magic comments 且 program 存在
-        tex_name = magic_comments['program'] # 使用 magic comments 中的 program 作为编译器
-        print(f"通过魔法注释设置编译器为 {tex_name}！")
-
-    # --------------------------------------------------------------------------------
-    # 编译程序运行
-    # --------------------------------------------------------------------------------
-
-    if file_name: # 如果存在 file_name
-        if args.clean:
-            remove_aux(file_name)
-        elif args.Clean:
-            remove_aux(file_name)
-            remove_result(outdir)
-            remove_result_in_root(file_name)
-        elif args.clean_pdf:
-            clean_all_pdf('.', outdir, file_name)
-        else:
-            compile(start_time, tex_name, file_name, not args.no_quiet, outdir)
-            
-    
-
-if __name__ == "__main__":
-
+'''
+ =======================================================================
+ ····Y88b···d88P················888b·····d888·d8b·······················
+ ·····Y88b·d88P·················8888b···d8888·Y8P·······················
+ ······Y88o88P··················88888b·d88888···························
+ ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
+ ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
+ ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
+ ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
+ ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
+ ·······························································888·····
+ ··························································Y8b·d88P·····
+ ···························································"Y88P"······
+ =======================================================================
+
+ -----------------------------------------------------------------------
+Author       : 焱铭
+Date         : 2024-02-28 23:11:52 +0800
+LastEditTime : 2024-04-27 10:17:11 +0800
+Github       : https://github.com/YanMing-lxb/
+FilePath     : \PyTeXMK\src\pytexmk\__main__.py
+Description  : 
+ -----------------------------------------------------------------------
+'''
+# -*- coding: utf-8 -*-
+import argparse
+import datetime
+from .version import script_name, __version__
+from .compile_model import compile_tex, compile_bib, compile_index, compile_xdv
+from .additional_operation import *
+from .info_print import time_count, time_print, print_message
+
+# ================================================================================
+# XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX 整体进行编译 XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
+# ================================================================================
+def compile(start_time,tex_name, file_name, quiet, outdir):
+    name_target_list = []
+    time_run_list = []
+
+    time_run_remove_aux, _ = time_count(remove_aux, file_name) # 清除已有辅助文件
+    name_target_list.append("清除旧辅助文件")
+    time_run_list.append(time_run_remove_aux)
+
+    time_run_tex, try_bool_tex = time_count(compile_tex, tex_name, file_name, 1, quiet) # 首次编译 tex 文档
+    if not try_bool_tex: print(f"{tex_name} 1st 编译失败，{'请用 -nq 模式运行以显示错误信息！' if quiet else '请检查上面的错误信息！'}"); return
+    time_run_bib, return_com_bib = time_count(compile_bib, file_name, quiet) # 编译参考文献
+    times_compile_tex_bib, print_bib, name_target_bib, try_bool_bib = return_com_bib # 获取 compile_bib 函数得到的参数
+    if not try_bool_bib: print(f"{name_target_bib} 编译失败，{'请用 -nq 模式运行以显示错误信息！' if quiet else '请检查上面的错误信息！'}"); return
+    time_run_index, return_com_index = time_count(compile_index, file_name) # 编译目录索引
+    times_compile_tex_index, print_index, name_target_index, try_bool_index = return_com_index # 获取 compile_index 函数得到的参数
+    if not try_bool_index: print(f"{name_target_bib} 编译失败，{'请用 -nq 模式运行以显示错误信息！' if quiet else '请检查上面的错误信息！'}"); return
+    
+    times_extra_complie = max(times_compile_tex_bib, times_compile_tex_index) # 计算额外编译 tex 文档次数
+
+    # 将获取到的编译项目名称 添加到对应的列表中
+    name_target_list.append(f'{tex_name} 1st')
+    time_run_list.append(time_run_tex)
+    
+    if times_compile_tex_bib != 0: # 存在参考文献编译过程
+        if name_target_bib:
+            name_target_list.append(name_target_bib)
+            time_run_list.append(time_run_bib)
+    if times_compile_tex_index != 0: # 存在目录索引编译过程
+        if name_target_index:
+            name_target_list.append(name_target_index)
+            time_run_list.append(time_run_index)
+
+    for i in range(times_extra_complie): # 进行额外编译 tex
+        time_run_tex, try_bool_tex = time_count(compile_tex, tex_name, file_name, i + 2, quiet)
+        if i+2 == 2: 
+            if not try_bool_tex: print(f"{tex_name} {i+2}nd 编译失败，{'请用 -nq 模式运行以显示错误信息！' if quiet else '请检查上面的错误信息！'}"); return
+            name_target_list.append(f'{tex_name} {i+2}nd')
+        if i+2 == 3:
+            if not try_bool_tex: print(f"{tex_name} {i+2}rd 编译失败，{'请用 -nq 模式运行以显示错误信息！' if quiet else '请检查上面的错误信息！'}"); return
+            name_target_list.append(f'{tex_name} {i+2}rd')
+            
+        time_run_list.append(time_run_tex)
+
+    if tex_name == "xelatex":  # 判断是否编译 xdv 文件
+        time_run_xdv, try_bool_xdv = time_count(compile_xdv, file_name, quiet) # 编译 xdv 文件
+        if not try_bool_xdv: print("dvipdfmx 编译失败，{'请用 -nq 模式运行以显示错误信息！' if quiet else '请检查上面的错误信息！'}"); return
+        name_target_list.append('dvipdfmx 编译')
+        time_run_list.append(time_run_xdv)
+
+    print("\n\n" + "=" * 80 + "\n" +
+          "▓" * 33 + " 完成所有编译 " + "▓" * 33 + "\n" +
+          "=" * 80 + "\n")
+    print(f"文档整体：{tex_name} 编译 {times_extra_complie+1} 次")
+    print(f"参考文献：{print_bib}")
+    print(f"目录索引：{print_index}")
+    print_message("开始执行编译以外的附加命令！")
+    
+    time_run_remove_res, _ = time_count(remove_result, outdir) # 清除已有结果文件
+    name_target_list.append("清除旧结果文件")
+    time_run_list.append(time_run_remove_res)
+    time_run_move_res, _ = time_count(move_result, file_name, outdir) # 移动生成结果文件
+    name_target_list.append("移动结果文件")
+    time_run_list.append(time_run_move_res)
+    time_run_remove_aux, _ = time_count(remove_aux, file_name) # 清除生成辅助文件
+    name_target_list.append("清除辅助文件")
+    time_run_list.append(time_run_remove_aux)
+
+    time_print(start_time, name_target_list, time_run_list) # 打印编译时长统计
+
+def main():
+    # ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓ 设置默认 ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓
+    tex_name = "xelatex"
+    outdir = "./Build/"
+    magic_comments_keys = ["program", "root", "outdir"]
+    # ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓
+
+    start_time = datetime.datetime.now() # 计算开始时间
+    
+    # --------------------------------------------------------------------------------
+    # 定义命令行参数
+    # --------------------------------------------------------------------------------
+    parser = argparse.ArgumentParser(description="LaTeX 辅助编译程序.")
+    parser.add_argument('-v', '--version', action='version', version=f'{script_name}: {__version__}')
+    parser.add_argument('-p', '--pdflatex', action='store_true', help="pdflatex 进行编译")
+    parser.add_argument('-x', '--xelatex', action='store_true', help="xelatex 进行编译")
+    parser.add_argument('-l', '--lualatex', action='store_true', help="lualatex 进行编译")
+    parser.add_argument('-c', '--clean', action='store_true', help="清除所有辅助文件")
+    parser.add_argument('-C', '--Clean', action='store_true', help="清除所有辅助文件和 pdf 文件")
+    parser.add_argument('-nq', '--no-quiet', action='store_true', help="非安静模式运行，此模式下显示编译过程")
+    parser.add_argument('-cp', '--clean-pdf', action='store_true', help="清理 pdf 文件，当 LaTeX 编译过程中警告 invalid X X R object 时，可使用此参数清理所有 pdf 文件")
+    
+    parser.add_argument('document', nargs='?', help="要被编译的文件名")
+    args = parser.parse_args()
+
+    tex_files = search_tex_file() # 运行 search_tex_file 函数搜索当前目录下所有 tex 文件
+    magic_comments = search_magic_comments(tex_files, magic_comments_keys) # 运行 search_magic_comments 函数搜索 tex_files 列表中是否存在 magic comments
+
+    # --------------------------------------------------------------------------------
+    # 输出文件路径判断
+    # --------------------------------------------------------------------------------
+    if magic_comments.get('outdir'): # 如果存在 magic comments 且 outdir 存在
+        outdir = magic_comments['outdir'] # 使用 magic comments 中的 outdir 作为输出目录
+        print(f"通过魔法注释找到输出目录为 {outdir}！")
+
+    # --------------------------------------------------------------------------------
+    # 主文件逻辑判断
+    # --------------------------------------------------------------------------------
+    if args.document: # pytexmk 指定 latex 文件
+        file_name = check_file_name(args.document) # check_file_name 函数检查 args.document 参数输入的文件名是否正确
+    else: # pytexmk 未指定 latex 文件
+        if magic_comments.get('root'): # 如果存在 magic comments 且 root 存在
+            file_name = check_file_name(magic_comments['root']) # 使用 magic comments 中的 root 作为文件名
+            print(f"通过魔法注释找到 {file_name}.tex 文件！")
+        else: # pytexmk 和魔法注释都不存在，使用search_main_file方法搜索主文件
+            file_name = search_main_file(tex_files)
+
+    # --------------------------------------------------------------------------------
+    # 编译类型判断
+    # --------------------------------------------------------------------------------
+    if args.xelatex:
+        tex_name = "xelatex"
+    elif args.pdflatex:
+        tex_name = "pdflatex"
+    elif args.lualatex:
+        tex_name = "lualatex"
+    elif magic_comments.get('program'): # 如果存在 magic comments 且 program 存在
+        tex_name = magic_comments['program'] # 使用 magic comments 中的 program 作为编译器
+        print(f"通过魔法注释设置编译器为 {tex_name}！")
+
+    # --------------------------------------------------------------------------------
+    # 编译程序运行
+    # --------------------------------------------------------------------------------
+    if file_name: # 如果存在 file_name
+        if args.clean:
+            remove_aux(file_name)
+        elif args.Clean:
+            remove_aux(file_name)
+            remove_result(outdir)
+            remove_result_in_root(file_name)
+        elif args.clean_pdf:
+            clean_pdf('.', outdir, file_name)
+        else:
+            compile(start_time, tex_name, file_name, not args.no_quiet, outdir)
+            
+    
+
+if __name__ == "__main__":
+
     main()
```

### Comparing `pytexmk-0.5.1.240426/src/pytexmk/additional_operation.py` & `pytexmk-0.5.4.240427/src/pytexmk/additional_operation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,200 +1,200 @@
-'''
- =======================================================================
- ····Y88b···d88P················888b·····d888·d8b·······················
- ·····Y88b·d88P·················8888b···d8888·Y8P·······················
- ······Y88o88P··················88888b·d88888···························
- ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
- ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
- ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
- ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
- ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
- ·······························································888·····
- ··························································Y8b·d88P·····
- ···························································"Y88P"······
- =======================================================================
-
- -----------------------------------------------------------------------
-Author       : 焱铭
-Date         : 2024-02-29 16:02:37 +0800
-LastEditTime : 2024-04-26 23:10:42 +0800
-Github       : https://github.com/YanMing-lxb/
-FilePath     : /PyTeXMK/src/pytexmk/additional_operation.py
-Description  : 
- -----------------------------------------------------------------------
-'''
-# -*- coding: utf-8 -*-
-import os
-import fitz
-import shutil
-from rich import print
-
-# --------------------------------------------------------------------------------
-# 定义清除辅助文件命令
-# --------------------------------------------------------------------------------
-def remove_aux(file_name):
-    auxiliary_files = [
-        f"{file_name}{ext}" for ext in [".aux", ".bbl", ".blg", ".log", ".out", ".toc", ".bcf",
-                                        ".xml", ".nlo", ".nls", ".bak", ".ind", ".idx", ".ilg", ".lof",
-                                        ".lot", ".ent-x", ".tmp", ".ltx", ".los", ".lol", ".loc", ".listing", ".gz",
-                                        ".userbak", ".nav", ".snm", ".vrb", ".fls", ".xdv", ".fdb_latexmk", ".run.xml", ".ist", ".glo", ".gls"]
-    ]
-    file_exists = False
-    for file in auxiliary_files:
-        if os.path.exists(file):
-            try:
-                os.remove(file)
-                file_exists = True
-            except FileNotFoundError:
-                pass
-    if file_exists:
-        print("已清除辅助文件！")
-    else:
-        print("当前没有辅助文件！")
-
-# --------------------------------------------------------------------------------
-# 定义清除已有结果文件
-# --------------------------------------------------------------------------------
-def remove_result(outdir):
-    if os.path.exists(outdir):
-        shutil.rmtree(outdir)  # 删除整个文件夹
-        print(f"已删除 {outdir} 中的旧结果文件！")
-    
-def remove_result_in_root(file_name):
-    extensions = [".pdf", ".synctex.gz", ".synctex"]
-    for ext in extensions:
-        file = file_name + ext
-        if os.path.exists(file):
-            try:
-                os.remove(file)
-                print(f"{file} 已删除！")
-            except FileNotFoundError:
-                print(f"{file} 未能删除！")
-        else:
-            print(f"根目录下不存在 {file}")
-
-# --------------------------------------------------------------------------------
-# 定义移动生成文件
-# --------------------------------------------------------------------------------
-def move_result(file_name, outdir):
-    result_files = [f"{file_name}{ext}" for ext in [".pdf", ".synctex.gz"]]
-    os.mkdir(outdir)  # 创建空的 outdir 文件夹
-    for file in result_files:
-        if os.path.exists(file):
-            shutil.move(file, outdir)
-            print(f"{file} 移动到 {outdir}")
-        else:
-            print(f'{file} 不存在！')
-
-# --------------------------------------------------------------------------------
-# 定义清理所有 pdf 文件
-# --------------------------------------------------------------------------------
-def clean_all_pdf(root_dir, excluded_folder, file_name):
-    pdf_files = []
-    for root, dirs, files in os.walk(root_dir):
-        if excluded_folder in dirs:
-            dirs.remove(excluded_folder)  # 不包括名为excluded_folder的文件夹中的pdf文件
-        
-        if root == root_dir:
-            # 如果当前处理的是根目录文件，则跳过
-            continue 
-
-        for file in files:
-            if file.endswith('.pdf') and file != f'{file_name}.pdf':
-                pdf_files.append(os.path.join(root, file))  # 仅清理子文件夹中的pdf文件
-    
-    # 对pdf文件进行打开和关闭操作，解决origin批量导出pdf文件时由于未关闭pdf导致的报错
-    if pdf_files:
-        print(f"共发现 {len(pdf_files)} 个PDF文件。")
-        for pdf_file in pdf_files:
-            try:
-                doc = fitz.open(pdf_file)
-                doc.close()
-                print(f"已处理: {pdf_file}")
-            except Exception as e:
-                print(f"处理出错 {pdf_file}: {e}")
-        print("所有PDF文件已处理完成。")
-    else:
-        print("当前路径下未发现PDF文件。")
-    
-# --------------------------------------------------------------------------------
-# 定义输入检查函数
-# --------------------------------------------------------------------------------
-def check_file_name(file_name):
-    base_name, file_extension = os.path.splitext(
-        os.path.basename(file_name))  # 去掉路径，提取文件名和后缀
-    if file_extension == '.tex':  # 判断后缀是否是 .tex
-        file_name_return = base_name
-    elif '.' not in file_name:  # 判断输入 file_name 中没有 后缀
-        if '/' in file_name or '\\' in file_name:  # 判断是否是没有后缀的路径
-            file_name_return = None
-            print("错误：文件路径无效！")
-        else:
-            file_name_return = file_name
-    else:
-        file_name_return = None
-        print("提示：文件后缀不是.tex")
-
-    return file_name_return
-
-# --------------------------------------------------------------------------------
-# 定义 tex 文件检索函数
-# --------------------------------------------------------------------------------
-def search_tex_file():
-    current_path = os.getcwd() # 获取当前路径
-    # 遍历当前路径下的所有文件
-    tex_files = [file for file in os.listdir(current_path) if file.endswith('.tex')]
-    return tex_files
-
-# --------------------------------------------------------------------------------
-# 定义 tex 主文件检索函数
-# --------------------------------------------------------------------------------
-def search_main_file(tex_files):
-    current_path = os.getcwd() # 获取当前路径
-    if tex_files:
-        # 如果存在多个.tex文件
-        if 'main.tex' in tex_files:
-            # 存在名为main.tex的文件
-            file_name = 'main'
-            print(f"找到 {file_name}.tex 文件！")
-        # 如果只有一个.tex文件，则直接提取文件名并打印
-        elif len(tex_files) == 1:
-            file_name = os.path.splitext(tex_files[0])[0]
-            print(f"找到 {file_name}.tex 文件！")
-        elif len(tex_files) > 1:
-            # 存在多个.tex文件，但没有名为main.tex的文件
-            for file_path in tex_files:  # 遍历tex文件列表
-                with open(file_path, 'r') as file:  # 打开文件
-                    for _ in range(200):  # 遍历文件的前200行
-                        line = file.readline()  # 读取一行内容
-                        if "\documentclass" in line or "\begin{document}" in line:
-                            # 找到 \documentclass 或 \begin{document} 指令，提取文件名
-                            file_name = check_file_name(file_path)
-                            print(f"找到 {file_name}.tex 文件！")
-        else:
-            # 不存在名为main.tex的文件，打印所有找到的.tex文件
-            file_name = None
-            print("存在多个 .tex 文件，请：修改主文件名为 main.tex 或在文件中加入魔法注释 “% !TEX = <主文件名>” 或在终端输入：pytexmk <主文件名> 名进行编译")
-            print("[bold][red]注意：主文件名一定要放在项目根目录下[/red][/bold]")
-    else:
-        # 不存在.tex文件，打印当前路径并提示
-        file_name = None
-        print("终端路径下不存在 .tex 文件！请检查终端显示路径是否是项目路径")
-        print(f"当前终端路径是：{current_path}")
-
-    return file_name
-
-# --------------------------------------------------------------------------------
-# 定义魔法注释检索函数
-# --------------------------------------------------------------------------------
-def search_magic_comments(tex_files, magic_comments_keys):
-    magic_comments = {}  # 创建空字典用于存储结果
-    if len(tex_files):
-        for file_path in tex_files:  # 遍历tex文件列表
-            with open(file_path, 'r') as file:  # 打开文件
-                for _ in range(50):  # 遍历文件的前50行
-                    line = file.readline()  # 读取一行内容
-                    for magic_comments_key in magic_comments_keys:  # 遍历关键字列表
-                        if f"% !TEX {magic_comments_key} =" in line:  # 如果关键字出现在这一行
-                            magic_comment = line.split(f"% !TEX {magic_comments_key} = ")[1].strip()  # 提取对应的值
-                            magic_comments[magic_comments_key] = magic_comment  # 将键值对存入字典
+'''
+ =======================================================================
+ ····Y88b···d88P················888b·····d888·d8b·······················
+ ·····Y88b·d88P·················8888b···d8888·Y8P·······················
+ ······Y88o88P··················88888b·d88888···························
+ ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
+ ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
+ ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
+ ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
+ ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
+ ·······························································888·····
+ ··························································Y8b·d88P·····
+ ···························································"Y88P"······
+ =======================================================================
+
+ -----------------------------------------------------------------------
+Author       : 焱铭
+Date         : 2024-02-29 16:02:37 +0800
+LastEditTime : 2024-04-27 10:01:49 +0800
+Github       : https://github.com/YanMing-lxb/
+FilePath     : \PyTeXMK\src\pytexmk\additional_operation.py
+Description  : 
+ -----------------------------------------------------------------------
+'''
+# -*- coding: utf-8 -*-
+import os
+import fitz
+import shutil
+from rich import print
+
+# --------------------------------------------------------------------------------
+# 定义清除辅助文件命令
+# --------------------------------------------------------------------------------
+def remove_aux(file_name):
+    auxiliary_files = [
+        f"{file_name}{ext}" for ext in [".aux", ".bbl", ".blg", ".log", ".out", ".toc", ".bcf",
+                                        ".xml", ".nlo", ".nls", ".bak", ".ind", ".idx", ".ilg", ".lof", ".spl",
+                                        ".lot", ".ent-x", ".tmp", ".ltx", ".los", ".lol", ".loc", ".listing", ".gz",
+                                        ".userbak", ".nav", ".snm", ".vrb", ".fls", ".xdv", ".fdb_latexmk", ".run.xml", ".ist", ".glo", ".gls"]
+    ]
+    file_exists = False
+    for file in auxiliary_files:
+        if os.path.exists(file):
+            try:
+                os.remove(file)
+                file_exists = True
+            except FileNotFoundError:
+                pass
+    if file_exists:
+        print("已清除辅助文件！")
+    else:
+        print("当前没有辅助文件！")
+
+# --------------------------------------------------------------------------------
+# 定义清除已有结果文件
+# --------------------------------------------------------------------------------
+def remove_result(outdir):
+    if os.path.exists(outdir):
+        shutil.rmtree(outdir)  # 删除整个文件夹
+        print(f"已删除 {outdir} 中的旧结果文件！")
+    
+def remove_result_in_root(file_name):
+    extensions = [".pdf", ".synctex.gz", ".synctex"]
+    for ext in extensions:
+        file = file_name + ext
+        if os.path.exists(file):
+            try:
+                os.remove(file)
+                print(f"{file} 已删除！")
+            except FileNotFoundError:
+                print(f"{file} 未能删除！")
+        else:
+            print(f"根目录下不存在 {file}")
+
+# --------------------------------------------------------------------------------
+# 定义移动生成文件
+# --------------------------------------------------------------------------------
+def move_result(file_name, outdir):
+    result_files = [f"{file_name}{ext}" for ext in [".pdf", ".synctex.gz"]]
+    os.mkdir(outdir)  # 创建空的 outdir 文件夹
+    for file in result_files:
+        if os.path.exists(file):
+            shutil.move(file, outdir)
+            print(f"{file} 移动到 {outdir}")
+        else:
+            print(f'{file} 不存在！')
+
+# --------------------------------------------------------------------------------
+# 定义清理所有 pdf 文件
+# --------------------------------------------------------------------------------
+def clean_pdf(root_dir, excluded_folder, file_name):
+    pdf_files = []
+    for root, dirs, files in os.walk(root_dir):
+        if excluded_folder in dirs:
+            dirs.remove(excluded_folder)  # 不包括名为excluded_folder的文件夹中的pdf文件
+        if root == root_dir: # 如果当前处理的是根目录文件，则跳过
+            continue 
+        for file in files:
+            if file.endswith('.pdf') and file != f'{file_name}.pdf':
+                pdf_files.append(os.path.join(root, file))  # 仅清理子文件夹中的pdf文件
+    
+    # 对pdf文件进行打开和关闭操作，解决origin批量导出pdf文件时由于未关闭pdf导致的报错
+    if pdf_files:
+        print(f"共发现 {len(pdf_files)} 个PDF文件。")
+        for pdf_file in pdf_files:
+            try:
+                doc = fitz.open(pdf_file)
+                doc.close()
+                print(f"已处理: {pdf_file}")
+            except Exception as e:
+                print(f"处理出错 {pdf_file}: {e}")
+        print("所有PDF文件已处理完成。")
+    else:
+        print("当前路径下未发现PDF文件。")
+    
+# --------------------------------------------------------------------------------
+# 定义输入检查函数
+# --------------------------------------------------------------------------------
+def check_file_name(file_name):
+    base_name, file_extension = os.path.splitext(
+        os.path.basename(file_name))  # 去掉路径，提取文件名和后缀
+    if file_extension == '.tex':  # 判断后缀是否是 .tex
+        file_name_return = base_name
+    elif '.' not in file_name:  # 判断输入 file_name 中没有 后缀
+        if '/' in file_name or '\\' in file_name:  # 判断是否是没有后缀的路径
+            file_name_return = None
+            print("错误：文件路径无效！")
+        else:
+            file_name_return = file_name
+    else:
+        file_name_return = None
+        print("提示：文件后缀不是.tex")
+
+    return file_name_return
+
+# --------------------------------------------------------------------------------
+# 定义 tex 文件检索函数
+# --------------------------------------------------------------------------------
+def search_tex_file():
+    current_path = os.getcwd() # 获取当前路径
+    # 遍历当前路径下的所有文件
+    tex_files = [file for file in os.listdir(current_path) if file.endswith('.tex')]
+    return tex_files
+
+# --------------------------------------------------------------------------------
+# 定义 tex 主文件检索函数
+# --------------------------------------------------------------------------------
+def search_main_file(tex_files):
+    current_path = os.getcwd() # 获取当前路径
+    if tex_files:
+        # 如果存在多个.tex文件
+        if 'main.tex' in tex_files:
+            # 存在名为main.tex的文件
+            file_name = 'main'
+            print(f"找到 {file_name}.tex 文件！")
+        # 如果只有一个.tex文件，则直接提取文件名并打印
+        elif len(tex_files) == 1:
+            file_name = os.path.splitext(tex_files[0])[0]
+            print(f"找到 {file_name}.tex 文件！")
+        elif len(tex_files) > 1:
+            # 存在多个.tex文件，但没有名为main.tex的文件
+            for file_path in tex_files:  # 遍历tex文件列表
+                with open(file_path, 'r', encoding='utf-8') as file:  # 打开文件
+                    for _ in range(200):  # 遍历文件的前200行
+                        line = file.readline()  # 读取一行内容
+                        if line.strip().startswith('%'):  # 如果是以 % 开头的行则跳过
+                            continue
+                        if ("\documentclass" in line or r"\begin{document}" in line):
+                            # 找到 \documentclass 或 \begin{document} 指令，提取文件名
+                            file_name = check_file_name(file_path)
+                            print(f"通过 \documentclass 或 \\begin{{document}} 指令，找到 {file_name}.tex 文件！")
+                            break
+        else:
+            # 不存在名为main.tex的文件，打印所有找到的.tex文件
+            file_name = None
+            print("存在多个 .tex 文件，请：修改主文件名为 main.tex 或在文件中加入魔法注释 “% !TEX = <主文件名>” 或在终端输入：pytexmk <主文件名> 名进行编译")
+            print("[bold][red]注意：主文件名一定要放在项目根目录下[/red][/bold]")
+    else:
+        # 不存在.tex文件，打印当前路径并提示
+        file_name = None
+        print("终端路径下不存在 .tex 文件！请检查终端显示路径是否是项目路径")
+        print(f"当前终端路径是：{current_path}")
+
+    return file_name
+
+# --------------------------------------------------------------------------------
+# 定义魔法注释检索函数
+# --------------------------------------------------------------------------------
+def search_magic_comments(tex_files, magic_comments_keys):
+    magic_comments = {}  # 创建空字典用于存储结果
+    if len(tex_files):
+        for file_path in tex_files:  # 遍历tex文件列表
+            with open(file_path, 'r', encoding='utf-8') as file:  # 打开文件
+                for _ in range(50):  # 遍历文件的前50行
+                    line = file.readline()  # 读取一行内容
+                    for magic_comments_key in magic_comments_keys:  # 遍历关键字列表
+                        if f"% !TEX {magic_comments_key} =" in line:  # 如果关键字出现在这一行
+                            magic_comment = line.split(f"% !TEX {magic_comments_key} = ")[1].strip()  # 提取对应的值
+                            magic_comments[magic_comments_key] = magic_comment  # 将键值对存入字典
     return magic_comments  # 返回提取的键值对字典
```

### Comparing `pytexmk-0.5.1.240426/src/pytexmk/compile_model.py` & `pytexmk-0.5.4.240427/src/pytexmk/compile_model.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-'''
- =======================================================================
- ····Y88b···d88P················888b·····d888·d8b·······················
- ·····Y88b·d88P·················8888b···d8888·Y8P·······················
- ······Y88o88P··················88888b·d88888···························
- ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
- ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
- ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
- ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
- ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
- ·······························································888·····
- ··························································Y8b·d88P·····
- ···························································"Y88P"······
- =======================================================================
-
- -----------------------------------------------------------------------
-Author       : 焱铭
-Date         : 2024-02-29 15:43:26 +0800
-LastEditTime : 2024-03-22 14:50:13 +0800
-Github       : https://github.com/YanMing-lxb/
-FilePath     : /PyTeXMK/src/pytexmk/compile_model.py
-Description  : 
- -----------------------------------------------------------------------
-'''
-# -*- coding: utf-8 -*-
-import os
-import re
-import subprocess
-from .info_print import print_message
-from rich import console
-console = console.Console()  # 设置宽度为80
-
-# --------------------------------------------------------------------------------
-# 定义编译 TeX 文件命令
-# --------------------------------------------------------------------------------
-def compile_tex(tex_name, file_name, tex_times, quiet):
-    options = [tex_name, "-shell-escape", "-file-line-error", "-halt-on-error", "-synctex=1", f'{file_name}.tex']
-    print_message(f"{tex_times} 次 {tex_name} 编译")
-    if tex_name == 'xelatex':
-        options.insert(5, "-no-pdf")
-    if quiet:
-        options.insert(4, "-interaction=batchmode") # 静默编译
-    else:
-        options.insert(4, "-interaction=nonstopmode") # 非静默编译
-    console.print(f"[bold]运行命令：[/bold][red][cyan]{' '.join(options)}[/cyan][/red]\n")
-    
-    try:
-        subprocess.run(options, check=True, text=True, capture_output=True)
-        return True
-    except subprocess.CalledProcessError as e:
-        print(e.output)
-        return False
-# --------------------------------------------------------------------------------
-# 定义编译参考文献命令
-# --------------------------------------------------------------------------------
-def compile_bib(file_name, quiet):
-    if os.path.exists(f"{file_name}.aux"):
-        with open(f"{file_name}.aux", 'r', encoding='utf-8') as aux_file:
-            aux_content = aux_file.read()
-
-        if re.search(r'\\bibdata|\\abx@aux@cite', aux_content):
-            if re.search(r'\\abx@aux@refcontext', aux_content):
-                name_target = "biber 编译"
-                print_message('biber 文献编译')
-                options = ["biber", file_name]
-                if quiet:
-                    options.insert(1, "-quiet") # 静默编译
-                console.print(f"[bold]运行命令：[/bold][cyan]{' '.join(options)}[/cyan]\n")
-            elif re.search(r'\\bibdata', aux_content):
-                name_target = 'bibtex 编译'
-                print_message('bibtex 文献编译')
-                options = ['bibtex', file_name]
-                console.print(f"[bold]运行命令：[/bold][cyan]{' '.join(options)}[/cyan]\n")
-            try:
-                subprocess.run(options, check=True, text=True, capture_output=True)
-                compile_tex_times = 2 # 参考文献需要额外编译的次数
-                print_bib = f"{name_target}参考文献"
-            except subprocess.CalledProcessError as e:
-                print(e.output)
-                return compile_tex_times, print_bib, name_target, False
-            
-        elif re.search(r'\\bibcite', aux_content):
-            compile_tex_times = 1
-            name_target = None
-            print_bib = "thebibliography 环境实现排版 "
-        else:
-            compile_tex_times = 0
-            name_target = None
-            print_bib = "没有引用参考文献或编译工具不属于 bibtex 或 biber "
-    else:
-        compile_tex_times = 0
-        name_target = None
-        print_bib = "文档没有参考文献"
-    return compile_tex_times, print_bib, name_target, True
-
-# --------------------------------------------------------------------------------
-# 定义编译目录索引命令
-# --------------------------------------------------------------------------------
-def compile_index(file_name):
-    if any(os.path.exists(f"{file_name}{ext}") for ext in [".glo", ".nlo", ".idx", ".toc"]):
-        if os.path.exists(f"{file_name}.glo"):
-            with open(f"{file_name}.glo", "r", encoding='utf-8') as f:
-                content = f.read()
-            if content.strip():  # Check if content is not empty
-                compile_tex_times = 1 # 目录和符号索引需要额外编译的次数
-                name_target = "glossaries 宏包"
-                print_message("glossaries 宏包")
-                print_index = "glossaries 宏包生成符号索引"
-                print(print_index,"\n")
-                options = ["makeindex", "-s", f"{file_name}.ist", "-o", f"{file_name}.gls", f"{file_name}.glo"]
-                console.print(f"[bold]运行命令：[/bold][cyan]{' '.join(options)}[/cyan]\n")
-                try:
-                    subprocess.run(options, check=True, text=True, capture_output=True)
-                except subprocess.CalledProcessError as e:
-                    print(e.output)
-                    return compile_tex_times, print_index, name_target, False
-            else:
-                compile_tex_times = 0
-                name_target = None
-                print_index = "glossaries 宏包没有进行索引"
-
-        elif os.path.exists(f"{file_name}.nlo"):
-            with open(f"{file_name}.nlo", "r", encoding='utf-8') as f:
-                content = f.read()
-            if content.strip():  # Check if content is not empty
-                compile_tex_times = 1
-                name_target = "nomencl 宏包"
-                print_message("nomencl 宏包")
-                print_index = "nomencl 宏包生成符号索引"
-                print(print_index,"\n")
-                options = ["makeindex", "-s", "nomencl.ist", "-o", f"{file_name}.nls", f"{file_name}.nlo"]
-                console.print(f"[bold]运行命令：[/bold][cyan]{' '.join(options)}[/cyan]\n")
-                try:
-                    subprocess.run(options, check=True, text=True, capture_output=True)
-                except subprocess.CalledProcessError as e:
-                    print(e.output)
-                    return compile_tex_times, print_index, name_target, False
-            else:
-                compile_tex_times = 0
-                name_target = None
-                print_index = "nomencl 宏包没有进行索引"
-        elif os.path.exists(f"{file_name}.idx"):
-            with open(f"{file_name}.idx", "r", encoding='utf-8') as f:
-                content = f.read()
-            if content.strip():  # Check if content is not empty
-                compile_tex_times = 1
-                name_target = "makeidx 宏包"
-                print_message("makeidx 宏包")
-                print_index = "makeidx 宏包生成索引"
-                print(print_index,"\n")
-                options = ["makeindex", f"{file_name}.idx"]
-                console.print(f"[bold]运行命令：[/bold][cyan]{' '.join(options)}[/cyan]\n")
-                try:
-                    subprocess.run(options, check=True, text=True, capture_output=True)
-                except subprocess.CalledProcessError as e:
-                    print(e.output)
-                    return compile_tex_times, print_index, name_target, False
-            else:
-                compile_tex_times = 0
-                name_target = None
-                print_index = "makeidx 宏包没有进行索引"  
-
-        else:
-            name_target = None
-            if os.path.exists(f"{file_name}.toc"):
-                compile_tex_times = 1 # 目录需要额外编译 1 次
-                print_index = "含有图/表/章节目录"
-            else:
-                compile_tex_times = 0
-                print_index = "没有图/表/章节目录"
-
-    else: 
-        compile_tex_times = 0
-        name_target = None
-        print_index = "没有插入任何目录或者使用 makeidx、glossaries、nomencl 等宏包"
-
-    return compile_tex_times, print_index, name_target, True
-
-# --------------------------------------------------------------------------------
-# 定义编译 xdv 文件命令
-# --------------------------------------------------------------------------------
-def compile_xdv(file_name, quiet):
-    print_message("dvipdfmx 编译")
-    options = ["dvipdfmx", "-V", "2.0", f"{file_name}"]
-    if quiet:
-        options.insert(1, "-q") # 静默编译
-    console.print(f"[bold]运行命令：[/bold][cyan]{' '.join(options)}[/cyan]\n")
-    try:
-        subprocess.run(options, check=True, text=True, capture_output=True)
-        return True
-    except subprocess.CalledProcessError as e:
-        print(e.output)
+'''
+ =======================================================================
+ ····Y88b···d88P················888b·····d888·d8b·······················
+ ·····Y88b·d88P·················8888b···d8888·Y8P·······················
+ ······Y88o88P··················88888b·d88888···························
+ ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
+ ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
+ ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
+ ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
+ ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
+ ·······························································888·····
+ ··························································Y8b·d88P·····
+ ···························································"Y88P"······
+ =======================================================================
+
+ -----------------------------------------------------------------------
+Author       : 焱铭
+Date         : 2024-02-29 15:43:26 +0800
+LastEditTime : 2024-03-22 14:50:13 +0800
+Github       : https://github.com/YanMing-lxb/
+FilePath     : /PyTeXMK/src/pytexmk/compile_model.py
+Description  : 
+ -----------------------------------------------------------------------
+'''
+# -*- coding: utf-8 -*-
+import os
+import re
+import subprocess
+from .info_print import print_message
+from rich import console
+console = console.Console()  # 设置宽度为80
+
+# --------------------------------------------------------------------------------
+# 定义编译 TeX 文件命令
+# --------------------------------------------------------------------------------
+def compile_tex(tex_name, file_name, tex_times, quiet):
+    options = [tex_name, "-shell-escape", "-file-line-error", "-halt-on-error", "-synctex=1", f'{file_name}.tex']
+    print_message(f"{tex_times} 次 {tex_name} 编译")
+    if tex_name == 'xelatex':
+        options.insert(5, "-no-pdf")
+    if quiet:
+        options.insert(4, "-interaction=batchmode") # 静默编译
+    else:
+        options.insert(4, "-interaction=nonstopmode") # 非静默编译
+    console.print(f"[bold]运行命令：[/bold][red][cyan]{' '.join(options)}[/cyan][/red]\n")
+    
+    try:
+        subprocess.run(options, check=True, text=True, capture_output=True)
+        return True
+    except subprocess.CalledProcessError as e:
+        print(e.output)
+        return False
+# --------------------------------------------------------------------------------
+# 定义编译参考文献命令
+# --------------------------------------------------------------------------------
+def compile_bib(file_name, quiet):
+    if os.path.exists(f"{file_name}.aux"):
+        with open(f"{file_name}.aux", 'r', encoding='utf-8') as aux_file:
+            aux_content = aux_file.read()
+
+        if re.search(r'\\bibdata|\\abx@aux@cite', aux_content):
+            if re.search(r'\\abx@aux@refcontext', aux_content):
+                name_target = "biber 编译"
+                print_message('biber 文献编译')
+                options = ["biber", file_name]
+                if quiet:
+                    options.insert(1, "-quiet") # 静默编译
+                console.print(f"[bold]运行命令：[/bold][cyan]{' '.join(options)}[/cyan]\n")
+            elif re.search(r'\\bibdata', aux_content):
+                name_target = 'bibtex 编译'
+                print_message('bibtex 文献编译')
+                options = ['bibtex', file_name]
+                console.print(f"[bold]运行命令：[/bold][cyan]{' '.join(options)}[/cyan]\n")
+            try:
+                subprocess.run(options, check=True, text=True, capture_output=True)
+                compile_tex_times = 2 # 参考文献需要额外编译的次数
+                print_bib = f"{name_target}参考文献"
+            except subprocess.CalledProcessError as e:
+                print(e.output)
+                return compile_tex_times, print_bib, name_target, False
+            
+        elif re.search(r'\\bibcite', aux_content):
+            compile_tex_times = 1
+            name_target = None
+            print_bib = "thebibliography 环境实现排版 "
+        else:
+            compile_tex_times = 0
+            name_target = None
+            print_bib = "没有引用参考文献或编译工具不属于 bibtex 或 biber "
+    else:
+        compile_tex_times = 0
+        name_target = None
+        print_bib = "文档没有参考文献"
+    return compile_tex_times, print_bib, name_target, True
+
+# --------------------------------------------------------------------------------
+# 定义编译目录索引命令
+# --------------------------------------------------------------------------------
+def compile_index(file_name):
+    if any(os.path.exists(f"{file_name}{ext}") for ext in [".glo", ".nlo", ".idx", ".toc"]):
+        if os.path.exists(f"{file_name}.glo"):
+            with open(f"{file_name}.glo", "r", encoding='utf-8') as f:
+                content = f.read()
+            if content.strip():  # Check if content is not empty
+                compile_tex_times = 1 # 目录和符号索引需要额外编译的次数
+                name_target = "glossaries 宏包"
+                print_message("glossaries 宏包")
+                print_index = "glossaries 宏包生成符号索引"
+                print(print_index,"\n")
+                options = ["makeindex", "-s", f"{file_name}.ist", "-o", f"{file_name}.gls", f"{file_name}.glo"]
+                console.print(f"[bold]运行命令：[/bold][cyan]{' '.join(options)}[/cyan]\n")
+                try:
+                    subprocess.run(options, check=True, text=True, capture_output=True)
+                except subprocess.CalledProcessError as e:
+                    print(e.output)
+                    return compile_tex_times, print_index, name_target, False
+            else:
+                compile_tex_times = 0
+                name_target = None
+                print_index = "glossaries 宏包没有进行索引"
+
+        elif os.path.exists(f"{file_name}.nlo"):
+            with open(f"{file_name}.nlo", "r", encoding='utf-8') as f:
+                content = f.read()
+            if content.strip():  # Check if content is not empty
+                compile_tex_times = 1
+                name_target = "nomencl 宏包"
+                print_message("nomencl 宏包")
+                print_index = "nomencl 宏包生成符号索引"
+                print(print_index,"\n")
+                options = ["makeindex", "-s", "nomencl.ist", "-o", f"{file_name}.nls", f"{file_name}.nlo"]
+                console.print(f"[bold]运行命令：[/bold][cyan]{' '.join(options)}[/cyan]\n")
+                try:
+                    subprocess.run(options, check=True, text=True, capture_output=True)
+                except subprocess.CalledProcessError as e:
+                    print(e.output)
+                    return compile_tex_times, print_index, name_target, False
+            else:
+                compile_tex_times = 0
+                name_target = None
+                print_index = "nomencl 宏包没有进行索引"
+        elif os.path.exists(f"{file_name}.idx"):
+            with open(f"{file_name}.idx", "r", encoding='utf-8') as f:
+                content = f.read()
+            if content.strip():  # Check if content is not empty
+                compile_tex_times = 1
+                name_target = "makeidx 宏包"
+                print_message("makeidx 宏包")
+                print_index = "makeidx 宏包生成索引"
+                print(print_index,"\n")
+                options = ["makeindex", f"{file_name}.idx"]
+                console.print(f"[bold]运行命令：[/bold][cyan]{' '.join(options)}[/cyan]\n")
+                try:
+                    subprocess.run(options, check=True, text=True, capture_output=True)
+                except subprocess.CalledProcessError as e:
+                    print(e.output)
+                    return compile_tex_times, print_index, name_target, False
+            else:
+                compile_tex_times = 0
+                name_target = None
+                print_index = "makeidx 宏包没有进行索引"  
+
+        else:
+            name_target = None
+            if os.path.exists(f"{file_name}.toc"):
+                compile_tex_times = 1 # 目录需要额外编译 1 次
+                print_index = "含有图/表/章节目录"
+            else:
+                compile_tex_times = 0
+                print_index = "没有图/表/章节目录"
+
+    else: 
+        compile_tex_times = 0
+        name_target = None
+        print_index = "没有插入任何目录或者使用 makeidx、glossaries、nomencl 等宏包"
+
+    return compile_tex_times, print_index, name_target, True
+
+# --------------------------------------------------------------------------------
+# 定义编译 xdv 文件命令
+# --------------------------------------------------------------------------------
+def compile_xdv(file_name, quiet):
+    print_message("dvipdfmx 编译")
+    options = ["dvipdfmx", "-V", "2.0", f"{file_name}"]
+    if quiet:
+        options.insert(1, "-q") # 静默编译
+    console.print(f"[bold]运行命令：[/bold][cyan]{' '.join(options)}[/cyan]\n")
+    try:
+        subprocess.run(options, check=True, text=True, capture_output=True)
+        return True
+    except subprocess.CalledProcessError as e:
+        print(e.output)
         return False
```

### Comparing `pytexmk-0.5.1.240426/src/pytexmk/info_print.py` & `pytexmk-0.5.4.240427/src/pytexmk/info_print.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-'''
- =======================================================================
- ····Y88b···d88P················888b·····d888·d8b·······················
- ·····Y88b·d88P·················8888b···d8888·Y8P·······················
- ······Y88o88P··················88888b·d88888···························
- ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
- ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
- ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
- ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
- ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
- ·······························································888·····
- ··························································Y8b·d88P·····
- ···························································"Y88P"······
- =======================================================================
-
- -----------------------------------------------------------------------
-Author       : 焱铭
-Date         : 2024-03-03 10:34:41 +0800
-LastEditTime : 2024-03-22 14:50:06 +0800
-Github       : https://github.com/YanMing-lxb/
-FilePath     : /PyTeXMK/src/pytexmk/info_print.py
-Description  : 
- -----------------------------------------------------------------------
-'''
-# -*- coding: utf-8 -*-
-import datetime
-from rich.console import Console
-from rich.table import Table
-from rich import box
-from rich import print
-console = Console() # 创建控制台对象
-# --------------------------------------------------------------------------------
-# 定义时间统计函数
-# --------------------------------------------------------------------------------
-def time_count(fun, *args):
-    time_start = datetime.datetime.now()
-    fun_return = fun(*args)
-    time_end = datetime.datetime.now()
-    time_run = time_end - time_start
-
-    time_run = round(time_run.total_seconds(), 4)
-    return time_run, fun_return
-
-# --------------------------------------------------------------------------------
-# 定义信息打印函数
-# --------------------------------------------------------------------------------
-def print_message(message):
-    padding_size = 80 - (len(message) + sum(1 for c in message if not c.isascii()))-4  # 计算左右两侧 X 的数量
-    left_padding = int(padding_size / 2)
-    right_padding = padding_size - left_padding
-    banner = "[not bold]X[/not bold]" * left_padding + f"| {message} |" + "[not bold]X[/not bold]" * right_padding
-    console.print("\n\n" + "=" * 80, style="yellow bold")
-    console.print(banner, style="red on white bold")
-    console.print("=" * 80 + "\n\n", style="yellow bold")
-    
-
-# --------------------------------------------------------------------------------
-# 定义统计时间打印函数
-# --------------------------------------------------------------------------------
-def time_print(start_time, name_target_list, time_run_list):
-    end_time = datetime.datetime.now() # 计算结束时间
-    run_time = end_time - start_time
-    hours, remainder = divmod(run_time.seconds, 3600)
-    minutes, seconds = divmod(remainder, 60)
-    milliseconds = run_time.microseconds // 1000  # 获取毫秒部分
-
-    number_programmes_run = len(name_target_list)-4
-    
-    time_compile = sum(time_run_list)
-    name_target_list.append('LaTeX 编译时长')
-    time_run_list.append(time_compile)
-
-    time_other_operating = float(run_time.total_seconds()) - time_compile
-    name_target_list.append('Python 运行时长')
-    time_run_list.append(time_other_operating)
-
-    time_pytexmk = float(run_time.total_seconds())
-    name_target_list.append('PyTeXMK 运行时长')
-    time_run_list.append(time_pytexmk)
-
-    # 创建表格对象
-    table = Table(show_header=True, header_style="bold magenta", box=box.ASCII_DOUBLE_HEAD, 
-                title="PyTeXMK 运行时长统计表")
-
-    # 定义列名
-    table.add_column("序号", justify="center", no_wrap=True)
-    table.add_column("运行项目", style="cyan", justify="center", no_wrap=True)
-    table.add_column("运行时长", style="green", justify="center", no_wrap=True)
-    table.add_column("序号", justify="center", no_wrap=True)
-    table.add_column("运行项目", style="cyan", justify="center")
-    table.add_column("运行时长", style="green", justify="center", no_wrap=True)
-
-    # 判断统计项目列数是否是偶数
-    length = len(name_target_list)/2 # 计算打印表格列数
-    row_num = None
-
-    # 判断统计项目列数是否是偶数
-    if length - int(length) < 0.5:
-        row_num = int(length)
-    else: # 是偶数则加一
-        row_num = int(length) + 1 
-
-    # 添加数据到表格
-    for i in range(row_num):
-        table.add_row(
-            str(i+1),
-            name_target_list[i],
-            "{:.4f} s".format(time_run_list[i]),
-            str(i+1+row_num) if i+row_num <= len(name_target_list) else "",
-            name_target_list[i+row_num] if i+row_num < len(name_target_list) else "",
-            "{:.4f} s".format(time_run_list[i+row_num]) if i+row_num < len(name_target_list) else ""  
-        )
-
-    print("\n" + "=" * 80 + "\n")
-    console.print(table) # 打印表格
-
-    print(f"PyTeXMK 运行时长：{hours} 小时 {minutes} 分 {seconds} 秒 {milliseconds} 毫秒 ({run_time.total_seconds():.3f} s total)")
+'''
+ =======================================================================
+ ····Y88b···d88P················888b·····d888·d8b·······················
+ ·····Y88b·d88P·················8888b···d8888·Y8P·······················
+ ······Y88o88P··················88888b·d88888···························
+ ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
+ ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
+ ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
+ ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
+ ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
+ ·······························································888·····
+ ··························································Y8b·d88P·····
+ ···························································"Y88P"······
+ =======================================================================
+
+ -----------------------------------------------------------------------
+Author       : 焱铭
+Date         : 2024-03-03 10:34:41 +0800
+LastEditTime : 2024-03-22 14:50:06 +0800
+Github       : https://github.com/YanMing-lxb/
+FilePath     : /PyTeXMK/src/pytexmk/info_print.py
+Description  : 
+ -----------------------------------------------------------------------
+'''
+# -*- coding: utf-8 -*-
+import datetime
+from rich.console import Console
+from rich.table import Table
+from rich import box
+from rich import print
+console = Console() # 创建控制台对象
+# --------------------------------------------------------------------------------
+# 定义时间统计函数
+# --------------------------------------------------------------------------------
+def time_count(fun, *args):
+    time_start = datetime.datetime.now()
+    fun_return = fun(*args)
+    time_end = datetime.datetime.now()
+    time_run = time_end - time_start
+
+    time_run = round(time_run.total_seconds(), 4)
+    return time_run, fun_return
+
+# --------------------------------------------------------------------------------
+# 定义信息打印函数
+# --------------------------------------------------------------------------------
+def print_message(message):
+    padding_size = 80 - (len(message) + sum(1 for c in message if not c.isascii()))-4  # 计算左右两侧 X 的数量
+    left_padding = int(padding_size / 2)
+    right_padding = padding_size - left_padding
+    banner = "[not bold]X[/not bold]" * left_padding + f"| {message} |" + "[not bold]X[/not bold]" * right_padding
+    console.print("\n\n" + "=" * 80, style="yellow bold")
+    console.print(banner, style="red on white bold")
+    console.print("=" * 80 + "\n\n", style="yellow bold")
+    
+
+# --------------------------------------------------------------------------------
+# 定义统计时间打印函数
+# --------------------------------------------------------------------------------
+def time_print(start_time, name_target_list, time_run_list):
+    end_time = datetime.datetime.now() # 计算结束时间
+    run_time = end_time - start_time
+    hours, remainder = divmod(run_time.seconds, 3600)
+    minutes, seconds = divmod(remainder, 60)
+    milliseconds = run_time.microseconds // 1000  # 获取毫秒部分
+
+    number_programmes_run = len(name_target_list)-4
+    
+    time_compile = sum(time_run_list)
+    name_target_list.append('LaTeX 编译时长')
+    time_run_list.append(time_compile)
+
+    time_other_operating = float(run_time.total_seconds()) - time_compile
+    name_target_list.append('Python 运行时长')
+    time_run_list.append(time_other_operating)
+
+    time_pytexmk = float(run_time.total_seconds())
+    name_target_list.append('PyTeXMK 运行时长')
+    time_run_list.append(time_pytexmk)
+
+    # 创建表格对象
+    table = Table(show_header=True, header_style="bold magenta", box=box.ASCII_DOUBLE_HEAD, 
+                title="PyTeXMK 运行时长统计表")
+
+    # 定义列名
+    table.add_column("序号", justify="center", no_wrap=True)
+    table.add_column("运行项目", style="cyan", justify="center", no_wrap=True)
+    table.add_column("运行时长", style="green", justify="center", no_wrap=True)
+    table.add_column("序号", justify="center", no_wrap=True)
+    table.add_column("运行项目", style="cyan", justify="center")
+    table.add_column("运行时长", style="green", justify="center", no_wrap=True)
+
+    # 判断统计项目列数是否是偶数
+    length = len(name_target_list)/2 # 计算打印表格列数
+    row_num = None
+
+    # 判断统计项目列数是否是偶数
+    if length - int(length) < 0.5:
+        row_num = int(length)
+    else: # 是偶数则加一
+        row_num = int(length) + 1 
+
+    # 添加数据到表格
+    for i in range(row_num):
+        table.add_row(
+            str(i+1),
+            name_target_list[i],
+            "{:.4f} s".format(time_run_list[i]),
+            str(i+1+row_num) if i+row_num <= len(name_target_list) else "",
+            name_target_list[i+row_num] if i+row_num < len(name_target_list) else "",
+            "{:.4f} s".format(time_run_list[i+row_num]) if i+row_num < len(name_target_list) else ""  
+        )
+
+    print("\n" + "=" * 80 + "\n")
+    console.print(table) # 打印表格
+
+    print(f"PyTeXMK 运行时长：{hours} 小时 {minutes} 分 {seconds} 秒 {milliseconds} 毫秒 ({run_time.total_seconds():.3f} s total)")
     print(f"运行函数：{number_programmes_run} 个")
```

### Comparing `pytexmk-0.5.1.240426/src/pytexmk/version.py` & `pytexmk-0.5.4.240427/src/pytexmk/version.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-'''
- =======================================================================
- ····Y88b···d88P················888b·····d888·d8b·······················
- ·····Y88b·d88P·················8888b···d8888·Y8P·······················
- ······Y88o88P··················88888b·d88888···························
- ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
- ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
- ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
- ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
- ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
- ·······························································888·····
- ··························································Y8b·d88P·····
- ···························································"Y88P"······
- =======================================================================
-
- -----------------------------------------------------------------------
-Author       : 焱铭
-Date         : 2024-03-01 15:52:28 +0800
-LastEditTime : 2024-04-26 23:19:26 +0800
-Github       : https://github.com/YanMing-lxb/
-FilePath     : /PyTeXMK/src/pytexmk/version.py
-Description  : 
- -----------------------------------------------------------------------
-'''
-# -*- coding: utf-8 -*-
-#!/usr/bin/env python
-
-script_name = 'PyTeXMK'
-__version__ = '0.5.1.240426'
+'''
+ =======================================================================
+ ····Y88b···d88P················888b·····d888·d8b·······················
+ ·····Y88b·d88P·················8888b···d8888·Y8P·······················
+ ······Y88o88P··················88888b·d88888···························
+ ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
+ ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
+ ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
+ ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
+ ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
+ ·······························································888·····
+ ··························································Y8b·d88P·····
+ ···························································"Y88P"······
+ =======================================================================
+
+ -----------------------------------------------------------------------
+Author       : 焱铭
+Date         : 2024-03-01 15:52:28 +0800
+LastEditTime : 2024-04-27 09:34:31 +0800
+Github       : https://github.com/YanMing-lxb/
+FilePath     : \PyTeXMK\src\pytexmk\version.py
+Description  : 
+ -----------------------------------------------------------------------
+'''
+# -*- coding: utf-8 -*-
+#!/usr/bin/env python
+
+script_name = 'PyTeXMK'
+__version__ = '0.5.4.240427'
```

### Comparing `pytexmk-0.5.1.240426/src/pytexmk.egg-info/PKG-INFO` & `pytexmk-0.5.4.240427/src/pytexmk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,152 +1,158 @@
-Metadata-Version: 2.1
-Name: pytexmk
-Version: 0.5.1.240426
-Summary: LaTeX 辅助编译命令行工具 LaTeX Auxiliary Compilation Command Line Tool
-Author-email: 焱铭 <lxb-yanming@foxmail.com>
-Project-URL: Homepage, https://github.com/YanMing-lxb/PyTeXMK
-Project-URL: Bug Tracker, https://github.com/YanMing-lxb/PyTeXMK/issues
-Keywords: LaTeX,build,latexmk
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers 
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: rich
-Requires-Dist: pymupdf
-
-<!--
- *  =======================================================================
- *  ····Y88b···d88P················888b·····d888·d8b·······················
- *  ·····Y88b·d88P·················8888b···d8888·Y8P·······················
- *  ······Y88o88P··················88888b·d88888···························
- *  ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
- *  ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
- *  ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
- *  ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
- *  ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
- *  ·······························································888·····
- *  ··························································Y8b·d88P·····
- *  ···························································"Y88P"······
- *  =======================================================================
- * 
- *  -----------------------------------------------------------------------
- * Author       : 焱铭
- * Date         : 2024-02-29 10:23:19 +0800
- * LastEditTime : 2024-04-26 22:37:00 +0800
- * Github       : https://github.com/YanMing-lxb/
- * FilePath     : /PyTeXMK/README.md
- * Description  : 
- *  -----------------------------------------------------------------------
- -->
-
-# PyTeXMK
-
-[![GitHub](https://img.shields.io/badge/Github-PyTeXMK-000000.svg)](https://github.com/YanMing-lxb/PyTeXMK) [![License](https://img.shields.io/badge/license-GPLv3-aff)](https://www.latex-project.org/lppl/) ![OS](https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg) [![GitHub release](https://img.shields.io/github/release/YanMing-lxb/PyTeXMK.svg?color=blueviolet&label=version&style=popout)](https://github.com/YanMing-lxb/PyTeXMK/releases/latest) [![Last Commit](https://img.shields.io/github/last-commit/YanMing-lxb/PyTeXMK)](https://github.com/YanMing-lxb/PyTeXMK/zipball/master) [![Issues](https://img.shields.io/github/issues/YanMing-lxb/PyTeXMK)](https://github.com/YanMing-lxb/PyTeXMK/issues) [![Github Action](https://github.com/YanMing-lxb/PyTeXMK/workflows/Test/badge.svg)](https://github.com/YanMing-lxb/PyTeXMK/actions) [![PyPI version](https://img.shields.io/pypi/v/pytexmk.svg)](https://pypi.python.org/pypi/pytexmk/) [![PyPI Downloads](https://img.shields.io/pypi/dm/pytexmk.svg?label=PyPI%20downloads)](https://pypi.org/project/pytexmk/) ![GitHub repo size](https://img.shields.io/github/repo-size/YanMing-lxb/PyTeXMK)
-
-LaTeX 辅助编译命令行程序 LaTeX Auxiliary Compilation Command Line Tool
-
----
-
-## 安装
-
-官方版本 PyTeXMK 发布在 [PyPI](https://pypi.org/project/pytexmk/) 上，并且可以通过 pip 包管理器从 PyPI 镜像轻松安装。
-
-请注意，您必须使用 Python 3 版本pip：
-
-```
-pip3 install pytexmk
-```
-
-## 升级
-
-```
-pip3 install --upgrade pytexmk
-```
-
-## 使用入门
-
-PyTeXMK 默认参数：`xelatex` 编译、主文件名 main、batch 模式（编译过程信息不显，如需显示编译过程信息请使用 `-nq` 参数）、编译结果存放在 LaTeX 项目的 Build 文件夹下 ( VSCode 用户则需要在 `settings.json` 中注意设置 `"latex-workshop.latex.outDir": "./Build",` 使得latex workshop 能够找到pdf )。
-
-请仔细阅读：[主文件及编译类型选定逻辑](#主文件及编译类型选定逻辑)
-
-### 编译命令
-PyTeXMK 支持：
-
-- 编译命令：`xelatex` `pdflatex` `lualatex`
-- 参考文献：`bibtex` `biblatex` `thebibliography`
-- 符号索引：`glossaries` `nomencl` `mkeidx`
-
-位置参数:
-| Option              | Description                    |
-|---------------------|-------------------------------|
-| document          | 要被编译的文件名                   |
-
-选项:
-| Option           | Description                                |
-|------------------|--------------------------------------------|
-| -h, --help       | 显示帮助信息                                 |
-| -v, --version    | 显示程序版本号                               |
-| -p, --pdflatex   | pdflatex 进行编译                           |
-| -x, --xelatex    | xelatex 进行编译                            |
-| -l, --lualatex   | lualatex 进行编译                           |
-| -c, --clean      | 清除所有辅助文件                              |
-| -C, --Clean      | 清除所有辅助文件和 pdf 文件                    |
-| -nq, --no-quiet  | 非安静模式运行，此模式下显示编译过程             |
-| -cp, --clean-pdf  | 清理所有 pdf 文件             |
-
-**说明：**
-`-cp` 参数的功能是 "当 LaTeX 编译过程中报类似 `invalid X X R object at offset XXXXX` 的警告时，可使用此参数清理所有 pdf 文件"
-
-### 魔法注释
-
-PyTeXMK 支持使用魔法注释来自定义编译命令、编译类型、编译结果存放位置等。    
-
-| Magic Comment | Description                                |
-|---------------|----------|
-| `% !TEX program = xelatex` | 指定编译类型，可选 `xelatex` `pdflatex` `lualatex` |
-| `% !TEX root = file.tex` | 指定主 LaTeX 文件名，仅支持主文件在项目根目录下的情况 |
-| `% !TEX outdir = PDFfile` | 指定编译结果存放位置，仅支持文件夹名称，如果使用 LaTeX-Workshop，则需要在 `settings.json` 中设置 `"latex-workshop.latex.outDir": "./PDFfile",` |
-
-### 主文件及编译类型选定逻辑
-- PyTeXMK 优先使用终端输入命令 `-p` `-x` `-l` 参数指定的编译类型，如果没有指定，则会使用 `% !TEX program = xelatex` 指定的编译类型，如果没有指定，则会使用默认的编译类型 `xelatex`
-- PyTeXMK 主文件选定逻辑顺序：
-    1. 使用终端输入的文件名
-    2. 使用 `% !TEX root = file.tex` 指定的主 LaTeX 文件名
-    3. 使用默认的主文件名 `main`
-    4. 检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
-    5. 根目录下 TeX 文件中只有一个文件，则选择该文件作为主文件
-        
-- PyTeXMK 会优先使用 `% !TEX outdir = PDFfile` 指定的编译结果存放位置，如果没有指定，则会使用默认的编译结果存放位置 `Build`
-
-# 更新日志
-
-- 2024-03-22 完善编译过程出错后的中断处理机制：在编译过程中出现错误时，程序会自动中断，并提示 `请用 -nq 模式运行以显示错误信息！`,使用 `-nq` 参数运行时，则会显示错误信息。
-- 2024-04-26 增加：
-    1. 魔法注释功能，使得用户可以自定义编译命令、编译类型、编译结果存放位置等
-    2. 完善主文件及编译类型选定逻辑
-
-
-# 未来工作方向
-
-- [X] 完善编译过程出错后的中断处理机制
-- [ ] 完善检索主 LaTeX 文件的功能：
-    - [X] 根据魔法注释 `% !TEX root = file.tex` 找到主 LaTeX 文件
-    - [ ] 通过检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
-- [ ] 完善自动判断编译类型：
-    - [X] 根据魔法注释 `% !TEX program = xelatex` 设置需要编译的类型
-- [x] 通过魔法注释设置编译结果存放位置
-- [X] 通过魔法注释实现编译命令的自定义
-- [ ] 增加配置文件功能，用于改变默认设置
-    - [ ] 指定生成的结果文件存放位置（目前默认存放在 `Build` 子文件夹下）
-    - [ ] 默认的编译命令（目前默认编译命令是 `xelatex`）
-- [ ] texlive 宏包检缺失并自动安装
-- [ ] 多主文件编译功能
+Metadata-Version: 2.1
+Name: pytexmk
+Version: 0.5.4.240427
+Summary: LaTeX 辅助编译命令行工具 LaTeX Auxiliary Compilation Command Line Tool
+Author-email: 焱铭 <lxb-yanming@foxmail.com>
+Project-URL: Homepage, https://github.com/YanMing-lxb/PyTeXMK
+Project-URL: Bug Tracker, https://github.com/YanMing-lxb/PyTeXMK/issues
+Keywords: LaTeX,build,latexmk
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers 
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: rich
+Requires-Dist: pymupdf
+
+<!--
+ *  =======================================================================
+ *  ····Y88b···d88P················888b·····d888·d8b·······················
+ *  ·····Y88b·d88P·················8888b···d8888·Y8P·······················
+ *  ······Y88o88P··················88888b·d88888···························
+ *  ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
+ *  ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
+ *  ········888···d888888·888··888·888··Y8P··888·888·888··888·888··888·····
+ *  ········888··888··888·888··888·888···"···888·888·888··888·Y88b·888·····
+ *  ········888··"Y888888·888··888·888·······888·888·888··888··"Y88888·····
+ *  ·······························································888·····
+ *  ··························································Y8b·d88P·····
+ *  ···························································"Y88P"······
+ *  =======================================================================
+ * 
+ *  -----------------------------------------------------------------------
+ * Author       : 焱铭
+ * Date         : 2024-02-29 10:23:19 +0800
+ * LastEditTime : 2024-04-27 10:10:51 +0800
+ * Github       : https://github.com/YanMing-lxb/
+ * FilePath     : \PyTeXMK\README.md
+ * Description  : 
+ *  -----------------------------------------------------------------------
+ -->
+
+# PyTeXMK
+
+[![GitHub](https://img.shields.io/badge/Github-PyTeXMK-000000.svg)](https://github.com/YanMing-lxb/PyTeXMK) [![License](https://img.shields.io/badge/license-GPLv3-aff)](https://www.latex-project.org/lppl/) ![OS](https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg) [![GitHub release](https://img.shields.io/github/release/YanMing-lxb/PyTeXMK.svg?color=blueviolet&label=version&style=popout)](https://github.com/YanMing-lxb/PyTeXMK/releases/latest) [![Last Commit](https://img.shields.io/github/last-commit/YanMing-lxb/PyTeXMK)](https://github.com/YanMing-lxb/PyTeXMK/zipball/master) [![Issues](https://img.shields.io/github/issues/YanMing-lxb/PyTeXMK)](https://github.com/YanMing-lxb/PyTeXMK/issues) [![Github Action](https://github.com/YanMing-lxb/PyTeXMK/workflows/Test/badge.svg)](https://github.com/YanMing-lxb/PyTeXMK/actions) [![PyPI version](https://img.shields.io/pypi/v/pytexmk.svg)](https://pypi.python.org/pypi/pytexmk/) [![PyPI Downloads](https://img.shields.io/pypi/dm/pytexmk.svg?label=PyPI%20downloads)](https://pypi.org/project/pytexmk/) ![GitHub repo size](https://img.shields.io/github/repo-size/YanMing-lxb/PyTeXMK)
+
+LaTeX 辅助编译命令行程序 LaTeX Auxiliary Compilation Command Line Tool
+
+---
+
+## 安装
+
+官方版本 PyTeXMK 发布在 [PyPI](https://pypi.org/project/pytexmk/) 上，并且可以通过 pip 包管理器从 PyPI 镜像轻松安装。
+
+请注意，您必须使用 Python 3 版本pip：
+
+```
+pip3 install pytexmk
+```
+
+## 升级
+
+```
+pip3 install --upgrade pytexmk
+```
+
+## 使用入门
+
+PyTeXMK 默认参数：`xelatex` 编译、主文件名 main.tex、batch 模式（编译过程信息不显，如需显示编译过程信息请使用 `-nq` 参数）、编译结果存放在 LaTeX 项目的 Build 文件夹下 ( VSCode 用户则需要在 `settings.json` 中注意设置 `"latex-workshop.latex.outDir": "./Build",` 使得 LaTeX-Workshop 能够找到 pdf )。
+
+请仔细阅读：[主文件及编译类型选定逻辑](#主文件及编译类型选定逻辑)
+
+> PyTeXMK，仅支持 utf-8 编码的 TeX 文件。
+
+### 编译命令
+PyTeXMK 支持：
+
+- 编译命令：`xelatex` `pdflatex` `lualatex`
+- 参考文献：`bibtex` `biblatex` `thebibliography`
+- 符号索引：`glossaries` `nomencl` `mkeidx`
+
+位置参数:
+| Option              | Description                    |
+|---------------------|-------------------------------|
+| document          | 要被编译的文件名                   |
+
+选项:
+| Option           | Description                                |
+|------------------|--------------------------------------------|
+| -h, --help       | 显示帮助信息                                 |
+| -v, --version    | 显示程序版本号                               |
+| -p, --pdflatex   | pdflatex 进行编译                           |
+| -x, --xelatex    | xelatex 进行编译                            |
+| -l, --lualatex   | lualatex 进行编译                           |
+| -c, --clean      | 清除所有辅助文件                              |
+| -C, --Clean      | 清除所有辅助文件和 pdf 文件                    |
+| -nq, --no-quiet  | 非安静模式运行，此模式下显示编译过程             |
+| -cp, --clean-pdf  | 清理所有 pdf 文件                          |
+
+**说明：**
+`-cp` 参数的功能是 "当 LaTeX 编译过程中报类似 `invalid X X R object at offset XXXXX` 的警告时，可使用此参数清理所有 pdf 文件"
+
+### 魔法注释
+
+PyTeXMK 支持使用魔法注释来自定义编译命令、编译类型、编译结果存放位置等（仅支持检索文档前 50 行）。    
+
+| Magic Comment | Description                                |
+|---------------|----------|
+| `% !TEX program = xelatex` | 指定编译类型，可选 `xelatex` `pdflatex` `lualatex` |
+| `% !TEX root = file.tex` | 指定主 LaTeX 文件名，仅支持主文件在项目根目录下的情况 |
+| `% !TEX outdir = PDFfile` | 指定编译结果存放位置，仅支持文件夹名称，如果使用 LaTeX-Workshop，则需要在 `settings.json` 中设置 `"latex-workshop.latex.outDir": "./PDFfile",` |
+
+### 主文件及编译类型选定逻辑
+
+- PyTeXMK 优先使用终端输入命令 `-p` `-x` `-l` 参数指定的编译类型，如果没有指定，则会使用 `% !TEX program = xelatex` 指定的编译类型，如果没有指定，则会使用默认的编译类型 `xelatex`
+- PyTeXMK 主文件选定逻辑顺序：
+    1. 使用终端输入的文件名
+    2. 使用 `% !TEX root = file.tex` 指定的主 LaTeX 文件名
+    3. 使用默认的主文件名 `main.tex`
+    4. 检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断（仅支持检索文档前 200 行）
+    5. 根目录下 TeX 文件中只有一个文件，则选择该文件作为主文件
+        
+- PyTeXMK 会优先使用 `% !TEX outdir = PDFfile` 指定的编译结果存放位置，如果没有指定，则会使用默认的编译结果存放位置 `Build`
+
+# 更新日志
+
+- 2024-03-22 完善编译过程出错后的中断处理机制：在编译过程中出现错误时，程序会自动中断，并提示 `请用 -nq 模式运行以显示错误信息！`，使用 `-nq` 参数运行时，则会显示错误信息。
+- 2024-04-26 增加：
+    1. 魔法注释功能，使得用户可以自定义编译命令、编译类型、编译结果存放位置等
+    2. 完善主文件及编译类型选定逻辑
+- 2024-04-26 
+    1. 修复边 \documentclass 和 \begin{document} 检索逻辑。
+    2. 解决文档读取编码导致的报错。
+
+
+# 未来工作方向
+
+- [X] 完善编译过程出错后的中断处理机制
+- [ ] 完善检索主 LaTeX 文件的功能：
+    - [X] 根据魔法注释 `% !TEX root = file.tex` 找到主 LaTeX 文件
+    - [X] 通过检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
+- [ ] 完善自动判断编译类型：
+    - [X] 根据魔法注释 `% !TEX program = xelatex` 设置需要编译的类型
+- [x] 通过魔法注释设置编译结果存放位置
+- [X] 通过魔法注释实现编译命令的自定义
+- [ ] 增加配置文件功能，用于改变默认设置
+    - [ ] 指定生成的结果文件存放位置（目前默认存放在 `Build` 子文件夹下）
+    - [ ] 默认的编译命令（目前默认编译命令是 `xelatex`）
+- [ ] texlive 宏包检缺失并自动安装
+- [ ] 多主文件编译功能
```

### Comparing `pytexmk-0.5.1.240426/tests/test.py` & `pytexmk-0.5.4.240427/tests/test.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,209 +1,209 @@
-import os
-import shutil
-import datetime
-import argparse
-import subprocess
-from rich.console import Console
-from rich.table import Table
-
-def copy(source_folder, destination_folder):
-    # 确保目标文件夹存在，如果不存在则创建
-    if not os.path.exists(destination_folder):
-        os.makedirs(destination_folder)
-
-    # 遍历源文件夹中的所有文件
-    for filename in os.listdir(source_folder):
-        source_file = os.path.join(source_folder, filename)
-        destination_file = os.path.join(destination_folder, filename)
-
-        # 判断源文件是否是文件
-        if os.path.isfile(source_file):
-            # 复制文件到目标文件夹
-            shutil.copy(source_file, destination_file)
-
-# 修改函数为可运行函数
-def file_modify(destination_folder):
-    # 读取原始文件内容
-    for root, dirs, files in os.walk(destination_folder):
-        for file_name in files:
-            if file_name.endswith('.py'):
-                file_path = os.path.join(root, file_name)
-                with open(file_path, 'r', encoding='utf-8') as file:
-                    content = file.read()
-                content = content.replace('from .', 'from ') # 替换 from . 为 from
-                with open(file_path, 'w', encoding='utf-8') as file: 
-                    file.write(content) # 写入更新后的内容到同一文件
-
-# --------------------------------------------------------------------------------
-# 测试函数
-# --------------------------------------------------------------------------------
-def test(test_files, test_file_type, command, run_command, destination_folder):
-    # 存储所有要打印的内容
-    print_output = []
-    # 测试 biblatex, bibtex, 图目录表目录目录, 目录, glossaries, nomencl
-    for i in range(len(test_files)):
-        try:
-            time_start = datetime.datetime.now()
-            result = subprocess.run(run_command + [test_files[i]], cwd=destination_folder)
-            time_end = datetime.datetime.now()
-            time_run = round((time_end - time_start).total_seconds(), 4)
-            if result.returncode == 0:
-                print_output.append([test_file_type[i], time_run, "[green]通过"])  # 绿色
-            else:
-                print_output.append([test_file_type[i], time_run, "[red]未通过"])  # 红色
-        except Exception as e:
-            print_output.append([test_file_type[i], 0, "[red]未通过"])  # 红色
-    # 测试 pytexmk 参数
-    for i in range(len(command)):
-        try:
-            if command[i] == "-nq":
-                time_start = datetime.datetime.now()
-                result = subprocess.run(run_command + ['-nq', 'main'], cwd=destination_folder)
-                time_end = datetime.datetime.now()
-                time_run = round((time_end - time_start).total_seconds(), 4)
-                if result.returncode == 0:
-                    print_output.append([command[i], time_run, "[green]通过"])  # 绿色
-                else:
-                    print_output.append([command[i], time_run, "[red]未通过"])  
-            elif command[i] == "-c" and "-C":
-                time_start = datetime.datetime.now()
-                subprocess.run(['xelatex', "-shell-escape", "-file-line-error", "-halt-on-error", "-interaction=batchmode", 'main'], cwd=destination_folder)
-                result = subprocess.run(run_command + [command[i]], cwd=destination_folder)
-                time_end = datetime.datetime.now()
-                time_run = round((time_end - time_start).total_seconds(), 4)
-                if result.returncode == 0:
-                    print_output.append([command[i], time_run, "[green]通过"])  # 绿色
-                else:
-                    print_output.append([command[i], time_run, "[red]未通过"])  # 红色
-            else:
-                time_start = datetime.datetime.now()
-                result = subprocess.run(run_command + [command[i]], cwd=destination_folder)
-                time_end = datetime.datetime.now()
-                time_run = round((time_end - time_start).total_seconds(), 4)
-                if result.returncode == 0:
-                    print_output.append([command[i], time_run, "[green]通过"])  # 绿色
-                else:
-                    print_output.append([command[i], time_run, "[red]未通过"])  # 红色
-        except Exception as e:
-            print_output.append([i, 0, "[red]未通过"])  # 红色
-    return print_output
-
-# --------------------------------------------------------------------------------
-# 清除临时测试文件夹函数
-# --------------------------------------------------------------------------------
-def remove(path):
-    if os.path.exists(path):
-        shutil.rmtree(path)  # 删除整个文件夹
-        print("删除临时测试文件夹\n")
-
-# --------------------------------------------------------------------------------
-# 测试统计表打印函数
-# --------------------------------------------------------------------------------
-def print_table(data):
-    console = Console() # 创建Console对象
-
-    table = Table(show_header=True, header_style="bold magenta", 
-                title="PyTeXMK 测试统计表")
-
-    # 定义列名
-    table.add_column("序号", style="yellow", justify="center", no_wrap=True)
-    table.add_column("测试项目", style="cyan", justify="left", no_wrap=True)
-    table.add_column("测试时长", style="green", justify="left", no_wrap=True)
-    table.add_column("状态", justify="center", no_wrap=True)
-    table.add_column("序号", style="yellow", justify="center", no_wrap=True)
-    table.add_column("测试项目", style="cyan", justify="left")
-    table.add_column("测试时长", style="green", justify="left", no_wrap=True)
-    table.add_column("状态", justify="center", no_wrap=True)
-
-    # 判断统计项目列数是否是偶数
-    length = len(data)/2 # 计算打印表格列数
-    row_num = ""
-    # 判断统计项目列数是否是偶数
-    if length - int(length) < 0.5:
-        row_num = int(length)
-    else: # 是偶数则加一
-        row_num = int(length) + 1
-
-    # 添加数据到表格
-    for i in range(row_num):
-        table.add_row(
-            str(i+1),
-            data[i][0],
-            "{:.4f} s".format(data[i][1]),
-            data[i][2],
-            str(i+1+row_num) if i+row_num <= len(data) else "",
-            data[i+row_num][0] if i+row_num < len(data) else "",
-            "{:.4f} s".format(data[i+row_num][1]) if i+row_num < len(data) else "",
-            data[i+row_num][2] if i+row_num < len(data) else ""
-        )
-
-    console.print(table) # 打印表格
-
-# --------------------------------------------------------------------------------
-# 测试目标
-# --------------------------------------------------------------------------------
-parser = argparse.ArgumentParser(description="辅助测试文件.")
-parser.add_argument('-v', '--version', action='version', version='test: v 0.1')
-parser.add_argument('-w', '--whl', action='store_true', help="测试 whl 文件")
-args = parser.parse_args()
-
-
-test_files = [
-    "biblatex-test",
-    "bibtex-test",
-    "thebibliography-test",
-    "contents-figrue-table-test",
-    "contents-test",
-    "glossaries-test",
-    "nomencl-test",
-    "makeidx-test"
-]
-test_file_type = ['biblatex', 'bibtex', 'thebibliography', '图表目录', '目录', 'glossaries', 'nomencl', "makeidx"]
-command = ['-v', '-h', '-nq', '-c', '-C']
-
-source_folder = 'src/pytexmk' # 源文件夹路径
-tests_folder = 'tests' # 测试文件路径
-destination_folder = 'test-temp' # 目标文件夹路径
-run_file = "__main__.py"
-run_command = ["python", "__main__.py"]
-if args.whl:
-    run_command = ["pytexmk"]
-
-# --------------------------------------------------------------------------------
-# 运行测试流程
-# --------------------------------------------------------------------------------
-start_time = datetime.datetime.now() # 计算开始时间
-remove(destination_folder) # 删除临时测试文件夹
-copy(source_folder, destination_folder) # 复制测试对象到目标位置
-copy(tests_folder, destination_folder) # 复制测试文件到目标位置
-file_modify(destination_folder) # 修改测试对象使其可运行
-data = test(test_files, test_file_type, command, run_command, destination_folder)
-remove(destination_folder) # 删除临时测试文件夹
-print_table(data)
-# subprocess.run([run_command, test_file, '-C'], cwd=destination_folder)
-
-# --------------------------------------------------------------------------------
-# 打印统计s
-# --------------------------------------------------------------------------------
-end_time = datetime.datetime.now() # 计算结束时间
-run_time = end_time - start_time
-hours, remainder = divmod(run_time.seconds, 3600)
-minutes, seconds = divmod(remainder, 60)
-milliseconds = run_time.microseconds // 1000  # 获取毫秒部分
-print("\n" + "=" * 80)
-print(f"测试时长为：{hours} 小时 {minutes} 分 {seconds} 秒 {milliseconds} 毫秒 ({run_time.total_seconds():.3f} s total)\n")
-# def your_function():
-#     try:
-#         command = ['xelatex', "-shell-escape", "-file-line-error", "-halt-on-error", "-interaction=batchmode", 'main.tex']
-#         completed_process = subprocess.run(command, check=True, text=True, capture_output=True)
-#         print("Process completed successfully!")
-#     except subprocess.CalledProcessError as e:
-#         # print(f"Error running command: {e}")
-#         # print(f"Return code: {e.returncode}")
-#         print(f"Output: {e.output}")
-#         # print(f"Error running command: {e.stderr}")
-#         return
-
-#     print("Done!")
-
-# your_function()
+import os
+import shutil
+import datetime
+import argparse
+import subprocess
+from rich.console import Console
+from rich.table import Table
+
+def copy(source_folder, destination_folder):
+    # 确保目标文件夹存在，如果不存在则创建
+    if not os.path.exists(destination_folder):
+        os.makedirs(destination_folder)
+
+    # 遍历源文件夹中的所有文件
+    for filename in os.listdir(source_folder):
+        source_file = os.path.join(source_folder, filename)
+        destination_file = os.path.join(destination_folder, filename)
+
+        # 判断源文件是否是文件
+        if os.path.isfile(source_file):
+            # 复制文件到目标文件夹
+            shutil.copy(source_file, destination_file)
+
+# 修改函数为可运行函数
+def file_modify(destination_folder):
+    # 读取原始文件内容
+    for root, dirs, files in os.walk(destination_folder):
+        for file_name in files:
+            if file_name.endswith('.py'):
+                file_path = os.path.join(root, file_name)
+                with open(file_path, 'r', encoding='utf-8') as file:
+                    content = file.read()
+                content = content.replace('from .', 'from ') # 替换 from . 为 from
+                with open(file_path, 'w', encoding='utf-8') as file: 
+                    file.write(content) # 写入更新后的内容到同一文件
+
+# --------------------------------------------------------------------------------
+# 测试函数
+# --------------------------------------------------------------------------------
+def test(test_files, test_file_type, command, run_command, destination_folder):
+    # 存储所有要打印的内容
+    print_output = []
+    # 测试 biblatex, bibtex, 图目录表目录目录, 目录, glossaries, nomencl
+    for i in range(len(test_files)):
+        try:
+            time_start = datetime.datetime.now()
+            result = subprocess.run(run_command + [test_files[i]], cwd=destination_folder)
+            time_end = datetime.datetime.now()
+            time_run = round((time_end - time_start).total_seconds(), 4)
+            if result.returncode == 0:
+                print_output.append([test_file_type[i], time_run, "[green]通过"])  # 绿色
+            else:
+                print_output.append([test_file_type[i], time_run, "[red]未通过"])  # 红色
+        except Exception as e:
+            print_output.append([test_file_type[i], 0, "[red]未通过"])  # 红色
+    # 测试 pytexmk 参数
+    for i in range(len(command)):
+        try:
+            if command[i] == "-nq":
+                time_start = datetime.datetime.now()
+                result = subprocess.run(run_command + ['-nq', 'main'], cwd=destination_folder)
+                time_end = datetime.datetime.now()
+                time_run = round((time_end - time_start).total_seconds(), 4)
+                if result.returncode == 0:
+                    print_output.append([command[i], time_run, "[green]通过"])  # 绿色
+                else:
+                    print_output.append([command[i], time_run, "[red]未通过"])  
+            elif command[i] == "-c" and "-C":
+                time_start = datetime.datetime.now()
+                subprocess.run(['xelatex', "-shell-escape", "-file-line-error", "-halt-on-error", "-interaction=batchmode", 'main'], cwd=destination_folder)
+                result = subprocess.run(run_command + [command[i]], cwd=destination_folder)
+                time_end = datetime.datetime.now()
+                time_run = round((time_end - time_start).total_seconds(), 4)
+                if result.returncode == 0:
+                    print_output.append([command[i], time_run, "[green]通过"])  # 绿色
+                else:
+                    print_output.append([command[i], time_run, "[red]未通过"])  # 红色
+            else:
+                time_start = datetime.datetime.now()
+                result = subprocess.run(run_command + [command[i]], cwd=destination_folder)
+                time_end = datetime.datetime.now()
+                time_run = round((time_end - time_start).total_seconds(), 4)
+                if result.returncode == 0:
+                    print_output.append([command[i], time_run, "[green]通过"])  # 绿色
+                else:
+                    print_output.append([command[i], time_run, "[red]未通过"])  # 红色
+        except Exception as e:
+            print_output.append([i, 0, "[red]未通过"])  # 红色
+    return print_output
+
+# --------------------------------------------------------------------------------
+# 清除临时测试文件夹函数
+# --------------------------------------------------------------------------------
+def remove(path):
+    if os.path.exists(path):
+        shutil.rmtree(path)  # 删除整个文件夹
+        print("删除临时测试文件夹\n")
+
+# --------------------------------------------------------------------------------
+# 测试统计表打印函数
+# --------------------------------------------------------------------------------
+def print_table(data):
+    console = Console() # 创建Console对象
+
+    table = Table(show_header=True, header_style="bold magenta", 
+                title="PyTeXMK 测试统计表")
+
+    # 定义列名
+    table.add_column("序号", style="yellow", justify="center", no_wrap=True)
+    table.add_column("测试项目", style="cyan", justify="left", no_wrap=True)
+    table.add_column("测试时长", style="green", justify="left", no_wrap=True)
+    table.add_column("状态", justify="center", no_wrap=True)
+    table.add_column("序号", style="yellow", justify="center", no_wrap=True)
+    table.add_column("测试项目", style="cyan", justify="left")
+    table.add_column("测试时长", style="green", justify="left", no_wrap=True)
+    table.add_column("状态", justify="center", no_wrap=True)
+
+    # 判断统计项目列数是否是偶数
+    length = len(data)/2 # 计算打印表格列数
+    row_num = ""
+    # 判断统计项目列数是否是偶数
+    if length - int(length) < 0.5:
+        row_num = int(length)
+    else: # 是偶数则加一
+        row_num = int(length) + 1
+
+    # 添加数据到表格
+    for i in range(row_num):
+        table.add_row(
+            str(i+1),
+            data[i][0],
+            "{:.4f} s".format(data[i][1]),
+            data[i][2],
+            str(i+1+row_num) if i+row_num <= len(data) else "",
+            data[i+row_num][0] if i+row_num < len(data) else "",
+            "{:.4f} s".format(data[i+row_num][1]) if i+row_num < len(data) else "",
+            data[i+row_num][2] if i+row_num < len(data) else ""
+        )
+
+    console.print(table) # 打印表格
+
+# --------------------------------------------------------------------------------
+# 测试目标
+# --------------------------------------------------------------------------------
+parser = argparse.ArgumentParser(description="辅助测试文件.")
+parser.add_argument('-v', '--version', action='version', version='test: v 0.1')
+parser.add_argument('-w', '--whl', action='store_true', help="测试 whl 文件")
+args = parser.parse_args()
+
+
+test_files = [
+    "biblatex-test",
+    "bibtex-test",
+    "thebibliography-test",
+    "contents-figrue-table-test",
+    "contents-test",
+    "glossaries-test",
+    "nomencl-test",
+    "makeidx-test"
+]
+test_file_type = ['biblatex', 'bibtex', 'thebibliography', '图表目录', '目录', 'glossaries', 'nomencl', "makeidx"]
+command = ['-v', '-h', '-nq', '-c', '-C']
+
+source_folder = 'src/pytexmk' # 源文件夹路径
+tests_folder = 'tests' # 测试文件路径
+destination_folder = 'test-temp' # 目标文件夹路径
+run_file = "__main__.py"
+run_command = ["python", "__main__.py"]
+if args.whl:
+    run_command = ["pytexmk"]
+
+# --------------------------------------------------------------------------------
+# 运行测试流程
+# --------------------------------------------------------------------------------
+start_time = datetime.datetime.now() # 计算开始时间
+remove(destination_folder) # 删除临时测试文件夹
+copy(source_folder, destination_folder) # 复制测试对象到目标位置
+copy(tests_folder, destination_folder) # 复制测试文件到目标位置
+file_modify(destination_folder) # 修改测试对象使其可运行
+data = test(test_files, test_file_type, command, run_command, destination_folder)
+remove(destination_folder) # 删除临时测试文件夹
+print_table(data)
+# subprocess.run([run_command, test_file, '-C'], cwd=destination_folder)
+
+# --------------------------------------------------------------------------------
+# 打印统计s
+# --------------------------------------------------------------------------------
+end_time = datetime.datetime.now() # 计算结束时间
+run_time = end_time - start_time
+hours, remainder = divmod(run_time.seconds, 3600)
+minutes, seconds = divmod(remainder, 60)
+milliseconds = run_time.microseconds // 1000  # 获取毫秒部分
+print("\n" + "=" * 80)
+print(f"测试时长为：{hours} 小时 {minutes} 分 {seconds} 秒 {milliseconds} 毫秒 ({run_time.total_seconds():.3f} s total)\n")
+# def your_function():
+#     try:
+#         command = ['xelatex', "-shell-escape", "-file-line-error", "-halt-on-error", "-interaction=batchmode", 'main.tex']
+#         completed_process = subprocess.run(command, check=True, text=True, capture_output=True)
+#         print("Process completed successfully!")
+#     except subprocess.CalledProcessError as e:
+#         # print(f"Error running command: {e}")
+#         # print(f"Return code: {e.returncode}")
+#         print(f"Output: {e.output}")
+#         # print(f"Error running command: {e.stderr}")
+#         return
+
+#     print("Done!")
+
+# your_function()
```

