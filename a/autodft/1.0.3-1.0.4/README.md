# Comparing `tmp/autodft-1.0.3.tar.gz` & `tmp/autodft-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodft-1.0.3.tar", last modified: Mon Apr 29 06:36:58 2024, max compression
+gzip compressed data, was "autodft-1.0.4.tar", last modified: Mon May  6 19:25:07 2024, max compression
```

## Comparing `autodft-1.0.3.tar` & `autodft-1.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-29 06:36:58.294444 autodft-1.0.3/
--rw-r--r--   0 sting    (144291) shenvi   (10405)    35821 2024-04-29 06:35:15.000000 autodft-1.0.3/LICENSE.txt
--rw-r--r--   0 sting    (144291) shenvi   (10405)    11185 2024-04-29 06:36:58.293427 autodft-1.0.3/PKG-INFO
--rw-r--r--   0 sting    (144291) shenvi   (10405)    10989 2024-04-29 06:35:15.000000 autodft-1.0.3/README.md
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-29 06:36:58.271659 autodft-1.0.3/autodft/
--rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-04-29 06:35:16.000000 autodft-1.0.3/autodft/__init__.py
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-29 06:36:58.278017 autodft-1.0.3/autodft/config/
--rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-04-29 06:35:19.000000 autodft-1.0.3/autodft/config/__init__.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     1185 2024-04-29 06:35:19.000000 autodft-1.0.3/autodft/config/config.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     2882 2024-04-29 06:35:19.000000 autodft-1.0.3/autodft/config/default_parameters.yaml
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-29 06:36:58.281425 autodft-1.0.3/autodft/helpers/
--rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-04-29 06:35:19.000000 autodft-1.0.3/autodft/helpers/__init__.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     7402 2024-04-29 06:35:19.000000 autodft-1.0.3/autodft/helpers/crest_job.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)    11913 2024-04-29 06:35:19.000000 autodft-1.0.3/autodft/helpers/gaussian_inputfile.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     3660 2024-04-29 06:35:19.000000 autodft-1.0.3/autodft/helpers/gaussian_manager.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)    15771 2024-04-29 06:35:19.000000 autodft-1.0.3/autodft/helpers/user_input.py
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-29 06:36:58.286102 autodft-1.0.3/autodft/utils/
--rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-04-29 06:35:20.000000 autodft-1.0.3/autodft/utils/__init__.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     4269 2024-04-29 06:35:20.000000 autodft-1.0.3/autodft/utils/autodft_utils.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     2261 2024-04-29 06:35:20.000000 autodft-1.0.3/autodft/utils/files.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     5077 2024-04-29 06:35:20.000000 autodft-1.0.3/autodft/utils/gaussian_output.py
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-29 06:36:58.292279 autodft-1.0.3/autodft.egg-info/
--rw-r--r--   0 sting    (144291) shenvi   (10405)    11185 2024-04-29 06:36:57.000000 autodft-1.0.3/autodft.egg-info/PKG-INFO
--rw-r--r--   0 sting    (144291) shenvi   (10405)      747 2024-04-29 06:36:57.000000 autodft-1.0.3/autodft.egg-info/SOURCES.txt
--rw-r--r--   0 sting    (144291) shenvi   (10405)        1 2024-04-29 06:36:57.000000 autodft-1.0.3/autodft.egg-info/dependency_links.txt
--rw-r--r--   0 sting    (144291) shenvi   (10405)        1 2024-04-29 06:36:57.000000 autodft-1.0.3/autodft.egg-info/not-zip-safe
--rw-r--r--   0 sting    (144291) shenvi   (10405)       57 2024-04-29 06:36:57.000000 autodft-1.0.3/autodft.egg-info/requires.txt
--rw-r--r--   0 sting    (144291) shenvi   (10405)        8 2024-04-29 06:36:57.000000 autodft-1.0.3/autodft.egg-info/top_level.txt
-drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-04-29 06:36:58.291354 autodft-1.0.3/scripts/
--rw-r--r--   0 sting    (144291) shenvi   (10405)     2282 2024-04-29 06:35:17.000000 autodft-1.0.3/scripts/autodft_flow.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     2295 2024-04-29 06:35:17.000000 autodft-1.0.3/scripts/autodft_flow_xyz.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     9216 2024-04-29 06:35:17.000000 autodft-1.0.3/scripts/compile_results.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)     4975 2024-04-29 06:35:17.000000 autodft-1.0.3/scripts/gstatus.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)      500 2024-04-29 06:35:17.000000 autodft-1.0.3/scripts/run_autodft.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)      630 2024-04-29 06:35:17.000000 autodft-1.0.3/scripts/run_autodft_xyz.py
--rw-r--r--   0 sting    (144291) shenvi   (10405)       38 2024-04-29 06:36:58.294691 autodft-1.0.3/setup.cfg
--rw-r--r--   0 sting    (144291) shenvi   (10405)     1065 2024-04-29 06:35:15.000000 autodft-1.0.3/setup.py
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-05-06 19:25:07.758065 autodft-1.0.4/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)    35148 2024-05-06 19:24:17.000000 autodft-1.0.4/LICENSE.txt
+-rw-r--r--   0 sting    (144291) shenvi   (10405)    11075 2024-05-06 19:25:07.757294 autodft-1.0.4/PKG-INFO
+-rw-r--r--   0 sting    (144291) shenvi   (10405)    10626 2024-05-06 19:24:17.000000 autodft-1.0.4/README.md
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-05-06 19:25:07.744036 autodft-1.0.4/autodft/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/__init__.py
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-05-06 19:25:07.748676 autodft-1.0.4/autodft/config/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/config/__init__.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     1140 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/config/config.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     2844 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/config/default_parameters.yaml
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-05-06 19:25:07.751271 autodft-1.0.4/autodft/helpers/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/helpers/__init__.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     7179 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/helpers/crest_job.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)    11592 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/helpers/gaussian_inputfile.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     3554 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/helpers/gaussian_manager.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)    15382 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/helpers/user_input.py
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-05-06 19:25:07.753254 autodft-1.0.4/autodft/utils/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        0 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/utils/__init__.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     4153 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/utils/autodft_utils.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     2182 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/utils/files.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     4911 2024-05-06 19:24:17.000000 autodft-1.0.4/autodft/utils/gaussian_output.py
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-05-06 19:25:07.747322 autodft-1.0.4/autodft.egg-info/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)    11075 2024-05-06 19:25:07.744615 autodft-1.0.4/autodft.egg-info/PKG-INFO
+-rw-r--r--   0 sting    (144291) shenvi   (10405)      747 2024-05-06 19:25:07.745387 autodft-1.0.4/autodft.egg-info/SOURCES.txt
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        1 2024-05-06 19:25:07.746050 autodft-1.0.4/autodft.egg-info/dependency_links.txt
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        1 2024-05-06 19:25:07.746565 autodft-1.0.4/autodft.egg-info/not-zip-safe
+-rw-r--r--   0 sting    (144291) shenvi   (10405)       57 2024-05-06 19:25:07.747034 autodft-1.0.4/autodft.egg-info/requires.txt
+-rw-r--r--   0 sting    (144291) shenvi   (10405)        8 2024-05-06 19:25:07.747469 autodft-1.0.4/autodft.egg-info/top_level.txt
+drwxr-xr-x   0 sting    (144291) shenvi   (10405)        0 2024-05-06 19:25:07.756229 autodft-1.0.4/scripts/
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     2211 2024-05-06 19:24:17.000000 autodft-1.0.4/scripts/autodft_flow.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     2280 2024-05-06 19:24:17.000000 autodft-1.0.4/scripts/autodft_flow_xyz.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     8980 2024-05-06 19:24:17.000000 autodft-1.0.4/scripts/compile_results.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     4837 2024-05-06 19:24:17.000000 autodft-1.0.4/scripts/gstatus.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)      476 2024-05-06 19:24:17.000000 autodft-1.0.4/scripts/run_autodft.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)      604 2024-05-06 19:24:17.000000 autodft-1.0.4/scripts/run_autodft_xyz.py
+-rw-r--r--   0 sting    (144291) shenvi   (10405)       38 2024-05-06 19:25:07.758285 autodft-1.0.4/setup.cfg
+-rw-r--r--   0 sting    (144291) shenvi   (10405)     1030 2024-05-06 19:24:17.000000 autodft-1.0.4/setup.py
```

### Comparing `autodft-1.0.3/LICENSE.txt` & `autodft-1.0.4/LICENSE.txt`

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
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `autodft-1.0.3/PKG-INFO` & `autodft-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodft
-Version: 1.0.3
+Version: 1.0.4
 Summary: Automated conformer searching and DFT calculations
 Home-page: https://github.com/shenvilab/autodft
 Author: Shenvi Lab
 Author-email: sting@scripps.edu
 License: GPL-v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -36,15 +36,15 @@
 - ```ssh username@garibaldi.scripps.edu```
 
 Install the micromamba package manager if not already installed.
 (Note: The more common miniconda package manager can also be used, but is
 blocked by firewalls at Scripps Research)
 - ```curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba```
 - ```./bin/micromamba shell init -s bash -p ~/micromamba```
-- ```source ~/.bashrc```
+- Restart the terminal window and connect to the computing cluster again
 
 Create a micromamba environment and install packages (answer yes when prompted)
 - ```micromamba create -n autodft```
 - ```micromamba activate autodft```
 - ```micromamba install -c conda-forge pandas goodvibes rdkit=2023.09.5 cclib xtb crest pyyaml```
 - ```pip install autodft```
 
@@ -221,18 +221,16 @@
 Upload your ```config.yaml``` file to the computing cluster. When running
 AutoDFT in the future, you can respond ```n``` to the prompt about using the
 default settings for CREST, resources, etc. Then, type ```config.yaml``` 
 when prompted (make sure you are in the folder containing the ```config.yaml``` file).
 
 
 ```
-autodft_flow:                           # Settings for 'chaperone' job
-  mem: 128mb                            # Memory
-  processors: 1                         # Number of processors
-  time: '30:00:00'                      # Wall time (should be at least the sum of wall times for the CREST and Gaussian jobs)
+autodft_flow:
+  time: '30:00:00'                      # Wall time for AutoDFT (should be at least the sum of wall times for the CREST and Gaussian jobs)
 
 crest:
   method: gfn2                          # Method (for available options, see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
   solvent: ''                           # Solvent (do not include --gbsa flag) (for available solvents, see: https://xtb-docs.readthedocs.io/en/latest/gbsa.html#parameterized-solvents)
   mem: 2gb                              # Memory
   nprocshared: 12                       # Number of processors
   time: '6:00:00'                       # Wall time
@@ -262,9 +260,8 @@
   ecp_cutoff: null
   
 goodvibes:
   conc: '1'                             # Concentration (mol/L; 1 mol/L is solution phase standard state)
   f_cutoff: '100'                       # Frequency cutoff (cm-1) for quasiharmonic oscillator approximation
   qs: truhlar                           # Quasiharmonic oscillator approximation method
   keywords: ''                          # Additional keywords (see: https://goodvibespy.readthedocs.io/en/latest/source/README.html#using-goodvibes)
-
 ```
```

### Comparing `autodft-1.0.3/README.md` & `autodft-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,253 +1,250 @@
-# AutoDFT
-A program for automated conformer searching and DFT calculations, designed
-to be user-friendly for experimentalists with no computational background.
-
-Conformer searching is performed using CREST (Pract, P.; Bohle, F.; Grimme, S.
-Phys. Chem. Chem. Phys. 2020, 22, 7169). The lowest energy conformations within
-a user-specified window are then optimized with DFT using Gaussian.
-Scripts are provided to check the progress of Gaussian jobs and extract key
-thermodynamic data with Goodvibes (Luchini, G.; Alegre-Requena, J. V.;
-Funes-Ardoiz, I.; Paton, R. S. F1000 Research, 2020, 9, 291.).
-
-The program is designed for use on a Linux cluster with a SLURM scheduler,
-and has not been tested for use with Mac. The program is not compatible with
-Windows.
-
-## Installation (first time only)
-Open a terminal window: Macs can use the built-in Terminal program, and PCs
-can use the built-in Windows Terminal program. Connect to the computing cluster:
-- ```ssh username@garibaldi.scripps.edu```
-
-Install the micromamba package manager if not already installed.
-(Note: The more common miniconda package manager can also be used, but is
-blocked by firewalls at Scripps Research)
-- ```curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba```
-- ```./bin/micromamba shell init -s bash -p ~/micromamba```
-- ```source ~/.bashrc```
-
-Create a micromamba environment and install packages (answer yes when prompted)
-- ```micromamba create -n autodft```
-- ```micromamba activate autodft```
-- ```micromamba install -c conda-forge pandas goodvibes rdkit=2023.09.5 cclib xtb crest pyyaml```
-- ```pip install autodft```
-
-## Basic Usage
-
-Connect to computing cluster and activate the autodft environment if not
-done already:
-```
-micromamba activate autodft
-```
-
-Start running AutoDFT (then answer the on-screen prompts):
-```
-run_autodft.py
-```
-
-Check the detailed status of Gaussian jobs:
-```
-gstatus.py *
-```
-
-Compile key thermodynamic data for lowest energy conformers:
-```
-compile_results.py *
-```
-
-### Examples of what you'll see
-
-Sample usage of ```run_autodft.py```, showing on-screen prompts (user inputs highlighted in yellow):
-
-![sample_usage1a](images/sample_usage1a.png)
-
-Specifying custom level of theory with ```run_autodft.py```:
-
-![sample_usage1b](images/sample_usage1b.png)
-
-Sample output of ```gstatus.py```:
-
-![sample_usage2](images/sample_usage2.png)
-
-Sample output of ```compile_results.py``` (summary section only):
-
-![sample_usage3](images/sample_usage3.png)
-
-## Additional details
-
-### AutoDFT submission
-This is performed using the ```run_autodft.py``` script, which takes molecules as 
-SMILES strings. Alternatively, this can be performed using ```run_autodft_xyz.py```,
-which takes an .xyz files of molecules as input, which is preferred for
-transition metal complexes or organic structures for which automated generation
-of a 3D structure fails (e.g. bicyclo[1.1.1]pentanes)
-
-Connect to computing cluster and activate the autodft environment if not
-done already:
-```
-micromamba activate autodft
-```
-
-Use of ```run_autodft.py``` is simply done as shown below, followed by answering
-the provided prompts:
-```
-run_autodft.py
-```
-
-Use of ```run_autodft_xyz.py``` is analogously done with:
-```
-run_autodft_xyz.py
-```
-
-### Checking job status
-The script ```gstatus.py``` is provided to help check the status of Gaussian
-jobs submitted by AutoDFT or manually. Specify the name of all folders to check
-for .log files, separated by spaces. Wildcards can be used as part of the folder
-names. If no folders are specified, the script will look in the current
-directory. Note that an opt and freq job that both converge will be displayed
-as 2 completed optimizations, and 2 distinct sub-jobs.
-
-**Example:** See status of .log files in all folders (within the current one)
-```
-gstatus.py *
-```
-**Example:** See status of .log files in folders test1, test2, test3
-```
-gstatus.py test1 test2 test3
-```
-**Example:** See status of .log files in folders starting with test
-```
-gstatus.py test*
-```
-**Example:** See status of .log files in current directory
-```
-gstatus.py
-```
-
-### Compiling thermodynamic data
-The script ```compile_results.py``` is provided to compile the key results for
-all .log files in the specified directories. Specify the name of all folders to
-check for .log files, separated by spaces. Wildcards can be used as part of the
-folder names. If no folders are specified, the script will look in the current
-directory.
-
-Options:
-- ```-a``` Use all conformations. (Default: False (use lowest only))
-- ```-g``` Specify the name of the Goodvibes output file (Default: Goodvibes_output.csv)
-- ```-o``` Specify the name of the summary file (Default: Goodvibes_output_summary.csv)
-
-**Example:** Compile results from .log files in all folders (within the current one)
-```
-compile_results.py *
-```
-**Example:** Compile results from .log files in folders test1, test2, test3
-```
-compile_results.py test1 test2 test3
-```
-**Example:** Compile results from .log files in folders starting with test
-```
-compile_results.py test*
-```
-**Example:** Compile results from all .log files in current directory
-```
-compile_results.py
-```
-**Example:** Compile results from all conformers in directories starting with "test".
-Save Goodvibes results to custom_filename.csv and summarized results to custom_summary_filename.csv
-```
-compile_results.py test* -a -g custom_filename.csv -o custom_summary_filename.csv
-```
-
-### Getting SMILES strings
-Draw the molecule in ChemDraw and highlight it. In the top menu:
-**Edit > Copy as > SMILES**. Or use a keyboard shortcut
-(**PC: Ctrl + Alt + C, Mac: Option + Command + C**).
-
-Charged species and radicals are both acceptable. Radicals should contain no more
-than one unpaired electron.
-
-**Limitations:** Use of SMILES strings is poorly suited for metal complexes,
-carbenes/nitrenes, and hypervalent species (silicates, phosphoranes, sulfuranes,
-hypervalent iodine, etc.). For these, use of ```run_autodft_xyz.py``` is preferred.
-
-#### Points of caution
-
-It's safer to draw the molecule in a 2-dimensional representation to help
-ensure that stereochemistry is assigned properly. For fused rings, it's often
-safest to draw the stereochemistry of hydrogens/substituents at the ring
-junction, rather than to use endocyclic bonds.
-
-Be especially careful about specifying stereochemistry when you have highly
-bridged systems. If looking at a molecular model, make sure to view the
-bond that will be drawn as wedged/dashed from head-on as opposed to from the
-side:
-
-![stereo_example1](images/stereo_example1.png)
-
-Be careful about the directionality of wedges. Opposite directionality
-corresponds to opposite stereochemistry:
-
-![stereo_example2](images/stereo_example2.png)
-
-In certain cases, stereochemistry may be misintepreted as being at heteroatoms,
-which can ultimately lead to invalid structures. Pay attention to any ChemDraw warnings:
-
-![stereo_example3](images/stereo_example3.png)
-
-### Custom settings
-If you would like, you can specify custom AutoDFT settings to use (including
-DFT level of theory). This is recommended if you routinely preform calculations
-at a different level of theory. To do this, copy/paste the below text, which
-contains the default AutoDFT settings. Then, modify as desired, and save 
-as a new file named ```config.yaml```. The text following the '#' symbols are
-descriptive comments and do not affect the settings.
-
-Upload your ```config.yaml``` file to the computing cluster. When running
-AutoDFT in the future, you can respond ```n``` to the prompt about using the
-default settings for CREST, resources, etc. Then, type ```config.yaml``` 
-when prompted (make sure you are in the folder containing the ```config.yaml``` file).
-
-
-```
-autodft_flow:                           # Settings for 'chaperone' job
-  mem: 128mb                            # Memory
-  processors: 1                         # Number of processors
-  time: '30:00:00'                      # Wall time (should be at least the sum of wall times for the CREST and Gaussian jobs)
-
-crest:
-  method: gfn2                          # Method (for available options, see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
-  solvent: ''                           # Solvent (do not include --gbsa flag) (for available solvents, see: https://xtb-docs.readthedocs.io/en/latest/gbsa.html#parameterized-solvents)
-  mem: 2gb                              # Memory
-  nprocshared: 12                       # Number of processors
-  time: '6:00:00'                       # Wall time
-  rm_extra_files: true                  # Remove extra CREST files  
-  keywords: ''                          # Additional keywords (see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
-
-gaussian_input:
-  version: '16'                         # Version of Gaussian (09 or 16)
-  maxjobs: 10                           # Maximum number of jobs to submit
-  mem: 2gb                              # Memory per job
-  nprocshared: 12                       # Processors per job
-  time: '24:00:00'                      # Wall time per job
-  write_chk: false                      # Whether to write and keep .chk files. Always written if there are linked jobs, but this decides whether they are kept
-
-gaussian_jobs:                          # Dashes indicate beginning of data for a job (can add or remove jobs as desired)
-- functional: B3LYP                     # Functional (for options, see: https://gaussian.com/dft/)
-  basisset: GENECP                      # Basis set (for options, see: https://gaussian.com/basissets/) (write GENECP for split basis set) 
-  route: Opt Freq SCF=XQC               # Route line (for linked jobs, do not add geom=allcheck guess=read (added automatically))
-  ecp_basisset_light: 6-31G(d)          # For split basis sets, the basis set for light atoms (write null if not applicable)
-  ecp_basisset_heavy: SDD               # For split basis sets, the basis set for heavy atoms (write null if not applicable)
-  ecp_cutoff: 36                        # For split basis sets, the maximum atomic number for light atoms (write null if not applicable)
-- functional: M062X
-  basisset: def2TZVP
-  route: ''
-  ecp_basisset_light: null
-  ecp_basisset_heavy: null
-  ecp_cutoff: null
-  
-goodvibes:
-  conc: '1'                             # Concentration (mol/L; 1 mol/L is solution phase standard state)
-  f_cutoff: '100'                       # Frequency cutoff (cm-1) for quasiharmonic oscillator approximation
-  qs: truhlar                           # Quasiharmonic oscillator approximation method
-  keywords: ''                          # Additional keywords (see: https://goodvibespy.readthedocs.io/en/latest/source/README.html#using-goodvibes)
-
-```
+# AutoDFT
+A program for automated conformer searching and DFT calculations, designed
+to be user-friendly for experimentalists with no computational background.
+
+Conformer searching is performed using CREST (Pract, P.; Bohle, F.; Grimme, S.
+Phys. Chem. Chem. Phys. 2020, 22, 7169). The lowest energy conformations within
+a user-specified window are then optimized with DFT using Gaussian.
+Scripts are provided to check the progress of Gaussian jobs and extract key
+thermodynamic data with Goodvibes (Luchini, G.; Alegre-Requena, J. V.;
+Funes-Ardoiz, I.; Paton, R. S. F1000 Research, 2020, 9, 291.).
+
+The program is designed for use on a Linux cluster with a SLURM scheduler,
+and has not been tested for use with Mac. The program is not compatible with
+Windows.
+
+## Installation (first time only)
+Open a terminal window: Macs can use the built-in Terminal program, and PCs
+can use the built-in Windows Terminal program. Connect to the computing cluster:
+- ```ssh username@garibaldi.scripps.edu```
+
+Install the micromamba package manager if not already installed.
+(Note: The more common miniconda package manager can also be used, but is
+blocked by firewalls at Scripps Research)
+- ```curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba```
+- ```./bin/micromamba shell init -s bash -p ~/micromamba```
+- Restart the terminal window and connect to the computing cluster again
+
+Create a micromamba environment and install packages (answer yes when prompted)
+- ```micromamba create -n autodft```
+- ```micromamba activate autodft```
+- ```micromamba install -c conda-forge pandas goodvibes rdkit=2023.09.5 cclib xtb crest pyyaml```
+- ```pip install autodft```
+
+## Basic Usage
+
+Connect to computing cluster and activate the autodft environment if not
+done already:
+```
+micromamba activate autodft
+```
+
+Start running AutoDFT (then answer the on-screen prompts):
+```
+run_autodft.py
+```
+
+Check the detailed status of Gaussian jobs:
+```
+gstatus.py *
+```
+
+Compile key thermodynamic data for lowest energy conformers:
+```
+compile_results.py *
+```
+
+### Examples of what you'll see
+
+Sample usage of ```run_autodft.py```, showing on-screen prompts (user inputs highlighted in yellow):
+
+![sample_usage1a](images/sample_usage1a.png)
+
+Specifying custom level of theory with ```run_autodft.py```:
+
+![sample_usage1b](images/sample_usage1b.png)
+
+Sample output of ```gstatus.py```:
+
+![sample_usage2](images/sample_usage2.png)
+
+Sample output of ```compile_results.py``` (summary section only):
+
+![sample_usage3](images/sample_usage3.png)
+
+## Additional details
+
+### AutoDFT submission
+This is performed using the ```run_autodft.py``` script, which takes molecules as 
+SMILES strings. Alternatively, this can be performed using ```run_autodft_xyz.py```,
+which takes an .xyz files of molecules as input, which is preferred for
+transition metal complexes or organic structures for which automated generation
+of a 3D structure fails (e.g. bicyclo[1.1.1]pentanes)
+
+Connect to computing cluster and activate the autodft environment if not
+done already:
+```
+micromamba activate autodft
+```
+
+Use of ```run_autodft.py``` is simply done as shown below, followed by answering
+the provided prompts:
+```
+run_autodft.py
+```
+
+Use of ```run_autodft_xyz.py``` is analogously done with:
+```
+run_autodft_xyz.py
+```
+
+### Checking job status
+The script ```gstatus.py``` is provided to help check the status of Gaussian
+jobs submitted by AutoDFT or manually. Specify the name of all folders to check
+for .log files, separated by spaces. Wildcards can be used as part of the folder
+names. If no folders are specified, the script will look in the current
+directory. Note that an opt and freq job that both converge will be displayed
+as 2 completed optimizations, and 2 distinct sub-jobs.
+
+**Example:** See status of .log files in all folders (within the current one)
+```
+gstatus.py *
+```
+**Example:** See status of .log files in folders test1, test2, test3
+```
+gstatus.py test1 test2 test3
+```
+**Example:** See status of .log files in folders starting with test
+```
+gstatus.py test*
+```
+**Example:** See status of .log files in current directory
+```
+gstatus.py
+```
+
+### Compiling thermodynamic data
+The script ```compile_results.py``` is provided to compile the key results for
+all .log files in the specified directories. Specify the name of all folders to
+check for .log files, separated by spaces. Wildcards can be used as part of the
+folder names. If no folders are specified, the script will look in the current
+directory.
+
+Options:
+- ```-a``` Use all conformations. (Default: False (use lowest only))
+- ```-g``` Specify the name of the Goodvibes output file (Default: Goodvibes_output.csv)
+- ```-o``` Specify the name of the summary file (Default: Goodvibes_output_summary.csv)
+
+**Example:** Compile results from .log files in all folders (within the current one)
+```
+compile_results.py *
+```
+**Example:** Compile results from .log files in folders test1, test2, test3
+```
+compile_results.py test1 test2 test3
+```
+**Example:** Compile results from .log files in folders starting with test
+```
+compile_results.py test*
+```
+**Example:** Compile results from all .log files in current directory
+```
+compile_results.py
+```
+**Example:** Compile results from all conformers in directories starting with "test".
+Save Goodvibes results to custom_filename.csv and summarized results to custom_summary_filename.csv
+```
+compile_results.py test* -a -g custom_filename.csv -o custom_summary_filename.csv
+```
+
+### Getting SMILES strings
+Draw the molecule in ChemDraw and highlight it. In the top menu:
+**Edit > Copy as > SMILES**. Or use a keyboard shortcut
+(**PC: Ctrl + Alt + C, Mac: Option + Command + C**).
+
+Charged species and radicals are both acceptable. Radicals should contain no more
+than one unpaired electron.
+
+**Limitations:** Use of SMILES strings is poorly suited for metal complexes,
+carbenes/nitrenes, and hypervalent species (silicates, phosphoranes, sulfuranes,
+hypervalent iodine, etc.). For these, use of ```run_autodft_xyz.py``` is preferred.
+
+#### Points of caution
+
+It's safer to draw the molecule in a 2-dimensional representation to help
+ensure that stereochemistry is assigned properly. For fused rings, it's often
+safest to draw the stereochemistry of hydrogens/substituents at the ring
+junction, rather than to use endocyclic bonds.
+
+Be especially careful about specifying stereochemistry when you have highly
+bridged systems. If looking at a molecular model, make sure to view the
+bond that will be drawn as wedged/dashed from head-on as opposed to from the
+side:
+
+![stereo_example1](images/stereo_example1.png)
+
+Be careful about the directionality of wedges. Opposite directionality
+corresponds to opposite stereochemistry:
+
+![stereo_example2](images/stereo_example2.png)
+
+In certain cases, stereochemistry may be misintepreted as being at heteroatoms,
+which can ultimately lead to invalid structures. Pay attention to any ChemDraw warnings:
+
+![stereo_example3](images/stereo_example3.png)
+
+### Custom settings
+If you would like, you can specify custom AutoDFT settings to use (including
+DFT level of theory). This is recommended if you routinely preform calculations
+at a different level of theory. To do this, copy/paste the below text, which
+contains the default AutoDFT settings. Then, modify as desired, and save 
+as a new file named ```config.yaml```. The text following the '#' symbols are
+descriptive comments and do not affect the settings.
+
+Upload your ```config.yaml``` file to the computing cluster. When running
+AutoDFT in the future, you can respond ```n``` to the prompt about using the
+default settings for CREST, resources, etc. Then, type ```config.yaml``` 
+when prompted (make sure you are in the folder containing the ```config.yaml``` file).
+
+
+```
+autodft_flow:
+  time: '30:00:00'                      # Wall time for AutoDFT (should be at least the sum of wall times for the CREST and Gaussian jobs)
+
+crest:
+  method: gfn2                          # Method (for available options, see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
+  solvent: ''                           # Solvent (do not include --gbsa flag) (for available solvents, see: https://xtb-docs.readthedocs.io/en/latest/gbsa.html#parameterized-solvents)
+  mem: 2gb                              # Memory
+  nprocshared: 12                       # Number of processors
+  time: '6:00:00'                       # Wall time
+  rm_extra_files: true                  # Remove extra CREST files  
+  keywords: ''                          # Additional keywords (see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
+
+gaussian_input:
+  version: '16'                         # Version of Gaussian (09 or 16)
+  maxjobs: 10                           # Maximum number of jobs to submit
+  mem: 2gb                              # Memory per job
+  nprocshared: 12                       # Processors per job
+  time: '24:00:00'                      # Wall time per job
+  write_chk: false                      # Whether to write and keep .chk files. Always written if there are linked jobs, but this decides whether they are kept
+
+gaussian_jobs:                          # Dashes indicate beginning of data for a job (can add or remove jobs as desired)
+- functional: B3LYP                     # Functional (for options, see: https://gaussian.com/dft/)
+  basisset: GENECP                      # Basis set (for options, see: https://gaussian.com/basissets/) (write GENECP for split basis set) 
+  route: Opt Freq SCF=XQC               # Route line (for linked jobs, do not add geom=allcheck guess=read (added automatically))
+  ecp_basisset_light: 6-31G(d)          # For split basis sets, the basis set for light atoms (write null if not applicable)
+  ecp_basisset_heavy: SDD               # For split basis sets, the basis set for heavy atoms (write null if not applicable)
+  ecp_cutoff: 36                        # For split basis sets, the maximum atomic number for light atoms (write null if not applicable)
+- functional: M062X
+  basisset: def2TZVP
+  route: ''
+  ecp_basisset_light: null
+  ecp_basisset_heavy: null
+  ecp_cutoff: null
+  
+goodvibes:
+  conc: '1'                             # Concentration (mol/L; 1 mol/L is solution phase standard state)
+  f_cutoff: '100'                       # Frequency cutoff (cm-1) for quasiharmonic oscillator approximation
+  qs: truhlar                           # Quasiharmonic oscillator approximation method
+  keywords: ''                          # Additional keywords (see: https://goodvibespy.readthedocs.io/en/latest/source/README.html#using-goodvibes)
+```
```

### Comparing `autodft-1.0.3/autodft/config/config.py` & `autodft-1.0.4/autodft/config/config.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import os
-import yaml
-from dataclasses import dataclass
-
-
-# CONSTANTS
-DEFAULT_CONFIG_FILE = 'default_parameters.yaml'
-
-
-@dataclass
-class Config:
-    """A class that stores configuration information for autodft"""
-    
-    autodft_flow: dict
-    crest: dict
-    gaussian_input: dict
-    gaussian_jobs: dict    
-    goodvibes: dict
-
-
-    @classmethod
-    def default(cls):
-        """Constructor that creates a Config object from
-        the default .yaml configuration file"""
-        
-        script_dir = os.path.dirname(os.path.abspath(__file__))
-        config_file_path = os.path.join(script_dir, DEFAULT_CONFIG_FILE)
-        with open(config_file_path) as f:
-            config_dict = yaml.safe_load(f)
-            return cls(**config_dict)
-    
-    
-    @classmethod
-    def from_yaml(cls, yaml_file: str=None):
-        """Constructor that creates a Config object from
-        a custom .yaml configuration file"""
-        
-        if yaml_file is None:
-            return cls.default()
-            
-        with open(yaml_file) as f:
-            config_dict = yaml.safe_load(f)
-            return cls(**config_dict)
-        
-        
+import os
+import yaml
+from dataclasses import dataclass
+
+
+# CONSTANTS
+DEFAULT_CONFIG_FILE = 'default_parameters.yaml'
+
+
+@dataclass
+class Config:
+    """A class that stores configuration information for autodft"""
+    
+    autodft_flow: dict
+    crest: dict
+    gaussian_input: dict
+    gaussian_jobs: dict    
+    goodvibes: dict
+
+
+    @classmethod
+    def default(cls):
+        """Constructor that creates a Config object from
+        the default .yaml configuration file"""
+        
+        script_dir = os.path.dirname(os.path.abspath(__file__))
+        config_file_path = os.path.join(script_dir, DEFAULT_CONFIG_FILE)
+        with open(config_file_path) as f:
+            config_dict = yaml.safe_load(f)
+            return cls(**config_dict)
+    
+    
+    @classmethod
+    def from_yaml(cls, yaml_file: str=None):
+        """Constructor that creates a Config object from
+        a custom .yaml configuration file"""
+        
+        if yaml_file is None:
+            return cls.default()
+            
+        with open(yaml_file) as f:
+            config_dict = yaml.safe_load(f)
+            return cls(**config_dict)
+        
+
```

### Comparing `autodft-1.0.3/autodft/config/default_parameters.yaml` & `autodft-1.0.4/autodft/config/default_parameters.yaml`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-autodft_flow:
-  time: '30:00:00'                      # Wall time for AutoDFT (should be at least the sum of wall times for the CREST and Gaussian jobs)
-
-crest:
-  method: gfn2                          # Method (for available options, see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
-  solvent: ''                           # Solvent (do not include --gbsa flag) (for available solvents, see: https://xtb-docs.readthedocs.io/en/latest/gbsa.html#parameterized-solvents)
-  mem: 2gb                              # Memory
-  nprocshared: 12                       # Number of processors
-  time: '6:00:00'                       # Wall time
-  rm_extra_files: true                  # Remove extra CREST files  
-  keywords: ''                          # Additional keywords (see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
-
-gaussian_input:
-  version: '16'                         # Version of Gaussian (09 or 16)
-  maxjobs: 10                           # Maximum number of jobs to submit
-  mem: 2gb                              # Memory per job
-  nprocshared: 12                       # Processors per job
-  time: '24:00:00'                      # Wall time per job
-  write_chk: false                      # Whether to write and keep .chk files. Always written if there are linked jobs, but this decides whether they are kept
-
-gaussian_jobs:                          # Dashes indicate beginning of data for a job (can add or remove jobs as desired)
-- functional: B3LYP                     # Functional (for options, see: https://gaussian.com/dft/)
-  basisset: GENECP                      # Basis set (for options, see: https://gaussian.com/basissets/) (write GENECP for split basis set) 
-  route: Opt Freq SCF=XQC               # Route line (for linked jobs, do not add geom=allcheck guess=read (added automatically))
-  ecp_basisset_light: 6-31G(d)          # For split basis sets, the basis set for light atoms (write null if not applicable)
-  ecp_basisset_heavy: SDD               # For split basis sets, the basis set for heavy atoms (write null if not applicable)
-  ecp_cutoff: 36                        # For split basis sets, the maximum atomic number for light atoms (write null if not applicable)
-- functional: M062X
-  basisset: def2TZVP
-  route: ''
-  ecp_basisset_light: null
-  ecp_basisset_heavy: null
-  ecp_cutoff: null
-  
-goodvibes:
-  conc: '1'                             # Concentration (mol/L; 1 mol/L is solution phase standard state)
-  f_cutoff: '100'                       # Frequency cutoff (cm-1) for quasiharmonic oscillator approximation
-  qs: truhlar                           # Quasiharmonic oscillator approximation method
+autodft_flow:
+  time: '30:00:00'                      # Wall time for AutoDFT (should be at least the sum of wall times for the CREST and Gaussian jobs)
+
+crest:
+  method: gfn2                          # Method (for available options, see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
+  solvent: ''                           # Solvent (do not include --gbsa flag) (for available solvents, see: https://xtb-docs.readthedocs.io/en/latest/gbsa.html#parameterized-solvents)
+  mem: 2gb                              # Memory
+  nprocshared: 12                       # Number of processors
+  time: '6:00:00'                       # Wall time
+  rm_extra_files: true                  # Remove extra CREST files  
+  keywords: ''                          # Additional keywords (see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
+
+gaussian_input:
+  version: '16'                         # Version of Gaussian (09 or 16)
+  maxjobs: 10                           # Maximum number of jobs to submit
+  mem: 2gb                              # Memory per job
+  nprocshared: 12                       # Processors per job
+  time: '24:00:00'                      # Wall time per job
+  write_chk: false                      # Whether to write and keep .chk files. Always written if there are linked jobs, but this decides whether they are kept
+
+gaussian_jobs:                          # Dashes indicate beginning of data for a job (can add or remove jobs as desired)
+- functional: B3LYP                     # Functional (for options, see: https://gaussian.com/dft/)
+  basisset: GENECP                      # Basis set (for options, see: https://gaussian.com/basissets/) (write GENECP for split basis set) 
+  route: Opt Freq SCF=XQC               # Route line (for linked jobs, do not add geom=allcheck guess=read (added automatically))
+  ecp_basisset_light: 6-31G(d)          # For split basis sets, the basis set for light atoms (write null if not applicable)
+  ecp_basisset_heavy: SDD               # For split basis sets, the basis set for heavy atoms (write null if not applicable)
+  ecp_cutoff: 36                        # For split basis sets, the maximum atomic number for light atoms (write null if not applicable)
+- functional: M062X
+  basisset: def2TZVP
+  route: ''
+  ecp_basisset_light: null
+  ecp_basisset_heavy: null
+  ecp_cutoff: null
+  
+goodvibes:
+  conc: '1'                             # Concentration (mol/L; 1 mol/L is solution phase standard state)
+  f_cutoff: '100'                       # Frequency cutoff (cm-1) for quasiharmonic oscillator approximation
+  qs: truhlar                           # Quasiharmonic oscillator approximation method
   keywords: ''                          # Additional keywords (see: https://goodvibespy.readthedocs.io/en/latest/source/README.html#using-goodvibes)
```

### Comparing `autodft-1.0.3/autodft/helpers/crest_job.py` & `autodft-1.0.4/autodft/helpers/crest_job.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,223 +1,223 @@
-import logging
-import os
-import subprocess
-
-from dataclasses import dataclass
-from textwrap import dedent
-
-from rdkit import Chem
-from rdkit.Chem import AllChem
-
-from autodft.utils.autodft_utils import charge_from_smiles, multiplicity_from_smiles
-
-
-logger = logging.getLogger(__name__)
-
-
-# CONSTANTS
-CREST_SCRIPT = 'run_crest.sh'
-
-
-@dataclass(kw_only=True)
-class CrestJob:
-    """A class that can create, submit, and process a CREST job from
-    a .xyz file.
-
-    Creating an instance of this class leads to 4 processes:
-        1. Creation of a shell script (.sh) to submit the job to a SLURM cluster
-        2. Submission of the job to the computing cluster
-        3. Organization of the resulting files
-        4. Extraction of cartesian coordinates (as text blocks) of the
-            generated conformers, which are stored in the cartesians attribute
-            as a list of strings
-
-    Example usage:
-        from crest import CrestJob
-        crestjob = CrestJob(molname='test', xyzfile='test.xyz', e_cutoff=2)
-        for conf_cartesians in crestjob.cartesians:
-            print(conf_cartesians)
-    """
-
-    molname: str
-    xyzfile: str
-    charge: int
-    multiplicity: int
-    e_cutoff: float
-    
-    method: str = '--gfn2'
-    solvent: str = ''
-    nprocshared: int = 16
-    mem: str = '12gb'
-    time: str = '6:00:00'
-    keywords: str = None
-    
-    rm_extra_files: bool = True
-    rm_xyzfile: bool = False
-    
-
-    # Defined in __post_init__
-    conf_cartesians: list[str] = None
-
-    def __post_init__(self) -> None:
-        """Perform CREST calculation"""
-
-        self.write_sh_script()
-        self.run()
-        self.cleanup()
-        self.conf_cartesians = self.get_conf_cartesians()
-
-    def write_sh_script(self) -> None:
-        """Writes a shell script to submit a CREST job for the provided
-        input file"""
-
-        crest_command = (f'crest {self.xyzfile} --{self.method}'
-                         f' --chrg {self.charge} --uhf {self.multiplicity-1}'
-                         f' --ewin {self.e_cutoff} -T {self.nprocshared}')
-        if self.solvent:
-            crest_command += f' -g {self.solvent}'
-        if self.keywords is not None:
-            crest_command += f' {self.keywords}'
-
-        with open(CREST_SCRIPT, 'w') as f:
-            f.write(dedent(f"""\
-                           #!/bin/sh
-                           
-                           #SBATCH --nodes=1
-                           #SBATCH --ntasks=1
-                           #SBATCH --cpus-per-task={self.nprocshared}
-                           #SBATCH --mem={self.mem}
-                           #SBATCH --time={self.time}
-                           #SBATCH --output={self.molname}_crest.out
-                           #SBATCH --job-name={self.molname[-8:]}
-                           
-                           {crest_command}
-                           """))
-
-    def run(self) -> None:
-        """Submit a CREST job to the computing cluster"""
-
-        logger.info('Submitting CREST job to SLURM...')
-        subprocess.run(['sbatch', '-W', CREST_SCRIPT])
-        
-
-    def cleanup(self) -> None:
-        """Organizes files after completion of the CREST job"""
-
-        # Check for normal termination of CREST job
-        with open(f'{self.molname}_crest.out') as f:
-            last_line = f.readlines()[-1]
-            if 'CREST terminated normally.' not in last_line:
-                raise CRESTAbnormalTerminationError()
-        logger.info('CREST terminated normally.')
-
-        # Remove unnecessary files
-        if self.rm_extra_files:
-            to_keep = [f'{self.molname}.out',
-                       f'{self.molname}_crest.out',
-                       'crest_conformers.xyz',
-                       f'autodft_{self.molname}.json',
-                       'autodft_parameters.yaml']
-            if not self.rm_xyzfile:
-                to_keep.append(self.xyzfile)
-            to_remove = [f for f in os.listdir() if f not in to_keep]
-            for f in to_remove:
-                try:
-                    os.remove(f)
-                except OSError:
-                    print(f'Unable to delete: {f}')
-
-        # Rename output file
-        os.rename('crest_conformers.xyz',
-                  f'{self.molname}_crest_conformers.xyz')
-
-    def get_conf_cartesians(self) -> None:
-        """Returns cartesian coordinates for each conformer generated by CREST.
-        The conformers are ordered starting with the lowest energy."""
-
-        xyz_blocks = []
-
-        with open(self.molname + '_crest_conformers.xyz') as f:
-            n_atoms = int(f.readline().strip())
-            xyz_block_length = n_atoms + 2
-
-            f.seek(0)
-            data = f.read().splitlines(keepends=True)
-            xyz_blocks = [data[i:i+xyz_block_length]
-                          for i in range(0, len(data), xyz_block_length)]
-
-        conf_cartesians = [''.join(xyz_lines[2:]) for xyz_lines in xyz_blocks]
-        return conf_cartesians
-
-
-@dataclass(kw_only=True)
-class CrestJobFromSmiles:
-
-    molname: str
-    smiles: str
-    e_cutoff: float
-    
-    method: str = '--gfn2'
-    solvent: str = ''
-    nprocshared: int = 16
-    mem: str = '12gb'
-    time: str = '6:00:00'
-    keywords: str = None
-    
-    rm_extra_files: bool = True
-
-    # Defined in __post_init__
-    charge: int = None
-    multiplicity: int = None
-    conf_cartesians: list[str] = None
-
-    def __post_init__(self) -> None:
-        """Perform CREST calculation"""
-
-        self.smiles = Chem.CanonSmiles(self.smiles)
-        self.charge = charge_from_smiles(self.smiles)
-        self.multiplicity = multiplicity_from_smiles(self.smiles)
-
-        # Run CREST
-        self.make_xyzfile()
-        xyzfile = f'{self.molname}.xyz'
-        args = {i: j for i, j in vars(self).items()
-                if i not in ['smiles', 'conf_cartesians']}
-        crest_job = CrestJob(xyzfile=xyzfile, rm_xyzfile=True, **args)
-
-        # Get and store cartesian coordinates
-        self.conf_cartesians = crest_job.conf_cartesians
-
-    def make_xyzfile(self) -> None:
-        """Generates an .xyz file (CREST input) from a SMILES string"""
-
-        xyz_name = f'{self.molname}.xyz'
-
-        # Embed the molecule to generate an initial 3D structure
-        logger.info(f'Generating .xyz file (input for CREST): {xyz_name}')
-        mol = Chem.MolFromSmiles(self.smiles)
-        mol = Chem.AddHs(mol)
-        AllChem.EmbedMolecule(mol, randomSeed=0xf00d,
-                              useExpTorsionAnglePrefs=True,
-                              useBasicKnowledge=True)
-        if mol.GetNumConformers() == 0:
-            raise Struct3DFromSMILESError()
-
-        # Minimization with UFF force field
-        while True:
-            converged = not AllChem.UFFOptimizeMolecule(mol, maxIters=200)
-            if converged:
-                break
-
-        # Write to file
-        Chem.MolToXYZFile(mol, xyz_name)
-
-
-class Struct3DFromSMILESError(Exception):
-    """Raised when 3D generation from a SMILES string failed.
-    Check stereochemical specification for highly bridged systems."""
-    pass
-
-
-class CRESTAbnormalTerminationError(Exception):
-    """Raised when a CREST job does not terminate normally"""
-    pass
+import logging
+import os
+import subprocess
+
+from dataclasses import dataclass
+from textwrap import dedent
+
+from rdkit import Chem
+from rdkit.Chem import AllChem
+
+from autodft.utils.autodft_utils import charge_from_smiles, multiplicity_from_smiles
+
+
+logger = logging.getLogger(__name__)
+
+
+# CONSTANTS
+CREST_SCRIPT = 'run_crest.sh'
+
+
+@dataclass(kw_only=True)
+class CrestJob:
+    """A class that can create, submit, and process a CREST job from
+    a .xyz file.
+
+    Creating an instance of this class leads to 4 processes:
+        1. Creation of a shell script (.sh) to submit the job to a SLURM cluster
+        2. Submission of the job to the computing cluster
+        3. Organization of the resulting files
+        4. Extraction of cartesian coordinates (as text blocks) of the
+            generated conformers, which are stored in the cartesians attribute
+            as a list of strings
+
+    Example usage:
+        from crest import CrestJob
+        crestjob = CrestJob(molname='test', xyzfile='test.xyz', e_cutoff=2)
+        for conf_cartesians in crestjob.cartesians:
+            print(conf_cartesians)
+    """
+
+    molname: str
+    xyzfile: str
+    charge: int
+    multiplicity: int
+    e_cutoff: float
+    
+    method: str = '--gfn2'
+    solvent: str = ''
+    nprocshared: int = 16
+    mem: str = '12gb'
+    time: str = '6:00:00'
+    keywords: str = None
+    
+    rm_extra_files: bool = True
+    rm_xyzfile: bool = False
+    
+
+    # Defined in __post_init__
+    conf_cartesians: list[str] = None
+
+    def __post_init__(self) -> None:
+        """Perform CREST calculation"""
+
+        self.write_sh_script()
+        self.run()
+        self.cleanup()
+        self.conf_cartesians = self.get_conf_cartesians()
+
+    def write_sh_script(self) -> None:
+        """Writes a shell script to submit a CREST job for the provided
+        input file"""
+
+        crest_command = (f'crest {self.xyzfile} --{self.method}'
+                         f' --chrg {self.charge} --uhf {self.multiplicity-1}'
+                         f' --ewin {self.e_cutoff} -T {self.nprocshared}')
+        if self.solvent:
+            crest_command += f' -g {self.solvent}'
+        if self.keywords is not None:
+            crest_command += f' {self.keywords}'
+
+        with open(CREST_SCRIPT, 'w') as f:
+            f.write(dedent(f"""\
+                           #!/bin/sh
+                           
+                           #SBATCH --nodes=1
+                           #SBATCH --ntasks=1
+                           #SBATCH --cpus-per-task={self.nprocshared}
+                           #SBATCH --mem={self.mem}
+                           #SBATCH --time={self.time}
+                           #SBATCH --output={self.molname}_crest.out
+                           #SBATCH --job-name={self.molname[-8:]}
+                           
+                           {crest_command}
+                           """))
+
+    def run(self) -> None:
+        """Submit a CREST job to the computing cluster"""
+
+        logger.info('Submitting CREST job to SLURM...')
+        subprocess.run(['sbatch', '-W', CREST_SCRIPT])
+        
+
+    def cleanup(self) -> None:
+        """Organizes files after completion of the CREST job"""
+
+        # Check for normal termination of CREST job
+        with open(f'{self.molname}_crest.out') as f:
+            last_line = f.readlines()[-1]
+            if 'CREST terminated normally.' not in last_line:
+                raise CRESTAbnormalTerminationError()
+        logger.info('CREST terminated normally.')
+
+        # Remove unnecessary files
+        if self.rm_extra_files:
+            to_keep = [f'{self.molname}.out',
+                       f'{self.molname}_crest.out',
+                       'crest_conformers.xyz',
+                       f'autodft_{self.molname}.json',
+                       'autodft_parameters.yaml']
+            if not self.rm_xyzfile:
+                to_keep.append(self.xyzfile)
+            to_remove = [f for f in os.listdir() if f not in to_keep]
+            for f in to_remove:
+                try:
+                    os.remove(f)
+                except OSError:
+                    print(f'Unable to delete: {f}')
+
+        # Rename output file
+        os.rename('crest_conformers.xyz',
+                  f'{self.molname}_crest_conformers.xyz')
+
+    def get_conf_cartesians(self) -> None:
+        """Returns cartesian coordinates for each conformer generated by CREST.
+        The conformers are ordered starting with the lowest energy."""
+
+        xyz_blocks = []
+
+        with open(self.molname + '_crest_conformers.xyz') as f:
+            n_atoms = int(f.readline().strip())
+            xyz_block_length = n_atoms + 2
+
+            f.seek(0)
+            data = f.read().splitlines(keepends=True)
+            xyz_blocks = [data[i:i+xyz_block_length]
+                          for i in range(0, len(data), xyz_block_length)]
+
+        conf_cartesians = [''.join(xyz_lines[2:]) for xyz_lines in xyz_blocks]
+        return conf_cartesians
+
+
+@dataclass(kw_only=True)
+class CrestJobFromSmiles:
+
+    molname: str
+    smiles: str
+    e_cutoff: float
+    
+    method: str = '--gfn2'
+    solvent: str = ''
+    nprocshared: int = 16
+    mem: str = '12gb'
+    time: str = '6:00:00'
+    keywords: str = None
+    
+    rm_extra_files: bool = True
+
+    # Defined in __post_init__
+    charge: int = None
+    multiplicity: int = None
+    conf_cartesians: list[str] = None
+
+    def __post_init__(self) -> None:
+        """Perform CREST calculation"""
+
+        self.smiles = Chem.CanonSmiles(self.smiles)
+        self.charge = charge_from_smiles(self.smiles)
+        self.multiplicity = multiplicity_from_smiles(self.smiles)
+
+        # Run CREST
+        self.make_xyzfile()
+        xyzfile = f'{self.molname}.xyz'
+        args = {i: j for i, j in vars(self).items()
+                if i not in ['smiles', 'conf_cartesians']}
+        crest_job = CrestJob(xyzfile=xyzfile, rm_xyzfile=True, **args)
+
+        # Get and store cartesian coordinates
+        self.conf_cartesians = crest_job.conf_cartesians
+
+    def make_xyzfile(self) -> None:
+        """Generates an .xyz file (CREST input) from a SMILES string"""
+
+        xyz_name = f'{self.molname}.xyz'
+
+        # Embed the molecule to generate an initial 3D structure
+        logger.info(f'Generating .xyz file (input for CREST): {xyz_name}')
+        mol = Chem.MolFromSmiles(self.smiles)
+        mol = Chem.AddHs(mol)
+        AllChem.EmbedMolecule(mol, randomSeed=0xf00d,
+                              useExpTorsionAnglePrefs=True,
+                              useBasicKnowledge=True)
+        if mol.GetNumConformers() == 0:
+            raise Struct3DFromSMILESError()
+
+        # Minimization with UFF force field
+        while True:
+            converged = not AllChem.UFFOptimizeMolecule(mol, maxIters=200)
+            if converged:
+                break
+
+        # Write to file
+        Chem.MolToXYZFile(mol, xyz_name)
+
+
+class Struct3DFromSMILESError(Exception):
+    """Raised when 3D generation from a SMILES string failed.
+    Check stereochemical specification for highly bridged systems."""
+    pass
+
+
+class CRESTAbnormalTerminationError(Exception):
+    """Raised when a CREST job does not terminate normally"""
+    pass
```

### Comparing `autodft-1.0.3/autodft/helpers/gaussian_manager.py` & `autodft-1.0.4/autodft/helpers/gaussian_manager.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import logging
-import os
-import subprocess
-from dataclasses import dataclass
-from textwrap import dedent
-
-from autodft.utils.gaussian_output import move_redundant
-from autodft.helpers.crest_job import CrestJob
-from autodft.helpers.gaussian_inputfile import MolInfo, GaussianInputWriter
-
-
-logger = logging.getLogger(__name__)
-
-
-# CONSTANTS
-GAUSSIAN_SCRIPT = 'run_gaussian.sh'
-
-
-@dataclass(kw_only=True)
-class GaussianManager:
-    """A class that manages the submission of Gaussian jobs"""
-
-    molname: str
-    charge: int
-    multiplicity: int
-    gwriter: GaussianInputWriter
-
-    version: str = '16'
-    maxjobs: int = 10
-    nprocshared: int = 12
-    mem: str = '12gb'
-    time: str = '24:00:00'
-    write_chk: bool = False
-
-    submitted_comfiles: list[str] = None
-
-    def submit_from_crest_confs(self, crest_job: CrestJob) -> None:
-        """Submits Gaussian jobs for conformers generated by CREST.
-        Up to maxjobs conformers are submitted. The class also stores
-        a list of the .com files submitted."""
-
-        # Write a .com file for each conformer
-        conf_cartesians = crest_job.conf_cartesians
-        total = len(conf_cartesians)
-        comfiles = [f'{self.molname}-conf{i+1}.com' for i in range(total)]
-        conf_infos = [MolInfo(charge=self.charge,
-                              multiplicity=self.multiplicity,
-                              cartesians=x)
-                      for x in conf_cartesians]
-        for info, name in zip(conf_infos, comfiles):
-            self.gwriter.write(info, name)
-
-        # Determine number of jobs to submit
-        n_to_submit = min([total, self.maxjobs])
-        logger.info(f'Number of conformers generated by CREST: {total}')
-        logger.info('Submitting Gaussian calculations to SLURM...'
-               f'({n_to_submit} out of maximum {self.maxjobs} jobs)')
-
-        # Write shell script for job
-        self.write_script(n_to_submit=n_to_submit)
-        self.submitted_comfiles = comfiles[:n_to_submit]
-
-        # Submit job
-        subprocess.run(['sbatch', '-W', GAUSSIAN_SCRIPT])
-
-        # Handle extraneous files
-        logger.info('The submitted Gaussian jobs have completed.')
-        logfiles = [x.replace('.com', '.log') for x in self.submitted_comfiles]
-        move_redundant(logfiles)
-        self.delete_chk_files()
-
-    def write_script(self, n_to_submit: str) -> None:
-        """Writes a shell script to submit an array job to SLURM"""
-
-        with open(GAUSSIAN_SCRIPT, 'w') as f:
-            f.write(dedent(f"""\
-                #!/bin/sh
-                
-                #SBATCH --nodes=1
-                #SBATCH --ntasks=1
-                #SBATCH --cpus-per-task={self.nprocshared}
-                #SBATCH --mem={self.mem}
-                #SBATCH --time={self.time}
-                #SBATCH --output=/dev/null
-                #SBATCH --error=/dev/null
-                #SBATCH --job-name={self.molname[-8:]}
-                #SBATCH --array=1-{n_to_submit}
-                
-                cd $SLURM_SUBMIT_DIR
-                module load gaussian/{self.version}
-                g{self.version} {self.molname}-conf${{SLURM_ARRAY_TASK_ID}}.com
-                """))
-
-    def delete_chk_files(self) -> None:
-        """Deletes .chk files if requested"""
-
-        if self.write_chk:
-            return
-
-        chk_files = [x.replace('.com', '.chk')
-                     for x in self.submitted_comfiles]
-        for f in chk_files:
-            try:
-                os.remove(f)
-            except OSError:
-                print(f'Unable to delete: {f}')
+import logging
+import os
+import subprocess
+from dataclasses import dataclass
+from textwrap import dedent
+
+from autodft.utils.gaussian_output import move_redundant
+from autodft.helpers.crest_job import CrestJob
+from autodft.helpers.gaussian_inputfile import MolInfo, GaussianInputWriter
+
+
+logger = logging.getLogger(__name__)
+
+
+# CONSTANTS
+GAUSSIAN_SCRIPT = 'run_gaussian.sh'
+
+
+@dataclass(kw_only=True)
+class GaussianManager:
+    """A class that manages the submission of Gaussian jobs"""
+
+    molname: str
+    charge: int
+    multiplicity: int
+    gwriter: GaussianInputWriter
+
+    version: str = '16'
+    maxjobs: int = 10
+    nprocshared: int = 12
+    mem: str = '12gb'
+    time: str = '24:00:00'
+    write_chk: bool = False
+
+    submitted_comfiles: list[str] = None
+
+    def submit_from_crest_confs(self, crest_job: CrestJob) -> None:
+        """Submits Gaussian jobs for conformers generated by CREST.
+        Up to maxjobs conformers are submitted. The class also stores
+        a list of the .com files submitted."""
+
+        # Write a .com file for each conformer
+        conf_cartesians = crest_job.conf_cartesians
+        total = len(conf_cartesians)
+        comfiles = [f'{self.molname}-conf{i+1}.com' for i in range(total)]
+        conf_infos = [MolInfo(charge=self.charge,
+                              multiplicity=self.multiplicity,
+                              cartesians=x)
+                      for x in conf_cartesians]
+        for info, name in zip(conf_infos, comfiles):
+            self.gwriter.write(info, name)
+
+        # Determine number of jobs to submit
+        n_to_submit = min([total, self.maxjobs])
+        logger.info(f'Number of conformers generated by CREST: {total}')
+        logger.info('Submitting Gaussian calculations to SLURM...'
+               f'({n_to_submit} out of maximum {self.maxjobs} jobs)')
+
+        # Write shell script for job
+        self.write_script(n_to_submit=n_to_submit)
+        self.submitted_comfiles = comfiles[:n_to_submit]
+
+        # Submit job
+        subprocess.run(['sbatch', '-W', GAUSSIAN_SCRIPT])
+
+        # Handle extraneous files
+        logger.info('The submitted Gaussian jobs have completed.')
+        logfiles = [x.replace('.com', '.log') for x in self.submitted_comfiles]
+        move_redundant(logfiles)
+        self.delete_chk_files()
+
+    def write_script(self, n_to_submit: str) -> None:
+        """Writes a shell script to submit an array job to SLURM"""
+
+        with open(GAUSSIAN_SCRIPT, 'w') as f:
+            f.write(dedent(f"""\
+                #!/bin/sh
+                
+                #SBATCH --nodes=1
+                #SBATCH --ntasks=1
+                #SBATCH --cpus-per-task={self.nprocshared}
+                #SBATCH --mem={self.mem}
+                #SBATCH --time={self.time}
+                #SBATCH --output=/dev/null
+                #SBATCH --error=/dev/null
+                #SBATCH --job-name={self.molname[-8:]}
+                #SBATCH --array=1-{n_to_submit}
+                
+                cd $SLURM_SUBMIT_DIR
+                module load gaussian/{self.version}
+                g{self.version} {self.molname}-conf${{SLURM_ARRAY_TASK_ID}}.com
+                """))
+
+    def delete_chk_files(self) -> None:
+        """Deletes .chk files if requested"""
+
+        if self.write_chk:
+            return
+
+        chk_files = [x.replace('.com', '.chk')
+                     for x in self.submitted_comfiles]
+        for f in chk_files:
+            try:
+                os.remove(f)
+            except OSError:
+                print(f'Unable to delete: {f}')
```

### Comparing `autodft-1.0.3/autodft/helpers/user_input.py` & `autodft-1.0.4/autodft/helpers/user_input.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,480 +1,482 @@
-import json
-import os
-import sys
-from textwrap import dedent
-from typing import Tuple
-
-from rdkit import Chem
-
-from autodft.config.config import Config
-from autodft.utils.autodft_utils import charge_from_smiles, multiplicity_from_smiles
-
-
-# CONSTANTS
-COL_WIDTH1 = 55
-COL_WIDTH2 = 15
-DASHES = '-' * (COL_WIDTH1 + COL_WIDTH2)
-N_PROCESSORS = 1
-MEMORY = '128mb'
-
-
-class UserInputSMILES:
-    """A class to read and store user inputs from the command line for
-    an AutoDFT job using a SMILES string as input"""
-
-    def __init__(self) -> None:
-
-        # Info for all jobs
-        print_settings_header()
-        self.config = config_from_user()
-        self.gaussian_jobs = gaussian_jobs(self.config)
-        self.e_cutoff = e_cutoff_from_user()
-
-        # Info for individual jobs
-        self.print_mol_info_header()
-        self.mols = mols_from_user()
-
-        user_verification()
-        self.export_json()
-        self.write_sh_script()
-
-    def print_mol_info_header(self) -> None:
-        """Prints how to provide information about the molecule(s)."""
-
-        print(dedent(f"""\
-            {DASHES}
-              Molecule information. Please provide the following:
-            
-                  Molecule name: The name that will become the base of all
-                                 file names associated with this molecule.
-                                 Example: mol1
-                  SMILES string: Radical-bearing atoms require explicit
-                                 hydrogens. Maximum 1 radical per molecule.
-                               
-              Enter a blank molecule name to stop adding structures.
-            {DASHES}"""))
-
-    def export_json(self) -> None:
-        """Writes the user inputs to .json configuration files"""
-
-        data = vars(self).copy()
-        if data['config'] is not None:
-            data['config'] = '../' + data['config']
-        mols = data.pop('mols')
-        for mol in mols:
-            to_export = {}
-            to_export.update(data)
-            to_export.update(mol)
-            write_json(to_export)
-
-    def write_sh_script(self) -> None:
-        """Writes shell scripts to run AutoDFT"""
-
-        molnames = [m['molname'] for m in self.mols]
-        for name in molnames:
-            write_shell_script(molname=name, program='autodft_flow.py',
-                               config_file=self.config)
-
-
-class UserInputXYZ:
-    """A class to read and store user inputs from the command line for
-    an AutoDFT job using an XYZ file as input"""
-
-    def __init__(self) -> None:
-
-        # Info for all jobs
-        print_settings_header()
-        self.config = config_from_user()
-        self.gaussian_jobs = gaussian_jobs(self.config)
-        self.e_cutoff = e_cutoff_from_user()
-
-        # Info for individual jobs
-        self.print_mol_info_header()
-        self.mols = xyzs_from_user()
-
-        user_verification()
-        self.export_json()
-        self.write_sh_script()
-
-    def print_mol_info_header(self) -> None:
-        """Prints how to provide information about the molecule(s)."""
-
-        print(dedent(f"""\
-            {DASHES}
-              Molecule information
-              --------------------
-                  Molecule name: The name that will become the base of all
-                                 file names associated with this molecule.
-                                 Example: mol1
-                  XYZ file:      Include .xyz extension.
-                  Charge:        Charge of molecule.
-                  Multiplicity:  Spin multiplicity (number of unpaired
-                                 electrons + 1).
-
-              Enter a blank molecule name to stop adding structures.
-            {DASHES}"""))
-
-    def export_json(self) -> None:
-        """Writes the user inputs to .json configuration files"""
-
-        data = vars(self).copy()
-        mols = data.pop('mols')
-        for mol in mols:
-            to_export = {}
-            to_export.update(data)
-            to_export.update(mol)
-            write_json(to_export)
-
-    def write_sh_script(self) -> None:
-        """Writes shell scripts to run AutoDFT"""
-
-        molnames = [m['molname'] for m in self.mols]
-        for name in molnames:
-            write_shell_script(molname=name, program='autodft_flow_xyz.py',
-                               config_file=self.config)
-
-
-# Helper functions
-
-def print_settings_header() -> None:
-    """Print a header for the information prompts"""
-
-    template = f'{{:<{COL_WIDTH1}}}{{}}'
-    print('\n' + DASHES)
-    print(template.format('  Setting', 'Value'))
-    print(DASHES)
-
-
-def config_from_user() -> str:
-    """Get configuration file to use for autodft job, or use default
-    if not specified"""
-
-    print('  o  Use default autodft settings for CREST,')    
-    use_default = y_or_n('       computational resources, etc.? (y/n):')
-    if use_default:
-        return None
-
-    msg = '  o  Name of .yaml configuration file:'
-    file = prompt(msg)
-    while (not file.endswith('.yaml')) or (file not in os.listdir()):
-        if not file.endswith('.yaml'):
-            print('     File name must end with .yaml:')
-            file = prompt(msg)
-        if file not in os.listdir():
-            print('     File must be present in current directory:')
-            file = prompt(msg)
-    return file
-
-
-def gaussian_jobs(config_file: str = None) -> list[dict]:
-    """Returns a list of the Gaussian job(s) to use for constructing
-    Gaussian input files"""
-
-    config = Config.from_yaml(config_file)
-    if use_default_l_o_t(config_file):
-        return config.gaussian_jobs
-    else:
-        return alt_job_from_user()
-
-
-def use_default_l_o_t(config_file: str = None) -> bool:
-    """Get whether to use the default level of theory (default taken
-    from .yaml config file if one has been specified)"""
-
-    config = Config.from_yaml(config_file)
-    default_jobs = config.gaussian_jobs
-    total = len(default_jobs)
-
-    print('  o  Default computational method:\n')
-    for i, job in enumerate(default_jobs, start=1):
-        print(f'       Job {i} of {total}:')
-        print_l_o_t(job)
-    print('')
-    return y_or_n('     Use default method? (y/n):')
-
-
-def print_l_o_t(job: dict[str]) -> str:
-    """Takes a dictionary of information for a Gaussian job and 
-    prints a string representation of the level of theory"""
-
-    func, basis, route = job['functional'], job['basisset'], job['route']
-    print(f'         {func}/{basis} {route}')
-
-    if job['basisset'].lower() == 'genecp':
-        light = job['ecp_basisset_light']
-        heavy = job['ecp_basisset_heavy']
-        cutoff = job['ecp_cutoff']
-        print(f'         Basis set for atomic number <= {cutoff}: {light}')
-        print(f'         Basis set for atomic number >  {cutoff}: {heavy}')
-
-
-def individual_job_from_user() -> dict:
-    """Get alternate specification of an individual Gaussian job from user
-    (could be one of the linked jobs)"""
-
-    job = {}
-    tmp = f'      {{:<{COL_WIDTH1-6}}}'  # String template
-
-    job['functional'] = input(tmp.format('o  Functional (Example: B3LYP):'))
-    job['basisset'] = input(tmp.format('o  Basis set (Example: 6-31G(d)):'))
-    print(tmp.format('o  Keywords (leave blank if none).'))
-    job['route'] = input(tmp.format(
-        '   Example: opt freq scrf=(smd,solvent=water)'))
-
-    if job['basisset'].lower() != 'genecp':
-        job['ecp_basisset_light'] = None
-        job['ecp_basisset_heavy'] = None
-        job['ecp_cutoff'] = None
-    else:
-        print(tmp.format('GENECP specified. Provide ECP information.'))
-        job['ecp_basisset_light'] = input(
-            tmp.format('o  Basis set for light atoms:'))
-        job['ecp_basisset_heavy'] = input(
-            tmp.format('o  Basis set for heavy atoms:'))
-        job['ecp_cutoff'] = int(
-            input(tmp.format('o  Maximum atomic number for light atoms:')))
-
-    return job
-
-
-def alt_job_from_user() -> dict:
-    """Gets specifications for a Gaussian job specified by the user
-    (which includes linked jobs, if the user desires)"""
-
-    print('\n  Provide the information for the first job.')
-    jobs = [individual_job_from_user()]
-    while True:
-        print('')
-        msg = f'  {len(jobs)} job(s) provided. Add linked job? (y/n):'
-        add_job = y_or_n(msg)
-        if not add_job:
-            break
-        jobs.append(individual_job_from_user())
-
-    return jobs
-
-
-def mols_from_user() -> list[dict]:
-    """Asks the user to specify molecule names and SMILES until a blank
-    molecule name is entered. The molecule info is returned as a list
-    of dictionaries (with each corresponding to one molecule)."""
-
-    mols, molnames = [], []
-    while True:
-        print('  Molecule', len(mols) + 1)
-        name = molname_from_user(not_allowed=molnames)
-        if not name:
-            break
-        smiles, charge, multiplicity = mol_from_user_smiles()
-        molnames.append(name)
-        mols.append({'molname': name, 'smiles': smiles, 'charge': charge,
-                     'multiplicity': multiplicity})
-
-    if not mols:
-        print('  No molecules have been provided. Exiting.')
-        sys.exit(0)
-    return mols
-
-
-def molname_from_user(not_allowed: list[str]) -> str:
-    """Get desired name to use as the root for all file names to create.
-    Makes sure that the name does not match any of the specified names"""
-
-    msg = f'  o  {"Name:":<14}'
-    molname = input(msg)
-    while os.path.isdir(molname) or molname in not_allowed:
-        print('     This name has already been used.')
-        molname = input(msg)
-    return molname
-
-
-def xyzs_from_user() -> list[dict]:
-    """Asks the user to specify molecules (XYZ files with accompanying info)
-    until a blank molecule name is entered. The molecule info is returned as a list
-    of dictionaries (with each corresponding to one molecule)."""
-
-    mols, molnames = [], []
-    while True:
-        print('  Molecule', len(mols) + 1)
-        name = molname_from_user(not_allowed=molnames)
-        if not name:
-            break
-        molnames.append(name)
-        mols.append({'molname': name,
-                     'xyzfile': xyzfile_from_user(),
-                     'charge': charge_from_user(),
-                     'multiplicity': multiplicity_from_user()})
-
-    if not mols:
-        print('  No molecules have been provided. Exiting.')
-        sys.exit(0)
-    return mols
-
-
-def mol_from_user_smiles() -> Tuple[str, int, int]:
-    """Get SMILES string, charge, multiplicity from user-provided SMILES"""
-
-    msg = f'  o  {"SMILES:":<14}'
-    smiles = input(msg)
-
-    while not valid_smiles(smiles):
-        if not valid_structure(smiles):
-            print('     SMILES string does not correspond to a valid structure.')
-        elif '*' in smiles:
-            print('     SMILES string cannot contain wildcard (*)')
-        else:
-            print('     A maximum of 1 radical is allowed on the structure.')
-            print('     Radical-bearing atoms require explicit hydrogens.')
-        smiles = input(msg)
-
-    smiles = Chem.CanonSmiles(smiles)
-    charge = charge_from_smiles(smiles)
-    multiplicity = multiplicity_from_smiles(smiles)
-    return smiles, charge, multiplicity
-
-
-def xyzfile_from_user() -> str:
-    """Get the name of a .xyz file from the user"""
-
-    msg = f'  o  {"XYZ file:":<14}'
-    file = input(msg)
-    while (not file.endswith('.xyz')) or (file not in os.listdir()):
-        if not file.endswith('.xyz'):
-            print('     File name must end with .xyz:')
-            file = input(msg)
-        if file not in os.listdir():
-            print('     File must be present in current directory:')
-            file = input(msg)
-    return file
-
-
-def e_cutoff_from_user() -> str:
-    """Get energy cutoff in kcal/mol for conformer generation"""
-
-    print('  o  Energy cutoff for conformers in kcal/mol')
-    e_cutoff = prompt('       Recommended = 1 kcal/mol:')
-    while not is_positive_float(e_cutoff):
-        e_cutoff = prompt('     Energy cutoff must be a positive number:')
-    return float(e_cutoff)
-
-
-def charge_from_user() -> int:
-    """Prompts the user for an integer input"""
-
-    msg = f'  o  {"Charge:":<14}'
-    num = input(msg)
-    while not is_int(num):
-        print('  Please input an integer: ')
-        num = input(msg)
-    return int(num)
-
-
-def multiplicity_from_user() -> int:
-    """Get spin multiplicity from user"""
-
-    msg = f'  o  {"Multiplicity:":<14}'
-    mult = input(msg)
-    while not mult.isdigit() or int(mult) < 1:
-        print('  Please input an integer 1 or greater: ')
-        mult = input(msg)
-    return int(mult)
-
-
-def user_verification() -> None:
-    """Ask user to verify provided inputs"""
-
-    verified = y_or_n('  Confirm that the above information is correct (y/n):')
-    if not verified:
-        print('  Exiting. Please try again.\n')
-        sys.exit(0)
-    print(DASHES)
-
-
-def valid_smiles(smiles: str) -> bool:
-    """Returns whether a SMILES string is valid"""
-
-    if not valid_structure(smiles):
-        return False
-    if '*' in smiles:
-        return False
-    if multiplicity_from_smiles(smiles) not in [1, 2]:
-        return False
-    return True
-
-
-def valid_structure(smiles: str) -> bool:
-    """Returns whether the SMILES string corresponds to a valid structure """
-
-    return Chem.MolFromSmiles(smiles) is not None
-
-
-def is_positive_float(string: str) -> bool:
-    """Returns true if a string represents a positive float"""
-
-    try:
-        return float(string) > 0
-    except ValueError:
-        return False
-
-
-def is_int(string: str) -> bool:
-    """Returns true if a string represents an integer"""
-
-    try:
-        int(string)
-        return True
-    except ValueError:
-        return False
-
-
-def y_or_n(msg: str) -> bool:
-    """Prompts a user for a yes or no answer"""
-
-    response = prompt(msg).lower()
-    while response not in ['y', 'n']:
-        response = prompt('  Please input y or n: ').lower()
-    return response == 'y'
-
-
-def prompt(msg: str) -> str:
-    """Prompts the user using the provided message, to which string
-    formatting is applied"""
-
-    return input(f'{msg:<{COL_WIDTH1}}')
-
-
-def write_json(config_data: dict) -> None:
-    """Write .json configuration file for autodft_flow.py"""
-
-    molname = config_data['molname']
-    os.mkdir(molname)
-    json_path = f'{molname}/autodft_{molname}.json'
-    with open(json_path, 'w') as f:
-        json.dump(config_data, f, indent=4)
-
-
-def write_shell_script(molname: str, program: str,
-                       config_file: str = None) -> None:
-    """Writes a shell script to execute autodft_flow, which will
-    execute using the configuration data from the .json file.
-    The program can be 'autodft_flow.py' or autodft_xyz_flow.py"""
-
-    config = Config.from_yaml(config_file)
-    sh_path = f'{molname}/autodft_{molname}.sh'
-    
-    with open(sh_path, 'w') as f:
-        f.write(dedent(f"""\
-            #!/bin/sh
-            
-            #SBATCH --nodes=1
-            #SBATCH --ntasks=1
-            #SBATCH --cpus-per-task={N_PROCESSORS}
-            #SBATCH --mem={MEMORY}
-            #SBATCH --time={config.autodft_flow['time']}
-            #SBATCH --output=/dev/null
-            #SBATCH --error=/dev/null
-            #SBATCH --job-name={molname[-8:]}
-            
-            
-            {program}
-            """))
+import json
+import os
+import sys
+from textwrap import dedent
+from typing import Tuple
+
+from rdkit import Chem
+
+from autodft.config.config import Config
+from autodft.utils.autodft_utils import charge_from_smiles, multiplicity_from_smiles
+
+
+# CONSTANTS
+COL_WIDTH1 = 55
+COL_WIDTH2 = 15
+DASHES = '-' * (COL_WIDTH1 + COL_WIDTH2)
+N_PROCESSORS = 1
+MEMORY = '128mb'
+
+
+class UserInputSMILES:
+    """A class to read and store user inputs from the command line for
+    an AutoDFT job using a SMILES string as input"""
+
+    def __init__(self) -> None:
+
+        # Info for all jobs
+        print_settings_header()
+        self.config = config_from_user()
+        self.gaussian_jobs = gaussian_jobs(self.config)
+        self.e_cutoff = e_cutoff_from_user()
+
+        # Info for individual jobs
+        self.print_mol_info_header()
+        self.mols = mols_from_user()
+
+        user_verification()
+        self.export_json()
+        self.write_sh_script()
+
+    def print_mol_info_header(self) -> None:
+        """Prints how to provide information about the molecule(s)."""
+
+        print(dedent(f"""\
+            {DASHES}
+              Molecule information. Please provide the following:
+            
+                  Molecule name: The name that will become the base of all
+                                 file names associated with this molecule.
+                                 Example: mol1
+                  SMILES string: Radical-bearing atoms require explicit
+                                 hydrogens. Maximum 1 radical per molecule.
+                               
+              Enter a blank molecule name to stop adding structures.
+            {DASHES}"""))
+
+    def export_json(self) -> None:
+        """Writes the user inputs to .json configuration files"""
+
+        data = vars(self).copy()
+        if data['config'] is not None:
+            data['config'] = '../' + data['config']
+        mols = data.pop('mols')
+        for mol in mols:
+            to_export = {}
+            to_export.update(data)
+            to_export.update(mol)
+            write_json(to_export)
+
+    def write_sh_script(self) -> None:
+        """Writes shell scripts to run AutoDFT"""
+
+        molnames = [m['molname'] for m in self.mols]
+        for name in molnames:
+            write_shell_script(molname=name, program='autodft_flow.py',
+                               config_file=self.config)
+
+
+class UserInputXYZ:
+    """A class to read and store user inputs from the command line for
+    an AutoDFT job using an XYZ file as input"""
+
+    def __init__(self) -> None:
+
+        # Info for all jobs
+        print_settings_header()
+        self.config = config_from_user()
+        self.gaussian_jobs = gaussian_jobs(self.config)
+        self.e_cutoff = e_cutoff_from_user()
+
+        # Info for individual jobs
+        self.print_mol_info_header()
+        self.mols = xyzs_from_user()
+
+        user_verification()
+        self.export_json()
+        self.write_sh_script()
+
+    def print_mol_info_header(self) -> None:
+        """Prints how to provide information about the molecule(s)."""
+
+        print(dedent(f"""\
+            {DASHES}
+              Molecule information
+              --------------------
+                  Molecule name: The name that will become the base of all
+                                 file names associated with this molecule.
+                                 Example: mol1
+                  XYZ file:      Include .xyz extension.
+                  Charge:        Charge of molecule.
+                  Multiplicity:  Spin multiplicity (number of unpaired
+                                 electrons + 1).
+
+              Enter a blank molecule name to stop adding structures.
+            {DASHES}"""))
+
+    def export_json(self) -> None:
+        """Writes the user inputs to .json configuration files"""
+
+        data = vars(self).copy()
+        if data['config'] is not None:
+            data['config'] = '../' + data['config']
+        mols = data.pop('mols')
+        for mol in mols:
+            to_export = {}
+            to_export.update(data)
+            to_export.update(mol)
+            write_json(to_export)
+
+    def write_sh_script(self) -> None:
+        """Writes shell scripts to run AutoDFT"""
+
+        molnames = [m['molname'] for m in self.mols]
+        for name in molnames:
+            write_shell_script(molname=name, program='autodft_flow_xyz.py',
+                               config_file=self.config)
+
+
+# Helper functions
+
+def print_settings_header() -> None:
+    """Print a header for the information prompts"""
+
+    template = f'{{:<{COL_WIDTH1}}}{{}}'
+    print('\n' + DASHES)
+    print(template.format('  Setting', 'Value'))
+    print(DASHES)
+
+
+def config_from_user() -> str:
+    """Get configuration file to use for autodft job, or use default
+    if not specified"""
+
+    print('  o  Use default autodft settings for CREST,')    
+    use_default = y_or_n('       computational resources, etc.? (y/n):')
+    if use_default:
+        return None
+
+    msg = '  o  Name of .yaml configuration file:'
+    file = prompt(msg)
+    while (not file.endswith('.yaml')) or (file not in os.listdir()):
+        if not file.endswith('.yaml'):
+            print('     File name must end with .yaml:')
+            file = prompt(msg)
+        if file not in os.listdir():
+            print('     File must be present in current directory:')
+            file = prompt(msg)
+    return file
+
+
+def gaussian_jobs(config_file: str = None) -> list[dict]:
+    """Returns a list of the Gaussian job(s) to use for constructing
+    Gaussian input files"""
+
+    config = Config.from_yaml(config_file)
+    if use_default_l_o_t(config_file):
+        return config.gaussian_jobs
+    else:
+        return alt_job_from_user()
+
+
+def use_default_l_o_t(config_file: str = None) -> bool:
+    """Get whether to use the default level of theory (default taken
+    from .yaml config file if one has been specified)"""
+
+    config = Config.from_yaml(config_file)
+    default_jobs = config.gaussian_jobs
+    total = len(default_jobs)
+
+    print('  o  Default computational method:\n')
+    for i, job in enumerate(default_jobs, start=1):
+        print(f'       Job {i} of {total}:')
+        print_l_o_t(job)
+    print('')
+    return y_or_n('     Use default method? (y/n):')
+
+
+def print_l_o_t(job: dict[str]) -> str:
+    """Takes a dictionary of information for a Gaussian job and 
+    prints a string representation of the level of theory"""
+
+    func, basis, route = job['functional'], job['basisset'], job['route']
+    print(f'         {func}/{basis} {route}')
+
+    if job['basisset'].lower() == 'genecp':
+        light = job['ecp_basisset_light']
+        heavy = job['ecp_basisset_heavy']
+        cutoff = job['ecp_cutoff']
+        print(f'         Basis set for atomic number <= {cutoff}: {light}')
+        print(f'         Basis set for atomic number >  {cutoff}: {heavy}')
+
+
+def individual_job_from_user() -> dict:
+    """Get alternate specification of an individual Gaussian job from user
+    (could be one of the linked jobs)"""
+
+    job = {}
+    tmp = f'      {{:<{COL_WIDTH1-6}}}'  # String template
+
+    job['functional'] = input(tmp.format('o  Functional (Example: B3LYP):'))
+    job['basisset'] = input(tmp.format('o  Basis set (Example: 6-31G(d)):'))
+    print(tmp.format('o  Keywords (leave blank if none).'))
+    job['route'] = input(tmp.format(
+        '   Example: opt freq scrf=(smd,solvent=water)'))
+
+    if job['basisset'].lower() != 'genecp':
+        job['ecp_basisset_light'] = None
+        job['ecp_basisset_heavy'] = None
+        job['ecp_cutoff'] = None
+    else:
+        print(tmp.format('GENECP specified. Provide ECP information.'))
+        job['ecp_basisset_light'] = input(
+            tmp.format('o  Basis set for light atoms:'))
+        job['ecp_basisset_heavy'] = input(
+            tmp.format('o  Basis set for heavy atoms:'))
+        job['ecp_cutoff'] = int(
+            input(tmp.format('o  Maximum atomic number for light atoms:')))
+
+    return job
+
+
+def alt_job_from_user() -> dict:
+    """Gets specifications for a Gaussian job specified by the user
+    (which includes linked jobs, if the user desires)"""
+
+    print('\n  Provide the information for the first job.')
+    jobs = [individual_job_from_user()]
+    while True:
+        print('')
+        msg = f'  {len(jobs)} job(s) provided. Add linked job? (y/n):'
+        add_job = y_or_n(msg)
+        if not add_job:
+            break
+        jobs.append(individual_job_from_user())
+
+    return jobs
+
+
+def mols_from_user() -> list[dict]:
+    """Asks the user to specify molecule names and SMILES until a blank
+    molecule name is entered. The molecule info is returned as a list
+    of dictionaries (with each corresponding to one molecule)."""
+
+    mols, molnames = [], []
+    while True:
+        print('  Molecule', len(mols) + 1)
+        name = molname_from_user(not_allowed=molnames)
+        if not name:
+            break
+        smiles, charge, multiplicity = mol_from_user_smiles()
+        molnames.append(name)
+        mols.append({'molname': name, 'smiles': smiles, 'charge': charge,
+                     'multiplicity': multiplicity})
+
+    if not mols:
+        print('  No molecules have been provided. Exiting.')
+        sys.exit(0)
+    return mols
+
+
+def molname_from_user(not_allowed: list[str]) -> str:
+    """Get desired name to use as the root for all file names to create.
+    Makes sure that the name does not match any of the specified names"""
+
+    msg = f'  o  {"Name:":<14}'
+    molname = input(msg)
+    while os.path.isdir(molname) or molname in not_allowed:
+        print('     This name has already been used.')
+        molname = input(msg)
+    return molname
+
+
+def xyzs_from_user() -> list[dict]:
+    """Asks the user to specify molecules (XYZ files with accompanying info)
+    until a blank molecule name is entered. The molecule info is returned as a list
+    of dictionaries (with each corresponding to one molecule)."""
+
+    mols, molnames = [], []
+    while True:
+        print('  Molecule', len(mols) + 1)
+        name = molname_from_user(not_allowed=molnames)
+        if not name:
+            break
+        molnames.append(name)
+        mols.append({'molname': name,
+                     'xyzfile': xyzfile_from_user(),
+                     'charge': charge_from_user(),
+                     'multiplicity': multiplicity_from_user()})
+
+    if not mols:
+        print('  No molecules have been provided. Exiting.')
+        sys.exit(0)
+    return mols
+
+
+def mol_from_user_smiles() -> Tuple[str, int, int]:
+    """Get SMILES string, charge, multiplicity from user-provided SMILES"""
+
+    msg = f'  o  {"SMILES:":<14}'
+    smiles = input(msg)
+
+    while not valid_smiles(smiles):
+        if not valid_structure(smiles):
+            print('     SMILES string does not correspond to a valid structure.')
+        elif '*' in smiles:
+            print('     SMILES string cannot contain wildcard (*)')
+        else:
+            print('     A maximum of 1 radical is allowed on the structure.')
+            print('     Radical-bearing atoms require explicit hydrogens.')
+        smiles = input(msg)
+
+    smiles = Chem.CanonSmiles(smiles)
+    charge = charge_from_smiles(smiles)
+    multiplicity = multiplicity_from_smiles(smiles)
+    return smiles, charge, multiplicity
+
+
+def xyzfile_from_user() -> str:
+    """Get the name of a .xyz file from the user"""
+
+    msg = f'  o  {"XYZ file:":<14}'
+    file = input(msg)
+    while (not file.endswith('.xyz')) or (file not in os.listdir()):
+        if not file.endswith('.xyz'):
+            print('     File name must end with .xyz:')
+            file = input(msg)
+        if file not in os.listdir():
+            print('     File must be present in current directory:')
+            file = input(msg)
+    return file
+
+
+def e_cutoff_from_user() -> str:
+    """Get energy cutoff in kcal/mol for conformer generation"""
+
+    print('  o  Energy cutoff for conformers in kcal/mol')
+    e_cutoff = prompt('       Recommended = 1 kcal/mol:')
+    while not is_positive_float(e_cutoff):
+        e_cutoff = prompt('     Energy cutoff must be a positive number:')
+    return float(e_cutoff)
+
+
+def charge_from_user() -> int:
+    """Prompts the user for an integer input"""
+
+    msg = f'  o  {"Charge:":<14}'
+    num = input(msg)
+    while not is_int(num):
+        print('  Please input an integer: ')
+        num = input(msg)
+    return int(num)
+
+
+def multiplicity_from_user() -> int:
+    """Get spin multiplicity from user"""
+
+    msg = f'  o  {"Multiplicity:":<14}'
+    mult = input(msg)
+    while not mult.isdigit() or int(mult) < 1:
+        print('  Please input an integer 1 or greater: ')
+        mult = input(msg)
+    return int(mult)
+
+
+def user_verification() -> None:
+    """Ask user to verify provided inputs"""
+
+    verified = y_or_n('  Confirm that the above information is correct (y/n):')
+    if not verified:
+        print('  Exiting. Please try again.\n')
+        sys.exit(0)
+    print(DASHES)
+
+
+def valid_smiles(smiles: str) -> bool:
+    """Returns whether a SMILES string is valid"""
+
+    if not valid_structure(smiles):
+        return False
+    if '*' in smiles:
+        return False
+    if multiplicity_from_smiles(smiles) not in [1, 2]:
+        return False
+    return True
+
+
+def valid_structure(smiles: str) -> bool:
+    """Returns whether the SMILES string corresponds to a valid structure """
+
+    return Chem.MolFromSmiles(smiles) is not None
+
+
+def is_positive_float(string: str) -> bool:
+    """Returns true if a string represents a positive float"""
+
+    try:
+        return float(string) > 0
+    except ValueError:
+        return False
+
+
+def is_int(string: str) -> bool:
+    """Returns true if a string represents an integer"""
+
+    try:
+        int(string)
+        return True
+    except ValueError:
+        return False
+
+
+def y_or_n(msg: str) -> bool:
+    """Prompts a user for a yes or no answer"""
+
+    response = prompt(msg).lower()
+    while response not in ['y', 'n']:
+        response = prompt('  Please input y or n: ').lower()
+    return response == 'y'
+
+
+def prompt(msg: str) -> str:
+    """Prompts the user using the provided message, to which string
+    formatting is applied"""
+
+    return input(f'{msg:<{COL_WIDTH1}}')
+
+
+def write_json(config_data: dict) -> None:
+    """Write .json configuration file for autodft_flow.py"""
+
+    molname = config_data['molname']
+    os.mkdir(molname)
+    json_path = f'{molname}/autodft_{molname}.json'
+    with open(json_path, 'w') as f:
+        json.dump(config_data, f, indent=4)
+
+
+def write_shell_script(molname: str, program: str,
+                       config_file: str = None) -> None:
+    """Writes a shell script to execute autodft_flow, which will
+    execute using the configuration data from the .json file.
+    The program can be 'autodft_flow.py' or autodft_xyz_flow.py"""
+
+    config = Config.from_yaml(config_file)
+    sh_path = f'{molname}/autodft_{molname}.sh'
+    
+    with open(sh_path, 'w') as f:
+        f.write(dedent(f"""\
+            #!/bin/sh
+            
+            #SBATCH --nodes=1
+            #SBATCH --ntasks=1
+            #SBATCH --cpus-per-task={N_PROCESSORS}
+            #SBATCH --mem={MEMORY}
+            #SBATCH --time={config.autodft_flow['time']}
+            #SBATCH --output=/dev/null
+            #SBATCH --error=/dev/null
+            #SBATCH --job-name={molname[-8:]}
+            
+            
+            {program}
+            """))
```

### Comparing `autodft-1.0.3/autodft/utils/files.py` & `autodft-1.0.4/autodft/utils/files.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import glob
-import os
-import sys
-
-from autodft.utils.gaussian_output import is_gaussian_logfile
-
-
-# CONSTANTS
-INDENT = ' ' * 3
-
-
-def print_indent(msg: str) -> None:
-    """Prints an indented message"""
-
-    for line in msg.splitlines():
-        print(INDENT + line)
-    if msg.endswith('\n'):
-        print('')
-
-
-def log_files(dirs: list[str] = None) -> list[str]:
-    """Takes a sequence of directory names and returns a dictionary of
-    directories to Gaussian .log files. If no directories are given, the
-    current directory is used (denoted as '.')"""
-
-    dirs = ['.'] if not dirs else [d for d in dirs if os.path.isdir(d)]
-    logfile_dict = {}
-
-    for d in dirs:
-        logfiles_in_dir = [x for x in os.listdir(d) if is_gaussian_logfile(f'{d}/{x}')]
-        logfiles_in_dir.sort(key=lambda x: (molname_from_log(x), filenum(x)))
-        if logfiles_in_dir:
-            logfile_dict[d] = logfiles_in_dir
-    
-    if not logfile_dict:
-        print('\n  No .log files in the specified directory(s)\n')
-        sys.exit()
-    logfile_dict = dict(sorted(logfile_dict.items()))
-    return logfile_dict
-
-
-def filenum(filename: str) -> int:
-    """For a file name that has a number before the extension,
-    returns the number. Otherwise returns None.
-    
-    Example: filenum('Ni1a-conf2.log') # returns 2 """
-    
-    root = filename.split('.')[0]
-    root = root.removesuffix('(lowest)')
-    num = ''
-    for char in root[::-1]:
-        if not char.isdigit():
-            break
-        else:
-            num = char + num
-    try:
-        return int(num)
-    except ValueError:
-        return None
-
-
-def molname_from_log(filename: str) -> str:
-    """"Returns the molecule name from a .log file name.
-    If a label '-confxx' is present, it is removed."""
-
-    root = filename.split('.')[0]
-    num = filenum(filename)
-    return root if num is None else root.removesuffix(f'-conf{num}')
-
-
-def glob_dirs(dirs: list[str]) -> list[str]:
-    """Returns a list of directories with all wildcards parsed"""
-    
-    matches = []
-    for pattern in dirs:
-        matches += glob.glob(pattern)
-    match_dirs = [m for m in matches if os.path.isdir(m)]
-    return match_dirs
-    
+import glob
+import os
+import sys
+
+from autodft.utils.gaussian_output import is_gaussian_logfile
+
+
+# CONSTANTS
+INDENT = ' ' * 3
+
+
+def print_indent(msg: str) -> None:
+    """Prints an indented message"""
+
+    for line in msg.splitlines():
+        print(INDENT + line)
+    if msg.endswith('\n'):
+        print('')
+
+
+def log_files(dirs: list[str] = None) -> list[str]:
+    """Takes a sequence of directory names and returns a dictionary of
+    directories to Gaussian .log files. If no directories are given, the
+    current directory is used (denoted as '.')"""
+
+    dirs = ['.'] if not dirs else [d for d in dirs if os.path.isdir(d)]
+    logfile_dict = {}
+
+    for d in dirs:
+        logfiles_in_dir = [x for x in os.listdir(d) if is_gaussian_logfile(f'{d}/{x}')]
+        logfiles_in_dir.sort(key=lambda x: (molname_from_log(x), filenum(x)))
+        if logfiles_in_dir:
+            logfile_dict[d] = logfiles_in_dir
+    
+    if not logfile_dict:
+        print('\n  No .log files in the specified directory(s)\n')
+        sys.exit()
+    logfile_dict = dict(sorted(logfile_dict.items()))
+    return logfile_dict
+
+
+def filenum(filename: str) -> int:
+    """For a file name that has a number before the extension,
+    returns the number. Otherwise returns None.
+    
+    Example: filenum('Ni1a-conf2.log') # returns 2 """
+    
+    root = filename.split('.')[0]
+    root = root.removesuffix('(lowest)')
+    num = ''
+    for char in root[::-1]:
+        if not char.isdigit():
+            break
+        else:
+            num = char + num
+    try:
+        return int(num)
+    except ValueError:
+        return None
+
+
+def molname_from_log(filename: str) -> str:
+    """"Returns the molecule name from a .log file name.
+    If a label '-confxx' is present, it is removed."""
+
+    root = filename.split('.')[0]
+    num = filenum(filename)
+    return root if num is None else root.removesuffix(f'-conf{num}')
+
+
+def glob_dirs(dirs: list[str]) -> list[str]:
+    """Returns a list of directories with all wildcards parsed"""
+    
+    matches = []
+    for pattern in dirs:
+        matches += glob.glob(pattern)
+    match_dirs = [m for m in matches if os.path.isdir(m)]
+    return match_dirs
+
```

### Comparing `autodft-1.0.3/autodft/utils/gaussian_output.py` & `autodft-1.0.4/autodft/utils/gaussian_output.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-import itertools
-import logging
-import os
-
-import cclib
-from rdkit import Chem
-from rdkit.Chem import AllChem, rdDetermineBonds
-
-
-logger = logging.getLogger(__name__)
-
-
-# CONSTANTS
-RMSD_THRESH_H_POLARONLY = 0.003
-RMSD_THRESH_H_ALL = 0.015
-
-
-def move_redundant(logfiles: list[str]) -> None:
-    """Move Gaussian .log files for redundant structures into a new
-    subdirectory."""
-
-    subdir = 'duplicates'
-    for logfile in find_redundant(logfiles):
-        comfile = logfile.replace('.log', '.com')
-        new_comfile = f'{subdir}/{comfile}'
-        new_logfile = f'{subdir}/{logfile}'
-        try:
-            os.mkdir(subdir)
-        except FileExistsError:
-            pass
-        try:
-            os.rename(logfile, new_logfile)
-            os.rename(comfile, new_comfile)
-        except FileNotFoundError:
-            pass
-
-
-def find_redundant(logfiles: list[str]) -> list[str]:
-    """From a list of .log files, find which ones are for redundant
-    structures.
-
-    Redundant structures are determined based on their RMS deviation,
-    computed using structures without nonpolar hydrogens to speed
-    up GetBestRMS"""
-
-    optimized, polarH_only = optimized_mols(logfiles)
-    files = optimized.keys()
-    is_redundant = {f: False for f in files}
-    
-    for i, j in itertools.combinations(files, 2):
-        if is_redundant[i]:
-            continue
-        try:
-            rmsd = AllChem.GetBestRMS(optimized[i], optimized[j])
-            thresh = RMSD_THRESH_H_POLARONLY if polarH_only else RMSD_THRESH_H_ALL
-            if rmsd < thresh:
-                is_redundant[j] = True
-                logger.info(f'Duplicate structures found: {i} and {j}')
-        except RuntimeError:
-            # GetBestRMS fails when connectivity is different,
-            # in which case structures are not redundant
-            pass
-
-    redundant_files = [f for f in is_redundant if is_redundant[f]]
-    return redundant_files
-
-
-def is_gaussian_logfile(filename):
-    """Returns True if the file name is one of a Gaussian log file"""
-    
-    if not filename.lower().endswith('.log'):
-        return False
-
-    with open(filename) as f:
-        return 'Entering Gaussian System' in f.readline()
-
-
-def normal_termination(filename):
-    """Returns True if the Gaussian job terminated normally"""
-
-    if not is_gaussian_logfile:
-        return False
-
-    with open(filename) as f:
-        return 'Normal termination' in f.readlines()[-1]
-
-
-def error_termination(filename):
-    """Returns True if the Gaussian job terminated with an error"""
-    
-    with open(filename) as f:
-        return 'Error termination' in f.read()
-
-
-def has_linked_jobs(filename):
-    """Returns True if the .log file contains at least one linked job"""
-    
-    if not normal_termination(filename):
-        raise InvalidGaussianLogFileError()
-    
-    with open(filename) as f:
-        data = f.read()
-    n_jobs = data.count('Entering Link 1')
-    return n_jobs > 1
-
-
-def optimized_mols(logfiles):
-    """Read optimized structures from a list of Gaussian .log files.
-    Returns a list of rdkit molecules for the optimized structures,
-    and whether the molecule contains polar Hs only."""
-
-    files = [f for f in logfiles if normal_termination(f)]
-    opt_mols = {}
-
-    for f in files:
-        logdata = cclib.io.ccread(f)
-        charge = logdata.charge
-        multiplicity = logdata.mult
-        xyz_writer = cclib.io.XYZWriter(logdata, lastgeom=True)
-        xyz = xyz_writer.generate_repr()
-
-        mol = Chem.MolFromXYZBlock(xyz)
-        polarH_only = True
-        try:
-            if multiplicity == 2:
-                # Workaround since DetermineBonds fails for radicals
-                rdDetermineBonds.DetermineBonds(mol, charge=charge-1)
-            else:
-                rdDetermineBonds.DetermineBonds(mol, charge=charge)
-        except ValueError:
-            # Transition metal complexes fail with rdDetermineBonds
-            opt_mols[f] = mol
-            polarH_only = False
-        else:
-            opt_mols[f] = remove_nonpolar_Hs(mol)
-
-    return opt_mols, polarH_only
-
-
-def remove_atoms(mol, atoms_to_remove):
-    """Removes the specified atom numbers from an rdkit molecule"""
-
-    atoms_to_remove.sort(reverse=True)
-    edit_mol = Chem.EditableMol(mol)
-    for atom in atoms_to_remove:
-        edit_mol.RemoveAtom(atom)
-    return edit_mol.GetMol()
-
-
-def remove_nonpolar_Hs(mol):
-    """Removes all carbon-bound hydrogens from an rdkit molecule"""
-
-    nonpolar_Hs = []
-    for i, a in enumerate(mol.GetAtoms()):
-        if a.GetSymbol() == 'H':
-            bonded_to_C = any(
-                [neighbor.GetSymbol() == 'C' for neighbor in a.GetNeighbors()])
-            if bonded_to_C:
-                nonpolar_Hs.append(i)
-    return remove_atoms(mol, nonpolar_Hs)
-
-
-class InvalidGaussianLogFileError(Exception):
-    """Raised when a valid Gaussian .log file is required but
-    is not provided"""
-    pass
+import itertools
+import logging
+import os
+
+import cclib
+from rdkit import Chem
+from rdkit.Chem import AllChem, rdDetermineBonds
+
+
+logger = logging.getLogger(__name__)
+
+
+# CONSTANTS
+RMSD_THRESH_H_POLARONLY = 0.003
+RMSD_THRESH_H_ALL = 0.015
+
+
+def move_redundant(logfiles: list[str]) -> None:
+    """Move Gaussian .log files for redundant structures into a new
+    subdirectory."""
+
+    subdir = 'duplicates'
+    for logfile in find_redundant(logfiles):
+        comfile = logfile.replace('.log', '.com')
+        new_comfile = f'{subdir}/{comfile}'
+        new_logfile = f'{subdir}/{logfile}'
+        try:
+            os.mkdir(subdir)
+        except FileExistsError:
+            pass
+        try:
+            os.rename(logfile, new_logfile)
+            os.rename(comfile, new_comfile)
+        except FileNotFoundError:
+            pass
+
+
+def find_redundant(logfiles: list[str]) -> list[str]:
+    """From a list of .log files, find which ones are for redundant
+    structures.
+
+    Redundant structures are determined based on their RMS deviation,
+    computed using structures without nonpolar hydrogens to speed
+    up GetBestRMS"""
+
+    optimized, polarH_only = optimized_mols(logfiles)
+    files = optimized.keys()
+    is_redundant = {f: False for f in files}
+    
+    for i, j in itertools.combinations(files, 2):
+        if is_redundant[i]:
+            continue
+        try:
+            rmsd = AllChem.GetBestRMS(optimized[i], optimized[j])
+            thresh = RMSD_THRESH_H_POLARONLY if polarH_only else RMSD_THRESH_H_ALL
+            if rmsd < thresh:
+                is_redundant[j] = True
+                logger.info(f'Duplicate structures found: {i} and {j}')
+        except RuntimeError:
+            # GetBestRMS fails when connectivity is different,
+            # in which case structures are not redundant
+            pass
+
+    redundant_files = [f for f in is_redundant if is_redundant[f]]
+    return redundant_files
+
+
+def is_gaussian_logfile(filename):
+    """Returns True if the file name is one of a Gaussian log file"""
+    
+    if not filename.lower().endswith('.log'):
+        return False
+
+    with open(filename) as f:
+        return 'Entering Gaussian System' in f.readline()
+
+
+def normal_termination(filename):
+    """Returns True if the Gaussian job terminated normally"""
+
+    if not is_gaussian_logfile:
+        return False
+
+    with open(filename) as f:
+        return 'Normal termination' in f.readlines()[-1]
+
+
+def error_termination(filename):
+    """Returns True if the Gaussian job terminated with an error"""
+    
+    with open(filename) as f:
+        return 'Error termination' in f.read()
+
+
+def has_linked_jobs(filename):
+    """Returns True if the .log file contains at least one linked job"""
+    
+    if not normal_termination(filename):
+        raise InvalidGaussianLogFileError()
+    
+    with open(filename) as f:
+        data = f.read()
+    n_jobs = data.count('Entering Link 1')
+    return n_jobs > 1
+
+
+def optimized_mols(logfiles):
+    """Read optimized structures from a list of Gaussian .log files.
+    Returns a list of rdkit molecules for the optimized structures,
+    and whether the molecule contains polar Hs only."""
+
+    files = [f for f in logfiles if normal_termination(f)]
+    opt_mols = {}
+
+    for f in files:
+        logdata = cclib.io.ccread(f)
+        charge = logdata.charge
+        multiplicity = logdata.mult
+        xyz_writer = cclib.io.XYZWriter(logdata, lastgeom=True)
+        xyz = xyz_writer.generate_repr()
+
+        mol = Chem.MolFromXYZBlock(xyz)
+        polarH_only = True
+        try:
+            if multiplicity == 2:
+                # Workaround since DetermineBonds fails for radicals
+                rdDetermineBonds.DetermineBonds(mol, charge=charge-1)
+            else:
+                rdDetermineBonds.DetermineBonds(mol, charge=charge)
+        except ValueError:
+            # Transition metal complexes fail with rdDetermineBonds
+            opt_mols[f] = mol
+            polarH_only = False
+        else:
+            opt_mols[f] = remove_nonpolar_Hs(mol)
+
+    return opt_mols, polarH_only
+
+
+def remove_atoms(mol, atoms_to_remove):
+    """Removes the specified atom numbers from an rdkit molecule"""
+
+    atoms_to_remove.sort(reverse=True)
+    edit_mol = Chem.EditableMol(mol)
+    for atom in atoms_to_remove:
+        edit_mol.RemoveAtom(atom)
+    return edit_mol.GetMol()
+
+
+def remove_nonpolar_Hs(mol):
+    """Removes all carbon-bound hydrogens from an rdkit molecule"""
+
+    nonpolar_Hs = []
+    for i, a in enumerate(mol.GetAtoms()):
+        if a.GetSymbol() == 'H':
+            bonded_to_C = any(
+                [neighbor.GetSymbol() == 'C' for neighbor in a.GetNeighbors()])
+            if bonded_to_C:
+                nonpolar_Hs.append(i)
+    return remove_atoms(mol, nonpolar_Hs)
+
+
+class InvalidGaussianLogFileError(Exception):
+    """Raised when a valid Gaussian .log file is required but
+    is not provided"""
+    pass
```

### Comparing `autodft-1.0.3/autodft.egg-info/PKG-INFO` & `autodft-1.0.4/autodft.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodft
-Version: 1.0.3
+Version: 1.0.4
 Summary: Automated conformer searching and DFT calculations
 Home-page: https://github.com/shenvilab/autodft
 Author: Shenvi Lab
 Author-email: sting@scripps.edu
 License: GPL-v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -36,15 +36,15 @@
 - ```ssh username@garibaldi.scripps.edu```
 
 Install the micromamba package manager if not already installed.
 (Note: The more common miniconda package manager can also be used, but is
 blocked by firewalls at Scripps Research)
 - ```curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba```
 - ```./bin/micromamba shell init -s bash -p ~/micromamba```
-- ```source ~/.bashrc```
+- Restart the terminal window and connect to the computing cluster again
 
 Create a micromamba environment and install packages (answer yes when prompted)
 - ```micromamba create -n autodft```
 - ```micromamba activate autodft```
 - ```micromamba install -c conda-forge pandas goodvibes rdkit=2023.09.5 cclib xtb crest pyyaml```
 - ```pip install autodft```
 
@@ -221,18 +221,16 @@
 Upload your ```config.yaml``` file to the computing cluster. When running
 AutoDFT in the future, you can respond ```n``` to the prompt about using the
 default settings for CREST, resources, etc. Then, type ```config.yaml``` 
 when prompted (make sure you are in the folder containing the ```config.yaml``` file).
 
 
 ```
-autodft_flow:                           # Settings for 'chaperone' job
-  mem: 128mb                            # Memory
-  processors: 1                         # Number of processors
-  time: '30:00:00'                      # Wall time (should be at least the sum of wall times for the CREST and Gaussian jobs)
+autodft_flow:
+  time: '30:00:00'                      # Wall time for AutoDFT (should be at least the sum of wall times for the CREST and Gaussian jobs)
 
 crest:
   method: gfn2                          # Method (for available options, see: https://crest-lab.github.io/crest-docs/page/documentation/keywords.html)
   solvent: ''                           # Solvent (do not include --gbsa flag) (for available solvents, see: https://xtb-docs.readthedocs.io/en/latest/gbsa.html#parameterized-solvents)
   mem: 2gb                              # Memory
   nprocshared: 12                       # Number of processors
   time: '6:00:00'                       # Wall time
@@ -262,9 +260,8 @@
   ecp_cutoff: null
   
 goodvibes:
   conc: '1'                             # Concentration (mol/L; 1 mol/L is solution phase standard state)
   f_cutoff: '100'                       # Frequency cutoff (cm-1) for quasiharmonic oscillator approximation
   qs: truhlar                           # Quasiharmonic oscillator approximation method
   keywords: ''                          # Additional keywords (see: https://goodvibespy.readthedocs.io/en/latest/source/README.html#using-goodvibes)
-
 ```
```

### Comparing `autodft-1.0.3/autodft.egg-info/SOURCES.txt` & `autodft-1.0.4/autodft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autodft-1.0.3/scripts/autodft_flow_xyz.py` & `autodft-1.0.4/scripts/autodft_flow_xyz.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,74 @@
-#!/usr/bin/python3
-
-import logging
-
-from autodft.config.config import Config
-from autodft.helpers.crest_job import CrestJob
-from autodft.helpers.gaussian_inputfile import GaussianInputWriter
-from autodft.helpers.gaussian_manager import GaussianManager
-from autodft.utils.autodft_utils import input_data, write_autodft_parameters, cleanup
-
-
-def setup_logger(logging_file):
-    logging.basicConfig(filename=logging_file, level=logging.INFO,
-                        format='%(asctime)s   %(message)s',
-                        datefmt='%Y-%m-%d %H:%M:%S')
-    logging.getLogger('cclib').propagate = False
-
-
-def main():
-
-    # Get user inputs and configuration settings
-    inputs = input_data()
-    molname = inputs['molname']
-    config_file = inputs['config']
-    config = Config.from_yaml(config_file)
-    gaussian_config = config.gaussian_input
-
-    logging_file = f'{molname}.out'
-    setup_logger(logging_file)
-    write_autodft_parameters(logging_file, inputs, config)
-
-    try:
-
-        # Initialization
-        gwriter = GaussianInputWriter.from_dicts(
-            job_info_list=inputs['gaussian_jobs'],
-            nprocshared=gaussian_config['nprocshared'],
-            mem=gaussian_config['mem'],
-            write_chk=gaussian_config['write_chk'])
-        logging.info('Initialized GaussianInputWriter.')
-        gsubmitter = GaussianManager(
-            molname=molname,
-            charge=inputs['charge'],
-            multiplicity=inputs['multiplicity'],
-            gwriter=gwriter,
-            **gaussian_config)
-        logging.info('Initialized GaussianManager.')
-
-        # Set up and run CREST job
-        crest_job = CrestJob(
-            molname=molname,
-            xyzfile=inputs['xyzfile'],
-            charge=inputs['charge'],
-            multiplicity=inputs['multiplicity'],
-            e_cutoff=inputs['e_cutoff'],
-            **config.crest)
-
-        # Set up and run Gaussian jobs
-        gsubmitter.submit_from_crest_confs(crest_job=crest_job)
-
-    except Exception:
-        logging.exception('AutoDFT terminated with an error\n\n')
-    
-    else:
-        logging.info('Normal termination of AutoDFT.')
-            
-    finally:
-        cleanup(molname)
-
-
-if __name__ == '__main__':
-    main()
+#!/usr/bin/python3
+
+import logging
+
+from autodft.config.config import Config
+from autodft.helpers.crest_job import CrestJob
+from autodft.helpers.gaussian_inputfile import GaussianInputWriter
+from autodft.helpers.gaussian_manager import GaussianManager
+from autodft.utils.autodft_utils import input_data, write_autodft_parameters, cleanup
+
+
+def setup_logger(logging_file):
+    logging.basicConfig(filename=logging_file, level=logging.INFO,
+                        format='%(asctime)s   %(message)s',
+                        datefmt='%Y-%m-%d %H:%M:%S')
+    logging.getLogger('cclib').propagate = False
+
+
+def main():
+
+    # Get user inputs and configuration settings
+    inputs = input_data()
+    molname = inputs['molname']
+    
+    # Get all other settings from .yaml config file
+    config_file = inputs['config']
+    config = Config.from_yaml(config_file)
+    gaussian_config = config.gaussian_input
+
+    logging_file = f'{molname}.out'
+    setup_logger(logging_file)
+    write_autodft_parameters(logging_file, inputs, config)
+
+    try:
+
+        # Initialization
+        gwriter = GaussianInputWriter.from_dicts(
+            job_info_list=inputs['gaussian_jobs'],
+            nprocshared=gaussian_config['nprocshared'],
+            mem=gaussian_config['mem'],
+            write_chk=gaussian_config['write_chk'])
+        logging.info('Initialized GaussianInputWriter.')
+        gsubmitter = GaussianManager(
+            molname=molname,
+            charge=inputs['charge'],
+            multiplicity=inputs['multiplicity'],
+            gwriter=gwriter,
+            **gaussian_config)
+        logging.info('Initialized GaussianManager.')
+
+        # Set up and run CREST job
+        crest_job = CrestJob(
+            molname=molname,
+            xyzfile=inputs['xyzfile'],
+            charge=inputs['charge'],
+            multiplicity=inputs['multiplicity'],
+            e_cutoff=inputs['e_cutoff'],
+            **config.crest)
+
+        # Set up and run Gaussian jobs
+        gsubmitter.submit_from_crest_confs(crest_job=crest_job)
+
+    except Exception:
+        logging.exception('AutoDFT terminated with an error\n\n')
+    
+    else:
+        logging.info('Normal termination of AutoDFT.')
+            
+    finally:
+        cleanup(molname)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `autodft-1.0.3/scripts/compile_results.py` & `autodft-1.0.4/scripts/compile_results.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,236 +1,236 @@
-#!/usr/bin/python3
-
-import argparse
-import os
-import subprocess
-from dataclasses import dataclass
-from io import StringIO
-
-import numpy as np
-import pandas as pd
-
-from autodft.config.config import Config
-from autodft.utils.files import glob_dirs, log_files, \
-    molname_from_log, print_indent
-from autodft.utils.gaussian_output import has_linked_jobs, \
-    is_gaussian_logfile, normal_termination, error_termination
-
-
-# CONSTANTS
-AU_TO_KCAL = 627.509541
-
-
-def cmdline_parser() -> None:
-    parser = argparse.ArgumentParser()
-    parser.add_argument(dest='dirs', nargs='*', action='store',
-        help='Folder(s) to run script on.')
-    parser.add_argument('-a', '--all', dest='use_all', action='store_true', default=0,
-        help='Optional: Compile all structures from each folder, not just the lowest energy ones')
-    parser.add_argument('-o', '--output', dest='summary_file', action='store', default='Goodvibes_output_summary.csv',
-        help='Name of .csv file to write summarized Goodvibes data to')
-    parser.add_argument('-g', '--gv_output', dest='gv_file', action='store', default='Goodvibes_output.csv',
-        help='Optional: Name of Goodvibes output file. Default: Goodvibes_output.csv')
-    parser.add_argument('-c', '--config', dest='config_file', action='store', default=None,
-        help='Optional: Name of .config file contianing goodvibes settings')
-    return parser.parse_args()
-
-
-@dataclass(kw_only=True)
-class GV_Summarizer:
-    """Generates a .csv file containing summarized Goodvibes results for all
-    .log files in the specified folders"""
-    
-    dirs: list[str] = None
-    qs: str = 'truhlar'
-    f_cutoff: str = '100'
-    conc: str = '1'
-    keywords: str = ''
-    lowest_confs_only: bool = True
-    gv_file: str = 'Goodvibes_output.csv'
-    summary_file: str = 'Goodvibes_output_summary.csv'
-    
-    summary_df: pd.DataFrame = None
-    
-    @property
-    def log_paths(self):
-        """Returns a dictionary of completed, incomplete, and errored .log files"""
-        
-        logs = log_files(self.dirs)
-        log_paths = [f'{folder}/{file}' for folder, files in logs.items()
-                                        for file in files]
-        log_paths = [f for f in log_paths if is_gaussian_logfile(f)]
-        
-        completed = [f for f in log_paths if normal_termination(f)]
-        errored = [f for f in log_paths if error_termination(f)]
-        incomplete = [f for f in log_paths if f not in completed + errored]
-
-        return {'completed': completed, 'incomplete': incomplete, 'errored': errored}
-
-    def run_goodvibes(self) -> None:
-        """Runs goodvibes with the specified options"""
-        
-        completed_jobs = self.log_paths['completed']
-        
-        if not completed_jobs:
-            with open(self.gv_file, 'w') as f:
-                f.write('None of the .log files terminated normally\n')
-            return
-        
-        # Check for consistent presence of linked jobs
-        has_linked = [has_linked_jobs(x) for x in completed_jobs]
-        consistent_linked = all([x == has_linked[0] for x in has_linked])
-        if not consistent_linked:
-            raise InconsistentLinkedJobsError()
-        linked = has_linked[0]
-        
-        # Run Goodvibes
-        command = ['python', '-m', 'goodvibes'] + completed_jobs \
-                + ['--qs', self.qs, '-f', self.f_cutoff, '-c', self.conc,
-                   '--imag', '--csv', '--output', 'temp']
-        command += self.keywords.split()
-        command += ['--spc', 'link'] if linked else []
-        print('')
-        subprocess.run(command)
-        os.replace('Goodvibes_temp.csv', self.gv_file)
-    
-    def summarize(self) -> None:
-        """Creates a DataFrame containing only the key thermodynamic data:
-        molecule name, imaginary frequencies, G (kcal/mol with all
-        corrections applied)"""
-        
-        if not self.log_paths['completed']:
-            return
-        
-        results = self.read_gv_csv()
-        cols = list(results)
-        g_name = [x for x in cols if 'qh-G(T)' in x][-1]
-        results['G(kcal/mol)'] = results[g_name] * AU_TO_KCAL
-        
-        if self.lowest_confs_only:
-            results['molname'] = results['Structure'].map(molname_from_log)
-            lowest_confs_idx = results.groupby('molname')['G(kcal/mol)'].idxmin()
-            results = results.loc[lowest_confs_idx]
-        
-        self.summary_df = results[['Structure', 'im_freq', 'G(kcal/mol)']]
-    
-    def read_gv_csv(self) -> None:
-        """Parses .csv file of Goodvibes output and returns a dataframe"""
-    
-        self.fix_gv_columns()
-        error_lines, thermo_lines = [], []
-        
-        with open(self.gv_file) as f:
-            is_thermo_data = False
-            elements_in_line = None
-            for line in f:
-                if '*****' in line:
-                    continue
-                if 'Warning! Couldn\'t find frequency information ...' in line:
-                    error_lines += line
-                    continue
-                if line.startswith('   Structure,'):
-                    is_thermo_data = True
-                    elements_in_line = line.count(',') # equal because Goodvibes adds an extra comma
-                if is_thermo_data:
-                    if line.count(',') == elements_in_line:
-                        line = line.replace(',\n', '\n')
-                    thermo_lines += line[3:] # Remove spaces and/or bullet point
-    
-        csv_string = ''.join(thermo_lines)
-        df = pd.read_csv(StringIO(csv_string))
-        return df
-
-    def report(self) -> None:
-        """Print and write summarized Goodvibes data for completed Gaussian jobs"""
-        
-        # Write message to file
-        if self.summary_df is None:
-            msg = 'None of the .log files terminated normally\n'
-            print_indent(msg)
-            with open(self.summary_file, 'w') as f:
-                f.write(msg + '\n')
-            return
-        
-        with open(self.summary_file, 'w') as f:
-            csv_string = self.summary_df.to_csv(index=False)
-            f.write(csv_string + '\n')
-        
-        # Print message to console
-        dashes = '*' * 70
-        template_header = '{:<45}{:>9}{:>16}'
-        template_data = '{:<45}{:>9}{:>16.6f}'
-        
-        print_indent(dashes)
-        print_indent(template_header.format('Structure', 'im_freq', 'G(kcal/mol)'))
-        print_indent(dashes)
-        for row in self.summary_df.itertuples(index=False):
-            name, im_freq, g = row
-            im_freq = im_freq if not np.isnan(im_freq) else ''
-            print_indent(template_data.format(name, im_freq, g))
-        print_indent(dashes + '\n')
-        
-    def report_failed(self) -> None:
-        """Print and write information about any incomplete/failed Gaussian jobs"""
-        
-        incomplete = self.log_paths['incomplete']
-        errored = self.log_paths['errored']        
-        warning = ''
-        
-        if incomplete:
-            warning += 'The following jobs did not complete and were not considered:\n'
-            for log_path in incomplete:
-                warning += f'   {log_path.split("/")[-1]}\n'
-            warning += '\n'
-        if errored:
-            warning += 'The following jobs errored and were not considered:\n'
-            for log_path in errored:
-                warning += f'   {log_path.split("/")[-1]}\n'
-            warning += '\n'
-
-        print_indent(warning.removesuffix('\n'))
-        with open(self.summary_file, 'a') as f:
-            f.write(warning)
-        
-    def fix_gv_columns(self) -> None:
-        """Fixes a typo in the column names of the goodvibes output file"""
-        
-        filedata = None
-        with open(self.gv_file) as f:
-            filedata = f.read()
-        with open(self.gv_file, 'w') as f_out:
-            f_out.write(filedata.replace(',im,freq', ',im_freq'))
-
-
-class InconsistentLinkedJobsError(Exception):
-    """Raised when some .log files contain linked Gaussian jobs but
-    others do not"""
-    pass
-
-
-def main() -> None:
-    args = cmdline_parser()
-    dirs = glob_dirs(args.dirs)
-    lowest_confs_only = not args.use_all
-    config_file = args.config_file
-    gv_file = args.gv_file
-    summary_file = args.summary_file
-
-    config = Config.from_yaml(config_file)
-    gv_config = config.goodvibes    
-    
-    summarizer = GV_Summarizer(dirs=dirs,
-                               qs=gv_config['qs'],
-                               f_cutoff=gv_config['f_cutoff'],
-                               conc=gv_config['conc'],
-                               keywords=gv_config['keywords'],
-                               gv_file=gv_file,
-                               lowest_confs_only=lowest_confs_only,
-                               summary_file=summary_file)
-    summarizer.run_goodvibes()
-    print('\nSummary of Goodvibes results:\n')
-    summarizer.summarize()
-    summarizer.report()
-    summarizer.report_failed()
-    
-if __name__ == '__main__':
-    main()
+#!/usr/bin/python3
+
+import argparse
+import os
+import subprocess
+from dataclasses import dataclass
+from io import StringIO
+
+import numpy as np
+import pandas as pd
+
+from autodft.config.config import Config
+from autodft.utils.files import glob_dirs, log_files, \
+    molname_from_log, print_indent
+from autodft.utils.gaussian_output import has_linked_jobs, \
+    is_gaussian_logfile, normal_termination, error_termination
+
+
+# CONSTANTS
+AU_TO_KCAL = 627.509541
+
+
+def cmdline_parser() -> None:
+    parser = argparse.ArgumentParser()
+    parser.add_argument(dest='dirs', nargs='*', action='store',
+        help='Folder(s) to run script on.')
+    parser.add_argument('-a', '--all', dest='use_all', action='store_true', default=0,
+        help='Optional: Compile all structures from each folder, not just the lowest energy ones')
+    parser.add_argument('-o', '--output', dest='summary_file', action='store', default='Goodvibes_output_summary.csv',
+        help='Name of .csv file to write summarized Goodvibes data to')
+    parser.add_argument('-g', '--gv_output', dest='gv_file', action='store', default='Goodvibes_output.csv',
+        help='Optional: Name of Goodvibes output file. Default: Goodvibes_output.csv')
+    parser.add_argument('-c', '--config', dest='config_file', action='store', default=None,
+        help='Optional: Name of .config file contianing goodvibes settings')
+    return parser.parse_args()
+
+
+@dataclass(kw_only=True)
+class GV_Summarizer:
+    """Generates a .csv file containing summarized Goodvibes results for all
+    .log files in the specified folders"""
+    
+    dirs: list[str] = None
+    qs: str = 'truhlar'
+    f_cutoff: str = '100'
+    conc: str = '1'
+    keywords: str = ''
+    lowest_confs_only: bool = True
+    gv_file: str = 'Goodvibes_output.csv'
+    summary_file: str = 'Goodvibes_output_summary.csv'
+    
+    summary_df: pd.DataFrame = None
+    
+    @property
+    def log_paths(self):
+        """Returns a dictionary of completed, incomplete, and errored .log files"""
+        
+        logs = log_files(self.dirs)
+        log_paths = [f'{folder}/{file}' for folder, files in logs.items()
+                                        for file in files]
+        log_paths = [f for f in log_paths if is_gaussian_logfile(f)]
+        
+        completed = [f for f in log_paths if normal_termination(f)]
+        errored = [f for f in log_paths if error_termination(f)]
+        incomplete = [f for f in log_paths if f not in completed + errored]
+
+        return {'completed': completed, 'incomplete': incomplete, 'errored': errored}
+
+    def run_goodvibes(self) -> None:
+        """Runs goodvibes with the specified options"""
+        
+        completed_jobs = self.log_paths['completed']
+        
+        if not completed_jobs:
+            with open(self.gv_file, 'w') as f:
+                f.write('None of the .log files terminated normally\n')
+            return
+        
+        # Check for consistent presence of linked jobs
+        has_linked = [has_linked_jobs(x) for x in completed_jobs]
+        consistent_linked = all([x == has_linked[0] for x in has_linked])
+        if not consistent_linked:
+            raise InconsistentLinkedJobsError()
+        linked = has_linked[0]
+        
+        # Run Goodvibes
+        command = ['python', '-m', 'goodvibes'] + completed_jobs \
+                + ['--qs', self.qs, '-f', self.f_cutoff, '-c', self.conc,
+                   '--imag', '--csv', '--output', 'temp']
+        command += self.keywords.split()
+        command += ['--spc', 'link'] if linked else []
+        print('')
+        subprocess.run(command)
+        os.replace('Goodvibes_temp.csv', self.gv_file)
+    
+    def summarize(self) -> None:
+        """Creates a DataFrame containing only the key thermodynamic data:
+        molecule name, imaginary frequencies, G (kcal/mol with all
+        corrections applied)"""
+        
+        if not self.log_paths['completed']:
+            return
+        
+        results = self.read_gv_csv()
+        cols = list(results)
+        g_name = [x for x in cols if 'qh-G(T)' in x][-1]
+        results['G(kcal/mol)'] = results[g_name] * AU_TO_KCAL
+        
+        if self.lowest_confs_only:
+            results['molname'] = results['Structure'].map(molname_from_log)
+            lowest_confs_idx = results.groupby('molname')['G(kcal/mol)'].idxmin()
+            results = results.loc[lowest_confs_idx]
+        
+        self.summary_df = results[['Structure', 'im_freq', 'G(kcal/mol)']]
+    
+    def read_gv_csv(self) -> None:
+        """Parses .csv file of Goodvibes output and returns a dataframe"""
+    
+        self.fix_gv_columns()
+        error_lines, thermo_lines = [], []
+        
+        with open(self.gv_file) as f:
+            is_thermo_data = False
+            elements_in_line = None
+            for line in f:
+                if '*****' in line:
+                    continue
+                if 'Warning! Couldn\'t find frequency information ...' in line:
+                    error_lines += line
+                    continue
+                if line.startswith('   Structure,'):
+                    is_thermo_data = True
+                    elements_in_line = line.count(',') # equal because Goodvibes adds an extra comma
+                if is_thermo_data:
+                    if line.count(',') == elements_in_line:
+                        line = line.replace(',\n', '\n')
+                    thermo_lines += line[3:] # Remove spaces and/or bullet point
+    
+        csv_string = ''.join(thermo_lines)
+        df = pd.read_csv(StringIO(csv_string))
+        return df
+
+    def report(self) -> None:
+        """Print and write summarized Goodvibes data for completed Gaussian jobs"""
+        
+        # Write message to file
+        if self.summary_df is None:
+            msg = 'None of the .log files terminated normally\n'
+            print_indent(msg)
+            with open(self.summary_file, 'w') as f:
+                f.write(msg + '\n')
+            return
+        
+        with open(self.summary_file, 'w') as f:
+            csv_string = self.summary_df.to_csv(index=False)
+            f.write(csv_string + '\n')
+        
+        # Print message to console
+        dashes = '*' * 70
+        template_header = '{:<45}{:>9}{:>16}'
+        template_data = '{:<45}{:>9}{:>16.6f}'
+        
+        print_indent(dashes)
+        print_indent(template_header.format('Structure', 'im_freq', 'G(kcal/mol)'))
+        print_indent(dashes)
+        for row in self.summary_df.itertuples(index=False):
+            name, im_freq, g = row
+            im_freq = im_freq if not np.isnan(im_freq) else ''
+            print_indent(template_data.format(name, im_freq, g))
+        print_indent(dashes + '\n')
+        
+    def report_failed(self) -> None:
+        """Print and write information about any incomplete/failed Gaussian jobs"""
+        
+        incomplete = self.log_paths['incomplete']
+        errored = self.log_paths['errored']        
+        warning = ''
+        
+        if incomplete:
+            warning += 'The following jobs did not complete and were not considered:\n'
+            for log_path in incomplete:
+                warning += f'   {log_path.split("/")[-1]}\n'
+            warning += '\n'
+        if errored:
+            warning += 'The following jobs errored and were not considered:\n'
+            for log_path in errored:
+                warning += f'   {log_path.split("/")[-1]}\n'
+            warning += '\n'
+
+        print_indent(warning.removesuffix('\n'))
+        with open(self.summary_file, 'a') as f:
+            f.write(warning)
+        
+    def fix_gv_columns(self) -> None:
+        """Fixes a typo in the column names of the goodvibes output file"""
+        
+        filedata = None
+        with open(self.gv_file) as f:
+            filedata = f.read()
+        with open(self.gv_file, 'w') as f_out:
+            f_out.write(filedata.replace(',im,freq', ',im_freq'))
+
+
+class InconsistentLinkedJobsError(Exception):
+    """Raised when some .log files contain linked Gaussian jobs but
+    others do not"""
+    pass
+
+
+def main() -> None:
+    args = cmdline_parser()
+    dirs = glob_dirs(args.dirs)
+    lowest_confs_only = not args.use_all
+    config_file = args.config_file
+    gv_file = args.gv_file
+    summary_file = args.summary_file
+
+    config = Config.from_yaml(config_file)
+    gv_config = config.goodvibes    
+    
+    summarizer = GV_Summarizer(dirs=dirs,
+                               qs=gv_config['qs'],
+                               f_cutoff=gv_config['f_cutoff'],
+                               conc=gv_config['conc'],
+                               keywords=gv_config['keywords'],
+                               gv_file=gv_file,
+                               lowest_confs_only=lowest_confs_only,
+                               summary_file=summary_file)
+    summarizer.run_goodvibes()
+    print('\nSummary of Goodvibes results:\n')
+    summarizer.summarize()
+    summarizer.report()
+    summarizer.report_failed()
+    
+if __name__ == '__main__':
+    main()
```

### Comparing `autodft-1.0.3/scripts/gstatus.py` & `autodft-1.0.4/scripts/gstatus.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-#!/usr/bin/python3
-
-import argparse
-
-from autodft.utils.files import log_files, glob_dirs, print_indent
-
-
-# CONSTANTS
-INDENT = ' ' * 2
-DASHES = '-' * 75
-
-
-def cmdline_parser():
-    parser = argparse.ArgumentParser()
-    parser.add_argument(dest='dirs', nargs='*', action='store',
-        help='Folders(s) to run script on, separated by spaces. Use * for wildcard. If none, will use current directory.')
-    return parser.parse_args()
-
-
-def status(logfile: str, folder: str = '.') -> str:
-    """Returns a string of status information for a Gaussian .log file
-    in the given directory. If no directory specified, will use the
-    current directory"""
-
-    # Initialize variables
-    optimizations_done = 0
-    opt_step_number = '-'
-    jobs_completed = 0
-    jobs_failed = '-'
-    converged_maxforce = '-'
-    converged_rmsforce = '-'
-    converged_maxdisplacement = '-'
-    converged_rmsdisplacement = '-'
-
-    # Initialize variables for scans only
-    is_scan = False
-    max_found = False
-    energies = []
-    energy = None
-
-    logfile_path = f'{folder}/{logfile}'
-    with open(logfile_path) as f:
-        for line in f:
-            if 'Optimized Parameters' in line:
-                optimizations_done += 1
-                opt_step_number = '-'
-                if is_scan:
-                    energies.append(energy)
-                    energy = None
-            if 'Step number' in line:
-                opt_step_number = line.split()[2]
-            if 'Maximum Force' in line:
-                converged_maxforce = line.split()[-1][0]
-            if 'RMS     Force' in line:
-                converged_rmsforce = line.split()[-1][0]
-            if 'Maximum Displacement' in line:
-                converged_maxdisplacement = line.split()[-1][0]
-            if 'RMS     Displacement' in line:
-                converged_rmsdisplacement = line.split()[-1][0]
-            if 'Normal termination' in line:
-                jobs_completed += 1
-                opt_step_number = '-'
-                converged_maxforce = converged_rmsforce = converged_maxdisplacement = converged_rmsdisplacement = '-'
-            if 'Error termination' in line:
-                jobs_failed = 'Y'
-                opt_step_number = '-'
-                converged_maxforce = converged_rmsforce = converged_maxdisplacement = converged_rmsdisplacement = '-'
-            if ('#' in line) and any(x in line.lower() for x in ('opt', 'modredundant')):
-                is_scan = True if not is_scan else is_scan
-            if ('SCF Done:' in line) and is_scan:
-                energy = float(line.split()[4])
-
-    convergence_criteria = ''.join(
-        [converged_maxforce, converged_rmsforce, converged_maxdisplacement, converged_rmsdisplacement])
-    convergence_criteria = convergence_criteria.replace('N', '-')
-    optimizations_done = '-' if not optimizations_done else optimizations_done
-    jobs_completed = '-' if not jobs_completed else jobs_completed
-
-    if is_scan:
-        if energy is not None:  # Append energy of last structure to list, even of optimization of that structure has not yet completed
-            energies.append(energy)
-        if len(energies) >= 2:
-            dE_signs = [e2 - e1 > 0 for e1, e2 in zip(energies, energies[1:])]
-            max_found = any(
-                [dE2 - dE1 == -1 for dE1, dE2 in zip(dE_signs, dE_signs[1:])])
-        if max_found:
-            optimizations_done = f'{optimizations_done}*'
-
-    logfile_root = logfile.removesuffix('.log')
-    status = '{:<35}{:>4}{:>8}{:>8}{:>8}{:>12}'.format(
-        logfile_root[:36], optimizations_done, jobs_completed,
-        jobs_failed, opt_step_number, convergence_criteria)
-    return status
-
-
-def print_header() -> None:
-    """Prints the header"""
-
-    print_indent('\n' + DASHES)
-    print_indent('{:<23}{:>16}{:>8}{:>8}{:>8}{:>12}'.format(
-        'File', 'Opts', 'Jobs', 'Jobs', 'Opt', 'Converged?'))
-    print_indent('{:<23}{:>16}{:>8}{:>8}{:>8}{:>12}'.format(
-        '', 'done', 'done', 'failed', 'step', ''))
-    print_indent(DASHES)
-
-
-def print_footer() -> None:
-    """Prints the footer"""
-
-    print_indent(DASHES)
-    print_indent(
-        'Convergence info: max force, RMS force, max displacement, RMS displacement')
-    print_indent(
-        'For scan jobs: Star (*) indicates that an energy maximum has been found')
-    print_indent(DASHES + '\n')
-
-
-def main() -> None:
-    """Print status of all .log files in the user-specified folder"""
-
-    args = cmdline_parser()
-    dirs = glob_dirs(args.dirs)
-
-    status_msgs = []
-    logs = log_files(dirs)
-    for folder, files in logs.items():
-        status_msgs += [status(file, folder=folder) for file in files]
-
-    if status_msgs:
-        print_header()
-        [print_indent(s) for s in status_msgs]
-        print_footer()
-    else:
-        print('\n\n')
-
-
-if __name__ == '__main__':
-    main()
+#!/usr/bin/python3
+
+import argparse
+
+from autodft.utils.files import log_files, glob_dirs, print_indent
+
+
+# CONSTANTS
+INDENT = ' ' * 2
+DASHES = '-' * 75
+
+
+def cmdline_parser():
+    parser = argparse.ArgumentParser()
+    parser.add_argument(dest='dirs', nargs='*', action='store',
+        help='Folders(s) to run script on, separated by spaces. Use * for wildcard. If none, will use current directory.')
+    return parser.parse_args()
+
+
+def status(logfile: str, folder: str = '.') -> str:
+    """Returns a string of status information for a Gaussian .log file
+    in the given directory. If no directory specified, will use the
+    current directory"""
+
+    # Initialize variables
+    optimizations_done = 0
+    opt_step_number = '-'
+    jobs_completed = 0
+    jobs_failed = '-'
+    converged_maxforce = '-'
+    converged_rmsforce = '-'
+    converged_maxdisplacement = '-'
+    converged_rmsdisplacement = '-'
+
+    # Initialize variables for scans only
+    is_scan = False
+    max_found = False
+    energies = []
+    energy = None
+
+    logfile_path = f'{folder}/{logfile}'
+    with open(logfile_path) as f:
+        for line in f:
+            if 'Optimized Parameters' in line:
+                optimizations_done += 1
+                opt_step_number = '-'
+                if is_scan:
+                    energies.append(energy)
+                    energy = None
+            if 'Step number' in line:
+                opt_step_number = line.split()[2]
+            if 'Maximum Force' in line:
+                converged_maxforce = line.split()[-1][0]
+            if 'RMS     Force' in line:
+                converged_rmsforce = line.split()[-1][0]
+            if 'Maximum Displacement' in line:
+                converged_maxdisplacement = line.split()[-1][0]
+            if 'RMS     Displacement' in line:
+                converged_rmsdisplacement = line.split()[-1][0]
+            if 'Normal termination' in line:
+                jobs_completed += 1
+                opt_step_number = '-'
+                converged_maxforce = converged_rmsforce = converged_maxdisplacement = converged_rmsdisplacement = '-'
+            if 'Error termination' in line:
+                jobs_failed = 'Y'
+                opt_step_number = '-'
+                converged_maxforce = converged_rmsforce = converged_maxdisplacement = converged_rmsdisplacement = '-'
+            if ('#' in line) and any(x in line.lower() for x in ('opt', 'modredundant')):
+                is_scan = True if not is_scan else is_scan
+            if ('SCF Done:' in line) and is_scan:
+                energy = float(line.split()[4])
+
+    convergence_criteria = ''.join(
+        [converged_maxforce, converged_rmsforce, converged_maxdisplacement, converged_rmsdisplacement])
+    convergence_criteria = convergence_criteria.replace('N', '-')
+    optimizations_done = '-' if not optimizations_done else optimizations_done
+    jobs_completed = '-' if not jobs_completed else jobs_completed
+
+    if is_scan:
+        if energy is not None:  # Append energy of last structure to list, even of optimization of that structure has not yet completed
+            energies.append(energy)
+        if len(energies) >= 2:
+            dE_signs = [e2 - e1 > 0 for e1, e2 in zip(energies, energies[1:])]
+            max_found = any(
+                [dE2 - dE1 == -1 for dE1, dE2 in zip(dE_signs, dE_signs[1:])])
+        if max_found:
+            optimizations_done = f'{optimizations_done}*'
+
+    logfile_root = logfile.removesuffix('.log')
+    status = '{:<35}{:>4}{:>8}{:>8}{:>8}{:>12}'.format(
+        logfile_root[:36], optimizations_done, jobs_completed,
+        jobs_failed, opt_step_number, convergence_criteria)
+    return status
+
+
+def print_header() -> None:
+    """Prints the header"""
+
+    print_indent('\n' + DASHES)
+    print_indent('{:<23}{:>16}{:>8}{:>8}{:>8}{:>12}'.format(
+        'File', 'Opts', 'Jobs', 'Jobs', 'Opt', 'Converged?'))
+    print_indent('{:<23}{:>16}{:>8}{:>8}{:>8}{:>12}'.format(
+        '', 'done', 'done', 'failed', 'step', ''))
+    print_indent(DASHES)
+
+
+def print_footer() -> None:
+    """Prints the footer"""
+
+    print_indent(DASHES)
+    print_indent(
+        'Convergence info: max force, RMS force, max displacement, RMS displacement')
+    print_indent(
+        'For scan jobs: Star (*) indicates that an energy maximum has been found')
+    print_indent(DASHES + '\n')
+
+
+def main() -> None:
+    """Print status of all .log files in the user-specified folder"""
+
+    args = cmdline_parser()
+    dirs = glob_dirs(args.dirs)
+
+    status_msgs = []
+    logs = log_files(dirs)
+    for folder, files in logs.items():
+        status_msgs += [status(file, folder=folder) for file in files]
+
+    if status_msgs:
+        print_header()
+        [print_indent(s) for s in status_msgs]
+        print_footer()
+    else:
+        print('\n\n')
+
+
+if __name__ == '__main__':
+    main()
```

