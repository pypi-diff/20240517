# Comparing `tmp/imsciences-0.5.6.7.tar.gz` & `tmp/imsciences-0.5.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.6.7.tar", last modified: Thu May 16 18:50:15 2024, max compression
+gzip compressed data, was "imsciences-0.5.6.8.tar", last modified: Fri May 17 09:27:55 2024, max compression
```

## Comparing `imsciences-0.5.6.7.tar` & `imsciences-0.5.6.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 18:50:15.445846 imsciences-0.5.6.7/
--rw-rw-rw-   0        0        0     9757 2024-05-16 18:50:15.439797 imsciences-0.5.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     9252 2024-05-16 11:38:25.000000 imsciences-0.5.6.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 18:50:15.402167 imsciences-0.5.6.7/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.6.7/imsciences/__init__.py
--rw-rw-rw-   0        0        0    78308 2024-05-16 18:50:01.000000 imsciences-0.5.6.7/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:50:15.434812 imsciences-0.5.6.7/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9757 2024-05-16 18:50:15.000000 imsciences-0.5.6.7/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-16 18:50:15.000000 imsciences-0.5.6.7/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 18:50:15.000000 imsciences-0.5.6.7/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 18:50:15.000000 imsciences-0.5.6.7/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 18:50:15.000000 imsciences-0.5.6.7/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 18:50:15.445846 imsciences-0.5.6.7/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-16 18:49:23.000000 imsciences-0.5.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:27:55.099352 imsciences-0.5.6.8/
+-rw-rw-rw-   0        0        0     9976 2024-05-17 09:27:55.093823 imsciences-0.5.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.6.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 09:27:55.060779 imsciences-0.5.6.8/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.6.8/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    80446 2024-05-17 09:27:32.000000 imsciences-0.5.6.8/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:27:55.089821 imsciences-0.5.6.8/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9976 2024-05-17 09:27:54.000000 imsciences-0.5.6.8/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-17 09:27:54.000000 imsciences-0.5.6.8/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 09:27:54.000000 imsciences-0.5.6.8/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 09:27:54.000000 imsciences-0.5.6.8/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-17 09:27:54.000000 imsciences-0.5.6.8/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 09:27:55.099352 imsciences-0.5.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-17 09:27:38.000000 imsciences-0.5.6.8/setup.py
```

### Comparing `imsciences-0.5.6.7/PKG-INFO` & `imsciences-0.5.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.6.7
+Version: 0.5.6.8
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -128,7 +128,11 @@
 ### 28. `format_numbers_with_commas(df, decimal_length_chosen=2)`
 - **Description**: Converts data in numerical format into numbers with commas and a chosen decimal place length.
 - **Usage**: `format_numbers_with_commas(df,1)`
 
 ### 29. `filter_df_on_multiple_conditions(df, filters_dict)`
 - **Description**: Filters dataframe on multiple conditions, which come in the form of a dictionary.
 - **Usage**: `filter_df_on_multiple_conditions(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''})`
+
+### 30. `read_and_concatenate_files(folder_path, file_type='csv')`
+- **Description**: Read and Concatinate all files of one type in a folder.
+- **Usage**: `read_and_concatenate_files(folder_path, file_type='csv')`
```

### Comparing `imsciences-0.5.6.7/README.md` & `imsciences-0.5.6.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,8 +112,12 @@
 
 ### 28. `format_numbers_with_commas(df, decimal_length_chosen=2)`
 - **Description**: Converts data in numerical format into numbers with commas and a chosen decimal place length.
 - **Usage**: `format_numbers_with_commas(df,1)`
 
 ### 29. `filter_df_on_multiple_conditions(df, filters_dict)`
 - **Description**: Filters dataframe on multiple conditions, which come in the form of a dictionary.
-- **Usage**: `filter_df_on_multiple_conditions(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''})`
+- **Usage**: `filter_df_on_multiple_conditions(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''})`
+
+### 30. `read_and_concatenate_files(folder_path, file_type='csv')`
+- **Description**: Read and Concatinate all files of one type in a folder.
+- **Usage**: `read_and_concatenate_files(folder_path, file_type='csv')`
```

### Comparing `imsciences-0.5.6.7/imsciences/datafunctions.py` & `imsciences-0.5.6.8/imsciences/datafunctions.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,14 +158,19 @@
         print("   - Usage: format_numbers_with_commas(df, decimal_length_chosen=2)")
         print("   - Example: format_numbers_with_commas(df,1)")         
     
         print("\n29. filter_df_on_multiple_conditions")
         print("   - Description: Filters dataframe on multiple conditions, which come in the form of a dictionary.")
         print("   - Usage: filter_df_on_multiple_conditions(df, filters_dict)")
         print("   - Example: filter_df_on_multiple_conditions(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''})")       
+
+        print("\n30. read_and_concatenate_files")
+        print("   - Description: Read and Concatinate all files of one type in a folder.")
+        print("   - Usage: read_and_concatenate_files(folder_path, file_type='csv')")
+        print("   - Example: read_and_concatenate_files(folder_path, file_type='csv')")       
     
     
     def get_wd_levels(self, levels):
         """
         Gets the current wd of whoever is working on it and gives the options to move the number of levels up.
 
         Parameters:
@@ -319,35 +324,38 @@
                 daily_records.append(daily_row)
 
         # Convert the list of daily records into a DataFrame
         daily_df = pd.DataFrame(daily_records)
         
         return daily_df
     
-    def plot_two(self, df1, col1, df2, col2, date_column, same_axis=True):
+    def plot_two(df1, col1, df2, col2, date_column, same_axis=True):
         """
         Plots specified columns from two different dataframes with both different and the same lengths,
         using a specified date column as the X-axis, and charting on either the same or separate y axes.
 
         :param df1: First DataFrame
         :param col1: Column name from the first DataFrame
         :param df2: Second DataFrame
         :param col2: Column name from the second DataFrame
         :param date_column: The name of the date column to use for the X-axis
         :param same_axis: If True, plot both traces on the same y-axis; otherwise, use separate y-axes.
         :return: Plotly figure
         """
-
+        # Ensure date columns are datetime
+        df1[date_column] = pd.to_datetime(df1[date_column])
+        df2[date_column] = pd.to_datetime(df2[date_column])
+        
         # Create traces for the first and second dataframes
         trace1 = go.Scatter(x=df1[date_column], y=df1[col1], mode='lines', name=col1, yaxis='y1')
         
         if same_axis:
             trace2 = go.Scatter(x=df2[date_column], y=df2[col2], mode='lines', name=col2, yaxis='y1')
         else:
-            trace2 = go.Scatter(x=np.array(df2[date_column].to_pydatetime()), y=df2[col2], mode='lines', name=col2, yaxis='y2')
+            trace2 = go.Scatter(x=df2[date_column], y=df2[col2], mode='lines', name=col2, yaxis='y2')
             
         # Define layout for the plot
         layout = go.Layout(
             title="",
             xaxis=dict(title="OBS", showline=True, linecolor='black'),
             yaxis=dict(title="", showline=True, linecolor='black', rangemode='tozero'),
             yaxis2=dict(title="", overlaying='y', side='right', showline=True, linecolor='black', rangemode='tozero'),
@@ -1121,14 +1129,57 @@
                 temp_mask = (df[col] < value)                          
             mask &= temp_mask
 
         # Create the filtered df by applying the conditions
         df_filtered = df[mask]
     
         return df_filtered
+    
+    def read_and_concatenate_files(folder_path, file_type='csv'):
+        """
+        Reads all files of a specified type (CSV or XLSX) from a given folder 
+        and concatenates them into a single DataFrame.
+        
+        Parameters:
+        folder_path (str): The path to the folder containing the files.
+        file_type (str): The type of files to read ('csv' or 'xlsx'). Defaults to 'csv'.
+        
+        Returns:
+        pd.DataFrame: A DataFrame containing the concatenated data from all files.
+        """
+        
+        # Initialize an empty list to hold dataframes
+        dataframes = []
+
+        # Define file extension based on file_type
+        if file_type == 'csv':
+            extension = '.csv'
+        elif file_type == 'xlsx':
+            extension = '.xlsx'
+        else:
+            raise ValueError("file_type must be either 'csv' or 'xlsx'")
+
+        # Loop through all files in the folder
+        for filename in os.listdir(folder_path):
+            # Check if the file has the correct extension
+            if filename.endswith(extension):
+                file_path = os.path.join(folder_path, filename)
+                # Read the file into a DataFrame
+                if file_type == 'csv':
+                    df = pd.read_csv(file_path)
+                elif file_type == 'xlsx':
+                    df = pd.read_excel(file_path)
+                # Append the DataFrame to the list
+                dataframes.append(df)
+
+        # Concatenate all DataFrames into a single DataFrame
+        combined_df = pd.concat(dataframes, ignore_index=True)
+        
+        return combined_df
+
 
 class datapull:
     
     def pull_help(self):
         print("This is the help section. The functions in the package are as follows:")
 
         print("\n1. pull_fred_data")
```

### Comparing `imsciences-0.5.6.7/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.6.8/imsciences.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.6.7
+Version: 0.5.6.8
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -128,7 +128,11 @@
 ### 28. `format_numbers_with_commas(df, decimal_length_chosen=2)`
 - **Description**: Converts data in numerical format into numbers with commas and a chosen decimal place length.
 - **Usage**: `format_numbers_with_commas(df,1)`
 
 ### 29. `filter_df_on_multiple_conditions(df, filters_dict)`
 - **Description**: Filters dataframe on multiple conditions, which come in the form of a dictionary.
 - **Usage**: `filter_df_on_multiple_conditions(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''})`
+
+### 30. `read_and_concatenate_files(folder_path, file_type='csv')`
+- **Description**: Read and Concatinate all files of one type in a folder.
+- **Usage**: `read_and_concatenate_files(folder_path, file_type='csv')`
```

### Comparing `imsciences-0.5.6.7/setup.py` & `imsciences-0.5.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.6.7'
+VERSION = '0.5.6.8'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

