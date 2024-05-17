# Comparing `tmp/t4_geom_convert-1.0.0.tar.gz` & `tmp/t4_geom_convert-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t4_geom_convert-1.0.0.tar", max compression
+gzip compressed data, was "t4_geom_convert-1.1.0.tar", max compression
```

## Comparing `t4_geom_convert-1.0.0.tar` & `t4_geom_convert-1.1.0.tar`

### file list

```diff
@@ -1,95 +1,96 @@
--rw-r--r--   0        0        0    35141 2020-01-07 12:20:18.320103 t4_geom_convert-1.0.0/MIP/LICENSE
--rw-r--r--   0        0        0        0 2019-07-23 12:07:01.746772 t4_geom_convert-1.0.0/MIP/__init__.py
--rw-r--r--   0        0        0        0 2019-07-23 12:06:54.208901 t4_geom_convert-1.0.0/MIP/geom/__init__.py
--rw-r--r--   0        0        0     2427 2021-07-05 09:19:23.710002 t4_geom_convert-1.0.0/MIP/geom/another_parser.py
--rw-r--r--   0        0        0     1393 2020-02-21 09:29:30.758624 t4_geom_convert-1.0.0/MIP/geom/cells.py
--rw-r--r--   0        0        0      551 2021-07-02 09:46:22.102009 t4_geom_convert-1.0.0/MIP/geom/composition.py
--rw-r--r--   0        0        0     2461 2019-07-23 12:06:54.244872 t4_geom_convert-1.0.0/MIP/geom/copt.py
--rw-r--r--   0        0        0    14112 2022-02-25 21:02:37.966808 t4_geom_convert-1.0.0/MIP/geom/forcad.py
--rw-r--r--   0        0        0      364 2019-07-23 12:06:54.262904 t4_geom_convert-1.0.0/MIP/geom/grammars/__init__.py
--rw-r--r--   0        0        0      340 2021-07-02 09:46:22.107010 t4_geom_convert-1.0.0/MIP/geom/grammars/geom.ebnf
--rw-r--r--   0        0        0     1699 2020-02-21 09:29:30.776628 t4_geom_convert-1.0.0/MIP/geom/grammars/multioperand.py
--rw-r--r--   0        0        0     3695 2023-11-07 17:34:40.529166 t4_geom_convert-1.0.0/MIP/geom/main.py
--rw-r--r--   0        0        0     2704 2020-02-21 09:29:30.780622 t4_geom_convert-1.0.0/MIP/geom/parsegeom.py
--rw-r--r--   0        0        0     3057 2021-07-05 09:19:23.713988 t4_geom_convert-1.0.0/MIP/geom/semantics.py
--rw-r--r--   0        0        0      859 2021-07-05 09:19:23.716988 t4_geom_convert-1.0.0/MIP/geom/surfaces.py
--rw-r--r--   0        0        0     1394 2019-07-23 12:06:54.360873 t4_geom_convert-1.0.0/MIP/geom/testgrammar.py
--rw-r--r--   0        0        0     1756 2022-03-03 10:29:08.794011 t4_geom_convert-1.0.0/MIP/geom/transforms.py
--rw-r--r--   0        0        0       49 2019-07-23 12:06:54.390871 t4_geom_convert-1.0.0/MIP/mip/__init__.py
--rw-r--r--   0        0        0     3088 2021-07-05 09:19:23.719998 t4_geom_convert-1.0.0/MIP/mip/blocks.py
--rw-r--r--   0        0        0     3697 2021-07-02 09:46:22.156011 t4_geom_convert-1.0.0/MIP/mip/cards.py
--rw-r--r--   0        0        0     3035 2021-07-05 09:19:23.723003 t4_geom_convert-1.0.0/MIP/mip/cellcard.py
--rw-r--r--   0        0        0     5144 2021-07-05 09:19:23.726989 t4_geom_convert-1.0.0/MIP/mip/datacard.py
--rw-r--r--   0        0        0     4830 2021-07-05 09:19:23.729992 t4_geom_convert-1.0.0/MIP/mip/main.py
--rw-r--r--   0        0        0      985 2019-07-23 12:06:54.506881 t4_geom_convert-1.0.0/MIP/mip/readme.rst
--rw-r--r--   0        0        0      386 2019-07-23 12:06:54.509911 t4_geom_convert-1.0.0/MIP/mip/surfacecard.py
--rw-r--r--   0        0        0      763 2019-07-23 12:06:54.516881 t4_geom_convert-1.0.0/MIP/mip/utils.py
--rw-r--r--   0        0        0     1073 2019-07-23 12:06:54.553872 t4_geom_convert-1.0.0/MIP/tests.py
--rw-r--r--   0        0        0    10140 2021-07-02 09:46:22.246004 t4_geom_convert-1.0.0/README.md
--rw-r--r--   0        0        0     4318 2023-11-08 14:01:52.582079 t4_geom_convert-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      966 2021-07-02 09:46:22.608020 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/BoundaryCondition/CBoundCond.py
--rw-r--r--   0        0        0     2192 2021-07-02 09:46:22.611003 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/BoundaryCondition/CConversionBoundaryCondition.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.614004 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/BoundaryCondition/__init__.py
--rw-r--r--   0        0        0     1698 2022-10-10 08:13:16.765702 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/Abundances.py
--rw-r--r--   0        0        0     1784 2021-07-02 09:46:22.620008 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/CCompositionMCNP.py
--rw-r--r--   0        0        0     1273 2021-07-02 09:46:22.623004 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/CCompositionT4.py
--rw-r--r--   0        0        0     1692 2021-07-02 09:46:22.626003 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/CDictCompositionMCNP.py
--rw-r--r--   0        0        0     3224 2022-10-10 08:13:16.985692 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/CompositionConversionMCNPToT4.py
--rw-r--r--   0        0        0     4271 2022-10-10 08:13:17.228693 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/ConstructCompositionT4.py
--rw-r--r--   0        0        0     1165 2021-07-02 09:46:22.635003 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/ConvertIsotope.py
--rw-r--r--   0        0        0     1483 2021-07-02 09:46:22.637009 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/EIsotopeAtomicNumberMCNP.py
--rw-r--r--   0        0        0     1419 2021-07-02 09:46:22.640000 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/EIsotopeNameElementT4.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.643003 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/__init__.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.646013 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Configuration/__init__.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.650007 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Exceptions/__init__.py
--rw-r--r--   0        0        0    14497 2023-11-07 17:34:40.574179 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPCell.py
--rw-r--r--   0        0        0     1529 2021-07-02 09:46:22.671006 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPComposition.py
--rw-r--r--   0        0        0     5944 2022-10-10 08:13:17.713686 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPSurface.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.690003 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Parser/__init__.py
--rw-r--r--   0        0        0     1434 2021-07-02 09:46:22.693002 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4BoundCond.py
--rw-r--r--   0        0        0     2865 2022-10-10 08:13:17.984694 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Composition.py
--rw-r--r--   0        0        0     1432 2021-07-02 09:46:22.698001 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4GeomComp.py
--rw-r--r--   0        0        0     5847 2022-10-10 08:13:18.290686 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Geometry.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.703007 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Writer/__init__.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.706999 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/__init__.py
--rw-r--r--   0        0        0     1493 2021-07-02 09:46:22.710003 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/GeomComp/CDictGeomCompT4.py
--rw-r--r--   0        0        0     1122 2021-07-02 09:46:22.712006 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/GeomComp/CGeomCompT4.py
--rw-r--r--   0        0        0     2047 2021-07-02 09:46:22.714010 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/GeomComp/ConstructGeomCompT4.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.717010 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/GeomComp/__init__.py
--rw-r--r--   0        0        0     2259 2022-10-10 08:13:18.524687 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Progress.py
--rw-r--r--   0        0        0     1366 2021-07-02 09:46:22.722010 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/CTransformationMCNP.py
--rw-r--r--   0        0        0     7036 2022-10-10 08:13:18.848685 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/CollectionDict.py
--rw-r--r--   0        0        0     1247 2022-02-23 12:53:03.770956 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/ConstructSurfaceT4.py
--rw-r--r--   0        0        0     9136 2022-10-10 08:13:19.083688 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/ConversionSurfaceMCNPToT4.py
--rw-r--r--   0        0        0     2721 2021-07-02 09:46:22.735005 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/DTypeConversion.py
--rw-r--r--   0        0        0     2317 2022-02-23 15:04:09.442326 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/Duplicates.py
--rw-r--r--   0        0        0     1597 2022-10-10 08:13:19.356675 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/ESurfaceTypeMCNP.py
--rw-r--r--   0        0        0     1011 2021-07-02 09:46:22.743001 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/ESurfaceTypeT4.py
--rw-r--r--   0        0        0    14833 2022-10-10 08:13:19.683699 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/MacroBodies.py
--rw-r--r--   0        0        0     2344 2022-10-10 08:13:19.918672 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/SurfaceCollection.py
--rw-r--r--   0        0        0      944 2021-07-02 09:46:22.750006 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/SurfaceConversionError.py
--rw-r--r--   0        0        0     1881 2022-10-10 08:13:20.152669 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/SurfaceMCNP.py
--rw-r--r--   0        0        0     3786 2022-10-10 08:13:20.360676 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/SurfaceT4.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.758998 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/__init__.py
--rw-r--r--   0        0        0    16355 2022-10-10 08:13:20.626679 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Transformation/Transformation.py
--rw-r--r--   0        0        0      988 2021-07-02 09:46:22.781001 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Transformation/TransformationError.py
--rw-r--r--   0        0        0     2931 2022-10-10 08:13:20.825327 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Transformation/TransformationQuad.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.786998 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Transformation/__init__.py
--rw-r--r--   0        0        0     2263 2021-07-05 09:19:23.949984 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Utils.py
--rw-r--r--   0        0        0    10819 2022-10-10 08:13:21.083311 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/VectUtils.py
--rw-r--r--   0        0        0     1204 2021-07-02 09:46:22.795998 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/ByUniverse.py
--rw-r--r--   0        0        0    21087 2023-03-23 14:23:26.078094 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/CellConversion.py
--rw-r--r--   0        0        0      983 2021-07-02 09:46:22.801001 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/CellConversionError.py
--rw-r--r--   0        0        0     4651 2021-07-02 09:46:22.803998 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/CellInlining.py
--rw-r--r--   0        0        0     3129 2023-03-23 14:23:25.791091 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/CellMCNP.py
--rw-r--r--   0        0        0     9265 2023-11-08 08:38:59.076417 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/ConstructVolumeT4.py
--rw-r--r--   0        0        0     1628 2021-07-02 09:46:22.823001 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/DictVolumeT4.py
--rw-r--r--   0        0        0    22672 2023-03-28 11:54:19.358217 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/Lattice.py
--rw-r--r--   0        0        0     3379 2021-07-02 09:46:22.828006 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/TreeFunctions.py
--rw-r--r--   0        0        0     2745 2022-10-10 08:13:22.410655 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/VolumeT4.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.834004 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/__init__.py
--rw-r--r--   0        0        0      792 2021-07-02 09:46:22.837000 t4_geom_convert-1.0.0/t4_geom_convert/Kernel/__init__.py
--rw-r--r--   0        0        0      960 2021-07-02 09:46:22.856998 t4_geom_convert-1.0.0/t4_geom_convert/__init__.py
--rw-r--r--   0        0        0     8289 2022-10-10 08:13:23.503675 t4_geom_convert-1.0.0/t4_geom_convert/conftest.py
--rw-r--r--   0        0        0     9457 2022-10-10 08:13:23.759324 t4_geom_convert-1.0.0/t4_geom_convert/main.py
--rw-r--r--   0        0        0    11475 1970-01-01 00:00:00.000000 t4_geom_convert-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2019-07-23 12:07:01.736765 t4_geom_convert-1.1.0/COPYING
+-rw-r--r--   0        0        0    35141 2020-01-07 12:20:18.320103 t4_geom_convert-1.1.0/MIP/LICENSE
+-rw-r--r--   0        0        0        0 2019-07-23 12:07:01.746772 t4_geom_convert-1.1.0/MIP/__init__.py
+-rw-r--r--   0        0        0        0 2019-07-23 12:06:54.208901 t4_geom_convert-1.1.0/MIP/geom/__init__.py
+-rw-r--r--   0        0        0     2427 2021-07-05 09:19:23.710002 t4_geom_convert-1.1.0/MIP/geom/another_parser.py
+-rw-r--r--   0        0        0     1393 2020-02-21 09:29:30.758624 t4_geom_convert-1.1.0/MIP/geom/cells.py
+-rw-r--r--   0        0        0      551 2021-07-02 09:46:22.102009 t4_geom_convert-1.1.0/MIP/geom/composition.py
+-rw-r--r--   0        0        0     2461 2019-07-23 12:06:54.244872 t4_geom_convert-1.1.0/MIP/geom/copt.py
+-rw-r--r--   0        0        0    14112 2022-02-25 21:02:37.966808 t4_geom_convert-1.1.0/MIP/geom/forcad.py
+-rw-r--r--   0        0        0      364 2019-07-23 12:06:54.262904 t4_geom_convert-1.1.0/MIP/geom/grammars/__init__.py
+-rw-r--r--   0        0        0      340 2021-07-02 09:46:22.107010 t4_geom_convert-1.1.0/MIP/geom/grammars/geom.ebnf
+-rw-r--r--   0        0        0     1699 2020-02-21 09:29:30.776628 t4_geom_convert-1.1.0/MIP/geom/grammars/multioperand.py
+-rw-r--r--   0        0        0     3695 2023-11-08 15:58:36.887629 t4_geom_convert-1.1.0/MIP/geom/main.py
+-rw-r--r--   0        0        0     2704 2020-02-21 09:29:30.780622 t4_geom_convert-1.1.0/MIP/geom/parsegeom.py
+-rw-r--r--   0        0        0     3057 2021-07-05 09:19:23.713988 t4_geom_convert-1.1.0/MIP/geom/semantics.py
+-rw-r--r--   0        0        0      859 2021-07-05 09:19:23.716988 t4_geom_convert-1.1.0/MIP/geom/surfaces.py
+-rw-r--r--   0        0        0     1394 2019-07-23 12:06:54.360873 t4_geom_convert-1.1.0/MIP/geom/testgrammar.py
+-rw-r--r--   0        0        0     1756 2022-03-03 10:29:08.794011 t4_geom_convert-1.1.0/MIP/geom/transforms.py
+-rw-r--r--   0        0        0       49 2019-07-23 12:06:54.390871 t4_geom_convert-1.1.0/MIP/mip/__init__.py
+-rw-r--r--   0        0        0     3088 2021-07-05 09:19:23.719998 t4_geom_convert-1.1.0/MIP/mip/blocks.py
+-rw-r--r--   0        0        0     3697 2021-07-02 09:46:22.156011 t4_geom_convert-1.1.0/MIP/mip/cards.py
+-rw-r--r--   0        0        0     3035 2021-07-05 09:19:23.723003 t4_geom_convert-1.1.0/MIP/mip/cellcard.py
+-rw-r--r--   0        0        0     5144 2021-07-05 09:19:23.726989 t4_geom_convert-1.1.0/MIP/mip/datacard.py
+-rw-r--r--   0        0        0     4830 2021-07-05 09:19:23.729992 t4_geom_convert-1.1.0/MIP/mip/main.py
+-rw-r--r--   0        0        0      985 2019-07-23 12:06:54.506881 t4_geom_convert-1.1.0/MIP/mip/readme.rst
+-rw-r--r--   0        0        0      386 2019-07-23 12:06:54.509911 t4_geom_convert-1.1.0/MIP/mip/surfacecard.py
+-rw-r--r--   0        0        0      763 2019-07-23 12:06:54.516881 t4_geom_convert-1.1.0/MIP/mip/utils.py
+-rw-r--r--   0        0        0     1073 2019-07-23 12:06:54.553872 t4_geom_convert-1.1.0/MIP/tests.py
+-rw-r--r--   0        0        0    10140 2021-07-02 09:46:22.246004 t4_geom_convert-1.1.0/README.md
+-rw-r--r--   0        0        0     4318 2024-05-17 06:41:30.216573 t4_geom_convert-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      975 2024-05-17 06:41:30.232574 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/BoundaryCondition/CBoundCond.py
+-rw-r--r--   0        0        0     2201 2024-05-17 06:41:30.236583 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/BoundaryCondition/CConversionBoundaryCondition.py
+-rw-r--r--   0        0        0      801 2024-05-17 06:41:30.240585 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/BoundaryCondition/__init__.py
+-rw-r--r--   0        0        0     1707 2024-05-17 06:41:30.244594 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/Abundances.py
+-rw-r--r--   0        0        0     1793 2024-05-17 06:41:30.249573 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/CCompositionMCNP.py
+-rw-r--r--   0        0        0     1282 2024-05-17 06:41:30.253571 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/CCompositionT4.py
+-rw-r--r--   0        0        0     1701 2024-05-17 06:41:30.257576 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/CDictCompositionMCNP.py
+-rw-r--r--   0        0        0     3233 2024-05-17 06:41:30.261571 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/CompositionConversionMCNPToT4.py
+-rw-r--r--   0        0        0     4280 2024-05-17 06:41:30.264590 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/ConstructCompositionT4.py
+-rw-r--r--   0        0        0     1174 2024-05-17 06:41:30.268602 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/ConvertIsotope.py
+-rw-r--r--   0        0        0     1492 2024-05-17 06:41:30.272592 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/EIsotopeAtomicNumberMCNP.py
+-rw-r--r--   0        0        0     1428 2024-05-17 06:41:30.276595 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/EIsotopeNameElementT4.py
+-rw-r--r--   0        0        0      801 2024-05-17 06:41:30.280633 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/__init__.py
+-rw-r--r--   0        0        0      801 2024-05-17 06:41:30.284577 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Configuration/__init__.py
+-rw-r--r--   0        0        0      801 2024-05-17 06:41:30.287648 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Exceptions/__init__.py
+-rw-r--r--   0        0        0    14506 2024-05-17 06:41:30.292632 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPCell.py
+-rw-r--r--   0        0        0     1538 2024-05-17 06:41:30.296629 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPComposition.py
+-rw-r--r--   0        0        0     5953 2024-05-17 06:41:30.300630 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPSurface.py
+-rw-r--r--   0        0        0      801 2024-05-17 06:41:30.304622 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Parser/__init__.py
+-rw-r--r--   0        0        0     1443 2024-05-17 06:41:30.309627 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4BoundCond.py
+-rw-r--r--   0        0        0     2874 2024-05-17 06:41:30.313622 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Composition.py
+-rw-r--r--   0        0        0     1441 2024-05-17 06:41:30.317630 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4GeomComp.py
+-rw-r--r--   0        0        0     5878 2024-05-17 06:41:30.321632 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Geometry.py
+-rw-r--r--   0        0        0      801 2024-05-17 06:41:30.325641 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Writer/__init__.py
+-rw-r--r--   0        0        0      801 2024-05-17 06:41:30.329632 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/__init__.py
+-rw-r--r--   0        0        0     1502 2024-05-17 06:41:30.334625 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/GeomComp/CDictGeomCompT4.py
+-rw-r--r--   0        0        0     1131 2024-05-17 06:41:30.338625 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/GeomComp/CGeomCompT4.py
+-rw-r--r--   0        0        0     2056 2024-05-17 06:41:30.342633 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/GeomComp/ConstructGeomCompT4.py
+-rw-r--r--   0        0        0      801 2024-05-17 06:41:30.346634 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/GeomComp/__init__.py
+-rw-r--r--   0        0        0     2268 2024-05-17 06:41:30.350629 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Progress.py
+-rw-r--r--   0        0        0     1375 2024-05-17 06:41:30.355624 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/CTransformationMCNP.py
+-rw-r--r--   0        0        0     7045 2024-05-17 06:41:30.359633 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/CollectionDict.py
+-rw-r--r--   0        0        0     1256 2024-05-17 06:41:30.363636 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/ConstructSurfaceT4.py
+-rw-r--r--   0        0        0     9145 2024-05-17 06:41:30.367631 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/ConversionSurfaceMCNPToT4.py
+-rw-r--r--   0        0        0     2730 2024-05-17 06:41:30.371647 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/DTypeConversion.py
+-rw-r--r--   0        0        0     2326 2024-05-17 06:41:30.375643 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/Duplicates.py
+-rw-r--r--   0        0        0     1606 2024-05-17 06:41:30.379631 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/ESurfaceTypeMCNP.py
+-rw-r--r--   0        0        0     1020 2024-05-17 06:41:30.383638 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/ESurfaceTypeT4.py
+-rw-r--r--   0        0        0    14842 2024-05-17 06:41:30.388626 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/MacroBodies.py
+-rw-r--r--   0        0        0     2353 2024-05-17 06:41:30.392634 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/SurfaceCollection.py
+-rw-r--r--   0        0        0      953 2024-05-17 06:41:30.396627 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/SurfaceConversionError.py
+-rw-r--r--   0        0        0     1890 2024-05-17 06:41:30.400637 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/SurfaceMCNP.py
+-rw-r--r--   0        0        0     3795 2024-05-17 06:41:30.404636 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/SurfaceT4.py
+-rw-r--r--   0        0        0      801 2024-05-17 06:41:30.408632 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/__init__.py
+-rw-r--r--   0        0        0    16364 2024-05-17 06:41:30.412631 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Transformation/Transformation.py
+-rw-r--r--   0        0        0      997 2024-05-17 06:41:30.416639 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Transformation/TransformationError.py
+-rw-r--r--   0        0        0     2940 2024-05-17 06:41:30.420636 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Transformation/TransformationQuad.py
+-rw-r--r--   0        0        0      801 2024-05-17 06:41:30.424633 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Transformation/__init__.py
+-rw-r--r--   0        0        0     2272 2024-05-17 06:41:30.428634 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Utils.py
+-rw-r--r--   0        0        0    10828 2024-05-17 06:41:30.432633 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/VectUtils.py
+-rw-r--r--   0        0        0     1213 2024-05-17 06:41:30.436631 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/ByUniverse.py
+-rw-r--r--   0        0        0    21096 2024-05-17 06:41:30.440685 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/CellConversion.py
+-rw-r--r--   0        0        0      992 2024-05-17 06:41:30.444653 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/CellConversionError.py
+-rw-r--r--   0        0        0     4660 2024-05-17 06:41:30.449623 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/CellInlining.py
+-rw-r--r--   0        0        0     3138 2024-05-17 06:41:30.452704 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/CellMCNP.py
+-rw-r--r--   0        0        0     9918 2024-05-17 06:41:30.457627 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/ConstructVolumeT4.py
+-rw-r--r--   0        0        0     1637 2024-05-17 06:41:30.461645 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/DictVolumeT4.py
+-rw-r--r--   0        0        0    22681 2024-05-17 06:41:30.465676 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/Lattice.py
+-rw-r--r--   0        0        0     3388 2024-05-17 06:41:30.469659 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/TreeFunctions.py
+-rw-r--r--   0        0        0     2754 2024-05-17 06:41:30.474630 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/VolumeT4.py
+-rw-r--r--   0        0        0      801 2024-05-17 06:41:30.478632 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/__init__.py
+-rw-r--r--   0        0        0      801 2024-05-17 06:41:30.482641 t4_geom_convert-1.1.0/t4_geom_convert/Kernel/__init__.py
+-rw-r--r--   0        0        0      969 2024-05-17 06:41:30.514638 t4_geom_convert-1.1.0/t4_geom_convert/__init__.py
+-rw-r--r--   0        0        0     8298 2024-05-17 06:41:30.519625 t4_geom_convert-1.1.0/t4_geom_convert/conftest.py
+-rw-r--r--   0        0        0     9466 2024-05-17 06:41:30.523629 t4_geom_convert-1.1.0/t4_geom_convert/main.py
+-rw-r--r--   0        0        0    11475 1970-01-01 00:00:00.000000 t4_geom_convert-1.1.0/PKG-INFO
```

### Comparing `t4_geom_convert-1.0.0/MIP/LICENSE` & `t4_geom_convert-1.1.0/MIP/LICENSE`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/geom/another_parser.py` & `t4_geom_convert-1.1.0/MIP/geom/another_parser.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/geom/cells.py` & `t4_geom_convert-1.1.0/MIP/geom/cells.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/geom/composition.py` & `t4_geom_convert-1.1.0/MIP/geom/composition.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/geom/copt.py` & `t4_geom_convert-1.1.0/MIP/geom/copt.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/geom/forcad.py` & `t4_geom_convert-1.1.0/MIP/geom/forcad.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/geom/grammars/multioperand.py` & `t4_geom_convert-1.1.0/MIP/geom/grammars/multioperand.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/geom/main.py` & `t4_geom_convert-1.1.0/MIP/geom/main.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/geom/parsegeom.py` & `t4_geom_convert-1.1.0/MIP/geom/parsegeom.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/geom/semantics.py` & `t4_geom_convert-1.1.0/MIP/geom/semantics.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/geom/surfaces.py` & `t4_geom_convert-1.1.0/MIP/geom/surfaces.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/geom/testgrammar.py` & `t4_geom_convert-1.1.0/MIP/geom/testgrammar.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/geom/transforms.py` & `t4_geom_convert-1.1.0/MIP/geom/transforms.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/mip/blocks.py` & `t4_geom_convert-1.1.0/MIP/mip/blocks.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/mip/cards.py` & `t4_geom_convert-1.1.0/MIP/mip/cards.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/mip/cellcard.py` & `t4_geom_convert-1.1.0/MIP/mip/cellcard.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/mip/datacard.py` & `t4_geom_convert-1.1.0/MIP/mip/datacard.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/mip/main.py` & `t4_geom_convert-1.1.0/MIP/mip/main.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/mip/readme.rst` & `t4_geom_convert-1.1.0/MIP/mip/readme.rst`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/mip/utils.py` & `t4_geom_convert-1.1.0/MIP/mip/utils.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/MIP/tests.py` & `t4_geom_convert-1.1.0/MIP/tests.py`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/README.md` & `t4_geom_convert-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `t4_geom_convert-1.0.0/pyproject.toml` & `t4_geom_convert-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "t4_geom_convert"
-version = "1.0.0"
+version = "1.1.0"
 description = "A tool to convert MCNP geometries into the TRIPOLI-4 format"
 authors = [
   "Davide Mancusi <davide.mancusi@cea.fr>",
   "François-Xavier Hugot <francois-xavier.hugot@cea.fr>",
   "Martin Maurey",
   "Jonathan Faustin"
 ]
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/BoundaryCondition/CBoundCond.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/BoundaryCondition/CBoundCond.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/BoundaryCondition/CConversionBoundaryCondition.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/BoundaryCondition/CConversionBoundaryCondition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/BoundaryCondition/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/BoundaryCondition/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/Abundances.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/Abundances.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/CCompositionMCNP.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/CCompositionMCNP.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/CCompositionT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/CCompositionT4.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/CDictCompositionMCNP.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/CDictCompositionMCNP.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/CompositionConversionMCNPToT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/CompositionConversionMCNPToT4.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/ConstructCompositionT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/ConstructCompositionT4.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/ConvertIsotope.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/ConvertIsotope.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/EIsotopeAtomicNumberMCNP.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/EIsotopeAtomicNumberMCNP.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/EIsotopeNameElementT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/EIsotopeNameElementT4.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Composition/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Composition/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Configuration/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Configuration/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Exceptions/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Exceptions/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPCell.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPCell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPComposition.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPComposition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPSurface.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Parser/ParseMCNPSurface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Parser/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Parser/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4BoundCond.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4BoundCond.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Composition.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Composition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4GeomComp.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4GeomComp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Geometry.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Writer/WriteT4Geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -86,20 +86,20 @@
             with t4_vol_cache_path.open('wb') as dicfile:
                 abspath = t4_vol_cache_path.resolve()
                 print(f'writing cells to file {abspath}...',
                       end='', flush=True)
                 pickle.dump(vol_conv, dicfile)
                 print(' done', flush=True)
 
-    dic_volume, mcnp_new_dict, dic_surface_t4, skipped_cells = vol_conv
+    dic_volume, mcnp_new_dict, dic_surface_t4, skipped_cells, union_ids = vol_conv
     if not args.skip_deduplication:
         dic_surface_t4, renumber = remove_duplicate_surfaces(dic_surface_t4)
         dic_volume = renumber_surfaces(dic_volume, renumber)
 
-    remove_empty_volumes(dic_volume)
+    remove_empty_volumes(dic_volume, union_ids)
     remove_unused_volumes(dic_volume)
 
     return (dic_surface_mcnp, dic_surface_t4, dic_volume, mcnp_new_dict,
             skipped_cells)
 
 
 def writeT4Geometry(dic_surface_t4, dic_volume, skipped_cells, ofile):
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/Writer/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/Writer/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/FileHandlers/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/FileHandlers/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/GeomComp/CDictGeomCompT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/GeomComp/CDictGeomCompT4.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/GeomComp/CGeomCompT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/GeomComp/CGeomCompT4.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/GeomComp/ConstructGeomCompT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/GeomComp/ConstructGeomCompT4.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/GeomComp/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/GeomComp/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Progress.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/CTransformationMCNP.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/CTransformationMCNP.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/CollectionDict.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/CollectionDict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/ConstructSurfaceT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/ConstructSurfaceT4.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/ConversionSurfaceMCNPToT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/ConversionSurfaceMCNPToT4.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/DTypeConversion.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/DTypeConversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/Duplicates.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/Duplicates.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/ESurfaceTypeMCNP.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/ESurfaceTypeMCNP.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/ESurfaceTypeT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/ESurfaceTypeT4.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/MacroBodies.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/MacroBodies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/SurfaceCollection.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/SurfaceCollection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/SurfaceConversionError.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/SurfaceConversionError.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/SurfaceMCNP.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/SurfaceMCNP.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/SurfaceT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/SurfaceT4.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Surface/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Surface/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Transformation/Transformation.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Transformation/Transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Transformation/TransformationError.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Transformation/TransformationError.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Transformation/TransformationQuad.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Transformation/TransformationQuad.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Transformation/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Transformation/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Utils.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/VectUtils.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/VectUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/ByUniverse.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/ByUniverse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/CellConversion.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/CellConversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/CellConversionError.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/CellConversionError.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/CellInlining.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/CellInlining.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/CellMCNP.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/CellMCNP.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/ConstructVolumeT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/ConstructVolumeT4.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -141,15 +141,15 @@
                                           f'{key})') from None
             if j is None:
                 # the converted cell is empty
                 continue
             dic_vol_t4[key] = dic_vol_t4[j].copy()
             dic_vol_t4[key].fictive = False
 
-    return dic_vol_t4, mcnp_dict, t4_surf_numbering, skipped_cells
+    return dic_vol_t4, mcnp_dict, t4_surf_numbering, skipped_cells, union_ids
 
 
 def extract_tr_surf_ids(mcnp_dict):
     '''Return the list of MCNP surface IDs above 1000.
 
     Surface IDs above 1000 are interpreted by MCNP as (surf_id + 1000*cell_id),
     where cell_id indicates a cell with a trcl card. The surface is modified by
@@ -158,25 +158,39 @@
     tr_surf_ids = []
     for value in mcnp_dict.values():
         surfs = extract_surfaces_list(value.geometry)
         tr_surf_ids.extend(abs(int(surf)) for surf in surfs if surf >= 1000)
     return set(tr_surf_ids)
 
 
-def remove_empty_volumes(dic_volume):
+def remove_empty_volumes(dic_volume, union_ids):
     '''Remove cells that are patently empty.'''
     removed = set()
-    to_remove = [key for key, val in dic_volume.items()
-                 if val.empty() and (val.ops is None or val.ops[0] != 'UNION')]
+    to_remove = [key for key, val in dic_volume.items() if val.empty()]
 
     while to_remove:
+        removed_at_this_step = set()
         for key in to_remove:
-            del dic_volume[key]
-        removed |= set(to_remove)
+            val = dic_volume[key]
+            if val.ops is None or val.ops[0] != 'UNION':
+                # This volume is just an intersection with an empty volume, so we can
+                # remove it
+                del dic_volume[key]
+                removed_at_this_step.add(key)
+                continue
+
+            # Here val is patently empty, but it also contains a union with other
+            # volumes, so it may not be empty after all. So we replace the surface
+            # definitions with an empty volume
+            val.pluses = set([union_ids[0]])
+            val.minuses = set([union_ids[1]])
+
+        removed |= removed_at_this_step
 
+        # update the list of volumes that must be removed
         to_remove = []
         for key, val in dic_volume.items():
             if val.ops is None:
                 continue
             if val.ops[0] == 'INTE' and any(x in removed for x in val.ops[1]):
                 to_remove.append(key)
             elif val.ops[0] == 'UNION':
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/DictVolumeT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/DictVolumeT4.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/Lattice.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/Lattice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/TreeFunctions.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/TreeFunctions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/VolumeT4.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/VolumeT4.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/Volume/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/Volume/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/Kernel/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/Kernel/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/__init__.py` & `t4_geom_convert-1.1.0/t4_geom_convert/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/conftest.py` & `t4_geom_convert-1.1.0/t4_geom_convert/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/t4_geom_convert/main.py` & `t4_geom_convert-1.1.0/t4_geom_convert/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 Davide Mancusi, Martin Maurey, Jonathan Faustin
+# Copyright 2019-2024 French Alternative Energies and Atomic Energy Commission
 #
 # This file is part of t4_geom_convert.
 #
 # t4_geom_convert is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
```

### Comparing `t4_geom_convert-1.0.0/PKG-INFO` & `t4_geom_convert-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4_geom_convert
-Version: 1.0.0
+Version: 1.1.0
 Summary: A tool to convert MCNP geometries into the TRIPOLI-4 format
 Home-page: https://www.cea.fr/energies/tripoli-4/tripoli-4/pre_post_tools/t4_geom_convert/
 License: GPL-3.0-or-later
 Author: Davide Mancusi
 Author-email: davide.mancusi@cea.fr
 Maintainer: Davide Mancusi
 Maintainer-email: davide.mancusi@cea.fr
```

