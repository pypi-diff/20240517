# Comparing `tmp/massivechem-3.2.tar.gz` & `tmp/massivechem-3.3.tar.gz`

## Comparing `massivechem-3.2.tar` & `massivechem-3.3.tar`

### file list

```diff
@@ -1,90 +1,133 @@
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 massivechem-3.2/molecule_image.png
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 massivechem-3.2/project_CH200.yml
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-3.2/project_final.yml
--rw-r--r--   0        0        0    35964 2020-02-02 00:00:00.000000 massivechem-3.2/THOMAS_IS_BEST/COPIED_VERSION.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 massivechem-3.2/THOMAS_IS_BEST/Preliminary_v2.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.2/THOMAS_IS_BEST/abundance.txt
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 massivechem-3.2/THOMAS_IS_BEST/abundance_simplified.txt
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 massivechem-3.2/THOMAS_IS_BEST/big_func.html
--rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 massivechem-3.2/THOMAS_IS_BEST/big_func.py
--rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 massivechem-3.2/THOMAS_IS_BEST/copy_file.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 massivechem-3.2/THOMAS_IS_BEST/functional_group_finder.py
--rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 massivechem-3.2/THOMAS_IS_BEST/functions.html
--rw-r--r--   0        0        0    38953 2020-02-02 00:00:00.000000 massivechem-3.2/THOMAS_IS_BEST/functions.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 massivechem-3.2/THOMAS_IS_BEST/names.txt
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 massivechem-3.2/THOMAS_IS_BEST/test.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 massivechem-3.2/Thomas/Copy_spectrometer.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 massivechem-3.2/Thomas/Thomas_return_pyplot.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 massivechem-3.2/Thomas/random_tests.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 massivechem-3.2/Thomas/tests.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.2/data/abundance.txt
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Acid_image.png
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Acyl_chloride_image.png
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Alcohol_image.png
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Aldehyde_image.png
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Alkene_image.png
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Alkyne_image.png
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Amide_image.png
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Amine_image.png
--rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Amino_acid_image.png
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Anhydride_image.png
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Azide_image.png
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Benzene_image.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Bromide_image.png
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Carbonate2_image.png
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Carbonate_image.png
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Disulfide_image.png
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Enamine2_image.png
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Enamine_2_image.png
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Enamine_image.png
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Enol_image.png
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Ester_image.png
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Ether_image.png
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Fluoride_image.png
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Halogen_image.png
--rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Hemiacetal_image.png
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Imide_image.png
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Imine_image.png
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Iodide_image.png
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Ketone_image.png
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Nitrile_image.png
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Nitro_image.png
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Peroxide_image.png
--rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Phosphate_image.png
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Phosphine_image.png
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Proline_image.png
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Sulfides_image.png
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Sulfone_image.png
--rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Sulfonic_acid_image.png
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Sulfoxide_image.png
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Thio_ether_image.png
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Thioester_image.png
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/Thiol_image.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.2/data/Functional groups images/molecule_image.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 massivechem-3.2/notebooks/project_report.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.2/notebooks/test.ipynb
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/SMILEs_interpreter.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/all_in_one.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/data_list_generator.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/delete_mol_image_file.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/delta_function_plotter.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/double_plot.py
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/functional_group_finder.py
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/functional_list_display.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/insaturation.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/ionisation_method.py
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/main_function.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/mol_web_show.html
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/mol_web_show.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/molecule_list_generator.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/peak_merger.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/save_molecule_image_to_file.py
--rw-r--r--   0        0        0    16139 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/spectrum.html
--rw-r--r--   0        0        0    21305 2020-02-02 00:00:00.000000 massivechem-3.2/scripts/spectrum.py
--rw-r--r--   0        0        0    49233 2020-02-02 00:00:00.000000 massivechem-3.2/src/MASSiveChem/MASSiveChem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.2/src/MASSiveChem/__init__.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 massivechem-3.2/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 massivechem-3.2/LICENSE.txt
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 massivechem-3.2/README.md
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 massivechem-3.2/pyproject.toml
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 massivechem-3.2/PKG-INFO
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 massivechem-3.3/molecule_image.png
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 massivechem-3.3/project_CH200.yml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-3.3/project_final.yml
+-rw-r--r--   0        0        0    35964 2020-02-02 00:00:00.000000 massivechem-3.3/THOMAS_IS_BEST/COPIED_VERSION.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 massivechem-3.3/THOMAS_IS_BEST/Preliminary_v2.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.3/THOMAS_IS_BEST/abundance.txt
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 massivechem-3.3/THOMAS_IS_BEST/abundance_simplified.txt
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 massivechem-3.3/THOMAS_IS_BEST/big_func.html
+-rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 massivechem-3.3/THOMAS_IS_BEST/big_func.py
+-rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 massivechem-3.3/THOMAS_IS_BEST/copy_file.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 massivechem-3.3/THOMAS_IS_BEST/functional_group_finder.py
+-rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 massivechem-3.3/THOMAS_IS_BEST/functions.html
+-rw-r--r--   0        0        0    38953 2020-02-02 00:00:00.000000 massivechem-3.3/THOMAS_IS_BEST/functions.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 massivechem-3.3/THOMAS_IS_BEST/names.txt
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 massivechem-3.3/THOMAS_IS_BEST/test.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 massivechem-3.3/Thomas/Copy_spectrometer.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 massivechem-3.3/Thomas/Thomas_return_pyplot.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 massivechem-3.3/Thomas/random_tests.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 massivechem-3.3/Thomas/tests.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.3/data/abundance.txt
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Acid_image.png
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Acyl_chloride_image.png
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Alcohol_image.png
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Aldehyde_image.png
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Alkene_image.png
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Alkyne_image.png
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Amide_image.png
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Amine_image.png
+-rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Amino_acid_image.png
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Anhydride_image.png
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Azide_image.png
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Benzene_image.png
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Bromide_image.png
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Carbonate2_image.png
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Carbonate_image.png
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Disulfide_image.png
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Enamine2_image.png
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Enamine_2_image.png
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Enamine_image.png
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Enol_image.png
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Ester_image.png
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Ether_image.png
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Fluoride_image.png
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Halogen_image.png
+-rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Hemiacetal_image.png
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Imide_image.png
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Imine_image.png
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Iodide_image.png
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Ketone_image.png
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Nitrile_image.png
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Nitro_image.png
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Peroxide_image.png
+-rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Phosphate_image.png
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Phosphine_image.png
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Proline_image.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Sulfides_image.png
+-rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Sulfone_image.png
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Sulfonic_acid_image.png
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Sulfoxide_image.png
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Thio_ether_image.png
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Thioester_image.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/Thiol_image.png
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.3/data/Functional groups images/molecule_image.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 massivechem-3.3/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.3/notebooks/test.ipynb
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/SMILEs_interpreter.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/all_in_one.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/data_list_generator.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/delete_mol_image_file.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/delta_function_plotter.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/double_plot.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/functional_group_finder.py
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/functional_list_display.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/insaturation.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/ionisation_method.py
+-rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/main_function.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/mol_web_show.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/molecule_list_generator.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/peak_merger.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/save_molecule_image_to_file.py
+-rw-r--r--   0        0        0    16047 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/spectrum.html
+-rw-r--r--   0        0        0    21303 2020-02-02 00:00:00.000000 massivechem-3.3/scripts/spectrum.py
+-rw-r--r--   0        0        0    49233 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/MASSiveChem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/__init__.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/abundance.txt
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Acid_image.png
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Acyl_chloride_image.png
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Alcohol_image.png
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Aldehyde_image.png
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Alkene_image.png
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Alkyne_image.png
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Amide_image.png
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Amine_image.png
+-rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Amino_acid_image.png
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Anhydride_image.png
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Azide_image.png
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Benzene_image.png
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Bromide_image.png
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Carbonate2_image.png
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Carbonate_image.png
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Disulfide_image.png
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Enamine2_image.png
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Enamine_2_image.png
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Enamine_image.png
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Enol_image.png
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Ester_image.png
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Ether_image.png
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Fluoride_image.png
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Halogen_image.png
+-rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Hemiacetal_image.png
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Imide_image.png
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Imine_image.png
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Iodide_image.png
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Ketone_image.png
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Nitrile_image.png
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Nitro_image.png
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Peroxide_image.png
+-rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Phosphate_image.png
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Phosphine_image.png
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Proline_image.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Sulfides_image.png
+-rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Sulfone_image.png
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Sulfonic_acid_image.png
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Sulfoxide_image.png
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Thio_ether_image.png
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Thioester_image.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/Thiol_image.png
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.3/src/MASSiveChem/data/Functional groups images/molecule_image.png
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 massivechem-3.3/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 massivechem-3.3/LICENSE.txt
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 massivechem-3.3/README.md
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 massivechem-3.3/pyproject.toml
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 massivechem-3.3/PKG-INFO
```

### Comparing `massivechem-3.2/project_CH200.yml` & `massivechem-3.3/project_CH200.yml`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/project_final.yml` & `massivechem-3.3/project_final.yml`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/THOMAS_IS_BEST/COPIED_VERSION.py` & `massivechem-3.3/THOMAS_IS_BEST/COPIED_VERSION.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/THOMAS_IS_BEST/Preliminary_v2.py` & `massivechem-3.3/THOMAS_IS_BEST/Preliminary_v2.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/THOMAS_IS_BEST/abundance.txt` & `massivechem-3.3/THOMAS_IS_BEST/abundance.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/THOMAS_IS_BEST/abundance_simplified.txt` & `massivechem-3.3/THOMAS_IS_BEST/abundance_simplified.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/THOMAS_IS_BEST/big_func.html` & `massivechem-3.3/THOMAS_IS_BEST/big_func.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/THOMAS_IS_BEST/big_func.py` & `massivechem-3.3/THOMAS_IS_BEST/big_func.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/THOMAS_IS_BEST/copy_file.py` & `massivechem-3.3/THOMAS_IS_BEST/copy_file.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/THOMAS_IS_BEST/functional_group_finder.py` & `massivechem-3.3/THOMAS_IS_BEST/functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/THOMAS_IS_BEST/functions.html` & `massivechem-3.3/THOMAS_IS_BEST/functions.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/THOMAS_IS_BEST/functions.py` & `massivechem-3.3/THOMAS_IS_BEST/functions.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/THOMAS_IS_BEST/test.py` & `massivechem-3.3/THOMAS_IS_BEST/test.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/Thomas/Copy_spectrometer.py` & `massivechem-3.3/Thomas/Copy_spectrometer.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/Thomas/Thomas_return_pyplot.py` & `massivechem-3.3/Thomas/Thomas_return_pyplot.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/Thomas/tests.py` & `massivechem-3.3/Thomas/tests.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/abundance.txt` & `massivechem-3.3/data/abundance.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Acid_image.png` & `massivechem-3.3/data/Functional groups images/Acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Acyl_chloride_image.png` & `massivechem-3.3/data/Functional groups images/Acyl_chloride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Alcohol_image.png` & `massivechem-3.3/data/Functional groups images/Alcohol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Aldehyde_image.png` & `massivechem-3.3/data/Functional groups images/Aldehyde_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Alkene_image.png` & `massivechem-3.3/data/Functional groups images/Alkene_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Alkyne_image.png` & `massivechem-3.3/data/Functional groups images/Alkyne_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Amide_image.png` & `massivechem-3.3/data/Functional groups images/Amide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Amine_image.png` & `massivechem-3.3/data/Functional groups images/Amine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Amino_acid_image.png` & `massivechem-3.3/data/Functional groups images/Amino_acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Anhydride_image.png` & `massivechem-3.3/data/Functional groups images/Anhydride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Azide_image.png` & `massivechem-3.3/data/Functional groups images/Azide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Benzene_image.png` & `massivechem-3.3/data/Functional groups images/Benzene_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Bromide_image.png` & `massivechem-3.3/data/Functional groups images/Bromide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Carbonate2_image.png` & `massivechem-3.3/data/Functional groups images/Carbonate2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Carbonate_image.png` & `massivechem-3.3/data/Functional groups images/Carbonate_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Disulfide_image.png` & `massivechem-3.3/data/Functional groups images/Disulfide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Enamine2_image.png` & `massivechem-3.3/data/Functional groups images/Enamine2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Enamine_2_image.png` & `massivechem-3.3/data/Functional groups images/Enamine_2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Enamine_image.png` & `massivechem-3.3/data/Functional groups images/Enamine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Enol_image.png` & `massivechem-3.3/data/Functional groups images/Enol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Ester_image.png` & `massivechem-3.3/data/Functional groups images/Ester_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Ether_image.png` & `massivechem-3.3/data/Functional groups images/Ether_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Fluoride_image.png` & `massivechem-3.3/data/Functional groups images/Fluoride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Halogen_image.png` & `massivechem-3.3/data/Functional groups images/Halogen_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Hemiacetal_image.png` & `massivechem-3.3/data/Functional groups images/Hemiacetal_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Imide_image.png` & `massivechem-3.3/data/Functional groups images/Imide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Imine_image.png` & `massivechem-3.3/data/Functional groups images/Imine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Iodide_image.png` & `massivechem-3.3/data/Functional groups images/Iodide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Ketone_image.png` & `massivechem-3.3/data/Functional groups images/Ketone_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Nitrile_image.png` & `massivechem-3.3/data/Functional groups images/Nitrile_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Nitro_image.png` & `massivechem-3.3/data/Functional groups images/Nitro_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Peroxide_image.png` & `massivechem-3.3/data/Functional groups images/Peroxide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Phosphate_image.png` & `massivechem-3.3/data/Functional groups images/Phosphate_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Phosphine_image.png` & `massivechem-3.3/data/Functional groups images/Phosphine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Proline_image.png` & `massivechem-3.3/data/Functional groups images/Proline_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Sulfides_image.png` & `massivechem-3.3/data/Functional groups images/Sulfides_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Sulfone_image.png` & `massivechem-3.3/data/Functional groups images/Sulfone_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Sulfonic_acid_image.png` & `massivechem-3.3/data/Functional groups images/Sulfonic_acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Sulfoxide_image.png` & `massivechem-3.3/data/Functional groups images/Sulfoxide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Thio_ether_image.png` & `massivechem-3.3/data/Functional groups images/Thio_ether_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Thioester_image.png` & `massivechem-3.3/data/Functional groups images/Thioester_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/Thiol_image.png` & `massivechem-3.3/data/Functional groups images/Thiol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/data/Functional groups images/molecule_image.png` & `massivechem-3.3/data/Functional groups images/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/SMILEs_interpreter.py` & `massivechem-3.3/scripts/SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/all_in_one.py` & `massivechem-3.3/scripts/all_in_one.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/data_list_generator.py` & `massivechem-3.3/scripts/data_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/delete_mol_image_file.py` & `massivechem-3.3/scripts/delete_mol_image_file.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/delta_function_plotter.py` & `massivechem-3.3/scripts/delta_function_plotter.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/double_plot.py` & `massivechem-3.3/scripts/double_plot.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/functional_group_finder.py` & `massivechem-3.3/scripts/functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/functional_list_display.py` & `massivechem-3.3/scripts/functional_list_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/insaturation.py` & `massivechem-3.3/scripts/insaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/ionisation_method.py` & `massivechem-3.3/scripts/ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/main_function.py` & `massivechem-3.3/scripts/main_function.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/mol_web_show.py` & `massivechem-3.3/scripts/mol_web_show.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/molecule_list_generator.py` & `massivechem-3.3/scripts/molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/peak_merger.py` & `massivechem-3.3/scripts/peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/save_molecule_image_to_file.py` & `massivechem-3.3/scripts/save_molecule_image_to_file.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/scripts/spectrum.html` & `massivechem-3.3/scripts/spectrum.html`

 * *Files 13% similar despite different names*

```diff
@@ -16,27 +16,27 @@
     <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-widgets-3.4.1.min.js"></script>
     <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-tables-3.4.1.min.js"></script>
     <script type="text/javascript">
         Bokeh.set_log_level("info");
     </script>
   </head>
   <body>
-    <div id="eaf775c9-b03b-464f-9352-d9eddc67a71b" data-root-id="p1287" style="display: contents;"></div>
+    <div id="b161d680-e8bb-478c-bec0-c1cfcee2a4dc" data-root-id="p1287" style="display: contents;"></div>
   
-    <script type="application/json" id="bd2090b9-ac4c-4f9c-8102-6850dcd4affe">
-      {"7bdc3857-cd80-464f-afe8-4a1810b59148":{"version":"3.4.1","title":"Bokeh Application","roots":[{"type":"object","name":"Row","id":"p1287","attributes":{"children":[{"type":"object","name":"Column","id":"p1226","attributes":{"children":[{"type":"object","name":"Figure","id":"p1066","attributes":{"height":500,"x_range":{"type":"object","name":"DataRange1d","id":"p1067","attributes":{"js_property_callbacks":{"type":"map","entries":[["change:start",[{"type":"object","name":"CustomJS","id":"p1224","attributes":{"args":{"type":"map","entries":[["box",{"type":"object","name":"BoxAnnotation","id":"p1219","attributes":{"left":0,"right":0,"top":0,"bottom":0,"line_color":"red","fill_color":"cornflowerblue","fill_alpha":0.1}}]]},"code":"\n        box['left'] = cb_obj.start\n        box['right'] = cb_obj.end\n    "}}]],["change:end",[{"id":"p1224"}]]]}}},"y_range":{"type":"object","name":"DataRange1d","id":"p1068","attributes":{"js_property_callbacks":{"type":"map","entries":[["change:start",[{"type":"object","name":"CustomJS","id":"p1225","attributes":{"args":{"type":"map","entries":[["box",{"id":"p1219"}]]},"code":"\n        box['bottom'] = cb_obj.start\n        box['top'] = cb_obj.end\n    "}}]],["change:end",[{"id":"p1225"}]]]}}},"x_scale":{"type":"object","name":"LinearScale","id":"p1075"},"y_scale":{"type":"object","name":"LinearScale","id":"p1076"},"title":{"type":"object","name":"Title","id":"p1073"},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1107","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1101","attributes":{"selected":{"type":"object","name":"Selection","id":"p1102","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1103"},"data":{"type":"map","entries":[["x",[88.842,89.042,89.042,89.042,90.0425,90.0425,90.0425,90.04650000000001,90.04650000000001,90.04650000000001,91.038,91.038,91.038,91.049,91.049,91.049,92.042,92.042,92.042,93.038,93.038,93.038,93.238]],["y",[0,0,0.9078494837406402,0,0,0.007262795869925122,0,0,0.04878116844702188,0,0,0.04022359846924959,0,0,0.00067384170792336,0,0,0.0017895230865995768,0,0,0.00019108597847624506,0,0]]]}}},"view":{"type":"object","name":"CDSView","id":"p1108","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1109"}}},"glyph":{"type":"object","name":"Line","id":"p1104","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4"}},"nonselection_glyph":{"type":"object","name":"Line","id":"p1105","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.1}},"muted_glyph":{"type":"object","name":"Line","id":"p1106","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.2}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1074","attributes":{"tools":[{"type":"object","name":"PanTool","id":"p1087"},{"type":"object","name":"WheelZoomTool","id":"p1088","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1089","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1090","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1095"},{"type":"object","name":"ResetTool","id":"p1096"},{"type":"object","name":"HelpTool","id":"p1097"},{"type":"object","name":"WheelPanTool","id":"p1099","attributes":{"dimension":"height"}},{"type":"object","name":"WheelZoomTool","id":"p1100","attributes":{"dimensions":"height","renderers":"auto"}}]}},"left":[{"type":"object","name":"LinearAxis","id":"p1082","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1083","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1084"},"axis_label":"Abundance","major_label_policy":{"type":"object","name":"AllLabels","id":"p1085"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1077","attributes":{"ticker":{"type":"object","name":"FixedTicker","id":"p1098","attributes":{"ticks":[89.042,90.0425,90.04650000000001,91.038,92.042],"minor_ticks":[]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1079"},"axis_label":"[m/z]","major_label_policy":{"type":"object","name":"AllLabels","id":"p1080"}}}],"center":[{"type":"object","name":"Grid","id":"p1081","attributes":{"axis":{"id":"p1077"}}},{"type":"object","name":"Grid","id":"p1086","attributes":{"dimension":1,"axis":{"id":"p1082"}}}]}},{"type":"object","name":"Figure","id":"p1176","attributes":{"height":250,"x_range":{"type":"object","name":"DataRange1d","id":"p1177"},"y_range":{"type":"object","name":"DataRange1d","id":"p1178"},"x_scale":{"type":"object","name":"LinearScale","id":"p1185"},"y_scale":{"type":"object","name":"LinearScale","id":"p1186"},"title":{"type":"object","name":"Title","id":"p1183"},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1214","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1208","attributes":{"selected":{"type":"object","name":"Selection","id":"p1209","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1210"},"data":{"type":"map","entries":[["x",[88.842,89.042,89.042,89.042,90.0425,90.0425,90.0425,90.04650000000001,90.04650000000001,90.04650000000001,91.038,91.038,91.038,91.049,91.049,91.049,92.042,92.042,92.042,93.038,93.038,93.038,93.238]],["y",[0,0,0.9078494837406402,0,0,0.007262795869925122,0,0,0.04878116844702188,0,0,0.04022359846924959,0,0,0.00067384170792336,0,0,0.0017895230865995768,0,0,0.00019108597847624506,0,0]]]}}},"view":{"type":"object","name":"CDSView","id":"p1215","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1216"}}},"glyph":{"type":"object","name":"Line","id":"p1211","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4"}},"nonselection_glyph":{"type":"object","name":"Line","id":"p1212","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.1}},"muted_glyph":{"type":"object","name":"Line","id":"p1213","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.2}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1184","attributes":{"tools":[{"type":"object","name":"PanTool","id":"p1197"},{"type":"object","name":"WheelZoomTool","id":"p1198","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1199","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1200","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1205"},{"type":"object","name":"ResetTool","id":"p1206"},{"type":"object","name":"HelpTool","id":"p1207"}]}},"toolbar_location":null,"left":[{"type":"object","name":"LinearAxis","id":"p1192","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1193","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1194"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1195"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1187","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1188","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1189"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1190"}}}],"center":[{"type":"object","name":"Grid","id":"p1191","attributes":{"axis":{"id":"p1187"}}},{"type":"object","name":"Grid","id":"p1196","attributes":{"dimension":1,"axis":{"id":"p1192"}}},{"type":"object","name":"Legend","id":"p1217","attributes":{"items":[{"type":"object","name":"LegendItem","id":"p1218","attributes":{"label":{"type":"value","value":"Mass spectrum"},"renderers":[{"id":"p1214"}]}}]}},{"id":"p1219"}]}}]}},{"type":"object","name":"Column","id":"p1286","attributes":{"children":[{"type":"object","name":"Figure","id":"p1227","attributes":{"width":350,"height":350,"x_range":{"type":"object","name":"Range1d","id":"p1236"},"y_range":{"type":"object","name":"Range1d","id":"p1237"},"x_scale":{"type":"object","name":"LinearScale","id":"p1238"},"y_scale":{"type":"object","name":"LinearScale","id":"p1239"},"title":{"type":"object","name":"Title","id":"p1234"},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1267","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1261","attributes":{"selected":{"type":"object","name":"Selection","id":"p1262","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1263"},"data":{"type":"map","entries":[["url",["/Users/thomaschristiansson/Documents/GitHub/ppchem-project-Christiansson-Gonteri-Humery/molecule_image.png"]]]}}},"view":{"type":"object","name":"CDSView","id":"p1268","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1269"}}},"glyph":{"type":"object","name":"ImageURL","id":"p1264","attributes":{"url":{"type":"field","field":"url"},"x":{"type":"value","value":0},"y":{"type":"value","value":1},"w":{"type":"value","value":1},"h":{"type":"value","value":1}}},"nonselection_glyph":{"type":"object","name":"ImageURL","id":"p1265","attributes":{"url":{"type":"field","field":"url"},"x":{"type":"value","value":0},"y":{"type":"value","value":1},"w":{"type":"value","value":1},"h":{"type":"value","value":1},"global_alpha":{"type":"value","value":0.1}}},"muted_glyph":{"type":"object","name":"ImageURL","id":"p1266","attributes":{"url":{"type":"field","field":"url"},"x":{"type":"value","value":0},"y":{"type":"value","value":1},"w":{"type":"value","value":1},"h":{"type":"value","value":1},"global_alpha":{"type":"value","value":0.2}}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1235","attributes":{"tools":[{"type":"object","name":"PanTool","id":"p1250"},{"type":"object","name":"WheelZoomTool","id":"p1251","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1252","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1253","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1258"},{"type":"object","name":"ResetTool","id":"p1259"},{"type":"object","name":"HelpTool","id":"p1260"}]}},"toolbar_location":null,"left":[{"type":"object","name":"LinearAxis","id":"p1245","attributes":{"visible":false,"ticker":{"type":"object","name":"BasicTicker","id":"p1246","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1247"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1248"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1240","attributes":{"visible":false,"ticker":{"type":"object","name":"BasicTicker","id":"p1241","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1242"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1243"}}}],"center":[{"type":"object","name":"Grid","id":"p1244","attributes":{"axis":{"id":"p1240"},"grid_line_color":null}},{"type":"object","name":"Grid","id":"p1249","attributes":{"dimension":1,"axis":{"id":"p1245"},"grid_line_color":null}}]}},{"type":"object","name":"DataTable","id":"p1280","attributes":{"width":250,"height":260,"source":{"type":"object","name":"ColumnDataSource","id":"p1270","attributes":{"selected":{"type":"object","name":"Selection","id":"p1271","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1272"},"data":{"type":"map","entries":[["groups",["Sulfide"]],["images",["&lt;img src=\"../data/Functional groups images/Sulfides_image.png\" style=\"width:50px;height:50px;\"&gt;"]]]}}},"view":{"type":"object","name":"CDSView","id":"p1284","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1285"}}},"columns":[{"type":"object","name":"TableColumn","id":"p1273","attributes":{"field":"groups","title":"Functional Groups","formatter":{"type":"object","name":"StringFormatter","id":"p1274"},"editor":{"type":"object","name":"StringEditor","id":"p1275"}}},{"type":"object","name":"TableColumn","id":"p1277","attributes":{"field":"images","title":"Images","width":200,"formatter":{"type":"object","name":"HTMLTemplateFormatter","id":"p1276","attributes":{"template":"\n    &lt;div&gt;\n    &lt;%= value %&gt;\n    &lt;/div&gt;\n    "}},"editor":{"type":"object","name":"StringEditor","id":"p1279"}}}],"row_height":60}}]}}]}}]}}
+    <script type="application/json" id="fe2a708b-1188-4fdc-bad4-92328431300a">
+      {"b9f5ede7-e933-4c7b-ad53-7350a5fa67d0":{"version":"3.4.1","title":"Bokeh Application","roots":[{"type":"object","name":"Row","id":"p1287","attributes":{"children":[{"type":"object","name":"Column","id":"p1226","attributes":{"children":[{"type":"object","name":"Figure","id":"p1066","attributes":{"height":500,"x_range":{"type":"object","name":"DataRange1d","id":"p1067","attributes":{"js_property_callbacks":{"type":"map","entries":[["change:start",[{"type":"object","name":"CustomJS","id":"p1224","attributes":{"args":{"type":"map","entries":[["box",{"type":"object","name":"BoxAnnotation","id":"p1219","attributes":{"left":0,"right":0,"top":0,"bottom":0,"line_color":"red","fill_color":"cornflowerblue","fill_alpha":0.1}}]]},"code":"\n        box['left'] = cb_obj.start\n        box['right'] = cb_obj.end\n    "}}]],["change:end",[{"id":"p1224"}]]]}}},"y_range":{"type":"object","name":"DataRange1d","id":"p1068","attributes":{"js_property_callbacks":{"type":"map","entries":[["change:start",[{"type":"object","name":"CustomJS","id":"p1225","attributes":{"args":{"type":"map","entries":[["box",{"id":"p1219"}]]},"code":"\n        box['bottom'] = cb_obj.start\n        box['top'] = cb_obj.end\n    "}}]],["change:end",[{"id":"p1225"}]]]}}},"x_scale":{"type":"object","name":"LinearScale","id":"p1075"},"y_scale":{"type":"object","name":"LinearScale","id":"p1076"},"title":{"type":"object","name":"Title","id":"p1073"},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1107","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1101","attributes":{"selected":{"type":"object","name":"Selection","id":"p1102","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1103"},"data":{"type":"map","entries":[["x",[60.811,61.011,61.011,61.011,62.015,62.015,62.015,63.003,63.003,63.003,63.007,63.007,63.007,63.018,63.018,63.018,64.01,64.01,64.01,65.006,65.006,65.006,65.206]],["y",[0,0,0.9287137253553642,0,0,0.028685997422045542,0,0,0.007429709802842914,0,0,0.041148019193286506,0,0,0.00011488799521531493,0,0,0.0009153249972217419,0,0,0.00019547752585884323,0,0]]]}}},"view":{"type":"object","name":"CDSView","id":"p1108","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1109"}}},"glyph":{"type":"object","name":"Line","id":"p1104","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4"}},"nonselection_glyph":{"type":"object","name":"Line","id":"p1105","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.1}},"muted_glyph":{"type":"object","name":"Line","id":"p1106","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.2}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1074","attributes":{"tools":[{"type":"object","name":"PanTool","id":"p1087"},{"type":"object","name":"WheelZoomTool","id":"p1088","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1089","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1090","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1095"},{"type":"object","name":"ResetTool","id":"p1096"},{"type":"object","name":"HelpTool","id":"p1097"},{"type":"object","name":"WheelPanTool","id":"p1099","attributes":{"dimension":"height"}},{"type":"object","name":"WheelZoomTool","id":"p1100","attributes":{"dimensions":"height","renderers":"auto"}}]}},"left":[{"type":"object","name":"LinearAxis","id":"p1082","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1083","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1084"},"axis_label":"Abundance","major_label_policy":{"type":"object","name":"AllLabels","id":"p1085"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1077","attributes":{"ticker":{"type":"object","name":"FixedTicker","id":"p1098","attributes":{"ticks":[61.011,62.015,63.003,63.007],"minor_ticks":[]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1079"},"axis_label":"[m/z]","major_label_policy":{"type":"object","name":"AllLabels","id":"p1080"}}}],"center":[{"type":"object","name":"Grid","id":"p1081","attributes":{"axis":{"id":"p1077"}}},{"type":"object","name":"Grid","id":"p1086","attributes":{"dimension":1,"axis":{"id":"p1082"}}}]}},{"type":"object","name":"Figure","id":"p1176","attributes":{"height":250,"x_range":{"type":"object","name":"DataRange1d","id":"p1177"},"y_range":{"type":"object","name":"DataRange1d","id":"p1178"},"x_scale":{"type":"object","name":"LinearScale","id":"p1185"},"y_scale":{"type":"object","name":"LinearScale","id":"p1186"},"title":{"type":"object","name":"Title","id":"p1183"},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1214","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1208","attributes":{"selected":{"type":"object","name":"Selection","id":"p1209","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1210"},"data":{"type":"map","entries":[["x",[60.811,61.011,61.011,61.011,62.015,62.015,62.015,63.003,63.003,63.003,63.007,63.007,63.007,63.018,63.018,63.018,64.01,64.01,64.01,65.006,65.006,65.006,65.206]],["y",[0,0,0.9287137253553642,0,0,0.028685997422045542,0,0,0.007429709802842914,0,0,0.041148019193286506,0,0,0.00011488799521531493,0,0,0.0009153249972217419,0,0,0.00019547752585884323,0,0]]]}}},"view":{"type":"object","name":"CDSView","id":"p1215","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1216"}}},"glyph":{"type":"object","name":"Line","id":"p1211","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4"}},"nonselection_glyph":{"type":"object","name":"Line","id":"p1212","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.1}},"muted_glyph":{"type":"object","name":"Line","id":"p1213","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.2}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1184","attributes":{"tools":[{"type":"object","name":"PanTool","id":"p1197"},{"type":"object","name":"WheelZoomTool","id":"p1198","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1199","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1200","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1205"},{"type":"object","name":"ResetTool","id":"p1206"},{"type":"object","name":"HelpTool","id":"p1207"}]}},"toolbar_location":null,"left":[{"type":"object","name":"LinearAxis","id":"p1192","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1193","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1194"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1195"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1187","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1188","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1189"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1190"}}}],"center":[{"type":"object","name":"Grid","id":"p1191","attributes":{"axis":{"id":"p1187"}}},{"type":"object","name":"Grid","id":"p1196","attributes":{"dimension":1,"axis":{"id":"p1192"}}},{"type":"object","name":"Legend","id":"p1217","attributes":{"items":[{"type":"object","name":"LegendItem","id":"p1218","attributes":{"label":{"type":"value","value":"Mass spectrum"},"renderers":[{"id":"p1214"}]}}]}},{"id":"p1219"}]}}]}},{"type":"object","name":"Column","id":"p1286","attributes":{"children":[{"type":"object","name":"Figure","id":"p1227","attributes":{"width":350,"height":350,"x_range":{"type":"object","name":"Range1d","id":"p1236"},"y_range":{"type":"object","name":"Range1d","id":"p1237"},"x_scale":{"type":"object","name":"LinearScale","id":"p1238"},"y_scale":{"type":"object","name":"LinearScale","id":"p1239"},"title":{"type":"object","name":"Title","id":"p1234"},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1267","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1261","attributes":{"selected":{"type":"object","name":"Selection","id":"p1262","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1263"},"data":{"type":"map","entries":[["url",["/Users/thomaschristiansson/Documents/GitHub/ppchem-project-Christiansson-Gonteri-Humery/molecule_image.png"]]]}}},"view":{"type":"object","name":"CDSView","id":"p1268","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1269"}}},"glyph":{"type":"object","name":"ImageURL","id":"p1264","attributes":{"url":{"type":"field","field":"url"},"x":{"type":"value","value":0},"y":{"type":"value","value":1},"w":{"type":"value","value":1},"h":{"type":"value","value":1}}},"nonselection_glyph":{"type":"object","name":"ImageURL","id":"p1265","attributes":{"url":{"type":"field","field":"url"},"x":{"type":"value","value":0},"y":{"type":"value","value":1},"w":{"type":"value","value":1},"h":{"type":"value","value":1},"global_alpha":{"type":"value","value":0.1}}},"muted_glyph":{"type":"object","name":"ImageURL","id":"p1266","attributes":{"url":{"type":"field","field":"url"},"x":{"type":"value","value":0},"y":{"type":"value","value":1},"w":{"type":"value","value":1},"h":{"type":"value","value":1},"global_alpha":{"type":"value","value":0.2}}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1235","attributes":{"tools":[{"type":"object","name":"PanTool","id":"p1250"},{"type":"object","name":"WheelZoomTool","id":"p1251","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1252","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1253","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1258"},{"type":"object","name":"ResetTool","id":"p1259"},{"type":"object","name":"HelpTool","id":"p1260"}]}},"toolbar_location":null,"left":[{"type":"object","name":"LinearAxis","id":"p1245","attributes":{"visible":false,"ticker":{"type":"object","name":"BasicTicker","id":"p1246","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1247"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1248"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1240","attributes":{"visible":false,"ticker":{"type":"object","name":"BasicTicker","id":"p1241","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1242"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1243"}}}],"center":[{"type":"object","name":"Grid","id":"p1244","attributes":{"axis":{"id":"p1240"},"grid_line_color":null}},{"type":"object","name":"Grid","id":"p1249","attributes":{"dimension":1,"axis":{"id":"p1245"},"grid_line_color":null}}]}},{"type":"object","name":"DataTable","id":"p1280","attributes":{"width":250,"height":260,"source":{"type":"object","name":"ColumnDataSource","id":"p1270","attributes":{"selected":{"type":"object","name":"Selection","id":"p1271","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1272"},"data":{"type":"map","entries":[["groups",["Thiol"]],["images",["&lt;img src=\"../data/Functional groups images/Thiol_image.png\" style=\"width:50px;height:50px;\"&gt;"]]]}}},"view":{"type":"object","name":"CDSView","id":"p1284","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1285"}}},"columns":[{"type":"object","name":"TableColumn","id":"p1273","attributes":{"field":"groups","title":"Functional Groups","formatter":{"type":"object","name":"StringFormatter","id":"p1274"},"editor":{"type":"object","name":"StringEditor","id":"p1275"}}},{"type":"object","name":"TableColumn","id":"p1277","attributes":{"field":"images","title":"Images","width":200,"formatter":{"type":"object","name":"HTMLTemplateFormatter","id":"p1276","attributes":{"template":"\n    &lt;div&gt;\n    &lt;%= value %&gt;\n    &lt;/div&gt;\n    "}},"editor":{"type":"object","name":"StringEditor","id":"p1279"}}}],"row_height":60}}]}}]}}]}}
     </script>
     <script type="text/javascript">
       (function() {
         const fn = function() {
           Bokeh.safely(function() {
             (function(root) {
               function embed_document(root) {
-              const docs_json = document.getElementById('bd2090b9-ac4c-4f9c-8102-6850dcd4affe').textContent;
-              const render_items = [{"docid":"7bdc3857-cd80-464f-afe8-4a1810b59148","roots":{"p1287":"eaf775c9-b03b-464f-9352-d9eddc67a71b"},"root_ids":["p1287"]}];
+              const docs_json = document.getElementById('fe2a708b-1188-4fdc-bad4-92328431300a').textContent;
+              const render_items = [{"docid":"b9f5ede7-e933-4c7b-ad53-7350a5fa67d0","roots":{"p1287":"b161d680-e8bb-478c-bec0-c1cfcee2a4dc"},"root_ids":["p1287"]}];
               root.Bokeh.embed.embed_items(docs_json, render_items);
               }
               if (root.Bokeh !== undefined) {
                 embed_document(root);
               } else {
                 let attempts = 0;
                 const timer = setInterval(function(root) {
```

### Comparing `massivechem-3.2/scripts/spectrum.py` & `massivechem-3.3/scripts/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
         'Iodide': 'I',
         'Alkene': 'C=C',
         'Alkyne': 'C#C',
         'Imine': 'C=N*',
         'Amino acid': '[Nh2][Ch1*]C(=O)O',
         'Proline': '[Nh1][Ch1*]C(=O)O',
         'Thiol': '[Sh1]',
-        'Sulfide': '*[Sh0]*',
+        'Sulfide': '*[S]*',
         'Acyl Chloride': 'CC(=O)Cl',
         'Anhydride': '*[Ch0](=O)O[Ch0](=O)*',
         'Nitro': 'C[N+](=O)[O-]',
         'Enamine': 'C=C[Nh0]',
         'Enamine2': 'C=C[Nh1]',
         'Enamine3': 'C=C[Nh2]',
         'Imide': 'C(=O)NC(=O)*',
@@ -589,8 +589,8 @@
     data_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
 
 
     last = column(p, data_table)
     final = row(layout, last)
     return final
 
-show(spectrum('CCSCC',True,0.01))
+show(spectrum('CCS', True, 0.01))
```

### Comparing `massivechem-3.2/src/MASSiveChem/MASSiveChem.py` & `massivechem-3.3/src/MASSiveChem/MASSiveChem.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/.gitignore` & `massivechem-3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/LICENSE.txt` & `massivechem-3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/README.md` & `massivechem-3.3/README.md`

 * *Files identical despite different names*

### Comparing `massivechem-3.2/pyproject.toml` & `massivechem-3.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 4d41 5353 4956 4543 6865 6d22 0d0a   "MASSIVEChem"..
-00000070: 7665 7273 696f 6e20 3d20 2233 2e32 220d  version = "3.2".
+00000070: 7665 7273 696f 6e20 3d20 2233 2e33 220d  version = "3.3".
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 00000090: 4d41 5353 4956 4543 6865 6d20 6973 2061  MASSIVEChem is a
 000000a0: 2070 6970 2d69 6e73 7461 6c6c 6162 6c65   pip-installable
 000000b0: 2070 6163 6b61 6765 2066 6f72 2061 6e61   package for ana
 000000c0: 6c79 7469 6361 6c20 6368 656d 6973 7472  lytical chemistr
 000000d0: 792e 2049 7420 7369 6d75 6c61 7465 7320  y. It simulates 
 000000e0: 6d6f 6c65 6375 6c65 206d 6173 7320 7370  molecule mass sp
```

### Comparing `massivechem-3.2/PKG-INFO` & `massivechem-3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MASSIVEChem
-Version: 3.2
+Version: 3.3
 Summary: MASSIVEChem is a pip-installable package for analytical chemistry. It simulates molecule mass spectra and graphically displays them. It includes tools like a functional group finder and unsaturation calculator to aid chemical analysis.
 Project-URL: Homepage, https://github.com/ThomasCsson/MASSIVEChem.git
 Project-URL: GitHub_Thomas_Christiansson, https://github.com/ThomasCsson
 Project-URL: GitHub_Igor_Gonteri, https://github.com/igorgonteri
 Project-URL: GitHub_Arthur_Humery, https://github.com/Arthurhmy
 Author-email: Thomas Viking Christiansson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
```

