# Comparing `tmp/xbox_python_api-0.1.tar.gz` & `tmp/xbox_python_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbox_python_api-0.1.tar", last modified: Fri May 17 19:02:25 2024, max compression
+gzip compressed data, was "xbox_python_api-0.1.1.tar", last modified: Fri May 17 20:30:51 2024, max compression
```

## Comparing `xbox_python_api-0.1.tar` & `xbox_python_api-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 19:02:25.865426 xbox_python_api-0.1/
--rw-rw-rw-   0        0        0     1084 2024-05-17 17:32:14.000000 xbox_python_api-0.1/LICENSE
--rw-rw-rw-   0        0        0      203 2024-05-17 19:02:25.864419 xbox_python_api-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       73 2024-05-17 17:32:14.000000 xbox_python_api-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 19:02:25.865426 xbox_python_api-0.1/setup.cfg
--rw-rw-rw-   0        0        0      284 2024-05-17 19:01:55.000000 xbox_python_api-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 19:02:25.863419 xbox_python_api-0.1/xbox_python_api.egg-info/
--rw-rw-rw-   0        0        0      203 2024-05-17 19:02:25.000000 xbox_python_api-0.1/xbox_python_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-17 19:02:25.000000 xbox_python_api-0.1/xbox_python_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 19:02:25.000000 xbox_python_api-0.1/xbox_python_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-17 19:02:25.000000 xbox_python_api-0.1/xbox_python_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-17 19:02:25.000000 xbox_python_api-0.1/xbox_python_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 19:02:25.862426 xbox_python_api-0.1/xpa/
--rw-rw-rw-   0        0        0     5035 2024-05-17 18:13:33.000000 xbox_python_api-0.1/xpa/URLs.py
--rw-rw-rw-   0        0        0    28616 2024-05-17 18:38:24.000000 xbox_python_api-0.1/xpa/XPA.py
--rw-rw-rw-   0        0        0      384 2024-05-17 17:49:56.000000 xbox_python_api-0.1/xpa/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 20:30:51.518580 xbox_python_api-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2024-05-17 17:32:14.000000 xbox_python_api-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      872 2024-05-17 20:30:51.517580 xbox_python_api-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2024-05-17 20:10:15.000000 xbox_python_api-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 20:30:51.518580 xbox_python_api-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      507 2024-05-17 20:30:22.000000 xbox_python_api-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 20:30:51.516581 xbox_python_api-0.1.1/xbox_python_api.egg-info/
+-rw-rw-rw-   0        0        0      872 2024-05-17 20:30:51.000000 xbox_python_api-0.1.1/xbox_python_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-17 20:30:51.000000 xbox_python_api-0.1.1/xbox_python_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 20:30:51.000000 xbox_python_api-0.1.1/xbox_python_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-17 20:30:51.000000 xbox_python_api-0.1.1/xbox_python_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-17 20:30:51.000000 xbox_python_api-0.1.1/xbox_python_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 20:30:51.515581 xbox_python_api-0.1.1/xpa/
+-rw-rw-rw-   0        0        0     5035 2024-05-17 18:13:33.000000 xbox_python_api-0.1.1/xpa/URLs.py
+-rw-rw-rw-   0        0        0    30090 2024-05-17 20:09:20.000000 xbox_python_api-0.1.1/xpa/XPA.py
+-rw-rw-rw-   0        0        0      384 2024-05-17 17:49:56.000000 xbox_python_api-0.1.1/xpa/__init__.py
```

### Comparing `xbox_python_api-0.1/LICENSE` & `xbox_python_api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xbox_python_api-0.1/xpa/URLs.py` & `xbox_python_api-0.1.1/xpa/URLs.py`

 * *Files identical despite different names*

### Comparing `xbox_python_api-0.1/xpa/XPA.py` & `xbox_python_api-0.1.1/xpa/XPA.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             avatar=user_data["avatar"],
             linkedAccounts=user_data["linkedAccounts"],
             colorTheme=user_data["colorTheme"],
             preferredPlatforms=user_data["preferredPlatforms"],
         )
         return account_info
 
-    def get_presence(self, xuid: str):
+    def get_presence(self, xuid: str) -> XUID_PRESENCE:
         """
         Get user presence information
 
         Args:
             xuid (str): xuid of specified user
 
         Returns:
@@ -245,15 +245,15 @@
             list: user achievements for the specified title.
         """
         endpoint = self.url.player360_achievements_xuid_url(xuid, titleId)
         response = self._make_request(endpoint).json()
         user_data = response["achievements"]
         return user_data
 
-    def get_club_details(self, clubId: str):
+    def get_club_details(self, clubId: str) -> CLUB_DETAILS:
         """
         Get club details
 
         Args:
             clubId (str): clubId of specified club
 
         Returns:
@@ -349,23 +349,64 @@
             associatedTitles=club_data["profile"]["associatedTitles"]["value"],
             primaryColor=club_data["profile"]["primaryColor"]["value"],
             secondaryColor=club_data["profile"]["secondaryColor"]["value"],
             tertiaryColor=club_data["profile"]["tertiaryColor"]["value"]
         )
         return club_details
 
-    def get_friends_xuid(self, xuid: str):
+    def get_friends_xuid(self, xuid: str) -> ACCOUNT_INFO_GAMERTAG:
         """
         Get user friends
 
         Args:
             xuid (str): xuid of specified user
 
         Returns:
-            list: user friends.
+            ACCOUNT_INFO_GAMERTAG: user friends.
+            Object attributes:
+            - xuid: str
+            - displayName: str
+            - realName: str
+            - displayPicRaw: str
+            - showUserAsAvatar: str
+            - gamertag: str
+            - gamerScore: str
+            - modernGamertag: str
+            - modernGamertagSuffix: str
+            - uniqueModernGamertag: str
+            - xboxOneRep: str
+            - presenceState: str
+            - presenceText: str
+            - presenceDevices: list
+            - isBroadcasting: bool
+            - isCloaked: bool
+            - isQuarantined: bool
+            - isXbox360Gamerpic: bool
+            - lastSeenDateTimeUtc: str
+            - preferredColor: dict
+            - presenceDetails: dict
+            - titlePresence: dict
+            - titleSummaries: list
+            - accountTier: str
+            - bio: str
+            - isVerified: bool
+            - location: str
+            - tenure: str
+            - watermarks: dict
+            - blocked: bool
+            - mute: bool
+            - followerCount: int
+            - followingCount: int
+            - hasGamePass: bool
+            - socialManager: str
+            - broadcast: str
+            - avatar: str
+            - linkedAccounts: list
+            - colorTheme: str
+            - preferredPlatforms: dict
         """
         endpoint = self.url.friends_xuid_url(xuid)
         response = self._make_request(endpoint).json()
         friend_data = response['people'][0]
         friend_details = ACCOUNT_INFO_GAMERTAG(
             xuid=friend_data["xuid"],
             displayName=friend_data["displayName"],
@@ -406,15 +447,15 @@
             avatar=friend_data["avatar"],
             linkedAccounts=friend_data["linkedAccounts"],
             colorTheme=friend_data["colorTheme"],
             preferredPlatforms=friend_data["preferredPlatforms"],
         )
         return friend_details
 
-    def search_friend_list(self, gamertag: str):
+    def search_friend_list(self, gamertag: str) -> FRIEND_INFO_GAMERTAG:
         """
         Search for a friend
 
         Args:
             gamertag (str): gamertag of specified user
 
         Returns:
@@ -594,15 +635,15 @@
             list: marketplace games.
         """
         endpoint = self.url.marketplace_searchgame_url(titleId=titleId)
         response = self._make_request(endpoint).json()
         games_list = response["Products"]
         return games_list
 
-    def get_player_summary(self, xuid: str):
+    def get_player_summary(self, xuid: str) -> PLAYER_SUMMARY:
         """
         Get player summary
 
         Args:
             xuid (str): xuid of specified user
 
         Returns:
```

