# Comparing `tmp/awsutils-s3-0.3.20.tar.gz` & `tmp/awsutils-s3-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/awsutils-s3-0.3.20.tar", last modified: Thu Jan  2 20:03:02 2020, max compression
+gzip compressed data, was "dist/awsutils-s3-0.3.9.tar", last modified: Tue Jul  9 18:36:13 2019, max compression
```

## Comparing `awsutils-s3-0.3.20.tar` & `awsutils-s3-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/
--rw-r--r--   0 Stephen    (501) staff       (20)       15 2018-08-29 18:47:04.000000 awsutils-s3-0.3.20/MANIFEST.in
--rw-r--r--   0 Stephen    (501) staff       (20)      284 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/PKG-INFO
-drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/awsutils/
--rw-r--r--   0 Stephen    (501) staff       (20)       55 2019-03-28 16:49:41.000000 awsutils-s3-0.3.20/awsutils/__init__.py
-drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/awsutils/s3/
--rw-r--r--   0 Stephen    (501) staff       (20)      164 2019-04-15 13:39:17.000000 awsutils-s3-0.3.20/awsutils/s3/__init__.py
--rw-r--r--   0 Stephen    (501) staff       (20)     2843 2019-09-10 20:10:13.000000 awsutils-s3-0.3.20/awsutils/s3/__main__.py
--rw-r--r--   0 Stephen    (501) staff       (20)       23 2020-01-02 19:10:44.000000 awsutils-s3-0.3.20/awsutils/s3/_version.py
--rw-r--r--   0 Stephen    (501) staff       (20)     6741 2020-01-02 19:48:44.000000 awsutils-s3-0.3.20/awsutils/s3/commands.py
--rw-r--r--   0 Stephen    (501) staff       (20)    13300 2020-01-02 20:00:06.000000 awsutils-s3-0.3.20/awsutils/s3/s3.py
--rw-r--r--   0 Stephen    (501) staff       (20)     1833 2020-01-02 19:21:01.000000 awsutils-s3-0.3.20/awsutils/s3/url.py
-drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/awsutils_s3.egg-info/
--rw-r--r--   0 Stephen    (501) staff       (20)      284 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/awsutils_s3.egg-info/PKG-INFO
--rw-r--r--   0 Stephen    (501) staff       (20)      430 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/awsutils_s3.egg-info/SOURCES.txt
--rw-r--r--   0 Stephen    (501) staff       (20)        1 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/awsutils_s3.egg-info/dependency_links.txt
--rw-r--r--   0 Stephen    (501) staff       (20)       53 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/awsutils_s3.egg-info/entry_points.txt
--rw-r--r--   0 Stephen    (501) staff       (20)        9 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/awsutils_s3.egg-info/namespace_packages.txt
--rw-r--r--   0 Stephen    (501) staff       (20)       48 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/awsutils_s3.egg-info/requires.txt
--rw-r--r--   0 Stephen    (501) staff       (20)       15 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/awsutils_s3.egg-info/top_level.txt
--rw-r--r--   0 Stephen    (501) staff       (20)       38 2020-01-02 20:03:02.000000 awsutils-s3-0.3.20/setup.cfg
--rw-r--r--   0 Stephen    (501) staff       (20)      966 2019-08-12 15:43:10.000000 awsutils-s3-0.3.20/setup.py
+drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/
+-rw-r--r--   0 Stephen    (501) staff       (20)       15 2018-08-29 18:47:04.000000 awsutils-s3-0.3.9/MANIFEST.in
+-rw-r--r--   0 Stephen    (501) staff       (20)      283 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/PKG-INFO
+drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/awsutils/
+-rw-r--r--   0 Stephen    (501) staff       (20)       55 2019-03-28 16:49:41.000000 awsutils-s3-0.3.9/awsutils/__init__.py
+drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/awsutils/s3/
+-rw-r--r--   0 Stephen    (501) staff       (20)      164 2019-04-15 13:39:17.000000 awsutils-s3-0.3.9/awsutils/s3/__init__.py
+-rw-r--r--   0 Stephen    (501) staff       (20)     2900 2019-07-09 18:26:07.000000 awsutils-s3-0.3.9/awsutils/s3/__main__.py
+-rw-r--r--   0 Stephen    (501) staff       (20)       22 2019-07-09 18:36:02.000000 awsutils-s3-0.3.9/awsutils/s3/_version.py
+-rw-r--r--   0 Stephen    (501) staff       (20)     5977 2019-07-09 16:25:25.000000 awsutils-s3-0.3.9/awsutils/s3/commands.py
+-rw-r--r--   0 Stephen    (501) staff       (20)    12808 2019-07-09 16:24:35.000000 awsutils-s3-0.3.9/awsutils/s3/s3.py
+-rw-r--r--   0 Stephen    (501) staff       (20)     1652 2019-04-15 15:38:09.000000 awsutils-s3-0.3.9/awsutils/s3/url.py
+drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/awsutils_s3.egg-info/
+-rw-r--r--   0 Stephen    (501) staff       (20)      283 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/awsutils_s3.egg-info/PKG-INFO
+-rw-r--r--   0 Stephen    (501) staff       (20)      430 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/awsutils_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 Stephen    (501) staff       (20)        1 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/awsutils_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 Stephen    (501) staff       (20)       53 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/awsutils_s3.egg-info/entry_points.txt
+-rw-r--r--   0 Stephen    (501) staff       (20)        9 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/awsutils_s3.egg-info/namespace_packages.txt
+-rw-r--r--   0 Stephen    (501) staff       (20)       47 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/awsutils_s3.egg-info/requires.txt
+-rw-r--r--   0 Stephen    (501) staff       (20)       15 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/awsutils_s3.egg-info/top_level.txt
+-rw-r--r--   0 Stephen    (501) staff       (20)       38 2019-07-09 18:36:13.000000 awsutils-s3-0.3.9/setup.cfg
+-rw-r--r--   0 Stephen    (501) staff       (20)      965 2019-07-09 17:00:00.000000 awsutils-s3-0.3.9/setup.py
```

### Comparing `awsutils-s3-0.3.20/awsutils/s3/__main__.py` & `awsutils-s3-0.3.9/awsutils/s3/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import os
 from argparse import ArgumentParser
 
 from awsutils.s3.s3 import S3, bucket_uri
 
 
 def print_output(event, bucket=None, local_path=None, remote_path=None):
-    string = '{0}: {1} => {2}' if not event.lower().startswith('download') else '{0}: {2} to {1}'
-    print(string.format(event, local_path, os.path.join(bucket_uri(bucket), remote_path if remote_path else '')))
+    print('{0}: {1} to {2}'.format(event, local_path,
+                                   os.path.join(bucket_uri(bucket), remote_path if remote_path else '')))
 
 
 def upload(bucket=None, local_path=None, remote_path=None):
     """Upload a file or folder to an AWS S3 bucket."""
-    S3(str(bucket), quiet=False).upload(local_path=local_path, remote_path=remote_path)
+    S3(str(bucket)).upload(local_path=local_path, remote_path=remote_path)
+    print_output('Uploaded', bucket, local_path, remote_path)
 
 
 def download(bucket=None, local_path=None, remote_path=None, recursive=False):
     """Download a file or folder to an AWS S3 bucket."""
-    S3(str(bucket), quiet=False).download(local_path=local_path, remote_path=remote_path, recursive=recursive)
+    S3(str(bucket)).download(local_path=local_path, remote_path=remote_path, recursive=recursive)
+    print_output('Downloaded', bucket, local_path, remote_path)
 
 
 def sync(bucket=None, local_path=None, remote_path=None, delete=False, remote_source=False):
     """Sync files or folders to an AWS S3 bucket."""
-    S3(str(bucket), quiet=False).sync(local_path=local_path, remote_path=remote_path, delete=delete,
-                                      remote_source=remote_source)
+    S3(str(bucket)).sync(local_path=local_path, remote_path=remote_path, delete=delete, remote_source=remote_source)
+    print_output('Synced', bucket, local_path, remote_path)
 
 
 def main():
     # Declare argparse argument descriptions
     usage = 'AWS S3 command-line-interface wrapper.'
     description = 'Execute AWS S3 commands.'
     helpers = {
```

### Comparing `awsutils-s3-0.3.20/awsutils/s3/commands.py` & `awsutils-s3-0.3.9/awsutils/s3/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 def clean_path(path):
     """Return a path string with double quote wrappers if the path contains a space."""
-    return '"{0}"'.format(path) if path and '"' not in path else "'{0}'".format(path)
+    return '"{0}"'.format(path) if path and ' ' in path else path
 
 
 def move_or_copy(command, object1, object2, recursive=False, include=None, exclude=None, acl='private', quiet=True):
     """
     Copy file(s)/folder(s) from one S3 bucket location to another
 
     :param command: Execute a 'move' or a 'copy' command
@@ -128,26 +128,7 @@
         with an HTTP GET request.
 
         :param uri: S3 object URI
         :param expiration: Number of seconds until the pre-signed URL expires
         :return: Command string
         """
         return 'aws s3 presign {uri} --expires-in {expiration}'.format(uri=clean_path(uri), expiration=expiration)
-
-    @staticmethod
-    def acceleration_enabled_status(bucket):
-        """
-        Check to see if transfer acceleration is enabled for an S3 bucket
-
-        :param bucket: Name of the bucket to check the acceleration status of
-        """
-        return 'aws s3api get-bucket-accelerate-configuration --bucket {bucket} --query "Status"'.format(bucket=bucket)
-
-    @staticmethod
-    def enable_transfer_acceleration(bucket):
-        """
-        Enable transfer acceleration for an S3 bucket
-
-        :param bucket: Name of the bucket to enable transfer acceleration
-        """
-        return 'aws s3api put-bucket-accelerate-configuration --bucket {bucket} --accelerate-configuration ' \
-               'Status=Enabled'.format(bucket=bucket)
```

### Comparing `awsutils-s3-0.3.20/awsutils/s3/s3.py` & `awsutils-s3-0.3.9/awsutils/s3/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,35 +31,34 @@
     :param recursive_default: Default value for recursive flag
     :return: Bool, true if both are directories
     """
     return True if all('.' not in os.path.basename(uri) for uri in uris) else recursive_default
 
 
 class S3:
-    def __init__(self, bucket, accelerate=False, quiet=False):
+    def __init__(self, bucket, accelerate=False, quiet=True):
         """
         AWS CLI S3 wrapper.
 
         https://docs.aws.amazon.com/cli/latest/reference/s3/
 
         :param bucket: S3 bucket name or S3 bucket url
         :param accelerate: Enable transfer acceleration
         :param quiet: When true, does not display the operations performed from the specified command
         """
-        self.cmd = S3Commands()
-
         # Extract the bucket name from the url if bucket var is a url
         self.bucket_name = bucket if not url_validator(bucket) else bucket_name(bucket)
-        self.accelerate = accelerate if accelerate and self.is_acceleration_enabled() else False
+        self.accelerate = accelerate
         self.quiet = quiet
+        self.cmd = S3Commands()
 
     @property
     def bucket_uri(self):
         """Retrieve a S3 bucket name in URI form."""
-        return bucket_uri(self.bucket_name, self.accelerate)
+        return bucket_uri(self.bucket_name)
 
     @property
     def bucket_url(self):
         """Retrieve a url endpoint for a S3 bucket."""
         return bucket_url(self.bucket_name, self.accelerate)
 
     @property
@@ -112,15 +111,16 @@
         return SystemCommand(
             self.cmd.copy(object1=uri1,
                           object2=uri2,
                           recursive=is_recursive_needed(uri1, uri2, recursive_default=recursive),
                           include=include,
                           exclude=exclude,
                           acl=acl,
-                          quiet=quiet if quiet else self.quiet)
+                          quiet=quiet if quiet else self.quiet),
+            False
         )
 
     def move(self, src_path, dst_path, dst_bucket=None, recursive=False, include=None, exclude=None):
         """
         Move an S3 file or folder to another
 
         :param src_path: Path to source file or folder in S3 bucket
@@ -138,15 +138,16 @@
 
         # Move recursively if both URI's are directories and NOT files
         return SystemCommand(
             self.cmd.move(object1=uri1,
                           object2=uri2,
                           recursive=is_recursive_needed(uri1, uri2, recursive_default=recursive),
                           include=include,
-                          exclude=exclude)
+                          exclude=exclude),
+            False
         )
 
     def exists(self, remote_path):
         """
         Check to see if an S3 key (file or directory) exists
         :return: Bool
         """
@@ -180,36 +181,38 @@
         :param acl: Access permissions, must be either 'private', 'public-read' or 'public-read-write'
         :param quiet: When true, does not display the operations performed from the specified command
         """
         # Recursively upload files if the local target is a folder
         # Use local_path file/folder name as remote_path if none is specified
         remote_path = os.path.basename(local_path) if not remote_path else remote_path
         assert_acl(acl)
-        return SystemCommand(
+        SystemCommand(
             self.cmd.copy(object1=local_path,
                           object2='{0}/{1}'.format(self.bucket_uri, remote_path),
                           recursive=True if os.path.isdir(local_path) else False,
                           acl=acl, quiet=quiet if quiet else self.quiet)
         )
+        return remote_path
 
     def download(self, remote_path, local_path=os.getcwd(), recursive=False, quiet=None):
         """
         Download a file or folder from an S3 bucket.
 
         :param remote_path: S3 key, aka remote path relative to S3 bucket's root
         :param local_path: Path to file on local disk
         :param recursive: Recursively download files/folders
         :param quiet: When true, does not display the operations performed from the specified command
         """
-        return SystemCommand(
+        SystemCommand(
             self.cmd.copy(object1='{0}/{1}'.format(self.bucket_uri, remote_path),
                           object2=local_path,
                           recursive=recursive,
-                          quiet=quiet if quiet else self.quiet)
+                          quiet=quiet if quiet else self.quiet), False
         )
+        return local_path
 
     def sync(self, local_path, remote_path=None, delete=False, acl='private', quiet=None, remote_source=False):
         """
         Synchronize local files with an S3 bucket.
 
         S3 sync only copies missing or outdated files or objects between
         the source and target.  However, you can also supply the --delete
@@ -231,45 +234,38 @@
 
         return SystemCommand(
             self.cmd.sync(
                 source=source,
                 destination=destination,
                 delete=delete,
                 acl=acl,
-                quiet=quiet if quiet else self.quiet)
+                quiet=quiet if quiet else self.quiet), False
         )
 
     def create_bucket(self, region='us-east-1'):
         """
         Create a new S3 bucket.
 
         :param region: Bucket's hosting region
         """
         # Validate that the bucket does not already exist
         assert self.bucket_name not in self.buckets, 'ERROR: Bucket `{0}` already exists.'.format(self.bucket_name)
-
-        # Create the bucket
-        create = SystemCommand(self.cmd.make_bucket(self.bucket_uri, region))
-
-        # Enable transfer acceleration
-        SystemCommand(self.cmd.enable_transfer_acceleration(self.bucket_name))
-
-        return create
+        return SystemCommand(self.cmd.make_bucket(self.bucket_uri, region), False)
 
     def delete_bucket(self, force=False):
         """
         Deletes an empty S3 bucket. A bucket must be completely empty of objects and versioned
         objects before it can be deleted. However, the force parameter can be used to delete
         the non-versioned objects in the bucket before the bucket is deleted.
 
         :param force: Deletes all objects in the bucket including the bucket itself
         """
         # Validate that the bucket does exist
         assert self.bucket_name in self.buckets, 'ERROR: Bucket `{0}` does not exists.'.format(self.bucket_name)
-        return SystemCommand(self.cmd.remove_bucket(self.bucket_uri, force))
+        return SystemCommand(self.cmd.remove_bucket(self.bucket_uri, force), False)
 
     def pre_sign(self, remote_path, expiration=3600):
         """
         Generate a pre-signed URL for an Amazon S3 object.
 
         This allows anyone who receives the pre-signed URL to retrieve the S3 object
         with an HTTP GET request.
@@ -280,16 +276,7 @@
         """
         return SystemCommand(self.cmd.pre_sign('{uri}/{src}'.format(uri=self.bucket_uri, src=remote_path),
                                                expiration))[0]
 
     def url(self, remote_path):
         """Retrieve a S3 bucket URL for a S3 object."""
         return '{url}/{src}'.format(url=self.bucket_url, src=remote_path)
-
-    def is_acceleration_enabled(self):
-        """Determine if transfer acceleration is enabled for an AWS S3 bucket."""
-        output = SystemCommand(self.cmd.acceleration_enabled_status(self.bucket_name)).output
-
-        if len(output) > 0:
-            return output[0].strip('"').lower() == 'enabled'
-        else:
-            return False
```

### Comparing `awsutils-s3-0.3.20/awsutils/s3/url.py` & `awsutils-s3-0.3.9/awsutils/s3/url.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,26 +10,25 @@
 
     :param url: URL
     :return: hostname
     """
     return '{uri.scheme}://{uri.netloc}/'.format(uri=urlparse(url))
 
 
-def bucket_uri(bucket, acceleration=False):
+def bucket_uri(bucket):
     """
     Convert a S3 bucket name string in to a S3 bucket uri.
 
     :param bucket: Bucket name
-    :param acceleration: Use transfer acceleration if the endpoint is available
     :return: Bucket URI
     """
-    return '{uri}://{bucket}'.format(uri='s3-accelerate' if acceleration else 's3', bucket=bucket)
+    return 's3://{bucket}'.format(bucket=bucket)
 
 
-def bucket_url(bucket, acceleration=False):
+def bucket_url(bucket, acceleration=True):
     """
     Convert a S3 bucket name string in to a S3 bucket url.
 
     :param bucket: Bucket name
     :param acceleration: Use transfer acceleration if the endpoint is available
     :return: Bucket URL
     """
@@ -45,15 +44,15 @@
     :param url: URL
     :return: Bucket name
     """
     result = url_extract(url)
     if result.subdomain == 's3':
         return url.replace(url_host(url), '').split('/')[0]
     else:
-        return result.subdomain.replace('.s3-accelerate', '').replace('.s3', '')
+        return result.subdomain.replace('.s3', '')
 
 
 def key_extract(url):
     """
     Retrieve an AWS object key from a URL.
 
     :param url: URL
```

### Comparing `awsutils-s3-0.3.20/setup.py` & `awsutils-s3-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 setup(
     name=name,
     version=get_version(),
     packages=find_packages(),
     namespace_packages=['awsutils'],
     install_requires=[
         'awscli',
-        'dirutility>=0.7.18',
+        'dirutility>=0.7.3',
         'tldextract',
         'validators'
     ],
     url='https://github.com/mrstephenneal/awsutils-s3',
     entry_points={
         'console_scripts': [
             'awss3 = awsutils.s3.__main__:main'
```

