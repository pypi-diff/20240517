# Comparing `tmp/massivechem-3.6.tar.gz` & `tmp/massivechem-3.9.tar.gz`

## Comparing `massivechem-3.6.tar` & `massivechem-3.9.tar`

### file list

```diff
@@ -1,143 +1,143 @@
--rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-3.6/IMG_2856.jpg
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 massivechem-3.6/molecule_image.png
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 massivechem-3.6/project_CH200.yml
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-3.6/project_final.yml
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 massivechem-3.6/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 massivechem-3.6/.idea/ppchem-project-Christiansson-Gonteri-Humery.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 massivechem-3.6/.idea/vcs.xml
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 massivechem-3.6/.idea/workspace.xml
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 massivechem-3.6/.idea/input/input.html
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 massivechem-3.6/.idea/input/input.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 massivechem-3.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    35964 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/COPIED_VERSION.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/Preliminary_v2.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/abundance.txt
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/abundance_simplified.txt
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/big_func.html
--rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/big_func.py
--rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/copy_file.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/functional_group_finder.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/functions.html
--rw-r--r--   0        0        0    38793 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/functions.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/molecule_image.png
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/names.txt
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 massivechem-3.6/THOMAS_IS_BEST/test.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 massivechem-3.6/Thomas/Copy_spectrometer.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 massivechem-3.6/Thomas/Thomas_return_pyplot.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 massivechem-3.6/Thomas/random_tests.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 massivechem-3.6/Thomas/tests.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.6/data/abundance.txt
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Acid_image.png
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Acyl_chloride_image.png
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Alcohol_image.png
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Aldehyde_image.png
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Alkene_image.png
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Alkyne_image.png
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Amide_image.png
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Amine_image.png
--rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Amino_acid_image.png
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Anhydride_image.png
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Azide_image.png
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Benzene_image.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Bromide_image.png
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Carbonate2_image.png
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Carbonate_image.png
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Disulfide_image.png
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Enamine2_image.png
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Enamine_2_image.png
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Enamine_image.png
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Enol_image.png
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Ester_image.png
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Ether_image.png
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Fluoride_image.png
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Halogen_image.png
--rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Hemiacetal_image.png
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Imide_image.png
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Imine_image.png
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Iodide_image.png
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Ketone_image.png
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Nitrile_image.png
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Nitro_image.png
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Peroxide_image.png
--rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Phosphate_image.png
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Phosphine_image.png
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Proline_image.png
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Sulfides_image.png
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Sulfone_image.png
--rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Sulfonic_acid_image.png
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Sulfoxide_image.png
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Thio_ether_image.png
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Thioester_image.png
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/Thiol_image.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.6/data/Functional groups images/molecule_image.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 massivechem-3.6/notebooks/project_report.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.6/notebooks/test.ipynb
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/SMILEs_interpreter.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/all_in_one.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/data_list_generator.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/delete_mol_image_file.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/delta_function_plotter.py
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/double_plot.py
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/functional_group_finder.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/functional_list_display.html
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/functional_list_display.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/insaturation.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/ionisation_method.py
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/main_function.py
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/mol_web_show.html
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/mol_web_show.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/molecule_list_generator.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/peak_merger.py
--rw-r--r--   0        0        0    16398 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/spectrum.html
--rw-r--r--   0        0        0    20744 2020-02-02 00:00:00.000000 massivechem-3.6/scripts/spectrum.py
--rw-r--r--   0        0        0    49233 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/MASSiveChem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/__init__.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/abundance.txt
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Acid_image.png
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Acyl_chloride_image.png
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Alcohol_image.png
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Aldehyde_image.png
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Alkene_image.png
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Alkyne_image.png
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Amide_image.png
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Amine_image.png
--rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Amino_acid_image.png
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Anhydride_image.png
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Azide_image.png
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Benzene_image.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Bromide_image.png
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Carbonate2_image.png
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Carbonate_image.png
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Disulfide_image.png
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Enamine2_image.png
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Enamine_2_image.png
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Enamine_image.png
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Enol_image.png
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Ester_image.png
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Ether_image.png
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Fluoride_image.png
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Halogen_image.png
--rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Hemiacetal_image.png
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Imide_image.png
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Imine_image.png
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Iodide_image.png
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Ketone_image.png
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Nitrile_image.png
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Nitro_image.png
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Peroxide_image.png
--rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Phosphate_image.png
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Phosphine_image.png
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Proline_image.png
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Sulfides_image.png
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Sulfone_image.png
--rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Sulfonic_acid_image.png
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Sulfoxide_image.png
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Thio_ether_image.png
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Thioester_image.png
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/Thiol_image.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.6/src/MASSiveChem/data/Functional groups images/molecule_image.png
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 massivechem-3.6/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 massivechem-3.6/LICENSE.txt
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 massivechem-3.6/README.md
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 massivechem-3.6/pyproject.toml
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 massivechem-3.6/PKG-INFO
+-rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-3.9/IMG_2856.jpg
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 massivechem-3.9/molecule_image.png
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 massivechem-3.9/project_CH200.yml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-3.9/project_final.yml
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/ppchem-project-Christiansson-Gonteri-Humery.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/vcs.xml
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/workspace.xml
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/input/input.html
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/input/input.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0    35964 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/COPIED_VERSION.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/Preliminary_v2.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/abundance.txt
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/abundance_simplified.txt
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/big_func.html
+-rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/big_func.py
+-rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/copy_file.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/functional_group_finder.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/functions.html
+-rw-r--r--   0        0        0    38793 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/functions.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/molecule_image.png
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/names.txt
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/test.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 massivechem-3.9/Thomas/Copy_spectrometer.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 massivechem-3.9/Thomas/Thomas_return_pyplot.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 massivechem-3.9/Thomas/random_tests.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 massivechem-3.9/Thomas/tests.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.9/data/abundance.txt
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Acid_image.png
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Acyl_chloride_image.png
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Alcohol_image.png
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Aldehyde_image.png
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Alkene_image.png
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Alkyne_image.png
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Amide_image.png
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Amine_image.png
+-rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Amino_acid_image.png
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Anhydride_image.png
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Azide_image.png
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Benzene_image.png
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Bromide_image.png
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Carbonate2_image.png
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Carbonate_image.png
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Disulfide_image.png
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Enamine2_image.png
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Enamine_2_image.png
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Enamine_image.png
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Enol_image.png
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Ester_image.png
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Ether_image.png
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Fluoride_image.png
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Halogen_image.png
+-rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Hemiacetal_image.png
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Imide_image.png
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Imine_image.png
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Iodide_image.png
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Ketone_image.png
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Nitrile_image.png
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Nitro_image.png
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Peroxide_image.png
+-rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Phosphate_image.png
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Phosphine_image.png
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Proline_image.png
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Sulfides_image.png
+-rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Sulfone_image.png
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Sulfonic_acid_image.png
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Sulfoxide_image.png
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Thio_ether_image.png
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Thioester_image.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Thiol_image.png
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/molecule_image.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 massivechem-3.9/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.9/notebooks/test.ipynb
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/all_in_one.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/data_list_generator.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/delete_mol_image_file.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/delta_function_plotter.py
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/double_plot.py
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/functional_group_finder.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/functional_list_display.html
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/functional_list_display.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/insaturation.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/ionisation_method.py
+-rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/main_function.py
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/mol_web_show.html
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/mol_web_show.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/molecule_list_generator.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/peak_merger.py
+-rw-r--r--   0        0        0    16398 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/spectrum.html
+-rw-r--r--   0        0        0    20744 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/spectrum.py
+-rw-r--r--   0        0        0    49233 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/MASSiveChem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/__init__.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/abundance.txt
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Acid_image.png
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Acyl_chloride_image.png
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Alcohol_image.png
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Aldehyde_image.png
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Alkene_image.png
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Alkyne_image.png
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Amide_image.png
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Amine_image.png
+-rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Amino_acid_image.png
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Anhydride_image.png
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Azide_image.png
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Benzene_image.png
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Bromide_image.png
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Carbonate2_image.png
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Carbonate_image.png
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Disulfide_image.png
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Enamine2_image.png
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Enamine_2_image.png
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Enamine_image.png
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Enol_image.png
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Ester_image.png
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Ether_image.png
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Fluoride_image.png
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Halogen_image.png
+-rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Hemiacetal_image.png
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Imide_image.png
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Imine_image.png
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Iodide_image.png
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Ketone_image.png
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Nitrile_image.png
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Nitro_image.png
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Peroxide_image.png
+-rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Phosphate_image.png
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Phosphine_image.png
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Proline_image.png
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Sulfides_image.png
+-rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Sulfone_image.png
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Sulfonic_acid_image.png
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Sulfoxide_image.png
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Thio_ether_image.png
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Thioester_image.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Thiol_image.png
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/molecule_image.png
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 massivechem-3.9/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 massivechem-3.9/LICENSE.txt
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 massivechem-3.9/README.md
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 massivechem-3.9/pyproject.toml
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 massivechem-3.9/PKG-INFO
```

### Comparing `massivechem-3.6/IMG_2856.jpg` & `massivechem-3.9/IMG_2856.jpg`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/molecule_image.png` & `massivechem-3.9/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/project_CH200.yml` & `massivechem-3.9/project_CH200.yml`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/project_final.yml` & `massivechem-3.9/project_final.yml`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/.idea/workspace.xml` & `massivechem-3.9/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/.idea/input/input.html` & `massivechem-3.9/.idea/input/input.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/.idea/input/input.py` & `massivechem-3.9/.idea/input/input.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/THOMAS_IS_BEST/COPIED_VERSION.py` & `massivechem-3.9/THOMAS_IS_BEST/COPIED_VERSION.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/THOMAS_IS_BEST/Preliminary_v2.py` & `massivechem-3.9/THOMAS_IS_BEST/Preliminary_v2.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/THOMAS_IS_BEST/abundance.txt` & `massivechem-3.9/THOMAS_IS_BEST/abundance.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/THOMAS_IS_BEST/abundance_simplified.txt` & `massivechem-3.9/THOMAS_IS_BEST/abundance_simplified.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/THOMAS_IS_BEST/big_func.html` & `massivechem-3.9/THOMAS_IS_BEST/big_func.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/THOMAS_IS_BEST/big_func.py` & `massivechem-3.9/THOMAS_IS_BEST/big_func.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/THOMAS_IS_BEST/copy_file.py` & `massivechem-3.9/THOMAS_IS_BEST/copy_file.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/THOMAS_IS_BEST/functional_group_finder.py` & `massivechem-3.9/THOMAS_IS_BEST/functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/THOMAS_IS_BEST/functions.html` & `massivechem-3.9/THOMAS_IS_BEST/functions.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/THOMAS_IS_BEST/functions.py` & `massivechem-3.9/THOMAS_IS_BEST/functions.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/THOMAS_IS_BEST/molecule_image.png` & `massivechem-3.9/THOMAS_IS_BEST/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/THOMAS_IS_BEST/test.py` & `massivechem-3.9/THOMAS_IS_BEST/test.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/Thomas/Copy_spectrometer.py` & `massivechem-3.9/Thomas/Copy_spectrometer.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/Thomas/Thomas_return_pyplot.py` & `massivechem-3.9/Thomas/Thomas_return_pyplot.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/Thomas/tests.py` & `massivechem-3.9/Thomas/tests.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/abundance.txt` & `massivechem-3.9/data/abundance.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Acid_image.png` & `massivechem-3.9/data/Functional groups images/Acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Acyl_chloride_image.png` & `massivechem-3.9/data/Functional groups images/Acyl_chloride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Alcohol_image.png` & `massivechem-3.9/data/Functional groups images/Alcohol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Aldehyde_image.png` & `massivechem-3.9/data/Functional groups images/Aldehyde_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Alkene_image.png` & `massivechem-3.9/data/Functional groups images/Alkene_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Alkyne_image.png` & `massivechem-3.9/data/Functional groups images/Alkyne_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Amide_image.png` & `massivechem-3.9/data/Functional groups images/Amide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Amine_image.png` & `massivechem-3.9/data/Functional groups images/Amine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Amino_acid_image.png` & `massivechem-3.9/data/Functional groups images/Amino_acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Anhydride_image.png` & `massivechem-3.9/data/Functional groups images/Anhydride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Azide_image.png` & `massivechem-3.9/data/Functional groups images/Azide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Benzene_image.png` & `massivechem-3.9/data/Functional groups images/Benzene_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Bromide_image.png` & `massivechem-3.9/data/Functional groups images/Bromide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Carbonate2_image.png` & `massivechem-3.9/data/Functional groups images/Carbonate2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Carbonate_image.png` & `massivechem-3.9/data/Functional groups images/Carbonate_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Disulfide_image.png` & `massivechem-3.9/data/Functional groups images/Disulfide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Enamine2_image.png` & `massivechem-3.9/data/Functional groups images/Enamine2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Enamine_2_image.png` & `massivechem-3.9/data/Functional groups images/Enamine_2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Enamine_image.png` & `massivechem-3.9/data/Functional groups images/Enamine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Enol_image.png` & `massivechem-3.9/data/Functional groups images/Enol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Ester_image.png` & `massivechem-3.9/data/Functional groups images/Ester_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Ether_image.png` & `massivechem-3.9/data/Functional groups images/Ether_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Fluoride_image.png` & `massivechem-3.9/data/Functional groups images/Fluoride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Halogen_image.png` & `massivechem-3.9/data/Functional groups images/Halogen_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Hemiacetal_image.png` & `massivechem-3.9/data/Functional groups images/Hemiacetal_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Imide_image.png` & `massivechem-3.9/data/Functional groups images/Imide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Imine_image.png` & `massivechem-3.9/data/Functional groups images/Imine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Iodide_image.png` & `massivechem-3.9/data/Functional groups images/Iodide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Ketone_image.png` & `massivechem-3.9/data/Functional groups images/Ketone_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Nitrile_image.png` & `massivechem-3.9/data/Functional groups images/Nitrile_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Nitro_image.png` & `massivechem-3.9/data/Functional groups images/Nitro_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Peroxide_image.png` & `massivechem-3.9/data/Functional groups images/Peroxide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Phosphate_image.png` & `massivechem-3.9/data/Functional groups images/Phosphate_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Phosphine_image.png` & `massivechem-3.9/data/Functional groups images/Phosphine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Proline_image.png` & `massivechem-3.9/data/Functional groups images/Proline_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Sulfides_image.png` & `massivechem-3.9/data/Functional groups images/Sulfides_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Sulfone_image.png` & `massivechem-3.9/data/Functional groups images/Sulfone_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Sulfonic_acid_image.png` & `massivechem-3.9/data/Functional groups images/Sulfonic_acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Sulfoxide_image.png` & `massivechem-3.9/data/Functional groups images/Sulfoxide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Thio_ether_image.png` & `massivechem-3.9/data/Functional groups images/Thio_ether_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Thioester_image.png` & `massivechem-3.9/data/Functional groups images/Thioester_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/Thiol_image.png` & `massivechem-3.9/data/Functional groups images/Thiol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/data/Functional groups images/molecule_image.png` & `massivechem-3.9/data/Functional groups images/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/SMILEs_interpreter.py` & `massivechem-3.9/scripts/SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/all_in_one.py` & `massivechem-3.9/scripts/all_in_one.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/data_list_generator.py` & `massivechem-3.9/scripts/data_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/delete_mol_image_file.py` & `massivechem-3.9/scripts/delete_mol_image_file.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/delta_function_plotter.py` & `massivechem-3.9/scripts/delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/double_plot.py` & `massivechem-3.9/scripts/double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/functional_group_finder.py` & `massivechem-3.9/scripts/functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/functional_list_display.html` & `massivechem-3.9/scripts/functional_list_display.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/functional_list_display.py` & `massivechem-3.9/scripts/functional_list_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/insaturation.py` & `massivechem-3.9/scripts/insaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/ionisation_method.py` & `massivechem-3.9/scripts/ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/main_function.py` & `massivechem-3.9/scripts/main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/mol_web_show.html` & `massivechem-3.9/scripts/mol_web_show.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/mol_web_show.py` & `massivechem-3.9/scripts/mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/molecule_list_generator.py` & `massivechem-3.9/scripts/molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/peak_merger.py` & `massivechem-3.9/scripts/peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/spectrum.html` & `massivechem-3.9/scripts/spectrum.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/scripts/spectrum.py` & `massivechem-3.9/scripts/spectrum.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/MASSiveChem.py` & `massivechem-3.9/src/MASSiveChem/MASSiveChem.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/abundance.txt` & `massivechem-3.9/src/MASSiveChem/data/abundance.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Acid_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Acyl_chloride_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Acyl_chloride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Alcohol_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Alcohol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Aldehyde_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Aldehyde_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Alkene_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Alkene_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Alkyne_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Alkyne_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Amide_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Amide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Amine_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Amine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Amino_acid_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Amino_acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Anhydride_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Anhydride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Azide_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Azide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Benzene_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Benzene_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Bromide_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Bromide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Carbonate2_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Carbonate2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Carbonate_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Carbonate_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Disulfide_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Disulfide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Enamine2_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Enamine2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Enamine_2_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Enamine_2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Enamine_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Enamine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Enol_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Enol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Ester_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Ester_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Ether_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Ether_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Fluoride_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Fluoride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Halogen_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Halogen_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Hemiacetal_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Hemiacetal_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Imide_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Imide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Imine_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Imine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Iodide_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Iodide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Ketone_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Ketone_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Nitrile_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Nitrile_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Nitro_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Nitro_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Peroxide_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Peroxide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Phosphate_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Phosphate_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Phosphine_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Phosphine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Proline_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Proline_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Sulfides_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Sulfides_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Sulfone_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Sulfone_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Sulfonic_acid_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Sulfonic_acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Sulfoxide_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Sulfoxide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Thio_ether_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Thio_ether_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Thioester_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Thioester_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/Thiol_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/Thiol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/src/MASSiveChem/data/Functional groups images/molecule_image.png` & `massivechem-3.9/src/MASSiveChem/data/Functional groups images/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/.gitignore` & `massivechem-3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/LICENSE.txt` & `massivechem-3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.6/README.md` & `massivechem-3.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 ![logo](IMG_2856.jpg)
-![Thomas](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
-![Thomas2](https://img.shields.io/badge/Brave-FF1B2D?style=for-the-badge&logo=Brave&logoColor=white)
+![Thomas1](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
+![Thomas2](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white)
+![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
+![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
+![Thomas5](	https://img.shields.io/badge/Electron-2B2E3A?style=for-the-badge&logo=electron&logoColor=9FEAF9)
+![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)
+![Thomas7](https://img.shields.io/badge/WeChat-07C160?style=for-the-badge&logo=wechat&logoColor=white)
 # -         MASSIVEChem       - 
  - Python package for applied analytical chemistry focused primarily on mass speectrometry 
 #### Project in practical programming in chemistry course -- EPFL CH-200
 
 ## Package description 
 MASSIVEChem, which stands for "Mass Analytical Spectrometry System for Investigation and Visual Extrapolation in Chemistry", is a pip-installable package developped at EPFL in 2024 focused on, as its name would suggest, analytical chemistry.
 The aim of this package is to provide the user functions in order to simulate the mass spectrum of a molecule and to display this spectrum on a graph. The package also provides other features that can facilitate the chemical analysis of a molecule such as a functional group finder and an unsaturation calculator.
```

### Comparing `massivechem-3.6/pyproject.toml` & `massivechem-3.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 4d41 5353 4956 4543 6865 6d22 0d0a   "MASSIVEChem"..
-00000070: 7665 7273 696f 6e20 3d20 2233 2e36 220d  version = "3.6".
+00000070: 7665 7273 696f 6e20 3d20 2233 2e39 220d  version = "3.9".
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 00000090: 4d41 5353 4956 4543 6865 6d20 6973 2061  MASSIVEChem is a
 000000a0: 2070 6970 2d69 6e73 7461 6c6c 6162 6c65   pip-installable
 000000b0: 2070 6163 6b61 6765 2066 6f72 2061 6e61   package for ana
 000000c0: 6c79 7469 6361 6c20 6368 656d 6973 7472  lytical chemistr
 000000d0: 792e 2049 7420 7369 6d75 6c61 7465 7320  y. It simulates 
 000000e0: 6d6f 6c65 6375 6c65 206d 6173 7320 7370  molecule mass sp
@@ -70,18 +70,18 @@
 00000450: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
 00000460: 3a20 4d49 5420 4c69 6365 6e73 6522 2c0d  : MIT License",.
 00000470: 0a20 2020 2022 4f70 6572 6174 696e 6720  .    "Operating 
 00000480: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
 00000490: 6570 656e 6465 6e74 220d 0a5d 0d0a 0d0a  ependent"..]....
 000004a0: 5b74 6f6f 6c2e 706f 6574 7279 2e66 696c  [tool.poetry.fil
 000004b0: 6573 5d0d 0a69 6e63 6c75 6465 203d 205b  es]..include = [
-000004c0: 2273 7263 2f4d 4153 5349 5645 4368 656d  "src/MASSIVEChem
+000004c0: 2273 7263 2f4d 4153 5369 7665 4368 656d  "src/MASSiveChem
 000004d0: 2f64 6174 612f 6162 756e 6461 6e63 652e  /data/abundance.
-000004e0: 7478 7422 2c22 7372 632f 4d41 5353 4956  txt","src/MASSIV
-000004f0: 4543 6865 6d2f 6461 7461 2f46 756e 6374  EChem/data/Funct
+000004e0: 7478 7422 2c22 7372 632f 4d41 5353 6976  txt","src/MASSiv
+000004f0: 6543 6865 6d2f 6461 7461 2f46 756e 6374  eChem/data/Funct
 00000500: 696f 6e61 6c20 6772 6f75 7073 2069 6d61  ional groups ima
 00000510: 6765 7322 5d0d 0a0d 0a0d 0a5b 7072 6f6a  ges"]......[proj
 00000520: 6563 742e 7572 6c73 5d0d 0a48 6f6d 6570  ect.urls]..Homep
 00000530: 6167 6520 3d20 2268 7474 7073 3a2f 2f67  age = "https://g
 00000540: 6974 6875 622e 636f 6d2f 5468 6f6d 6173  ithub.com/Thomas
 00000550: 4373 736f 6e2f 4d41 5353 4956 4543 6865  Csson/MASSIVEChe
 00000560: 6d2e 6769 7422 0d0a 4769 7448 7562 5f54  m.git"..GitHub_T
```

### Comparing `massivechem-3.6/PKG-INFO` & `massivechem-3.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MASSIVEChem
-Version: 3.6
+Version: 3.9
 Summary: MASSIVEChem is a pip-installable package for analytical chemistry. It simulates molecule mass spectra and graphically displays them. It includes tools like a functional group finder and unsaturation calculator to aid chemical analysis.
 Project-URL: Homepage, https://github.com/ThomasCsson/MASSIVEChem.git
 Project-URL: GitHub_Thomas_Christiansson, https://github.com/ThomasCsson
 Project-URL: GitHub_Igor_Gonteri, https://github.com/igorgonteri
 Project-URL: GitHub_Arthur_Humery, https://github.com/Arthurhmy
 Author-email: Thomas Viking Christiansson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
@@ -18,16 +18,21 @@
 Requires-Dist: bokeh
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: rdkit
 Description-Content-Type: text/markdown
 
 ![logo](IMG_2856.jpg)
-![Thomas](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
-![Thomas2](https://img.shields.io/badge/Brave-FF1B2D?style=for-the-badge&logo=Brave&logoColor=white)
+![Thomas1](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
+![Thomas2](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white)
+![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
+![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
+![Thomas5](	https://img.shields.io/badge/Electron-2B2E3A?style=for-the-badge&logo=electron&logoColor=9FEAF9)
+![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)
+![Thomas7](https://img.shields.io/badge/WeChat-07C160?style=for-the-badge&logo=wechat&logoColor=white)
 # -         MASSIVEChem       - 
  - Python package for applied analytical chemistry focused primarily on mass speectrometry 
 #### Project in practical programming in chemistry course -- EPFL CH-200
 
 ## Package description 
 MASSIVEChem, which stands for "Mass Analytical Spectrometry System for Investigation and Visual Extrapolation in Chemistry", is a pip-installable package developped at EPFL in 2024 focused on, as its name would suggest, analytical chemistry.
 The aim of this package is to provide the user functions in order to simulate the mass spectrum of a molecule and to display this spectrum on a graph. The package also provides other features that can facilitate the chemical analysis of a molecule such as a functional group finder and an unsaturation calculator.
```

