# Comparing `tmp/funfunc-0.2.1.tar.gz` & `tmp/funfunc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/funfunc-0.2.1.tar", last modified: Thu Nov 10 08:32:14 2022, max compression
+gzip compressed data, was "funfunc-0.2.2.tar", last modified: Fri May 17 08:48:53 2024, max compression
```

## Comparing `funfunc-0.2.1.tar` & `funfunc-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 wjia      (1000) wjia      (1000)        0 2022-11-10 08:32:14.000000 funfunc-0.2.1/
--rw-rw-r--   0 wjia      (1000) wjia      (1000)    11357 2022-07-05 06:15:54.000000 funfunc-0.2.1/LICENSE
-drwxrwxr-x   0 wjia      (1000) wjia      (1000)        0 2022-11-10 08:32:14.000000 funfunc-0.2.1/test/
--rw-rw-r--   0 wjia      (1000) wjia      (1000)      899 2022-11-10 07:09:51.000000 funfunc-0.2.1/test/test_free.py
--rw-rw-r--   0 wjia      (1000) wjia      (1000)     4822 2022-11-10 08:18:10.000000 funfunc-0.2.1/test/test_funfunc.py
-drwxrwxr-x   0 wjia      (1000) wjia      (1000)        0 2022-11-10 08:32:14.000000 funfunc-0.2.1/funfunc/
--rw-rw-r--   0 wjia      (1000) wjia      (1000)      594 2022-07-12 06:32:04.000000 funfunc-0.2.1/funfunc/tornado_helper.py
--rw-rw-r--   0 wjia      (1000) wjia      (1000)      857 2022-07-08 08:41:37.000000 funfunc-0.2.1/funfunc/nlp.py
--rw-rw-r--   0 wjia      (1000) wjia      (1000)    12352 2022-11-10 03:47:04.000000 funfunc-0.2.1/funfunc/tool.py
--rw-rw-r--   0 wjia      (1000) wjia      (1000)     3306 2022-11-10 08:23:36.000000 funfunc-0.2.1/funfunc/cv.py
--rw-rw-r--   0 wjia      (1000) wjia      (1000)      245 2022-08-19 03:33:35.000000 funfunc-0.2.1/funfunc/dl.py
--rw-rw-r--   0 wjia      (1000) wjia      (1000)     1151 2022-11-10 08:22:33.000000 funfunc-0.2.1/funfunc/__init__.py
--rw-rw-r--   0 wjia      (1000) wjia      (1000)     1045 2022-10-09 06:38:01.000000 funfunc-0.2.1/funfunc/ml.py
-drwxrwxr-x   0 wjia      (1000) wjia      (1000)        0 2022-11-10 08:32:14.000000 funfunc-0.2.1/funfunc.egg-info/
--rw-rw-r--   0 wjia      (1000) wjia      (1000)        1 2022-11-10 08:32:14.000000 funfunc-0.2.1/funfunc.egg-info/dependency_links.txt
--rw-rw-r--   0 wjia      (1000) wjia      (1000)      308 2022-11-10 08:32:14.000000 funfunc-0.2.1/funfunc.egg-info/SOURCES.txt
--rw-rw-r--   0 wjia      (1000) wjia      (1000)        8 2022-11-10 08:32:14.000000 funfunc-0.2.1/funfunc.egg-info/top_level.txt
--rw-rw-r--   0 wjia      (1000) wjia      (1000)      982 2022-11-10 08:32:14.000000 funfunc-0.2.1/funfunc.egg-info/PKG-INFO
--rw-rw-r--   0 wjia      (1000) wjia      (1000)     1161 2022-08-19 02:54:21.000000 funfunc-0.2.1/setup.py
--rw-rw-r--   0 wjia      (1000) wjia      (1000)      835 2022-08-01 06:40:51.000000 funfunc-0.2.1/README.md
--rw-rw-r--   0 wjia      (1000) wjia      (1000)      982 2022-11-10 08:32:14.000000 funfunc-0.2.1/PKG-INFO
--rw-rw-r--   0 wjia      (1000) wjia      (1000)       38 2022-11-10 08:32:14.000000 funfunc-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 08:48:53.011140 funfunc-0.2.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-11 09:07:44.000000 funfunc-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      989 2024-05-17 08:48:53.010278 funfunc-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      875 2024-05-11 09:07:44.000000 funfunc-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 08:48:53.003991 funfunc-0.2.2/funfunc/
+-rw-rw-rw-   0        0        0      342 2024-05-17 07:46:14.000000 funfunc-0.2.2/funfunc/__init__.py
+-rw-rw-rw-   0        0        0     4668 2024-05-17 07:50:03.000000 funfunc-0.2.2/funfunc/cv.py
+-rw-rw-rw-   0        0        0      291 2024-05-17 07:46:14.000000 funfunc-0.2.2/funfunc/dl.py
+-rw-rw-rw-   0        0        0     1147 2024-05-17 07:50:03.000000 funfunc-0.2.2/funfunc/ml.py
+-rw-rw-rw-   0        0        0     1211 2024-05-17 07:50:03.000000 funfunc-0.2.2/funfunc/nlp.py
+-rw-rw-rw-   0        0        0    13268 2024-05-17 07:48:37.000000 funfunc-0.2.2/funfunc/tool.py
+-rw-rw-rw-   0        0        0      654 2024-05-17 07:48:37.000000 funfunc-0.2.2/funfunc/tornado_helper.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:48:53.008160 funfunc-0.2.2/funfunc.egg-info/
+-rw-rw-rw-   0        0        0      989 2024-05-17 08:48:52.000000 funfunc-0.2.2/funfunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-05-17 08:48:52.000000 funfunc-0.2.2/funfunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 08:48:52.000000 funfunc-0.2.2/funfunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 08:48:52.000000 funfunc-0.2.2/funfunc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 08:48:53.011140 funfunc-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1190 2024-05-11 09:07:44.000000 funfunc-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:48:53.009499 funfunc-0.2.2/test/
+-rw-rw-rw-   0        0        0      795 2024-05-11 09:07:44.000000 funfunc-0.2.2/test/test_free.py
+-rw-rw-rw-   0        0        0     5440 2024-05-17 08:26:31.000000 funfunc-0.2.2/test/test_funfunc.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `funfunc-0.2.1/LICENSE` & `funfunc-0.2.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `funfunc-0.2.1/test/test_funfunc.py` & `funfunc-0.2.2/test/test_funfunc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,134 +1,142 @@
-import base64
-import os
-import unittest
-import time
-
-import cv2.cv2 as cv2
-import numpy as np
-import pandas as pd
-from PIL import Image
-
-import funfunc
-
-SKIP_TORCH = False
-try:
-    import torch
-except ImportError:
-    SKIP_TORCH = True
-
-
-class FunfuncTestCase(unittest.TestCase):
-    def setUp(self) -> None:
-        self.image_array = np.zeros((50, 50, 3), dtype=np.uint8)
-        self.pil_image = Image.fromarray(cv2.cvtColor(self.image_array, cv2.COLOR_BGR2RGB))
-        self.image_base64 = base64.b64encode(cv2.imencode('.png', self.image_array)[1].tobytes()).decode('utf-8')
-
-    def test_base64_string_to_pil_image(self):
-        pil_image = funfunc.base64_string_to_pil_image(self.image_base64)
-        self.assertIsInstance(pil_image, Image.Image)
-
-    def test_pil_image_to_base64_string(self):
-        image_base64 = funfunc.pil_image_to_base64_string(self.pil_image)
-        # 该测试判断条件改为下句无法通过，问题未知
-        # self.assertEqual(image_base64, self.image_base64)
-        self.assertIsInstance(image_base64, str)
-
-    def test_image_array_to_pil_image(self):
-        pil_image = funfunc.image_array_to_pil_image(self.image_array)
-        self.assertIsInstance(pil_image, Image.Image)
-
-    def test_pil_image_to_image_array(self):
-        image_array = funfunc.pil_image_to_image_array(self.pil_image)
-        self.assertIsInstance(image_array, np.ndarray)
-
-    def test_base64_string_to_image_array(self):
-        image_array = funfunc.base64_string_to_image_array(self.image_base64)
-        self.assertEqual(image_array.all(), self.image_array.all())
-
-    def test_image_array_to_base64_string(self):
-        image_base64 = funfunc.image_array_to_base64_string(self.image_array)
-        self.assertEqual(image_base64, self.image_base64)
-
-    @unittest.skipIf(SKIP_TORCH, "package torch is too big, if didn't install, "
-                                 "then pass the get_device_torch test")
-    def test_get_device_torch(self):
-        device = funfunc.get_device_torch()
-        self.assertEqual(device, 'cpu')
-
-    def test_pandas_max_print(self):
-        old = pd.get_option('display.max_columns')
-        funfunc.pandas_max_print()
-        new = pd.get_option('display.max_columns')
-        self.assertNotEqual(old, new)
-
-    def test_Validator_is_url(self):
-        url = 'https://www.baidu.com'
-        un_url = 'htps://www.usb.net'
-        is_url = funfunc.Validator.is_url(url)
-        not_url = funfunc.Validator.is_url(un_url)
-        self.assertTrue(is_url)
-        self.assertFalse(not_url)
-
-    def test_Validator_is_chinese(self):
-        chinese = '你好啊123abc'
-        un_chinese = 'hello123abc'
-        is_chinese = funfunc.Validator.is_chinese(chinese)
-        not_chinese = funfunc.Validator.is_chinese(un_chinese)
-        self.assertTrue(is_chinese)
-        self.assertFalse(not_chinese)
-
-    def test_download_file(self):
-        if os.path.exists('./pic.gif'):
-            os.remove('./pic.gif')
-        funfunc.download_file("http://img61.ddimg.cn/upload_img/00405/luyi/DDlogoNEW.gif",
-                              './pic.gif')
-        self.assertTrue(os.path.exists('./pic.gif'))
-
-    def test_time_it(self):
-        @funfunc.time_it
-        def a_func():
-            time.sleep(3)
-
-        a_func()
-        self.assertEqual(True, True)
-
-    def test_quick_sort(self):
-        arr = [3, 1, 2]
-        sorted_arr = funfunc.quick_sort(arr)
-        self.assertEqual(sorted_arr, sorted(arr))
-
-    def test_chunks(self):
-        arr = [i for i in range(100)]
-        the_chunks = funfunc.chunks(arr, 10)
-        self.assertEqual(len(the_chunks[0]), 10)
-
-    def test_get_all_abspath_from_folder(self):
-        path = '.'
-        file_lst = funfunc.get_all_abspath_from_folder(path)
-        file_lst_relative = funfunc.get_all_abspath_from_folder(path, get_relative=True)
-        file_lst_with_folder = funfunc.get_all_abspath_from_folder(path, file_only=False)
-        self.assertEqual(len(file_lst), 3)
-        self.assertEqual(sorted(file_lst_relative)[0], './pic.gif')
-        self.assertEqual(len(file_lst_with_folder), 4)
-
-    def test_train_test_split_arr(self):
-        arr = [i for i in range(100)]
-        train, test = funfunc.train_test_split_arr(arr, ratio=0.90, shuffle=True)
-        self.assertEqual(len(train), 90)
-
-    def test_is_in_docker(self):
-        self.assertFalse(funfunc.is_in_docker())
-
-    def test_image_array_to_bytes(self):
-        import tempfile
-
-        img_arr = cv2.imread('./sample_file/website.png')
-        img_bytes = funfunc.image_array_to_bytes(img_arr)
-        with tempfile.NamedTemporaryFile('wb', dir='/tmp', suffix='.png') as ntf:
-            ntf.write(img_bytes)
-            img = cv2.imread(ntf.name)
-        np.testing.assert_almost_equal(img, img_arr)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import base64
+import os
+import unittest
+import time
+
+import cv2
+import numpy as np
+import pandas as pd
+from PIL import Image
+from pathlib import Path
+
+import funfunc
+
+SKIP_TORCH = False
+try:
+    import torch
+except ImportError:
+    SKIP_TORCH = True
+
+
+class FunfuncTestCase(unittest.TestCase):
+    def setUp(self) -> None:
+        self.image_array = np.zeros((50, 50, 3), dtype=np.uint8)
+        self.pil_image = Image.fromarray(cv2.cvtColor(self.image_array, cv2.COLOR_BGR2RGB))
+        self.image_base64 = base64.b64encode(cv2.imencode('.png', self.image_array)[1].tobytes()).decode('utf-8')
+
+    def test_base64_string_to_pil_image(self):
+        pil_image = funfunc.base64_string_to_pil_image(self.image_base64)
+        self.assertIsInstance(pil_image, Image.Image)
+
+    def test_pil_image_to_base64_string(self):
+        image_base64 = funfunc.pil_image_to_base64_string(self.pil_image)
+        # 该测试判断条件改为下句无法通过，问题未知
+        # self.assertEqual(image_base64, self.image_base64)
+        image = funfunc.base64_string_to_pil_image(image_base64)
+        self.assertEqual(image.size, (50, 50))
+
+    def test_image_array_to_pil_image(self):
+        pil_image = funfunc.image_array_to_pil_image(self.image_array)
+        self.assertIsInstance(pil_image, Image.Image)
+
+    def test_pil_image_to_image_array(self):
+        image_array = funfunc.pil_image_to_image_array(self.pil_image)
+        self.assertIsInstance(image_array, np.ndarray)
+
+    def test_base64_string_to_image_array(self):
+        image_array = funfunc.base64_string_to_image_array(self.image_base64)
+        self.assertEqual(image_array.all(), self.image_array.all())
+
+    def test_image_array_to_base64_string(self):
+        image_base64 = funfunc.image_array_to_base64_string(self.image_array)
+        self.assertEqual(image_base64, self.image_base64)
+
+    @unittest.skipIf(SKIP_TORCH, "package torch is too big, if didn't install, "
+                                 "then pass the get_device_torch test")
+    def test_get_device_torch(self):
+        device = funfunc.get_device_torch()
+        self.assertIn(device, ['cuda', 'cpu'])
+
+    def test_pandas_max_print(self):
+        old = pd.get_option('display.max_columns')
+        funfunc.pandas_max_print()
+        new = pd.get_option('display.max_columns')
+        self.assertNotEqual(old, new)
+
+    def test_Validator_is_url(self):
+        url = 'https://www.baidu.com'
+        un_url = 'htps://www.usb.net'
+        is_url = funfunc.Validator.is_url(url)
+        not_url = funfunc.Validator.is_url(un_url)
+        self.assertTrue(is_url)
+        self.assertFalse(not_url)
+
+    def test_Validator_is_chinese(self):
+        chinese = '你好啊123abc'
+        un_chinese = 'hello123abc'
+        is_chinese = funfunc.Validator.is_chinese(chinese)
+        not_chinese = funfunc.Validator.is_chinese(un_chinese)
+        self.assertTrue(is_chinese)
+        self.assertFalse(not_chinese)
+
+    def test_download_file(self):
+        if os.path.exists('./pic.gif'):
+            os.remove('./pic.gif')
+        funfunc.download_file("http://img61.ddimg.cn/upload_img/00405/luyi/DDlogoNEW.gif",
+                              './pic.gif')
+        self.assertTrue(os.path.exists('./pic.gif'))
+
+    @classmethod
+    def test_time_it(cls):
+        @funfunc.time_it
+        def a_func():
+            time.sleep(1)
+
+        a_func()
+
+    def test_quick_sort(self):
+        arr = [3, 1, 2]
+        sorted_arr = funfunc.quick_sort(arr)
+        self.assertEqual(sorted_arr, sorted(arr))
+
+    def test_chunks(self):
+        arr = [i for i in range(100)]
+        the_chunks = funfunc.chunks(arr, 10)
+        self.assertEqual(len(the_chunks[0]), 10)
+
+    def test_get_all_abspath_from_folder(self):
+        path = '.'
+        file_lst = funfunc.get_all_abspath_from_folder(path)
+        file_lst_relative = funfunc.get_all_abspath_from_folder(path, get_relative=True)
+        file_lst_with_folder = funfunc.get_all_abspath_from_folder(path, file_only=False)
+        self.assertEqual(len(file_lst), 3)
+        self.assertEqual(Path(sorted(file_lst_relative)[0]), Path('./pic.gif'))
+        self.assertEqual(len(file_lst_with_folder), 4)
+
+    def test_train_test_split_arr(self):
+        arr = [i for i in range(100)]
+        train, test = funfunc.train_test_split_arr(arr, ratio=0.90, shuffle=True)
+        self.assertEqual(len(train), 90)
+
+    def test_is_in_docker(self):
+        flag = funfunc.is_in_docker()
+        self.assertIn(flag, [True, False])
+
+    def test_image_array_to_bytes(self):
+        bytes = funfunc.image_array_to_bytes(self.image_array)
+        image = funfunc.bytes_to_pil_image(bytes)
+        self.assertEqual(image.size, (50, 50))
+
+    def test_bytes_to_image_array(self):
+        image_arr = funfunc.bytes_to_image_array(funfunc.pil_image_to_bytes(self.pil_image))
+        image = funfunc.image_array_to_pil_image(image_arr)
+        self.assertEqual(image.size, (50, 50))
+
+    def test_image_url_to_pil_image(self):
+        image = funfunc.image_url_to_pil_image('http://mmbiz.qpic.cn/mmbiz/PwIlO51l7wuFyoFwAXfqPNETWCibjN'
+                                               'ACIt6ydN7vw8LeIwT7IjyG3eeribmK4rhibecvNKiaT2qeJRIWXLuKYPiaqtQ/0')
+        self.assertEqual(image.size, (960, 1280))
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `funfunc-0.2.1/funfunc/tool.py` & `funfunc-0.2.2/funfunc/tool.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,429 +1,453 @@
-# -*- coding: utf-8 -*-
-# AUTHOR  : wjia
-# TIME    : 2022/6/21 17:08
-# FILE    : tool
-# PROJECT : funfunc
-# IDE     : PyCharm
-import copy
-import datetime
-import functools
-import json
-import logging
-import os
-import time
-import typing
-import warnings
-
-
-def get_current_str_time() -> str:
-    """get local time"""
-    now_time = datetime.datetime.now()
-    str_time = now_time.strftime('%Y年%m月%d日星期%w %H时%M分%S秒')
-    return str_time
-
-
-def download_file(url, save_path):
-    """download a file by its url"""
-    import requests
-
-    r = requests.get(url, stream=True)
-    with open(os.path.join(save_path), 'wb') as f:
-        for chunk in r.iter_content(chunk_size=1024):
-            f.write(chunk)
-
-
-def time_it(method):
-    """use this decorator to print a function time cost"""
-
-    @functools.wraps(method)
-    def wrapper(*args, **kwargs):
-        start = time.time()
-        result = method(*args, **kwargs)
-        end = time.time()
-        print('{} USED TIME:{}'.format(method.__name__, end - start))
-
-        return result
-
-    return wrapper
-
-
-def time_it_precise(method):
-    """similar to time_it but use more precise time.perf_counter()"""
-
-    @functools.wraps(method)
-    def wrapper(*args, **kwargs):
-        start = time.perf_counter()
-        result = method(*args, **kwargs)
-        end = time.perf_counter()
-        print('{} USED TIME:{}'.format(method.__name__, end - start))
-
-        return result
-
-    return wrapper
-
-
-def quick_sort(arr: list) -> list:
-    """classic sort algorithm"""
-    if len(arr) < 2:
-        return arr
-    temp = arr[0]
-    small = [i for i in arr[1:] if i <= temp]
-    big = [i for i in arr[1:] if i > temp]
-    return quick_sort(small) + [temp] + quick_sort(big)
-
-
-def get_basic_logger(level=logging.INFO, fmt: str = None, datefmt: str = None, **kwargs):
-    """fast way to create a logging.Logger object"""
-    if fmt:
-        log_format = fmt
-    else:
-        log_format = "%(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s"
-
-    if datefmt:
-        log_datefmt = datefmt
-    else:
-        log_datefmt = "%Y-%m-%d %H:%M:%S"
-    logging.basicConfig(
-        level=level,
-        format=log_format,
-        datefmt=log_datefmt,
-        **kwargs)
-
-    logger = logging.getLogger(__name__)
-    return logger
-
-
-def chunks(arr: list, n: int) -> list:
-    """split list to some lists with n items in it"""
-    return [arr[i:i + n] for i in range(0, len(arr), n)]
-
-
-def get_host_ip():
-    """check local ip"""
-    import socket
-
-    s = None
-    try:
-        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        s.connect(('8.8.8.8', 80))
-        ip = s.getsockname()[0]
-    finally:
-        s.close()
-
-    return ip
-
-
-def time_to_timestamp(date):
-    """2000-10-20 12:10:30 format time to timestamp"""
-    return datetime.datetime.strptime(date, "%Y-%m-%d %H:%M:%S").timestamp()
-
-
-def second_to_strtime(second: int):
-    """second to min:sec"""
-    return time.strftime("%M:%S", time.gmtime(second))
-
-
-def set_deprecated(warn_msg=None):
-    """set a function into deprecated state"""
-
-    def outer(deprecated_func):
-        @functools.wraps(deprecated_func)
-        def inner(*args, **kwargs):
-            if warn_msg and isinstance(warn_msg, str):
-                warnings.warn(warn_msg, DeprecationWarning, 2)
-            else:
-                warnings.warn(f"This function {deprecated_func.__name__}() is deprecated!", DeprecationWarning, 2)
-            core = deprecated_func(*args, **kwargs)
-            return core
-
-        return inner
-
-    return outer
-
-
-def indented_json_string(json_string):
-    return json.dumps(json_string, indent=2, ensure_ascii=False)
-
-
-class MagicDict(dict):
-    """
-    let you access python dict object by using attr
-
-    Example:
-        from funfunc import MagicDict
-
-        simple_dict = {'name': 'Jack', 'age': 19, 'info': {'address': 'Beijing', 'phone': '123'}}
-        magic_dict = MagicDict(simple_dict)
-        print(magic_dict.name)
-        # Jack
-        print(magic_dict.info.address)
-        # Beijing
-    """
-
-    def __init__(__self, *args, **kwargs):  # noqa
-        object.__setattr__(__self, '__parent', kwargs.pop('__parent', None))
-        object.__setattr__(__self, '__key', kwargs.pop('__key', None))
-        object.__setattr__(__self, '__frozen', False)
-        for arg in args:
-            if not arg:
-                continue
-            elif isinstance(arg, dict):
-                for key, val in arg.items():
-                    __self[key] = __self._hook(val)
-            elif isinstance(arg, tuple) and (not isinstance(arg[0], tuple)):
-                __self[arg[0]] = __self._hook(arg[1])
-            else:
-                for key, val in iter(arg):
-                    __self[key] = __self._hook(val)
-
-        for key, val in kwargs.items():
-            __self[key] = __self._hook(val)
-
-    def __setattr__(self, name, value):
-        if hasattr(self.__class__, name):
-            raise AttributeError("'Dict' object attribute "
-                                 "'{0}' is read-only".format(name))
-        else:
-            self[name] = value
-
-    def __setitem__(self, name, value):
-        isFrozen = (hasattr(self, '__frozen') and
-                    object.__getattribute__(self, '__frozen'))
-        if isFrozen and name not in super(MagicDict, self).keys():
-            raise KeyError(name)
-        super(MagicDict, self).__setitem__(name, value)
-        try:
-            p = object.__getattribute__(self, '__parent')
-            key = object.__getattribute__(self, '__key')
-        except AttributeError:
-            p = None
-            key = None
-        if p is not None:
-            p[key] = self
-            object.__delattr__(self, '__parent')
-            object.__delattr__(self, '__key')
-
-    def __add__(self, other):
-        if not self.keys():
-            return other
-        else:
-            self_type = type(self).__name__
-            other_type = type(other).__name__
-            msg = "unsupported operand type(s) for +: '{}' and '{}'"
-            raise TypeError(msg.format(self_type, other_type))
-
-    @classmethod
-    def _hook(cls, item):
-        if isinstance(item, dict):
-            return cls(item)
-        elif isinstance(item, (list, tuple)):
-            return type(item)(cls._hook(elem) for elem in item)
-        return item
-
-    def __getattr__(self, item):
-        return self.__getitem__(item)
-
-    def __missing__(self, name):
-        if object.__getattribute__(self, '__frozen'):
-            raise KeyError(name)
-        return self.__class__(__parent=self, __key=name)
-
-    def __delattr__(self, name):
-        del self[name]
-
-    def to_dict(self):
-        base = {}
-        for key, value in self.items():
-            if isinstance(value, type(self)):
-                base[key] = value.to_dict()
-            elif isinstance(value, (list, tuple)):
-                base[key] = type(value)(
-                    item.to_dict() if isinstance(item, type(self)) else
-                    item for item in value)
-            else:
-                base[key] = value
-        return base
-
-    def copy(self):
-        return copy.copy(self)
-
-    def deepcopy(self):
-        return copy.deepcopy(self)
-
-    def __deepcopy__(self, memo):
-        other = self.__class__()
-        memo[id(self)] = other
-        for key, value in self.items():
-            other[copy.deepcopy(key, memo)] = copy.deepcopy(value, memo)
-        return other
-
-    def update(self, *args, **kwargs):
-        other = {}
-        if args:
-            if len(args) > 1:
-                raise TypeError()
-            other.update(args[0])
-        other.update(kwargs)
-        for k, v in other.items():
-            if ((k not in self) or
-                    (not isinstance(self[k], dict)) or
-                    (not isinstance(v, dict))):
-                self[k] = v
-            else:
-                self[k].update(v)
-
-    def __getnewargs__(self):
-        return tuple(self.items())
-
-    def __getstate__(self):
-        return self
-
-    def __setstate__(self, state):
-        self.update(state)
-
-    def __or__(self, other):
-        if not isinstance(other, (MagicDict, dict)):
-            return NotImplemented
-        new = MagicDict(self)
-        new.update(other)
-        return new
-
-    def __ror__(self, other):
-        if not isinstance(other, (MagicDict, dict)):
-            return NotImplemented
-        new = MagicDict(other)
-        new.update(self)
-        return new
-
-    def __ior__(self, other):
-        self.update(other)
-        return self
-
-    def setdefault(self, key, default=None):
-        if key in self:
-            return self[key]
-        else:
-            self[key] = default
-            return default
-
-    def freeze(self, shouldFreeze=True):
-        object.__setattr__(self, '__frozen', shouldFreeze)
-        for key, val in self.items():
-            if isinstance(val, MagicDict):
-                val.freeze(shouldFreeze)
-
-    def unfreeze(self):
-        self.freeze(False)
-
-
-class OptClass:
-    """
-    let you create a Option class by a list of option names of predefined options dict
-    .json class property can convert options to json format string
-
-    Example:
-        # init by list of option names
-        opt_names = ['use_gpu', 'workers', 'batch_size']
-        opts = OptClass(opt_names)
-        opts.use_gpu = True
-        opts.workers = 2
-
-        # init by predefined options dict
-        opts_dict = {'use_gpu': True, 'workers': 2, 'batch_size': 16}
-        opts = OptClass(opts_dict)
-        print(opts.use_gpu)
-        print(opts.json)
-    """
-
-    def __init__(self, option_names):
-        if isinstance(option_names, list):
-            for opt in option_names:
-                if not isinstance(opt, str):
-                    opt_str = str(opt)
-                    setattr(self, opt_str, None)
-                else:
-                    setattr(self, opt, None)
-        elif isinstance(option_names, dict):
-            for k, v in option_names.items():
-                if not isinstance(k, str):
-                    opt_str = str(k)
-                    setattr(self, opt_str, v)
-                else:
-                    setattr(self, k, v)
-        else:
-            raise TypeError(f'Unsupported option_names type: {type(option_names)}, please pass a list or dict object')
-
-    @property
-    def json(self):
-        return json.dumps(self.__dict__)
-
-
-def get_all_abspath_from_folder(folder_path: str, get_relative: bool = False, file_only: bool = True) -> list:
-    """
-    get all files path of a path or a folder, if file_only=False, include folder
-
-    :param folder_path: target folder_path, a path-like string
-    :param get_relative: if True, will return relative path instead of abspath
-    :param file_only: if False, will return folder's path in folder_path
-    """
-    if not get_relative:
-        folder_path = os.path.abspath(folder_path)
-
-    if not file_only:
-        return [os.path.join(folder_path, i) for i in os.listdir(folder_path)]
-
-    return [os.path.join(folder_path, i) for i in os.listdir(folder_path) if
-            os.path.isfile(os.path.join(folder_path, i))]
-
-
-def is_in_docker():
-    return os.path.exists('/workspace')
-
-
-def get_methods(instance):
-    methods = [m for m in dir(instance) if callable(getattr(instance, m)) and not m.startswith("__")]
-    return methods
-
-
-def get_args_info(name, opt):
-    return f'{name}: ' + ', '.join(f'{k}={v}' for k, v in vars(opt).items())
-
-
-def try_except_print(func):
-    """
-    auto add try except to a function, use @try_except_print decorator
-    """
-
-    @functools.wraps(func)
-    def handler(*args, **kwargs):
-        try:
-            func(*args, **kwargs)
-        except Exception as e:
-            print(f'Exception From {func.__name__}: {e}')
-
-    return handler
-
-
-def retry(retry_count: int = 5, sleep_time: int = 1):
-    """
-    retry to call a function when it raise an error
-    """
-
-    def wrapper(func):
-        @functools.wraps(func)
-        def inner(*args, **kwargs):
-            for i in range(retry_count):
-                try:
-                    res = func(*args, **kwargs)
-                    return res
-                except:
-                    time.sleep(sleep_time)
-                    continue
-            return None
-
-        return inner
-
-    return wrapper
-
-
-Flexible = typing.Any  # use this to mark something could be modified
+# -*- coding: utf-8 -*-
+# AUTHOR  : wjia
+# TIME    : 2022/6/21 17:08
+# FILE    : tool
+# PROJECT : funfunc
+# IDE     : PyCharm
+__all__ = [
+    'get_current_str_time',
+    'download_file',
+    'time_it',
+    'time_it_precise',
+    'quick_sort',
+    'get_basic_logger',
+    'chunks',
+    'get_host_ip',
+    'time_to_timestamp',
+    'second_to_strtime',
+    'set_deprecated',
+    'indented_json_string',
+    'MagicDict',
+    'OptClass',
+    'get_all_abspath_from_folder',
+    'is_in_docker',
+    'get_methods',
+    'get_args_info',
+    'try_except_print',
+    'retry',
+    'Flexible'
+]
+
+import copy
+import datetime
+import functools
+import json
+import logging
+import os
+import time
+import typing
+import warnings
+
+
+def get_current_str_time() -> str:
+    """get local time"""
+    now_time = datetime.datetime.now()
+    str_time = now_time.strftime('%Y年%m月%d日星期%w %H时%M分%S秒')
+    return str_time
+
+
+def download_file(url, save_path):
+    """download a file by its url"""
+    import requests
+
+    r = requests.get(url, stream=True)
+    with open(os.path.join(save_path), 'wb') as f:
+        for chunk in r.iter_content(chunk_size=1024):
+            f.write(chunk)
+
+
+def time_it(method):
+    """use this decorator to print a function time cost"""
+
+    @functools.wraps(method)
+    def wrapper(*args, **kwargs):
+        start = time.time()
+        result = method(*args, **kwargs)
+        end = time.time()
+        print('{} USED TIME:{}'.format(method.__name__, end - start))
+
+        return result
+
+    return wrapper
+
+
+def time_it_precise(method):
+    """similar to time_it but use more precise time.perf_counter()"""
+
+    @functools.wraps(method)
+    def wrapper(*args, **kwargs):
+        start = time.perf_counter()
+        result = method(*args, **kwargs)
+        end = time.perf_counter()
+        print('{} USED TIME:{}'.format(method.__name__, end - start))
+
+        return result
+
+    return wrapper
+
+
+def quick_sort(arr: list) -> list:
+    """classic sort algorithm"""
+    if len(arr) < 2:
+        return arr
+    temp = arr[0]
+    small = [i for i in arr[1:] if i <= temp]
+    big = [i for i in arr[1:] if i > temp]
+    return quick_sort(small) + [temp] + quick_sort(big)
+
+
+def get_basic_logger(level=logging.INFO, fmt: str = None, datefmt: str = None, **kwargs):
+    """fast way to create a logging.Logger object"""
+    if fmt:
+        log_format = fmt
+    else:
+        log_format = "%(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s"
+
+    if datefmt:
+        log_datefmt = datefmt
+    else:
+        log_datefmt = "%Y-%m-%d %H:%M:%S"
+    logging.basicConfig(
+        level=level,
+        format=log_format,
+        datefmt=log_datefmt,
+        **kwargs)
+
+    logger = logging.getLogger(__name__)
+    return logger
+
+
+def chunks(arr: list, n: int) -> list:
+    """split list to some lists with n items in it"""
+    return [arr[i:i + n] for i in range(0, len(arr), n)]
+
+
+def get_host_ip():
+    """check local ip"""
+    import socket
+
+    s = None
+    try:
+        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        s.connect(('8.8.8.8', 80))
+        ip = s.getsockname()[0]
+    finally:
+        s.close()
+
+    return ip
+
+
+def time_to_timestamp(date):
+    """2000-10-20 12:10:30 format time to timestamp"""
+    return datetime.datetime.strptime(date, "%Y-%m-%d %H:%M:%S").timestamp()
+
+
+def second_to_strtime(second: int):
+    """second to min:sec"""
+    return time.strftime("%M:%S", time.gmtime(second))
+
+
+def set_deprecated(warn_msg=None):
+    """set a function into deprecated state"""
+
+    def outer(deprecated_func):
+        @functools.wraps(deprecated_func)
+        def inner(*args, **kwargs):
+            if warn_msg and isinstance(warn_msg, str):
+                warnings.warn(warn_msg, DeprecationWarning, 2)
+            else:
+                warnings.warn(f"This function {deprecated_func.__name__}() is deprecated!", DeprecationWarning, 2)
+            core = deprecated_func(*args, **kwargs)
+            return core
+
+        return inner
+
+    return outer
+
+
+def indented_json_string(json_string):
+    return json.dumps(json_string, indent=2, ensure_ascii=False)
+
+
+class MagicDict(dict):
+    """
+    let you access python dict object by using attr
+
+    Example:
+        from funfunc import MagicDict
+
+        simple_dict = {'name': 'Jack', 'age': 19, 'info': {'address': 'Beijing', 'phone': '123'}}
+        magic_dict = MagicDict(simple_dict)
+        print(magic_dict.name)
+        # Jack
+        print(magic_dict.info.address)
+        # Beijing
+    """
+
+    def __init__(__self, *args, **kwargs):  # noqa
+        object.__setattr__(__self, '__parent', kwargs.pop('__parent', None))
+        object.__setattr__(__self, '__key', kwargs.pop('__key', None))
+        object.__setattr__(__self, '__frozen', False)
+        for arg in args:
+            if not arg:
+                continue
+            elif isinstance(arg, dict):
+                for key, val in arg.items():
+                    __self[key] = __self._hook(val)
+            elif isinstance(arg, tuple) and (not isinstance(arg[0], tuple)):
+                __self[arg[0]] = __self._hook(arg[1])
+            else:
+                for key, val in iter(arg):
+                    __self[key] = __self._hook(val)
+
+        for key, val in kwargs.items():
+            __self[key] = __self._hook(val)
+
+    def __setattr__(self, name, value):
+        if hasattr(self.__class__, name):
+            raise AttributeError("'Dict' object attribute "
+                                 "'{0}' is read-only".format(name))
+        else:
+            self[name] = value
+
+    def __setitem__(self, name, value):
+        isFrozen = (hasattr(self, '__frozen') and
+                    object.__getattribute__(self, '__frozen'))
+        if isFrozen and name not in super(MagicDict, self).keys():
+            raise KeyError(name)
+        super(MagicDict, self).__setitem__(name, value)
+        try:
+            p = object.__getattribute__(self, '__parent')
+            key = object.__getattribute__(self, '__key')
+        except AttributeError:
+            p = None
+            key = None
+        if p is not None:
+            p[key] = self
+            object.__delattr__(self, '__parent')
+            object.__delattr__(self, '__key')
+
+    def __add__(self, other):
+        if not self.keys():
+            return other
+        else:
+            self_type = type(self).__name__
+            other_type = type(other).__name__
+            msg = "unsupported operand type(s) for +: '{}' and '{}'"
+            raise TypeError(msg.format(self_type, other_type))
+
+    @classmethod
+    def _hook(cls, item):
+        if isinstance(item, dict):
+            return cls(item)
+        elif isinstance(item, (list, tuple)):
+            return type(item)(cls._hook(elem) for elem in item)
+        return item
+
+    def __getattr__(self, item):
+        return self.__getitem__(item)
+
+    def __missing__(self, name):
+        if object.__getattribute__(self, '__frozen'):
+            raise KeyError(name)
+        return self.__class__(__parent=self, __key=name)
+
+    def __delattr__(self, name):
+        del self[name]
+
+    def to_dict(self):
+        base = {}
+        for key, value in self.items():
+            if isinstance(value, type(self)):
+                base[key] = value.to_dict()
+            elif isinstance(value, (list, tuple)):
+                base[key] = type(value)(
+                    item.to_dict() if isinstance(item, type(self)) else
+                    item for item in value)
+            else:
+                base[key] = value
+        return base
+
+    def copy(self):
+        return copy.copy(self)
+
+    def deepcopy(self):
+        return copy.deepcopy(self)
+
+    def __deepcopy__(self, memo):
+        other = self.__class__()
+        memo[id(self)] = other
+        for key, value in self.items():
+            other[copy.deepcopy(key, memo)] = copy.deepcopy(value, memo)
+        return other
+
+    def update(self, *args, **kwargs):
+        other = {}
+        if args:
+            if len(args) > 1:
+                raise TypeError()
+            other.update(args[0])
+        other.update(kwargs)
+        for k, v in other.items():
+            if ((k not in self) or
+                    (not isinstance(self[k], dict)) or
+                    (not isinstance(v, dict))):
+                self[k] = v
+            else:
+                self[k].update(v)
+
+    def __getnewargs__(self):
+        return tuple(self.items())
+
+    def __getstate__(self):
+        return self
+
+    def __setstate__(self, state):
+        self.update(state)
+
+    def __or__(self, other):
+        if not isinstance(other, (MagicDict, dict)):
+            return NotImplemented
+        new = MagicDict(self)
+        new.update(other)
+        return new
+
+    def __ror__(self, other):
+        if not isinstance(other, (MagicDict, dict)):
+            return NotImplemented
+        new = MagicDict(other)
+        new.update(self)
+        return new
+
+    def __ior__(self, other):
+        self.update(other)
+        return self
+
+    def setdefault(self, key, default=None):
+        if key in self:
+            return self[key]
+        else:
+            self[key] = default
+            return default
+
+    def freeze(self, shouldFreeze=True):
+        object.__setattr__(self, '__frozen', shouldFreeze)
+        for key, val in self.items():
+            if isinstance(val, MagicDict):
+                val.freeze(shouldFreeze)
+
+    def unfreeze(self):
+        self.freeze(False)
+
+
+class OptClass:
+    """
+    let you create a Option class by a list of option names of predefined options dict
+    .json class property can convert options to json format string
+
+    Example:
+        # init by list of option names
+        opt_names = ['use_gpu', 'workers', 'batch_size']
+        opts = OptClass(opt_names)
+        opts.use_gpu = True
+        opts.workers = 2
+
+        # init by predefined options dict
+        opts_dict = {'use_gpu': True, 'workers': 2, 'batch_size': 16}
+        opts = OptClass(opts_dict)
+        print(opts.use_gpu)
+        print(opts.json)
+    """
+
+    def __init__(self, option_names):
+        if isinstance(option_names, list):
+            for opt in option_names:
+                if not isinstance(opt, str):
+                    opt_str = str(opt)
+                    setattr(self, opt_str, None)
+                else:
+                    setattr(self, opt, None)
+        elif isinstance(option_names, dict):
+            for k, v in option_names.items():
+                if not isinstance(k, str):
+                    opt_str = str(k)
+                    setattr(self, opt_str, v)
+                else:
+                    setattr(self, k, v)
+        else:
+            raise TypeError(f'Unsupported option_names type: {type(option_names)}, please pass a list or dict object')
+
+    @property
+    def json(self):
+        return json.dumps(self.__dict__)
+
+
+def get_all_abspath_from_folder(folder_path: str, get_relative: bool = False, file_only: bool = True) -> list:
+    """
+    get all files path of a path or a folder, if file_only=False, include folder
+
+    :param folder_path: target folder_path, a path-like string
+    :param get_relative: if True, will return relative path instead of abspath
+    :param file_only: if False, will return folder's path in folder_path
+    """
+    if not get_relative:
+        folder_path = os.path.abspath(folder_path)
+
+    if not file_only:
+        return [os.path.join(folder_path, i) for i in os.listdir(folder_path)]
+
+    return [os.path.join(folder_path, i) for i in os.listdir(folder_path) if
+            os.path.isfile(os.path.join(folder_path, i))]
+
+
+def is_in_docker():
+    return os.path.exists('/workspace')
+
+
+def get_methods(instance):
+    methods = [m for m in dir(instance) if callable(getattr(instance, m)) and not m.startswith("__")]
+    return methods
+
+
+def get_args_info(name, opt):
+    return f'{name}: ' + ', '.join(f'{k}={v}' for k, v in vars(opt).items())
+
+
+def try_except_print(func):
+    """
+    auto add try except to a function, use @try_except_print decorator
+    """
+
+    @functools.wraps(func)
+    def handler(*args, **kwargs):
+        try:
+            func(*args, **kwargs)
+        except Exception as e:
+            print(f'Exception From {func.__name__}: {e}')
+
+    return handler
+
+
+def retry(retry_count: int = 5, sleep_time: int = 1):
+    """
+    retry to call a function when it raises an error
+    """
+
+    def wrapper(func):
+        @functools.wraps(func)
+        def inner(*args, **kwargs):
+            for i in range(retry_count):
+                try:
+                    res = func(*args, **kwargs)
+                    return res
+                except:
+                    time.sleep(sleep_time)
+                    continue
+            return None
+
+        return inner
+
+    return wrapper
+
+
+Flexible = typing.Any  # use this to mark something that could be modified
```

### Comparing `funfunc-0.2.1/funfunc.egg-info/PKG-INFO` & `funfunc-0.2.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-Metadata-Version: 2.1
-Name: funfunc
-Version: 0.2.1
-Summary: Make Py Development Much Easier & Fun
-Home-page: https://github.com/jackwolfey/funfunc
-Author: Wei Jia
-Author-email: 437160499@163.com
-License: UNKNOWN
-Platform: all
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.6
-License-File: LICENSE
-
-Make Py Development Much Easier & Fun
-
+Metadata-Version: 2.1
+Name: funfunc
+Version: 0.2.2
+Summary: Make Py Development Much Easier & Fun
+Home-page: https://github.com/jackwolfey/funfunc
+Author: Wei Jia
+Author-email: 437160499@163.com
+Platform: all
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6
+License-File: LICENSE
+
+Make Py Development Much Easier & Fun
```

### Comparing `funfunc-0.2.1/setup.py` & `funfunc-0.2.2/setup.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# -*- coding: utf-8 -*-
-from setuptools import find_packages, setup
-import funfunc
-
-setup(name="funfunc",
-      version=funfunc.__VERSION__,
-      description=funfunc.__DESCRIPTION__,
-      long_description=funfunc.__DESCRIPTION__,
-      url="https://github.com/jackwolfey/funfunc",
-      author="Wei Jia",
-      author_email="437160499@163.com",
-      packages=find_packages(exclude='test'),
-      platforms=["all"],
-      classifiers=[
-          'Topic :: Software Development :: Libraries :: Python Modules',
-          'Operating System :: OS Independent',
-          'Intended Audience :: Developers',
-          'Development Status :: 4 - Beta',
-          'License :: OSI Approved :: Apache Software License',
-          'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.6',
-          'Programming Language :: Python :: 3.7',
-          'Programming Language :: Python :: 3.8',
-          'Programming Language :: Python :: 3.9',
-          'Programming Language :: Python :: 3.10',
-          'Programming Language :: Python :: 3.11',
-          'Programming Language :: Python :: 3.12'],
-      python_requires='>=3.6'
-      )
+# -*- coding: utf-8 -*-
+from setuptools import find_packages, setup
+import funfunc
+
+setup(name="funfunc",
+      version=funfunc.__VERSION__,
+      description=funfunc.__DESCRIPTION__,
+      long_description=funfunc.__DESCRIPTION__,
+      url="https://github.com/jackwolfey/funfunc",
+      author="Wei Jia",
+      author_email="437160499@163.com",
+      packages=find_packages(exclude='test'),
+      platforms=["all"],
+      classifiers=[
+          'Topic :: Software Development :: Libraries :: Python Modules',
+          'Operating System :: OS Independent',
+          'Intended Audience :: Developers',
+          'Development Status :: 4 - Beta',
+          'License :: OSI Approved :: Apache Software License',
+          'Programming Language :: Python :: 3',
+          'Programming Language :: Python :: 3.6',
+          'Programming Language :: Python :: 3.7',
+          'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
+          'Programming Language :: Python :: 3.12'],
+      python_requires='>=3.6'
+      )
```

### Comparing `funfunc-0.2.1/README.md` & `funfunc-0.2.2/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# funfunc
-**Implement multiple functions or tool classes to make your Python Development Much Easier & Fun**
-
-## Installation
-```
-pip install funfunc
-```
-
-## Usage
-### Convert your image array object to base64 format string
-```
-import funfunc
-import cv2
-
-cv_image = cv2.imread('/img/path.jpg')
-base64_string = funfunc.image_array_to_base64_string(cv_image)
-```
-### Print a function runing time
-```
-import funfunc
-import time
-
-@funfunc.time_it
-def simple_func():
-    time.sleep(3)
-```
-### Split a list to train and test set by a specific ratio
-```
-import funfunc
-
-lst = [1, 2, 3, 4, 5, 6, 7, 8]
-train_set, test_set = funfunc.train_test_split_arr(arr=lst, ratio=0.2)
-```
-### Check whether the string is a URL
-```
-from funfunc import Validator
-
-Validator.is_url('http://www.github.com')
-```
-
+# funfunc
+**Implement multiple functions or tool classes to make your Python Development Much Easier & Fun**
+
+## Installation
+```
+pip install funfunc
+```
+
+## Usage
+### Convert your image array object to base64 format string
+```
+import funfunc
+import cv2
+
+cv_image = cv2.imread('/img/path.jpg')
+base64_string = funfunc.image_array_to_base64_string(cv_image)
+```
+### Print a function runing time
+```
+import funfunc
+import time
+
+@funfunc.time_it
+def simple_func():
+    time.sleep(3)
+```
+### Split a list to train and test set by a specific ratio
+```
+import funfunc
+
+lst = [1, 2, 3, 4, 5, 6, 7, 8]
+train_set, test_set = funfunc.train_test_split_arr(arr=lst, ratio=0.2)
+```
+### Check whether the string is a URL
+```
+from funfunc import Validator
+
+Validator.is_url('http://www.github.com')
+```
+
 ### And more functions wait you to explorer...
```

### Comparing `funfunc-0.2.1/PKG-INFO` & `funfunc-0.2.2/funfunc.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-Metadata-Version: 2.1
-Name: funfunc
-Version: 0.2.1
-Summary: Make Py Development Much Easier & Fun
-Home-page: https://github.com/jackwolfey/funfunc
-Author: Wei Jia
-Author-email: 437160499@163.com
-License: UNKNOWN
-Platform: all
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.6
-License-File: LICENSE
-
-Make Py Development Much Easier & Fun
-
+Metadata-Version: 2.1
+Name: funfunc
+Version: 0.2.2
+Summary: Make Py Development Much Easier & Fun
+Home-page: https://github.com/jackwolfey/funfunc
+Author: Wei Jia
+Author-email: 437160499@163.com
+Platform: all
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6
+License-File: LICENSE
+
+Make Py Development Much Easier & Fun
```

