# Comparing `tmp/massivechem-3.4.tar.gz` & `tmp/massivechem-3.5.tar.gz`

## Comparing `massivechem-3.4.tar` & `massivechem-3.5.tar`

### file list

```diff
@@ -1,99 +1,143 @@
--rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-3.4/IMG_2856.jpg
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 massivechem-3.4/molecule_image.png
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 massivechem-3.4/project_CH200.yml
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-3.4/project_final.yml
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 massivechem-3.4/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 massivechem-3.4/.idea/ppchem-project-Christiansson-Gonteri-Humery.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 massivechem-3.4/.idea/vcs.xml
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 massivechem-3.4/.idea/workspace.xml
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 massivechem-3.4/.idea/input/input.html
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 massivechem-3.4/.idea/input/input.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 massivechem-3.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    35964 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/COPIED_VERSION.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/Preliminary_v2.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/abundance.txt
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/abundance_simplified.txt
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/big_func.html
--rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/big_func.py
--rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/copy_file.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/functional_group_finder.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/functions.html
--rw-r--r--   0        0        0    38793 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/functions.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/molecule_image.png
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/names.txt
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 massivechem-3.4/THOMAS_IS_BEST/test.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 massivechem-3.4/Thomas/Copy_spectrometer.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 massivechem-3.4/Thomas/Thomas_return_pyplot.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 massivechem-3.4/Thomas/random_tests.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 massivechem-3.4/Thomas/tests.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.4/data/abundance.txt
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Acid_image.png
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Acyl_chloride_image.png
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Alcohol_image.png
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Aldehyde_image.png
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Alkene_image.png
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Alkyne_image.png
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Amide_image.png
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Amine_image.png
--rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Amino_acid_image.png
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Anhydride_image.png
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Azide_image.png
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Benzene_image.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Bromide_image.png
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Carbonate2_image.png
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Carbonate_image.png
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Disulfide_image.png
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Enamine2_image.png
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Enamine_2_image.png
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Enamine_image.png
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Enol_image.png
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Ester_image.png
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Ether_image.png
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Fluoride_image.png
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Halogen_image.png
--rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Hemiacetal_image.png
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Imide_image.png
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Imine_image.png
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Iodide_image.png
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Ketone_image.png
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Nitrile_image.png
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Nitro_image.png
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Peroxide_image.png
--rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Phosphate_image.png
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Phosphine_image.png
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Proline_image.png
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Sulfides_image.png
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Sulfone_image.png
--rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Sulfonic_acid_image.png
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Sulfoxide_image.png
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Thio_ether_image.png
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Thioester_image.png
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/Thiol_image.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.4/data/Functional groups images/molecule_image.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 massivechem-3.4/notebooks/project_report.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.4/notebooks/test.ipynb
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/SMILEs_interpreter.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/all_in_one.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/data_list_generator.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/delete_mol_image_file.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/delta_function_plotter.py
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/double_plot.py
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/functional_group_finder.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/functional_list_display.html
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/functional_list_display.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/insaturation.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/ionisation_method.py
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/main_function.py
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/mol_web_show.html
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/mol_web_show.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/molecule_list_generator.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/peak_merger.py
--rw-r--r--   0        0        0    16398 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/spectrum.html
--rw-r--r--   0        0        0    20744 2020-02-02 00:00:00.000000 massivechem-3.4/scripts/spectrum.py
--rw-r--r--   0        0        0    49233 2020-02-02 00:00:00.000000 massivechem-3.4/src/MASSiveChem/MASSiveChem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.4/src/MASSiveChem/__init__.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 massivechem-3.4/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 massivechem-3.4/LICENSE.txt
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 massivechem-3.4/README.md
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 massivechem-3.4/pyproject.toml
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 massivechem-3.4/PKG-INFO
+-rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-3.5/IMG_2856.jpg
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 massivechem-3.5/molecule_image.png
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 massivechem-3.5/project_CH200.yml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-3.5/project_final.yml
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 massivechem-3.5/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 massivechem-3.5/.idea/ppchem-project-Christiansson-Gonteri-Humery.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 massivechem-3.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 massivechem-3.5/.idea/workspace.xml
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 massivechem-3.5/.idea/input/input.html
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 massivechem-3.5/.idea/input/input.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 massivechem-3.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0    35964 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/COPIED_VERSION.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/Preliminary_v2.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/abundance.txt
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/abundance_simplified.txt
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/big_func.html
+-rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/big_func.py
+-rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/copy_file.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/functional_group_finder.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/functions.html
+-rw-r--r--   0        0        0    38793 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/functions.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/molecule_image.png
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/names.txt
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 massivechem-3.5/THOMAS_IS_BEST/test.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 massivechem-3.5/Thomas/Copy_spectrometer.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 massivechem-3.5/Thomas/Thomas_return_pyplot.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 massivechem-3.5/Thomas/random_tests.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 massivechem-3.5/Thomas/tests.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.5/data/abundance.txt
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Acid_image.png
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Acyl_chloride_image.png
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Alcohol_image.png
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Aldehyde_image.png
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Alkene_image.png
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Alkyne_image.png
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Amide_image.png
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Amine_image.png
+-rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Amino_acid_image.png
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Anhydride_image.png
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Azide_image.png
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Benzene_image.png
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Bromide_image.png
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Carbonate2_image.png
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Carbonate_image.png
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Disulfide_image.png
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Enamine2_image.png
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Enamine_2_image.png
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Enamine_image.png
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Enol_image.png
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Ester_image.png
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Ether_image.png
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Fluoride_image.png
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Halogen_image.png
+-rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Hemiacetal_image.png
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Imide_image.png
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Imine_image.png
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Iodide_image.png
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Ketone_image.png
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Nitrile_image.png
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Nitro_image.png
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Peroxide_image.png
+-rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Phosphate_image.png
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Phosphine_image.png
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Proline_image.png
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Sulfides_image.png
+-rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Sulfone_image.png
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Sulfonic_acid_image.png
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Sulfoxide_image.png
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Thio_ether_image.png
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Thioester_image.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/Thiol_image.png
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.5/data/Functional groups images/molecule_image.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 massivechem-3.5/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.5/notebooks/test.ipynb
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/all_in_one.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/data_list_generator.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/delete_mol_image_file.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/delta_function_plotter.py
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/double_plot.py
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/functional_group_finder.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/functional_list_display.html
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/functional_list_display.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/insaturation.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/ionisation_method.py
+-rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/main_function.py
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/mol_web_show.html
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/mol_web_show.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/molecule_list_generator.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/peak_merger.py
+-rw-r--r--   0        0        0    16398 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/spectrum.html
+-rw-r--r--   0        0        0    20744 2020-02-02 00:00:00.000000 massivechem-3.5/scripts/spectrum.py
+-rw-r--r--   0        0        0    49233 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/MASSiveChem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/__init__.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/abundance.txt
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Acid_image.png
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Acyl_chloride_image.png
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Alcohol_image.png
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Aldehyde_image.png
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Alkene_image.png
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Alkyne_image.png
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Amide_image.png
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Amine_image.png
+-rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Amino_acid_image.png
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Anhydride_image.png
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Azide_image.png
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Benzene_image.png
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Bromide_image.png
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Carbonate2_image.png
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Carbonate_image.png
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Disulfide_image.png
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Enamine2_image.png
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Enamine_2_image.png
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Enamine_image.png
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Enol_image.png
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Ester_image.png
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Ether_image.png
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Fluoride_image.png
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Halogen_image.png
+-rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Hemiacetal_image.png
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Imide_image.png
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Imine_image.png
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Iodide_image.png
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Ketone_image.png
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Nitrile_image.png
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Nitro_image.png
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Peroxide_image.png
+-rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Phosphate_image.png
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Phosphine_image.png
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Proline_image.png
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Sulfides_image.png
+-rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Sulfone_image.png
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Sulfonic_acid_image.png
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Sulfoxide_image.png
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Thio_ether_image.png
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Thioester_image.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/Thiol_image.png
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.5/src/MASSiveChem/data/Functional groups images/molecule_image.png
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 massivechem-3.5/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 massivechem-3.5/LICENSE.txt
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 massivechem-3.5/README.md
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 massivechem-3.5/pyproject.toml
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 massivechem-3.5/PKG-INFO
```

### Comparing `massivechem-3.4/IMG_2856.jpg` & `massivechem-3.5/IMG_2856.jpg`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/molecule_image.png` & `massivechem-3.5/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/project_CH200.yml` & `massivechem-3.5/project_CH200.yml`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/project_final.yml` & `massivechem-3.5/project_final.yml`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/.idea/workspace.xml` & `massivechem-3.5/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/.idea/input/input.html` & `massivechem-3.5/.idea/input/input.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/.idea/input/input.py` & `massivechem-3.5/.idea/input/input.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/THOMAS_IS_BEST/COPIED_VERSION.py` & `massivechem-3.5/THOMAS_IS_BEST/COPIED_VERSION.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/THOMAS_IS_BEST/Preliminary_v2.py` & `massivechem-3.5/THOMAS_IS_BEST/Preliminary_v2.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/THOMAS_IS_BEST/abundance.txt` & `massivechem-3.5/THOMAS_IS_BEST/abundance.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/THOMAS_IS_BEST/abundance_simplified.txt` & `massivechem-3.5/THOMAS_IS_BEST/abundance_simplified.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/THOMAS_IS_BEST/big_func.html` & `massivechem-3.5/THOMAS_IS_BEST/big_func.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/THOMAS_IS_BEST/big_func.py` & `massivechem-3.5/THOMAS_IS_BEST/big_func.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/THOMAS_IS_BEST/copy_file.py` & `massivechem-3.5/THOMAS_IS_BEST/copy_file.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/THOMAS_IS_BEST/functional_group_finder.py` & `massivechem-3.5/THOMAS_IS_BEST/functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/THOMAS_IS_BEST/functions.html` & `massivechem-3.5/THOMAS_IS_BEST/functions.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/THOMAS_IS_BEST/functions.py` & `massivechem-3.5/THOMAS_IS_BEST/functions.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/THOMAS_IS_BEST/molecule_image.png` & `massivechem-3.5/THOMAS_IS_BEST/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/THOMAS_IS_BEST/test.py` & `massivechem-3.5/THOMAS_IS_BEST/test.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/Thomas/Copy_spectrometer.py` & `massivechem-3.5/Thomas/Copy_spectrometer.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/Thomas/Thomas_return_pyplot.py` & `massivechem-3.5/Thomas/Thomas_return_pyplot.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/Thomas/tests.py` & `massivechem-3.5/Thomas/tests.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/abundance.txt` & `massivechem-3.5/data/abundance.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Acid_image.png` & `massivechem-3.5/data/Functional groups images/Acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Acyl_chloride_image.png` & `massivechem-3.5/data/Functional groups images/Acyl_chloride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Alcohol_image.png` & `massivechem-3.5/data/Functional groups images/Alcohol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Aldehyde_image.png` & `massivechem-3.5/data/Functional groups images/Aldehyde_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Alkene_image.png` & `massivechem-3.5/data/Functional groups images/Alkene_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Alkyne_image.png` & `massivechem-3.5/data/Functional groups images/Alkyne_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Amide_image.png` & `massivechem-3.5/data/Functional groups images/Amide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Amine_image.png` & `massivechem-3.5/data/Functional groups images/Amine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Amino_acid_image.png` & `massivechem-3.5/data/Functional groups images/Amino_acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Anhydride_image.png` & `massivechem-3.5/data/Functional groups images/Anhydride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Azide_image.png` & `massivechem-3.5/data/Functional groups images/Azide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Benzene_image.png` & `massivechem-3.5/data/Functional groups images/Benzene_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Bromide_image.png` & `massivechem-3.5/data/Functional groups images/Bromide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Carbonate2_image.png` & `massivechem-3.5/data/Functional groups images/Carbonate2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Carbonate_image.png` & `massivechem-3.5/data/Functional groups images/Carbonate_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Disulfide_image.png` & `massivechem-3.5/data/Functional groups images/Disulfide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Enamine2_image.png` & `massivechem-3.5/data/Functional groups images/Enamine2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Enamine_2_image.png` & `massivechem-3.5/data/Functional groups images/Enamine_2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Enamine_image.png` & `massivechem-3.5/data/Functional groups images/Enamine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Enol_image.png` & `massivechem-3.5/data/Functional groups images/Enol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Ester_image.png` & `massivechem-3.5/data/Functional groups images/Ester_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Ether_image.png` & `massivechem-3.5/data/Functional groups images/Ether_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Fluoride_image.png` & `massivechem-3.5/data/Functional groups images/Fluoride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Halogen_image.png` & `massivechem-3.5/data/Functional groups images/Halogen_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Hemiacetal_image.png` & `massivechem-3.5/data/Functional groups images/Hemiacetal_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Imide_image.png` & `massivechem-3.5/data/Functional groups images/Imide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Imine_image.png` & `massivechem-3.5/data/Functional groups images/Imine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Iodide_image.png` & `massivechem-3.5/data/Functional groups images/Iodide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Ketone_image.png` & `massivechem-3.5/data/Functional groups images/Ketone_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Nitrile_image.png` & `massivechem-3.5/data/Functional groups images/Nitrile_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Nitro_image.png` & `massivechem-3.5/data/Functional groups images/Nitro_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Peroxide_image.png` & `massivechem-3.5/data/Functional groups images/Peroxide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Phosphate_image.png` & `massivechem-3.5/data/Functional groups images/Phosphate_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Phosphine_image.png` & `massivechem-3.5/data/Functional groups images/Phosphine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Proline_image.png` & `massivechem-3.5/data/Functional groups images/Proline_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Sulfides_image.png` & `massivechem-3.5/data/Functional groups images/Sulfides_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Sulfone_image.png` & `massivechem-3.5/data/Functional groups images/Sulfone_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Sulfonic_acid_image.png` & `massivechem-3.5/data/Functional groups images/Sulfonic_acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Sulfoxide_image.png` & `massivechem-3.5/data/Functional groups images/Sulfoxide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Thio_ether_image.png` & `massivechem-3.5/data/Functional groups images/Thio_ether_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Thioester_image.png` & `massivechem-3.5/data/Functional groups images/Thioester_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/Thiol_image.png` & `massivechem-3.5/data/Functional groups images/Thiol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/data/Functional groups images/molecule_image.png` & `massivechem-3.5/data/Functional groups images/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/SMILEs_interpreter.py` & `massivechem-3.5/scripts/SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/all_in_one.py` & `massivechem-3.5/scripts/all_in_one.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/data_list_generator.py` & `massivechem-3.5/scripts/data_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/delete_mol_image_file.py` & `massivechem-3.5/scripts/delete_mol_image_file.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/delta_function_plotter.py` & `massivechem-3.5/scripts/delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/double_plot.py` & `massivechem-3.5/scripts/double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/functional_group_finder.py` & `massivechem-3.5/scripts/functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/functional_list_display.html` & `massivechem-3.5/scripts/functional_list_display.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/functional_list_display.py` & `massivechem-3.5/scripts/functional_list_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/insaturation.py` & `massivechem-3.5/scripts/insaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/ionisation_method.py` & `massivechem-3.5/scripts/ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/main_function.py` & `massivechem-3.5/scripts/main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/mol_web_show.html` & `massivechem-3.5/scripts/mol_web_show.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/mol_web_show.py` & `massivechem-3.5/scripts/mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/molecule_list_generator.py` & `massivechem-3.5/scripts/molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/peak_merger.py` & `massivechem-3.5/scripts/peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/spectrum.html` & `massivechem-3.5/scripts/spectrum.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/scripts/spectrum.py` & `massivechem-3.5/scripts/spectrum.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/src/MASSiveChem/MASSiveChem.py` & `massivechem-3.5/src/MASSiveChem/MASSiveChem.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/.gitignore` & `massivechem-3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/LICENSE.txt` & `massivechem-3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/README.md` & `massivechem-3.5/README.md`

 * *Files identical despite different names*

### Comparing `massivechem-3.4/pyproject.toml` & `massivechem-3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 4d41 5353 4956 4543 6865 6d22 0d0a   "MASSIVEChem"..
-00000070: 7665 7273 696f 6e20 3d20 2233 2e34 220d  version = "3.4".
+00000070: 7665 7273 696f 6e20 3d20 2233 2e35 220d  version = "3.5".
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 00000090: 4d41 5353 4956 4543 6865 6d20 6973 2061  MASSIVEChem is a
 000000a0: 2070 6970 2d69 6e73 7461 6c6c 6162 6c65   pip-installable
 000000b0: 2070 6163 6b61 6765 2066 6f72 2061 6e61   package for ana
 000000c0: 6c79 7469 6361 6c20 6368 656d 6973 7472  lytical chemistr
 000000d0: 792e 2049 7420 7369 6d75 6c61 7465 7320  y. It simulates 
 000000e0: 6d6f 6c65 6375 6c65 206d 6173 7320 7370  molecule mass sp
```

### Comparing `massivechem-3.4/PKG-INFO` & `massivechem-3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MASSIVEChem
-Version: 3.4
+Version: 3.5
 Summary: MASSIVEChem is a pip-installable package for analytical chemistry. It simulates molecule mass spectra and graphically displays them. It includes tools like a functional group finder and unsaturation calculator to aid chemical analysis.
 Project-URL: Homepage, https://github.com/ThomasCsson/MASSIVEChem.git
 Project-URL: GitHub_Thomas_Christiansson, https://github.com/ThomasCsson
 Project-URL: GitHub_Igor_Gonteri, https://github.com/igorgonteri
 Project-URL: GitHub_Arthur_Humery, https://github.com/Arthurhmy
 Author-email: Thomas Viking Christiansson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
```

