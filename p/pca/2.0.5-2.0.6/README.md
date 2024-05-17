# Comparing `tmp/pca-2.0.5.tar.gz` & `tmp/pca-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pca-2.0.5.tar", last modified: Fri Aug 25 09:44:18 2023, max compression
+gzip compressed data, was "pca-2.0.6.tar", last modified: Fri May 17 15:25:24 2024, max compression
```

## Comparing `pca-2.0.5.tar` & `pca-2.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-25 09:44:18.587164 pca-2.0.5/
--rw-rw-rw-   0        0        0     1094 2022-05-07 12:53:27.000000 pca-2.0.5/LICENSE
--rw-rw-rw-   0        0        0      100 2022-05-07 12:53:27.000000 pca-2.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    10335 2023-08-25 09:44:18.586166 pca-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     9811 2023-05-28 19:59:46.000000 pca-2.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-25 09:44:18.530357 pca-2.0.5/pca/
--rw-rw-rw-   0        0        0     1246 2023-08-25 09:29:01.000000 pca-2.0.5/pca/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-25 09:44:18.578187 pca-2.0.5/pca/data/
--rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.5/pca/data/__init__.py
--rw-rw-rw-   0        0        0    34117 2023-08-25 09:37:37.000000 pca-2.0.5/pca/examples.py
--rw-rw-rw-   0        0        0    78781 2023-08-25 09:26:09.000000 pca-2.0.5/pca/pca.py
-drwxrwxrwx   0        0        0        0 2023-08-25 09:44:18.584172 pca-2.0.5/pca/tests/
--rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.5/pca/tests/__init__.py
--rw-rw-rw-   0        0        0    10683 2023-05-31 19:00:16.000000 pca-2.0.5/pca/tests/test_pca.py
-drwxrwxrwx   0        0        0        0 2023-08-25 09:44:18.576192 pca-2.0.5/pca.egg-info/
--rw-rw-rw-   0        0        0    10335 2023-08-25 09:44:18.000000 pca-2.0.5/pca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-08-25 09:44:18.000000 pca-2.0.5/pca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-25 09:44:18.000000 pca-2.0.5/pca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-08-25 09:44:18.000000 pca-2.0.5/pca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-25 09:44:18.000000 pca-2.0.5/pca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-25 09:44:18.588162 pca-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1700 2023-08-25 09:30:28.000000 pca-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:25:24.528645 pca-2.0.6/
+-rw-rw-rw-   0        0        0     1094 2024-03-06 18:53:46.000000 pca-2.0.6/LICENSE
+-rw-rw-rw-   0        0        0      100 2024-03-06 18:53:46.000000 pca-2.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    10738 2024-05-17 15:25:24.528137 pca-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9945 2024-05-17 15:23:58.000000 pca-2.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 15:25:24.488254 pca-2.0.6/pca/
+-rw-rw-rw-   0        0        0     1246 2024-05-17 15:24:20.000000 pca-2.0.6/pca/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:25:24.510693 pca-2.0.6/pca/data/
+-rw-rw-rw-   0        0        0        0 2024-03-06 18:53:47.000000 pca-2.0.6/pca/data/__init__.py
+-rw-rw-rw-   0        0        0    34990 2024-05-17 15:23:09.000000 pca-2.0.6/pca/examples.py
+-rw-rw-rw-   0        0        0    78857 2024-05-17 15:20:09.000000 pca-2.0.6/pca/pca.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:25:24.510693 pca-2.0.6/pca/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-06 18:53:47.000000 pca-2.0.6/pca/tests/__init__.py
+-rw-rw-rw-   0        0        0    10683 2024-03-06 18:53:47.000000 pca-2.0.6/pca/tests/test_pca.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:25:24.510693 pca-2.0.6/pca.egg-info/
+-rw-rw-rw-   0        0        0    10738 2024-05-17 15:25:24.000000 pca-2.0.6/pca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-17 15:25:24.000000 pca-2.0.6/pca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:25:24.000000 pca-2.0.6/pca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-05-17 15:25:24.000000 pca-2.0.6/pca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-17 15:25:24.000000 pca-2.0.6/pca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:25:24.528645 pca-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1717 2024-03-06 19:13:59.000000 pca-2.0.6/setup.py
```

### Comparing `pca-2.0.5/LICENSE` & `pca-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pca-2.0.5/PKG-INFO` & `pca-2.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pca
-Version: 2.0.5
-Summary: pca: A Python Package for Principal Component Analysis.
-Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.5.tar.gz
-Author: Erdogan Taskesen
-Author-email: erdogant@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 <p align="center">
   <a href="https://erdogant.github.io/pca/">
   <img src="https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png" width="600" />
   </a>
 </p>
 
@@ -37,49 +22,48 @@
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg?logo=github%20sponsors)](https://erdogant.github.io/pca/pages/html/Documentation.html#colab-notebook)
 ![GitHub repo size](https://img.shields.io/github/repo-size/erdogant/pca)
 [![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://erdogant.github.io/pca/pages/html/Documentation.html#)
 <!---[![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)-->
 <!---[![Coffee](https://img.shields.io/badge/coffee-black-grey.svg)](https://erdogant.github.io/donate/?currency=USD&amount=5)-->
 
 **pca** A Python Package for Principal Component Analysis. The core of PCA is build on sklearn functionality to find maximum compatibility when combining with other packages.
-But this package can do a lot more. Besides the regular pca, it can also perform **SparsePCA**, and **TruncatedSVD**. Depending on your input data, the best approach will be choosen.
+But this package can do a lot more. Besides the regular pca, it can also perform **SparsePCA**, and **TruncatedSVD**. Depending on your input data, the best approach will be chosen.
+**⭐️ Star this repo if you like it ⭐️**
+
 
 Other functionalities of PCA are:
 
   * **Biplot** to plot the loadings
   * Determine the **explained variance** 
   * Extract the best performing **features**
   * Scatter plot with the **loadings**
   * Outlier detection using **Hotelling T2 and/or SPE/Dmodx**
 
----
 
-**⭐️ Star this repo if you like it ⭐️**
+## Support
 
----
+Your ❤️ is important to keep maintaining my packages. You can support in various ways, have a look at the [sponser page](https://erdogant.github.io/pca/pages/html/Documentation.html). Report bugs, issues or help out with developing new features! If you don't have the time to help or are still learning, you can also take a [Medium Mebership using my referral link](https://erdogant.medium.com/) to keep reading all my hands-on blogs. If you also don't need that, there is always the coffee! Thank you! 
+<a href='https://www.buymeacoffee.com/erdogant' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi1.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
 
-## Read the Medium blog for more details.
+
+### Read the Medium blog for more details.
 
 #### [1. What are PCA loadings and how to effectively use Biplots?](https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559)
 
 #### [2. Outlier Detection Using Principal Component Analysis and Hotelling’s T2 and SPE/DmodX Methods](https://towardsdatascience.com/outlier-detection-using-principal-component-analysis-and-hotellings-t2-and-spe-dmodx-methods-625b3c90897)
 
 #### [3. Quantitative comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https://towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-mappings-c6453b80f303)
 
 
-#
-
-
----
 
 ## [Documentation pages](https://erdogant.github.io/pca/)
 
 On the [documentation pages](https://erdogant.github.io/pca/) you can find detailed information about the working of the ``pca`` with many examples. 
 
----
+
 
 ## Installation
 
 ```bash
 pip install pca
 ```
 
@@ -230,13 +214,7 @@
 #### Citation
 Please cite in your publications if this is useful for your research (see citation).
 
 ### Maintainers
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 
 ---
-
-## Support
-
-Your ❤️ is important to keep maintaining this package. You can [support](https://erdogant.github.io/pca/pages/html/Documentation.html) in various ways, have a look at the [sponser page](https://erdogant.github.io/pca/pages/html/Documentation.html). Report bugs, issues and feature extensions at [github page](https://github.com/erdogant/pca).
-
-<a href='https://www.buymeacoffee.com/erdogant' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi1.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
```

#### html2text {}

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1 Name: pca Version: 2.0.5 Summary: pca: A Python Package
-for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.5.tar.gz Author:
-Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE
    _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/_m_a_s_t_e_r_/_d_o_c_s_/_f_i_g_s_/_i_r_i_s___d_e_n_s_i_t_y_._p_n_g_]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
 pypi.org/project/pca/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-
 Green)](https://erdogant.github.io/pca/) [![LOC](https://sloc.xyz/github/
 erdogant/pca/?category=code)](https://github.com/erdogant/pca/) [![Downloads]
 (https://static.pepy.tech/personalized-badge/
@@ -31,32 +24,39 @@
 [GitHub repo size](https://img.shields.io/github/repo-size/erdogant/pca) [!
 [Donate](https://img.shields.io/badge/Support%20this%20project-
 grey.svg?logo=github%20sponsors)](https://erdogant.github.io/pca/pages/html/
 Documentation.html#) **pca** A Python Package for Principal Component Analysis.
 The core of PCA is build on sklearn functionality to find maximum compatibility
 when combining with other packages. But this package can do a lot more. Besides
 the regular pca, it can also perform **SparsePCA**, and **TruncatedSVD**.
-Depending on your input data, the best approach will be choosen. Other
-functionalities of PCA are: * **Biplot** to plot the loadings * Determine the
-**explained variance** * Extract the best performing **features** * Scatter
-plot with the **loadings** * Outlier detection using **Hotelling T2 and/or SPE/
-Dmodx** --- **â­ï¸ Star this repo if you like it â­ï¸** --- ## Read the
-Medium blog for more details. #### [1. What are PCA loadings and how to
-effectively use Biplots?](https://towardsdatascience.com/what-are-pca-loadings-
-and-biplots-9a7897f2e559) #### [2. Outlier Detection Using Principal Component
-Analysis and Hotellingâs T2 and SPE/DmodX Methods](https://
-towardsdatascience.com/outlier-detection-using-principal-component-analysis-
-and-hotellings-t2-and-spe-dmodx-methods-625b3c90897) #### [3. Quantitative
-comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https://
-towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-
-mappings-c6453b80f303) # --- ## [Documentation pages](https://
-erdogant.github.io/pca/) On the [documentation pages](https://
-erdogant.github.io/pca/) you can find detailed information about the working of
-the ``pca`` with many examples. --- ## Installation ```bash pip install pca ```
-##### Import pca package ```python from pca import pca ``` #
+Depending on your input data, the best approach will be chosen. **â­ï¸ Star
+this repo if you like it â­ï¸** Other functionalities of PCA are: *
+**Biplot** to plot the loadings * Determine the **explained variance** *
+Extract the best performing **features** * Scatter plot with the **loadings** *
+Outlier detection using **Hotelling T2 and/or SPE/Dmodx** ## Support Your
+â¤ï¸ is important to keep maintaining my packages. You can support in various
+ways, have a look at the [sponser page](https://erdogant.github.io/pca/pages/
+html/Documentation.html). Report bugs, issues or help out with developing new
+features! If you don't have the time to help or are still learning, you can
+also take a [Medium Mebership using my referral link](https://
+erdogant.medium.com/) to keep reading all my hands-on blogs. If you also don't
+need that, there is always the coffee! Thank you! _[_B_u_y_ _M_e_ _a_ _C_o_f_f_e_e_ _a_t_ _k_o_-
+_f_i_._c_o_m_]### Read the Medium blog for more details. #### [1. What are PCA
+loadings and how to effectively use Biplots?](https://towardsdatascience.com/
+what-are-pca-loadings-and-biplots-9a7897f2e559) #### [2. Outlier Detection
+Using Principal Component Analysis and Hotellingâs T2 and SPE/DmodX Methods]
+(https://towardsdatascience.com/outlier-detection-using-principal-component-
+analysis-and-hotellings-t2-and-spe-dmodx-methods-625b3c90897) #### [3.
+Quantitative comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https:/
+/towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-
+mappings-c6453b80f303) ## [Documentation pages](https://erdogant.github.io/pca/
+) On the [documentation pages](https://erdogant.github.io/pca/) you can find
+detailed information about the working of the ``pca`` with many examples. ##
+Installation ```bash pip install pca ``` ##### Import pca package ```python
+from pca import pca ``` #
 _QQ_uu_ii_cc_kk_ _ss_tt_aa_rr_tt                            _MM_aa_kk_ee_ _bb_ii_pp_ll_oo_tt
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/ _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/
 _m_a_s_t_e_r_/_d_o_c_s_/_f_i_g_s_/                      _m_a_s_t_e_r_/_d_o_c_s_/_f_i_g_s_/
 _f_i_g___s_c_a_t_t_e_r_._p_n_g_?_r_a_w_=_t_r_u_e_]              _c_u_s_t_o_m___e_x_a_m_p_l_e___2_._p_n_g_?_r_a_w_=_t_r_u_e_]
 #
 _PP_ll_oo_tt_ _EE_xx_pp_ll_aa_ii_nn_ee_dd_ _vv_aa_rr_ii_aa_nn_cc_ee                _33_DD_ _pp_ll_oo_tt_ss
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/ _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/
@@ -101,13 +101,8 @@
 visible status](https://erdogant.github.io/pca/pages/html/Plots.html#toggle-
 visible-status) # * [Example: Map unseen (new) datapoint to the transfomred
 space](https://erdogant.github.io/pca/pages/html/Examples.html#map-unseen-
 datapoints-into-fitted-space)
 ===============================================================================
 #### Citation Please cite in your publications if this is useful for your
 research (see citation). ### Maintainers * Erdogan Taskesen, github: [erdogant]
-(https://github.com/erdogant) --- ## Support Your â¤ï¸ is important to keep
-maintaining this package. You can [support](https://erdogant.github.io/pca/
-pages/html/Documentation.html) in various ways, have a look at the [sponser
-page](https://erdogant.github.io/pca/pages/html/Documentation.html). Report
-bugs, issues and feature extensions at [github page](https://github.com/
-erdogant/pca)._[_B_u_y_ _M_e_ _a_ _C_o_f_f_e_e_ _a_t_ _k_o_-_f_i_._c_o_m_]
+(https://github.com/erdogant) ---
```

### Comparing `pca-2.0.5/README.md` & `pca-2.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: pca
+Version: 2.0.6
+Summary: pca: A Python Package for Principal Component Analysis.
+Home-page: https://erdogant.github.io/pca
+Download-URL: https://github.com/erdogant/pca/archive/2.0.6.tar.gz
+Author: Erdogan Taskesen
+Author-email: erdogant@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: datazets
+Requires-Dist: statsmodels
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: colourmap>=1.1.15
+Requires-Dist: pandas
+Requires-Dist: scatterd>=1.3.7
+Requires-Dist: adjusttext
+
 
 <p align="center">
   <a href="https://erdogant.github.io/pca/">
   <img src="https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png" width="600" />
   </a>
 </p>
 
@@ -22,49 +47,48 @@
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg?logo=github%20sponsors)](https://erdogant.github.io/pca/pages/html/Documentation.html#colab-notebook)
 ![GitHub repo size](https://img.shields.io/github/repo-size/erdogant/pca)
 [![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://erdogant.github.io/pca/pages/html/Documentation.html#)
 <!---[![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)-->
 <!---[![Coffee](https://img.shields.io/badge/coffee-black-grey.svg)](https://erdogant.github.io/donate/?currency=USD&amount=5)-->
 
 **pca** A Python Package for Principal Component Analysis. The core of PCA is build on sklearn functionality to find maximum compatibility when combining with other packages.
-But this package can do a lot more. Besides the regular pca, it can also perform **SparsePCA**, and **TruncatedSVD**. Depending on your input data, the best approach will be choosen.
+But this package can do a lot more. Besides the regular pca, it can also perform **SparsePCA**, and **TruncatedSVD**. Depending on your input data, the best approach will be chosen.
+**⭐️ Star this repo if you like it ⭐️**
+
 
 Other functionalities of PCA are:
 
   * **Biplot** to plot the loadings
   * Determine the **explained variance** 
   * Extract the best performing **features**
   * Scatter plot with the **loadings**
   * Outlier detection using **Hotelling T2 and/or SPE/Dmodx**
 
----
 
-**⭐️ Star this repo if you like it ⭐️**
+## Support
 
----
+Your ❤️ is important to keep maintaining my packages. You can support in various ways, have a look at the [sponser page](https://erdogant.github.io/pca/pages/html/Documentation.html). Report bugs, issues or help out with developing new features! If you don't have the time to help or are still learning, you can also take a [Medium Mebership using my referral link](https://erdogant.medium.com/) to keep reading all my hands-on blogs. If you also don't need that, there is always the coffee! Thank you! 
+<a href='https://www.buymeacoffee.com/erdogant' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi1.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
 
-## Read the Medium blog for more details.
+
+### Read the Medium blog for more details.
 
 #### [1. What are PCA loadings and how to effectively use Biplots?](https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559)
 
 #### [2. Outlier Detection Using Principal Component Analysis and Hotelling’s T2 and SPE/DmodX Methods](https://towardsdatascience.com/outlier-detection-using-principal-component-analysis-and-hotellings-t2-and-spe-dmodx-methods-625b3c90897)
 
 #### [3. Quantitative comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https://towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-mappings-c6453b80f303)
 
 
-#
-
-
----
 
 ## [Documentation pages](https://erdogant.github.io/pca/)
 
 On the [documentation pages](https://erdogant.github.io/pca/) you can find detailed information about the working of the ``pca`` with many examples. 
 
----
+
 
 ## Installation
 
 ```bash
 pip install pca
 ```
 
@@ -215,13 +239,7 @@
 #### Citation
 Please cite in your publications if this is useful for your research (see citation).
 
 ### Maintainers
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 
 ---
-
-## Support
-
-Your ❤️ is important to keep maintaining this package. You can [support](https://erdogant.github.io/pca/pages/html/Documentation.html) in various ways, have a look at the [sponser page](https://erdogant.github.io/pca/pages/html/Documentation.html). Report bugs, issues and feature extensions at [github page](https://github.com/erdogant/pca).
-
-<a href='https://www.buymeacoffee.com/erdogant' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi1.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
```

#### html2text {}

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1 Name: pca Version: 2.0.6 Summary: pca: A Python Package
+for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
+Download-URL: https://github.com/erdogant/pca/archive/2.0.6.tar.gz Author:
+Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+datazets Requires-Dist: statsmodels Requires-Dist: matplotlib Requires-Dist:
+numpy Requires-Dist: scikit-learn Requires-Dist: scipy Requires-Dist:
+colourmap>=1.1.15 Requires-Dist: pandas Requires-Dist: scatterd>=1.3.7
+Requires-Dist: adjusttext
    _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/_m_a_s_t_e_r_/_d_o_c_s_/_f_i_g_s_/_i_r_i_s___d_e_n_s_i_t_y_._p_n_g_]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
 pypi.org/project/pca/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-
 Green)](https://erdogant.github.io/pca/) [![LOC](https://sloc.xyz/github/
 erdogant/pca/?category=code)](https://github.com/erdogant/pca/) [![Downloads]
 (https://static.pepy.tech/personalized-badge/
@@ -24,32 +35,39 @@
 [GitHub repo size](https://img.shields.io/github/repo-size/erdogant/pca) [!
 [Donate](https://img.shields.io/badge/Support%20this%20project-
 grey.svg?logo=github%20sponsors)](https://erdogant.github.io/pca/pages/html/
 Documentation.html#) **pca** A Python Package for Principal Component Analysis.
 The core of PCA is build on sklearn functionality to find maximum compatibility
 when combining with other packages. But this package can do a lot more. Besides
 the regular pca, it can also perform **SparsePCA**, and **TruncatedSVD**.
-Depending on your input data, the best approach will be choosen. Other
-functionalities of PCA are: * **Biplot** to plot the loadings * Determine the
-**explained variance** * Extract the best performing **features** * Scatter
-plot with the **loadings** * Outlier detection using **Hotelling T2 and/or SPE/
-Dmodx** --- **â­ï¸ Star this repo if you like it â­ï¸** --- ## Read the
-Medium blog for more details. #### [1. What are PCA loadings and how to
-effectively use Biplots?](https://towardsdatascience.com/what-are-pca-loadings-
-and-biplots-9a7897f2e559) #### [2. Outlier Detection Using Principal Component
-Analysis and Hotellingâs T2 and SPE/DmodX Methods](https://
-towardsdatascience.com/outlier-detection-using-principal-component-analysis-
-and-hotellings-t2-and-spe-dmodx-methods-625b3c90897) #### [3. Quantitative
-comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https://
-towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-
-mappings-c6453b80f303) # --- ## [Documentation pages](https://
-erdogant.github.io/pca/) On the [documentation pages](https://
-erdogant.github.io/pca/) you can find detailed information about the working of
-the ``pca`` with many examples. --- ## Installation ```bash pip install pca ```
-##### Import pca package ```python from pca import pca ``` #
+Depending on your input data, the best approach will be chosen. **â­ï¸ Star
+this repo if you like it â­ï¸** Other functionalities of PCA are: *
+**Biplot** to plot the loadings * Determine the **explained variance** *
+Extract the best performing **features** * Scatter plot with the **loadings** *
+Outlier detection using **Hotelling T2 and/or SPE/Dmodx** ## Support Your
+â¤ï¸ is important to keep maintaining my packages. You can support in various
+ways, have a look at the [sponser page](https://erdogant.github.io/pca/pages/
+html/Documentation.html). Report bugs, issues or help out with developing new
+features! If you don't have the time to help or are still learning, you can
+also take a [Medium Mebership using my referral link](https://
+erdogant.medium.com/) to keep reading all my hands-on blogs. If you also don't
+need that, there is always the coffee! Thank you! _[_B_u_y_ _M_e_ _a_ _C_o_f_f_e_e_ _a_t_ _k_o_-
+_f_i_._c_o_m_]### Read the Medium blog for more details. #### [1. What are PCA
+loadings and how to effectively use Biplots?](https://towardsdatascience.com/
+what-are-pca-loadings-and-biplots-9a7897f2e559) #### [2. Outlier Detection
+Using Principal Component Analysis and Hotellingâs T2 and SPE/DmodX Methods]
+(https://towardsdatascience.com/outlier-detection-using-principal-component-
+analysis-and-hotellings-t2-and-spe-dmodx-methods-625b3c90897) #### [3.
+Quantitative comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https:/
+/towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-
+mappings-c6453b80f303) ## [Documentation pages](https://erdogant.github.io/pca/
+) On the [documentation pages](https://erdogant.github.io/pca/) you can find
+detailed information about the working of the ``pca`` with many examples. ##
+Installation ```bash pip install pca ``` ##### Import pca package ```python
+from pca import pca ``` #
 _QQ_uu_ii_cc_kk_ _ss_tt_aa_rr_tt                            _MM_aa_kk_ee_ _bb_ii_pp_ll_oo_tt
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/ _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/
 _m_a_s_t_e_r_/_d_o_c_s_/_f_i_g_s_/                      _m_a_s_t_e_r_/_d_o_c_s_/_f_i_g_s_/
 _f_i_g___s_c_a_t_t_e_r_._p_n_g_?_r_a_w_=_t_r_u_e_]              _c_u_s_t_o_m___e_x_a_m_p_l_e___2_._p_n_g_?_r_a_w_=_t_r_u_e_]
 #
 _PP_ll_oo_tt_ _EE_xx_pp_ll_aa_ii_nn_ee_dd_ _vv_aa_rr_ii_aa_nn_cc_ee                _33_DD_ _pp_ll_oo_tt_ss
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/ _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/
@@ -94,13 +112,8 @@
 visible status](https://erdogant.github.io/pca/pages/html/Plots.html#toggle-
 visible-status) # * [Example: Map unseen (new) datapoint to the transfomred
 space](https://erdogant.github.io/pca/pages/html/Examples.html#map-unseen-
 datapoints-into-fitted-space)
 ===============================================================================
 #### Citation Please cite in your publications if this is useful for your
 research (see citation). ### Maintainers * Erdogan Taskesen, github: [erdogant]
-(https://github.com/erdogant) --- ## Support Your â¤ï¸ is important to keep
-maintaining this package. You can [support](https://erdogant.github.io/pca/
-pages/html/Documentation.html) in various ways, have a look at the [sponser
-page](https://erdogant.github.io/pca/pages/html/Documentation.html). Report
-bugs, issues and feature extensions at [github page](https://github.com/
-erdogant/pca)._[_B_u_y_ _M_e_ _a_ _C_o_f_f_e_e_ _a_t_ _k_o_-_f_i_._c_o_m_]
+(https://github.com/erdogant) ---
```

### Comparing `pca-2.0.5/pca/__init__.py` & `pca-2.0.6/pca/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     hotellingsT2,
     spe_dmodx,
     )
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.0.5'
+__version__ = '2.0.6'
 
 # module level doc-string
 __doc__ = """
 pca
 =====================================================================
 
 pca: A Python Package for Principal Component Analysis.
```

### Comparing `pca-2.0.5/pca/examples.py` & `pca-2.0.6/pca/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,42 @@
 import matplotlib as mpl
 from scatterd import scatterd
 
 import numpy as np
 from sklearn.datasets import load_iris
 import pandas as pd
 
+
+# %% issue 54
+# https://github.com/erdogant/pca/issues/54
+from pca import pca
+
+# Create dataset
+np.random.seed(42)
+X_orig = pd.DataFrame(np.random.randint(low=1, high=10, size=(10000, 10)))
+# Insert Outliers
+X_orig.iloc[500:510, 8:] = 15
+
+# PCA Training
+model = pca(n_components=5, alpha=0.05, n_std=3, normalize=True, random_state=42)
+results = model.fit_transform(X=X_orig)
+
+outliers_original = model.results['outliers']
+
+# Create New Data
+X_new = pd.DataFrame(np.random.randint(low=1, high=10, size=(1000, 10)))
+
+# Transform New Data
+model.transform(X=X_new, update_outlier_params=False)
+outliers_new = model.results['outliers']
+
+# Compare Original Points Outlier Results Before and After Transform
+print("Before:", outliers_original['y_bool'].value_counts())
+print("After:", outliers_new.iloc[:1]['y_bool'].value_counts())
+
 # %%
 # Load pca
 from pca import pca
 
 # Initialize pca
 model = pca(n_components=3)
 
@@ -29,15 +57,15 @@
 import pandas as pd
 from pca import pca
 
 # pd.options.mode.copy_on_write = True
 
 data = load_wine()
 df = pd.DataFrame(index=data.target, data=data.data, columns=data.feature_names)
-model = pca(normalize=True, detect_outliers=['ht2', 'spe'], n_std=2)
+model = pca(normalize=True, detect_outliers=['ht2', 'spe'], n_std=2, verbose='info')
 results = model.fit_transform(df)
 
 model.biplot(SPE=False, HT2=True, density=True)
 
 # %%
 # Load pca
 from pca import pca
```

### Comparing `pca-2.0.5/pca/pca.py` & `pca-2.0.6/pca/pca.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # %% Association learning across all variables
 class pca:
     """pca module.
 
     Parameters
     ----------
     n_components : [0..1] or [1..number of samples-1], (default: 0.95)
-        Number of PCs to be returned. When n_components is set >0, the specified number of PCs is returned.
+        Number of PCs to be returned. When n_components is set >=1, the specified number of PCs is returned.
         When n_components is set between [0..1], the number of PCs is returned that covers at least this percentage of variance.
         n_components=None : Return all PCs
         n_components=0.95 : Return the number of PCs that cover at least 95% of variance.
         n_components=3    : Return the top 3 PCs.
     n_feat : int, default: 10
         Number of features that explain the space the most, dervied from the loadings. This parameter is used for vizualization purposes only.
     method : 'pca' (default)
@@ -692,15 +692,17 @@
                            fontsize=fontsize,
                            fontweight=fontweight,
                            grid=grid,
                            dpi=dpi,
                            figsize=figsize,
                            visible=visible,
                            fig=fig,
-                           ax=ax)
+                           ax=ax,
+                           verbose=verbose,
+                           )
 
         # Plot the SPE with Elipse
         fig, ax = _add_plot_SPE(self, xs, ys, zs, SPE, d3, alpha, s, fig, ax)
         # Plot hotelling T2
         fig, ax = _add_plot_HT2(self, xs, ys, zs, HT2, d3, alpha, s, fig, ax)
         # Add figure properties
         fig, ax = _add_plot_properties(self, PC, d3, title, legend, labels, fig, ax, fontsize, verbose)
```

### Comparing `pca-2.0.5/pca/tests/test_pca.py` & `pca-2.0.6/pca/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `pca-2.0.5/pca.egg-info/PKG-INFO` & `pca-2.0.6/pca.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 Metadata-Version: 2.1
 Name: pca
-Version: 2.0.5
+Version: 2.0.6
 Summary: pca: A Python Package for Principal Component Analysis.
 Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.5.tar.gz
+Download-URL: https://github.com/erdogant/pca/archive/2.0.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: datazets
+Requires-Dist: statsmodels
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: colourmap>=1.1.15
+Requires-Dist: pandas
+Requires-Dist: scatterd>=1.3.7
+Requires-Dist: adjusttext
 
 
 <p align="center">
   <a href="https://erdogant.github.io/pca/">
   <img src="https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png" width="600" />
   </a>
 </p>
@@ -37,49 +47,48 @@
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg?logo=github%20sponsors)](https://erdogant.github.io/pca/pages/html/Documentation.html#colab-notebook)
 ![GitHub repo size](https://img.shields.io/github/repo-size/erdogant/pca)
 [![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://erdogant.github.io/pca/pages/html/Documentation.html#)
 <!---[![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)-->
 <!---[![Coffee](https://img.shields.io/badge/coffee-black-grey.svg)](https://erdogant.github.io/donate/?currency=USD&amount=5)-->
 
 **pca** A Python Package for Principal Component Analysis. The core of PCA is build on sklearn functionality to find maximum compatibility when combining with other packages.
-But this package can do a lot more. Besides the regular pca, it can also perform **SparsePCA**, and **TruncatedSVD**. Depending on your input data, the best approach will be choosen.
+But this package can do a lot more. Besides the regular pca, it can also perform **SparsePCA**, and **TruncatedSVD**. Depending on your input data, the best approach will be chosen.
+**⭐️ Star this repo if you like it ⭐️**
+
 
 Other functionalities of PCA are:
 
   * **Biplot** to plot the loadings
   * Determine the **explained variance** 
   * Extract the best performing **features**
   * Scatter plot with the **loadings**
   * Outlier detection using **Hotelling T2 and/or SPE/Dmodx**
 
----
 
-**⭐️ Star this repo if you like it ⭐️**
+## Support
 
----
+Your ❤️ is important to keep maintaining my packages. You can support in various ways, have a look at the [sponser page](https://erdogant.github.io/pca/pages/html/Documentation.html). Report bugs, issues or help out with developing new features! If you don't have the time to help or are still learning, you can also take a [Medium Mebership using my referral link](https://erdogant.medium.com/) to keep reading all my hands-on blogs. If you also don't need that, there is always the coffee! Thank you! 
+<a href='https://www.buymeacoffee.com/erdogant' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi1.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
 
-## Read the Medium blog for more details.
+
+### Read the Medium blog for more details.
 
 #### [1. What are PCA loadings and how to effectively use Biplots?](https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559)
 
 #### [2. Outlier Detection Using Principal Component Analysis and Hotelling’s T2 and SPE/DmodX Methods](https://towardsdatascience.com/outlier-detection-using-principal-component-analysis-and-hotellings-t2-and-spe-dmodx-methods-625b3c90897)
 
 #### [3. Quantitative comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https://towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-mappings-c6453b80f303)
 
 
-#
-
-
----
 
 ## [Documentation pages](https://erdogant.github.io/pca/)
 
 On the [documentation pages](https://erdogant.github.io/pca/) you can find detailed information about the working of the ``pca`` with many examples. 
 
----
+
 
 ## Installation
 
 ```bash
 pip install pca
 ```
 
@@ -230,13 +239,7 @@
 #### Citation
 Please cite in your publications if this is useful for your research (see citation).
 
 ### Maintainers
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 
 ---
-
-## Support
-
-Your ❤️ is important to keep maintaining this package. You can [support](https://erdogant.github.io/pca/pages/html/Documentation.html) in various ways, have a look at the [sponser page](https://erdogant.github.io/pca/pages/html/Documentation.html). Report bugs, issues and feature extensions at [github page](https://github.com/erdogant/pca).
-
-<a href='https://www.buymeacoffee.com/erdogant' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi1.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
```

#### html2text {}

```diff
@@ -1,14 +1,18 @@
-Metadata-Version: 2.1 Name: pca Version: 2.0.5 Summary: pca: A Python Package
+Metadata-Version: 2.1 Name: pca Version: 2.0.6 Summary: pca: A Python Package
 for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.5.tar.gz Author:
+Download-URL: https://github.com/erdogant/pca/archive/2.0.6.tar.gz Author:
 Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+datazets Requires-Dist: statsmodels Requires-Dist: matplotlib Requires-Dist:
+numpy Requires-Dist: scikit-learn Requires-Dist: scipy Requires-Dist:
+colourmap>=1.1.15 Requires-Dist: pandas Requires-Dist: scatterd>=1.3.7
+Requires-Dist: adjusttext
    _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/_m_a_s_t_e_r_/_d_o_c_s_/_f_i_g_s_/_i_r_i_s___d_e_n_s_i_t_y_._p_n_g_]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
 pypi.org/project/pca/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-
 Green)](https://erdogant.github.io/pca/) [![LOC](https://sloc.xyz/github/
 erdogant/pca/?category=code)](https://github.com/erdogant/pca/) [![Downloads]
 (https://static.pepy.tech/personalized-badge/
@@ -31,32 +35,39 @@
 [GitHub repo size](https://img.shields.io/github/repo-size/erdogant/pca) [!
 [Donate](https://img.shields.io/badge/Support%20this%20project-
 grey.svg?logo=github%20sponsors)](https://erdogant.github.io/pca/pages/html/
 Documentation.html#) **pca** A Python Package for Principal Component Analysis.
 The core of PCA is build on sklearn functionality to find maximum compatibility
 when combining with other packages. But this package can do a lot more. Besides
 the regular pca, it can also perform **SparsePCA**, and **TruncatedSVD**.
-Depending on your input data, the best approach will be choosen. Other
-functionalities of PCA are: * **Biplot** to plot the loadings * Determine the
-**explained variance** * Extract the best performing **features** * Scatter
-plot with the **loadings** * Outlier detection using **Hotelling T2 and/or SPE/
-Dmodx** --- **â­ï¸ Star this repo if you like it â­ï¸** --- ## Read the
-Medium blog for more details. #### [1. What are PCA loadings and how to
-effectively use Biplots?](https://towardsdatascience.com/what-are-pca-loadings-
-and-biplots-9a7897f2e559) #### [2. Outlier Detection Using Principal Component
-Analysis and Hotellingâs T2 and SPE/DmodX Methods](https://
-towardsdatascience.com/outlier-detection-using-principal-component-analysis-
-and-hotellings-t2-and-spe-dmodx-methods-625b3c90897) #### [3. Quantitative
-comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https://
-towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-
-mappings-c6453b80f303) # --- ## [Documentation pages](https://
-erdogant.github.io/pca/) On the [documentation pages](https://
-erdogant.github.io/pca/) you can find detailed information about the working of
-the ``pca`` with many examples. --- ## Installation ```bash pip install pca ```
-##### Import pca package ```python from pca import pca ``` #
+Depending on your input data, the best approach will be chosen. **â­ï¸ Star
+this repo if you like it â­ï¸** Other functionalities of PCA are: *
+**Biplot** to plot the loadings * Determine the **explained variance** *
+Extract the best performing **features** * Scatter plot with the **loadings** *
+Outlier detection using **Hotelling T2 and/or SPE/Dmodx** ## Support Your
+â¤ï¸ is important to keep maintaining my packages. You can support in various
+ways, have a look at the [sponser page](https://erdogant.github.io/pca/pages/
+html/Documentation.html). Report bugs, issues or help out with developing new
+features! If you don't have the time to help or are still learning, you can
+also take a [Medium Mebership using my referral link](https://
+erdogant.medium.com/) to keep reading all my hands-on blogs. If you also don't
+need that, there is always the coffee! Thank you! _[_B_u_y_ _M_e_ _a_ _C_o_f_f_e_e_ _a_t_ _k_o_-
+_f_i_._c_o_m_]### Read the Medium blog for more details. #### [1. What are PCA
+loadings and how to effectively use Biplots?](https://towardsdatascience.com/
+what-are-pca-loadings-and-biplots-9a7897f2e559) #### [2. Outlier Detection
+Using Principal Component Analysis and Hotellingâs T2 and SPE/DmodX Methods]
+(https://towardsdatascience.com/outlier-detection-using-principal-component-
+analysis-and-hotellings-t2-and-spe-dmodx-methods-625b3c90897) #### [3.
+Quantitative comparisons between t-SNE, UMAP, PCA, and Other Mappings.](https:/
+/towardsdatascience.com/the-similarity-between-t-sne-umap-pca-and-other-
+mappings-c6453b80f303) ## [Documentation pages](https://erdogant.github.io/pca/
+) On the [documentation pages](https://erdogant.github.io/pca/) you can find
+detailed information about the working of the ``pca`` with many examples. ##
+Installation ```bash pip install pca ``` ##### Import pca package ```python
+from pca import pca ``` #
 _QQ_uu_ii_cc_kk_ _ss_tt_aa_rr_tt                            _MM_aa_kk_ee_ _bb_ii_pp_ll_oo_tt
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/ _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/
 _m_a_s_t_e_r_/_d_o_c_s_/_f_i_g_s_/                      _m_a_s_t_e_r_/_d_o_c_s_/_f_i_g_s_/
 _f_i_g___s_c_a_t_t_e_r_._p_n_g_?_r_a_w_=_t_r_u_e_]              _c_u_s_t_o_m___e_x_a_m_p_l_e___2_._p_n_g_?_r_a_w_=_t_r_u_e_]
 #
 _PP_ll_oo_tt_ _EE_xx_pp_ll_aa_ii_nn_ee_dd_ _vv_aa_rr_ii_aa_nn_cc_ee                _33_DD_ _pp_ll_oo_tt_ss
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/ _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_p_c_a_/_b_l_o_b_/
@@ -101,13 +112,8 @@
 visible status](https://erdogant.github.io/pca/pages/html/Plots.html#toggle-
 visible-status) # * [Example: Map unseen (new) datapoint to the transfomred
 space](https://erdogant.github.io/pca/pages/html/Examples.html#map-unseen-
 datapoints-into-fitted-space)
 ===============================================================================
 #### Citation Please cite in your publications if this is useful for your
 research (see citation). ### Maintainers * Erdogan Taskesen, github: [erdogant]
-(https://github.com/erdogant) --- ## Support Your â¤ï¸ is important to keep
-maintaining this package. You can [support](https://erdogant.github.io/pca/
-pages/html/Documentation.html) in various ways, have a look at the [sponser
-page](https://erdogant.github.io/pca/pages/html/Documentation.html). Report
-bugs, issues and feature extensions at [github page](https://github.com/
-erdogant/pca)._[_B_u_y_ _M_e_ _a_ _C_o_f_f_e_e_ _a_t_ _k_o_-_f_i_._c_o_m_]
+(https://github.com/erdogant) ---
```

### Comparing `pca-2.0.5/setup.py` & `pca-2.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 getversion = re.search( r"^__version__ = ['\"]([^'\"]*)['\"]", open(VERSIONFILE, "rt").read(), re.M)
 if getversion:
     new_version = getversion.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 setuptools.setup(
      install_requires=['datazets',
                        'statsmodels',
                        'matplotlib',
                        'numpy',
                        'scikit-learn',
```

