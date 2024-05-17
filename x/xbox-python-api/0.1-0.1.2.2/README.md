# Comparing `tmp/xbox_python_api-0.1.tar.gz` & `tmp/xbox_python_api-0.1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbox_python_api-0.1.tar", last modified: Fri May 17 19:02:25 2024, max compression
+gzip compressed data, was "xbox_python_api-0.1.2.2.tar", last modified: Fri May 17 21:02:30 2024, max compression
```

## Comparing `xbox_python_api-0.1.tar` & `xbox_python_api-0.1.2.2.tar`

### file list

```diff
@@ -1,16 +1,24 @@
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
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:02:30.609167 xbox_python_api-0.1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-17 21:02:30.609167 xbox_python_api-0.1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 21:02:30.609167 xbox_python_api-0.1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:02:30.609167 xbox_python_api-0.1.2.2/xbox_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-17 21:02:30.000000 xbox_python_api-0.1.2.2/xbox_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-17 21:02:30.000000 xbox_python_api-0.1.2.2/xbox_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:02:30.000000 xbox_python_api-0.1.2.2/xbox_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 21:02:30.000000 xbox_python_api-0.1.2.2/xbox_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 21:02:30.000000 xbox_python_api-0.1.2.2/xbox_python_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:02:30.605167 xbox_python_api-0.1.2.2/xpa/
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/xpa/URLs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29300 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/xpa/XPA.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/xpa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:02:30.609167 xbox_python_api-0.1.2.2/xpa/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/xpa/classes/ACCOUNT_INFO_GAMERTAG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/xpa/classes/ACCOUNT_INFO_XUID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/xpa/classes/CLUB_DETAILS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/xpa/classes/FRIEND_INFO_GAMERTAG.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/xpa/classes/PLAYER_SUMMARY.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/xpa/classes/XUID_PRESENCE.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:02:26.000000 xbox_python_api-0.1.2.2/xpa/classes/__init__.py
```

### Comparing `xbox_python_api-0.1/xpa/URLs.py` & `xbox_python_api-0.1.2.2/xpa/URLs.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-class URLs:
-    def __init__(self):
-        self.base_url = "https://xbl.io/api/v2/"
-
-        # account
-        self.account_xuid = "account/{xuid}"
-        self.search_gamertag = "search/{gamertag}"
-        self.xuid_presence = "{xuid}/presence"
-
-        # achievements
-        self.achievements_xuid = "achievements/player/{xuid}"
-        self.title_achievements_xuid = "achievements/player/{xuid}/{titleId}"
-        self.title360_achievements_xuid = "achievements/player/{xuid}/title/{titleId}"
-        self.player360_achievements_xuid = "achievements/x360/{xuid}/title/{titleId}"
-
-        # clubs
-        self.club_details = "clubs/{clubId}"
-
-        # friends
-        self.friends_xuid = "friends/{xuid}"
-        self.search_friend = "friends/search/{gamertag}"
-
-        # gamepass
-        self.gamepass_all = "gamepass/all"
-        self.gamepass_pc = "gamepass/pc"
-        self.gamepass_eaplay = "gamepass/ea-play"
-        self.gamepass_nocontroller = "gamepass/no-controller"
-
-        # marketplace
-        self.marketplace_new = "marketplace/new"
-        self.marketplace_toppaid = "marketplace/top-paid"
-        self.marketplace_bestrated = "marketplace/best-rated"
-        self.marketplace_comingsoon = "marketplace/coming-soon"
-        self.marketplace_deals = "marketplace/deals"
-        self.marketplace_topfree = "marketplace/top-free"
-        self.marketplace_mostplayed = "marketplace/most-played"
-        self.marketplace_searchgame = "marketplace/title/{titleId}"
-
-        # player
-        self.player_summary = "player/summary/{xuid}"
-        self.player_titleHistory = "player/titleHistory/{xuid}"
-
-        # session
-        self.session_details = "session/{sessionName}"
-
-        # group
-        self.group_summary = "group/summary/{groupId}"
-        self.group_messages = "group/messages/{groupId}"
-
-    def base_url(self):
-        return self.base_url
-
-    def account_xuid_url(self, xuid):
-        return self.base_url + self.account_xuid.format(xuid=xuid)
-
-    def search_gamertag_url(self, gamertag):
-        return self.base_url + self.search_gamertag.format(gamertag=gamertag)
-
-    def xuid_presence_url(self, xuid):
-        return self.base_url + self.xuid_presence.format(xuid=xuid)
-
-    def achievements_xuid_url(self, xuid):
-        return self.base_url + self.achievements_xuid.format(xuid=xuid)
-
-    def title_achievements_xuid_url(self, xuid, titleId):
-        return self.base_url + self.title_achievements_xuid.format(xuid=xuid, titleId=titleId)
-
-    def title360_achievements_xuid_url(self, xuid, titleId):
-        return self.base_url + self.title360_achievements_xuid.format(xuid=xuid, titleId=titleId)
-
-    def player360_achievements_xuid_url(self, xuid, titleId):
-        return self.base_url + self.player360_achievements_xuid.format(xuid=xuid, titleId=titleId)
-
-    def club_details_url(self, clubId):
-        return self.base_url + self.club_details.format(clubId=clubId)
-
-    def friends_xuid_url(self, xuid):
-        return self.base_url + self.friends_xuid.format(xuid=xuid)
-
-    def search_friend_url(self, gamertag):
-        return self.base_url + self.search_friend.format(gamertag=gamertag)
-
-    def gamepass_all_url(self):
-        return self.base_url + self.gamepass_all
-
-    def gamepass_pc_url(self):
-        return self.base_url + self.gamepass_pc
-
-    def gamepass_eaplay_url(self):
-        return self.base_url + self.gamepass_eaplay
-
-    def gamepass_nocontroller_url(self):
-        return self.base_url + self.gamepass_nocontroller
-
-    def marketplace_new_url(self):
-        return self.base_url + self.marketplace_new
-
-    def marketplace_toppaid_url(self):
-        return self.base_url + self.marketplace_toppaid
-
-    def marketplace_bestrated_url(self):
-        return self.base_url + self.marketplace_bestrated
-
-    def marketplace_comingsoon_url(self):
-        return self.base_url + self.marketplace_comingsoon
-
-    def marketplace_deals_url(self):
-        return self.base_url + self.marketplace_deals
-
-    def marketplace_topfree_url(self):
-        return self.base_url + self.marketplace_topfree
-
-    def marketplace_mostplayed_url(self):
-        return self.base_url + self.marketplace_mostplayed
-
-    def marketplace_searchgame_url(self, titleId):
-        return self.base_url + self.marketplace_searchgame.format(titleId=titleId)
-
-    def player_summary_url(self, xuid):
-        return self.base_url + self.player_summary.format(xuid=xuid)
-
-    def player_titleHistory_url(self, xuid):
-        return self.base_url + self.player_titleHistory.format(xuid=xuid)
-
-    def session_details_url(self, sessionName):
-        return self.base_url + self.session_details.format(sessionName=sessionName)
-
-    def group_summary_url(self, groupId):
-        return self.base_url + self.group_summary.format(groupId=groupId)
-
-    def group_messages_url(self, groupId):
-        return self.base_url + self.group_messages.format(groupId=groupId)
+class URLs:
+    def __init__(self):
+        self.base_url = "https://xbl.io/api/v2/"
+
+        # account
+        self.account_xuid = "account/{xuid}"
+        self.search_gamertag = "search/{gamertag}"
+        self.xuid_presence = "{xuid}/presence"
+
+        # achievements
+        self.achievements_xuid = "achievements/player/{xuid}"
+        self.title_achievements_xuid = "achievements/player/{xuid}/{titleId}"
+        self.title360_achievements_xuid = "achievements/player/{xuid}/title/{titleId}"
+        self.player360_achievements_xuid = "achievements/x360/{xuid}/title/{titleId}"
+
+        # clubs
+        self.club_details = "clubs/{clubId}"
+
+        # friends
+        self.friends_xuid = "friends/{xuid}"
+        self.search_friend = "friends/search/{gamertag}"
+
+        # gamepass
+        self.gamepass_all = "gamepass/all"
+        self.gamepass_pc = "gamepass/pc"
+        self.gamepass_eaplay = "gamepass/ea-play"
+        self.gamepass_nocontroller = "gamepass/no-controller"
+
+        # marketplace
+        self.marketplace_new = "marketplace/new"
+        self.marketplace_toppaid = "marketplace/top-paid"
+        self.marketplace_bestrated = "marketplace/best-rated"
+        self.marketplace_comingsoon = "marketplace/coming-soon"
+        self.marketplace_deals = "marketplace/deals"
+        self.marketplace_topfree = "marketplace/top-free"
+        self.marketplace_mostplayed = "marketplace/most-played"
+        self.marketplace_searchgame = "marketplace/title/{titleId}"
+
+        # player
+        self.player_summary = "player/summary/{xuid}"
+        self.player_titleHistory = "player/titleHistory/{xuid}"
+
+        # session
+        self.session_details = "session/{sessionName}"
+
+        # group
+        self.group_summary = "group/summary/{groupId}"
+        self.group_messages = "group/messages/{groupId}"
+
+    def base_url(self):
+        return self.base_url
+
+    def account_xuid_url(self, xuid):
+        return self.base_url + self.account_xuid.format(xuid=xuid)
+
+    def search_gamertag_url(self, gamertag):
+        return self.base_url + self.search_gamertag.format(gamertag=gamertag)
+
+    def xuid_presence_url(self, xuid):
+        return self.base_url + self.xuid_presence.format(xuid=xuid)
+
+    def achievements_xuid_url(self, xuid):
+        return self.base_url + self.achievements_xuid.format(xuid=xuid)
+
+    def title_achievements_xuid_url(self, xuid, titleId):
+        return self.base_url + self.title_achievements_xuid.format(xuid=xuid, titleId=titleId)
+
+    def title360_achievements_xuid_url(self, xuid, titleId):
+        return self.base_url + self.title360_achievements_xuid.format(xuid=xuid, titleId=titleId)
+
+    def player360_achievements_xuid_url(self, xuid, titleId):
+        return self.base_url + self.player360_achievements_xuid.format(xuid=xuid, titleId=titleId)
+
+    def club_details_url(self, clubId):
+        return self.base_url + self.club_details.format(clubId=clubId)
+
+    def friends_xuid_url(self, xuid):
+        return self.base_url + self.friends_xuid.format(xuid=xuid)
+
+    def search_friend_url(self, gamertag):
+        return self.base_url + self.search_friend.format(gamertag=gamertag)
+
+    def gamepass_all_url(self):
+        return self.base_url + self.gamepass_all
+
+    def gamepass_pc_url(self):
+        return self.base_url + self.gamepass_pc
+
+    def gamepass_eaplay_url(self):
+        return self.base_url + self.gamepass_eaplay
+
+    def gamepass_nocontroller_url(self):
+        return self.base_url + self.gamepass_nocontroller
+
+    def marketplace_new_url(self):
+        return self.base_url + self.marketplace_new
+
+    def marketplace_toppaid_url(self):
+        return self.base_url + self.marketplace_toppaid
+
+    def marketplace_bestrated_url(self):
+        return self.base_url + self.marketplace_bestrated
+
+    def marketplace_comingsoon_url(self):
+        return self.base_url + self.marketplace_comingsoon
+
+    def marketplace_deals_url(self):
+        return self.base_url + self.marketplace_deals
+
+    def marketplace_topfree_url(self):
+        return self.base_url + self.marketplace_topfree
+
+    def marketplace_mostplayed_url(self):
+        return self.base_url + self.marketplace_mostplayed
+
+    def marketplace_searchgame_url(self, titleId):
+        return self.base_url + self.marketplace_searchgame.format(titleId=titleId)
+
+    def player_summary_url(self, xuid):
+        return self.base_url + self.player_summary.format(xuid=xuid)
+
+    def player_titleHistory_url(self, xuid):
+        return self.base_url + self.player_titleHistory.format(xuid=xuid)
+
+    def session_details_url(self, sessionName):
+        return self.base_url + self.session_details.format(sessionName=sessionName)
+
+    def group_summary_url(self, groupId):
+        return self.base_url + self.group_summary.format(groupId=groupId)
+
+    def group_messages_url(self, groupId):
+        return self.base_url + self.group_messages.format(groupId=groupId)
```

### Comparing `xbox_python_api-0.1/xpa/XPA.py` & `xbox_python_api-0.1.2.2/xpa/XPA.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,749 +1,790 @@
-import requests
-
-from .URLs import URLs
-from .classes.ACCOUNT_INFO_GAMERTAG import ACCOUNT_INFO_GAMERTAG
-from .classes.ACCOUNT_INFO_XUID import ACCOUNT_INFO_XUID
-from .classes.CLUB_DETAILS import CLUB_DETAILS
-from .classes.FRIEND_INFO_GAMERTAG import FRIEND_INFO_GAMERTAG
-from .classes.PLAYER_SUMMARY import PLAYER_SUMMARY
-from .classes.XUID_PRESENCE import XUID_PRESENCE
-
-
-class XPA:
-    def __init__(self, api_key):
-        self.api_key = api_key
-        self.url = URLs()
-
-    def _make_request(self, endpoint):
-        headers = {'x-authorization': self.api_key}
-        return requests.get(endpoint, headers=headers)
-
-    def _find_setting_by_id(self, settings, setting_id):
-        for setting in settings:
-            if setting['id'] == setting_id:
-                return setting['value']
-        return None
-
-    def get_account_info_xuid(self, xuid: str) -> ACCOUNT_INFO_XUID:
-        """Get someone's profile information
-
-        Args:
-            xuid (str): xuid of specified user.
-
-        Returns:
-            ACCOUNT_INFO_XUID: user account info.
-            
-            Object attributes:
-            - GameDisplayPicRaw: str
-            - Gamerscore: str
-            - Gamertag: str
-            - AccountTier: str
-            - XboxOneRep: str
-            - PreferredColor: str
-            - RealName: str
-            - Bio: str
-            - Location: str
-        """
-        endpoint = self.url.account_xuid_url(xuid)
-        response = self._make_request(endpoint).json()
-        user_data = response['profileUsers'][0]['settings']
-        account_info = ACCOUNT_INFO_XUID(
-            GameDisplayPicRaw=self._find_setting_by_id(user_data, 'GameDisplayPicRaw'),
-            Gamerscore=self._find_setting_by_id(user_data, 'Gamerscore'),
-            Gamertag=self._find_setting_by_id(user_data, 'Gamertag'),
-            AccountTier=self._find_setting_by_id(user_data, 'AccountTier'),
-            XboxOneRep=self._find_setting_by_id(user_data, 'XboxOneRep'),
-            PreferredColor=self._find_setting_by_id(user_data, 'PreferredColor'),
-            RealName=self._find_setting_by_id(user_data, 'RealName'),
-            Bio=self._find_setting_by_id(user_data, 'Bio'),
-            Location=self._find_setting_by_id(user_data, 'Location')
-        )
-        return account_info
-
-    def get_account_info_gamertag(self, gamertag: str) -> ACCOUNT_INFO_GAMERTAG:
-        """
-        Get someone's profile information
-
-        Args:
-            gamertag (str): gamertag of specified user
-
-        Returns:
-            ACCOUNT_INFO_GAMERTAG: user account info.
-            Object attributes:
-            - xuid: str
-            - displayName: str
-            - realName: str
-            - displayPicRaw: str
-            - showUserAsAvatar: str
-            - gamertag: str
-            - gamerScore: str
-            - modernGamertag: str
-            - modernGamertagSuffix: str
-            - uniqueModernGamertag: str
-            - xboxOneRep: str
-            - presenceState: str
-            - presenceText: str
-            - presenceDevices: list
-            - isBroadcasting: bool
-            - isCloaked: bool
-            - isQuarantined: bool
-            - isXbox360Gamerpic: bool
-            - lastSeenDateTimeUtc: str
-            - preferredColor: dict
-            - presenceDetails: dict
-            - titlePresence: dict
-            - titleSummaries: list
-            - accountTier: str
-            - bio: str
-            - isVerified: bool
-            - location: str
-            - tenure: str
-            - watermarks: dict
-            - blocked: bool
-            - mute: bool
-            - followerCount: int
-            - followingCount: int
-            - hasGamePass: bool
-            - socialManager: str
-            - broadcast: str
-            - avatar: str
-            - linkedAccounts: list
-            - colorTheme: str
-            - preferredPlatforms: dict
-        """
-        endpoint = self.url.search_gamertag_url(gamertag)
-        response = self._make_request(endpoint).json()
-        user_data = response['people'][0]
-        account_info = ACCOUNT_INFO_GAMERTAG(
-            xuid=user_data["xuid"],
-            displayName=user_data["displayName"],
-            realName=user_data["realName"],
-            displayPicRaw=user_data["displayPicRaw"],
-            showUserAsAvatar=user_data["showUserAsAvatar"],
-            gamertag=user_data["gamertag"],
-            gamerScore=user_data["gamerScore"],
-            modernGamertag=user_data["modernGamertag"],
-            modernGamertagSuffix=user_data["modernGamertagSuffix"],
-            uniqueModernGamertag=user_data["uniqueModernGamertag"],
-            xboxOneRep=user_data["xboxOneRep"],
-            presenceState=user_data["presenceState"],
-            presenceText=user_data["presenceText"],
-            presenceDevices=user_data["presenceDevices"],
-            isBroadcasting=user_data["isBroadcasting"],
-            isCloaked=user_data["isCloaked"],
-            isQuarantined=user_data["isQuarantined"],
-            isXbox360Gamerpic=user_data["isXbox360Gamerpic"],
-            lastSeenDateTimeUtc=user_data["lastSeenDateTimeUtc"],
-            preferredColor=user_data["preferredColor"],
-            presenceDetails=user_data["presenceDetails"],
-            titlePresence=user_data["titlePresence"],
-            titleSummaries=user_data["titleSummaries"],
-            accountTier=user_data["detail"]["accountTier"],
-            bio=user_data["detail"]["bio"],
-            isVerified=user_data["detail"]["isVerified"],
-            location=user_data["detail"]["location"],
-            tenure=user_data["detail"]["tenure"],
-            watermarks=user_data["detail"]["watermarks"],
-            blocked=user_data["detail"]["blocked"],
-            mute=user_data["detail"]["mute"],
-            followerCount=user_data["detail"]["followerCount"],
-            followingCount=user_data["detail"]["followingCount"],
-            hasGamePass=user_data["detail"]["hasGamePass"],
-            socialManager=user_data["socialManager"],
-            broadcast=user_data["broadcast"],
-            avatar=user_data["avatar"],
-            linkedAccounts=user_data["linkedAccounts"],
-            colorTheme=user_data["colorTheme"],
-            preferredPlatforms=user_data["preferredPlatforms"],
-        )
-        return account_info
-
-    def get_presence(self, xuid: str):
-        """
-        Get user presence information
-
-        Args:
-            xuid (str): xuid of specified user
-
-        Returns:
-            XUID_PRESENCE: user presence info.
-            Object attributes:
-            - state: str
-            - last_seen_device_type: str
-            - last_seen_title_id: str
-            - last_seen_title_name: str
-            - last_seen_timestamp: str
-        """
-        endpoint = self.url.xuid_presence_url(xuid)
-        response = self._make_request(endpoint).json()
-        user_data = response[0]
-        presence = XUID_PRESENCE(
-            state=user_data["state"],
-            last_seen_device_type=user_data["lastSeen"]["deviceType"],
-            last_seen_title_id=user_data["lastSeen"]["titleId"],
-            last_seen_title_name=user_data["lastSeen"]["titleName"],
-            last_seen_timestamp=user_data["lastSeen"]["timestamp"]
-        )
-        return presence
-
-    def get_user_achievements(self, xuid: str):
-        """
-        Get user achievements
-
-        Args:
-            xuid (str): xuid of specified user
-
-        Returns:
-            list: user achievements.
-        """
-        endpoint = self.url.achievements_xuid_url(xuid)
-        response = self._make_request(endpoint).json()
-        user_data = response['titles']
-        return user_data
-
-    def get_title_achievements(self, xuid: str, titleId: str):
-        """
-        Get user achievements for a specific title
-
-        Args:
-            xuid (str): xuid of specified user
-            titleId (str): titleId of specified title
-
-        Returns:
-            list: user achievements for the specified title.
-        """
-        endpoint = self.url.title_achievements_xuid_url(xuid, titleId)
-        response = self._make_request(endpoint).json()
-        user_data = response["achievements"]
-        return user_data
-
-    def get_title360_achievements(self, xuid: str, titleId: str):
-        """
-        Get user achievements for a specific title
-
-        Args:
-            xuid (str): xuid of specified user
-            titleId (str): titleId of specified title
-
-        Returns:
-            list: user achievements for the specified title.
-        """
-        endpoint = self.url.title360_achievements_xuid_url(xuid, titleId)
-        response = self._make_request(endpoint).json()
-        user_data = response["achievements"]
-        return user_data
-
-    def get_player360_achievements(self, xuid: str, titleId: str):
-        """
-        Get user achievements for a specific title
-
-        Args:
-            xuid (str): xuid of specified user
-            titleId (str): titleId of specified title
-
-        Returns:
-            list: user achievements for the specified title.
-        """
-        endpoint = self.url.player360_achievements_xuid_url(xuid, titleId)
-        response = self._make_request(endpoint).json()
-        user_data = response["achievements"]
-        return user_data
-
-    def get_club_details(self, clubId: str):
-        """
-        Get club details
-
-        Args:
-            clubId (str): clubId of specified club
-
-        Returns:
-            CLUB_DETAILS: club details.
-            Object attributes:
-            - identificator: str
-            - clubType: str
-            - creationDateUtc: str
-            - settings: list
-            - followersCount: int
-            - membersCount: int
-            - moderatorsCount: int
-            - recommendedCount: int
-            - requestedToJoinCount: int
-            - clubPresenceCount: int
-            - clubPresenceTodayCount: int
-            - clubPresenceInGameCount: int
-            - roster: list
-            - targetRoles: list
-            - recommendation: list
-            - clubPresence: list
-            - state: str
-            - suspendedUntilUtc: str
-            - reportCount: int
-            - reportedItemsCount: int
-            - maxMembersPerClub: int
-            - ownerXuid: str
-            - founderXuid: str
-            - description: str
-            - rules: str
-            - name: str
-            - shortName: str
-            - isSearchable: bool
-            - isRecommendable: bool
-            - requestToJoinEnabled: bool
-            - openJoinEnabled: bool
-            - leaveEnabled: bool
-            - transferOwnershipEnabled: bool
-            - matureContentEnabled: bool
-            - watchClubTitlesOnly: bool
-            - displayImageUrl: str
-            - backgroundImageUrl: str
-            - preferredLocale: str
-            - tags: list
-            - associatedTitles: list
-            - primaryColor: str
-            - secondaryColor: str
-            - tertiaryColor: str
-        """
-        endpoint = self.url.club_details_url(clubId)
-        response = self._make_request(endpoint).json()
-        club_data = response["clubs"][0]
-        club_details = CLUB_DETAILS(
-            identificator=club_data["id"],
-            clubType=club_data["clubType"],
-            creationDateUtc=club_data["creationDateUtc"],
-            settings=club_data["settings"],
-            followersCount=club_data["followersCount"],
-            membersCount=club_data["membersCount"],
-            moderatorsCount=club_data["moderatorsCount"],
-            recommendedCount=club_data["recommendedCount"],
-            requestedToJoinCount=club_data["requestedToJoinCount"],
-            clubPresenceCount=club_data["clubPresenceCount"],
-            clubPresenceTodayCount=club_data["clubPresenceTodayCount"],
-            clubPresenceInGameCount=club_data["clubPresenceInGameCount"],
-            roster=club_data["roster"],
-            targetRoles=club_data["targetRoles"],
-            recommendation=club_data["recommendation"],
-            clubPresence=club_data["clubPresence"],
-            state=club_data["state"],
-            suspendedUntilUtc=club_data["suspendedUntilUtc"],
-            reportCount=club_data["reportCount"],
-            reportedItemsCount=club_data["reportedItemsCount"],
-            maxMembersPerClub=club_data["maxMembersPerClub"],
-            ownerXuid=club_data["ownerXuid"],
-            founderXuid=club_data["founderXuid"],
-            description=club_data["profile"]["description"]["value"],
-            rules=club_data["profile"]["rules"]["value"],
-            name=club_data["profile"]["name"]["value"],
-            shortName=club_data["profile"]["shortName"]["value"],
-            isSearchable=club_data["profile"]["isSearchable"]["value"],
-            isRecommendable=club_data["profile"]["isRecommendable"]["value"],
-            requestToJoinEnabled=club_data["profile"]["requestToJoinEnabled"]["value"],
-            openJoinEnabled=club_data["profile"]["openJoinEnabled"]["value"],
-            leaveEnabled=club_data["profile"]["leaveEnabled"]["value"],
-            transferOwnershipEnabled=club_data["profile"]["transferOwnershipEnabled"]["value"],
-            matureContentEnabled=club_data["profile"]["matureContentEnabled"]["value"],
-            watchClubTitlesOnly=club_data["profile"]["watchClubTitlesOnly"]["value"],
-            displayImageUrl=club_data["profile"]["displayImageUrl"]["value"],
-            backgroundImageUrl=club_data["profile"]["backgroundImageUrl"]["value"],
-            preferredLocale=club_data["profile"]["preferredLocale"]["value"],
-            tags=club_data["profile"]["tags"]["value"],
-            associatedTitles=club_data["profile"]["associatedTitles"]["value"],
-            primaryColor=club_data["profile"]["primaryColor"]["value"],
-            secondaryColor=club_data["profile"]["secondaryColor"]["value"],
-            tertiaryColor=club_data["profile"]["tertiaryColor"]["value"]
-        )
-        return club_details
-
-    def get_friends_xuid(self, xuid: str):
-        """
-        Get user friends
-
-        Args:
-            xuid (str): xuid of specified user
-
-        Returns:
-            list: user friends.
-        """
-        endpoint = self.url.friends_xuid_url(xuid)
-        response = self._make_request(endpoint).json()
-        friend_data = response['people'][0]
-        friend_details = ACCOUNT_INFO_GAMERTAG(
-            xuid=friend_data["xuid"],
-            displayName=friend_data["displayName"],
-            realName=friend_data["realName"],
-            displayPicRaw=friend_data["displayPicRaw"],
-            showUserAsAvatar=friend_data["showUserAsAvatar"],
-            gamertag=friend_data["gamertag"],
-            gamerScore=friend_data["gamerScore"],
-            modernGamertag=friend_data["modernGamertag"],
-            modernGamertagSuffix=friend_data["modernGamertagSuffix"],
-            uniqueModernGamertag=friend_data["uniqueModernGamertag"],
-            xboxOneRep=friend_data["xboxOneRep"],
-            presenceState=friend_data["presenceState"],
-            presenceText=friend_data["presenceText"],
-            presenceDevices=friend_data["presenceDevices"],
-            isBroadcasting=friend_data["isBroadcasting"],
-            isCloaked=friend_data["isCloaked"],
-            isQuarantined=friend_data["isQuarantined"],
-            isXbox360Gamerpic=friend_data["isXbox360Gamerpic"],
-            lastSeenDateTimeUtc=friend_data["lastSeenDateTimeUtc"],
-            preferredColor=friend_data["preferredColor"],
-            presenceDetails=friend_data["presenceDetails"],
-            titlePresence=friend_data["titlePresence"],
-            titleSummaries=friend_data["titleSummaries"],
-            accountTier=friend_data["detail"]["accountTier"],
-            bio=friend_data["detail"]["bio"],
-            isVerified=friend_data["detail"]["isVerified"],
-            location=friend_data["detail"]["location"],
-            tenure=friend_data["detail"]["tenure"],
-            watermarks=friend_data["detail"]["watermarks"],
-            blocked=friend_data["detail"]["blocked"],
-            mute=friend_data["detail"]["mute"],
-            followerCount=friend_data["detail"]["followerCount"],
-            followingCount=friend_data["detail"]["followingCount"],
-            hasGamePass=friend_data["detail"]["hasGamePass"],
-            socialManager=friend_data["socialManager"],
-            broadcast=friend_data["broadcast"],
-            avatar=friend_data["avatar"],
-            linkedAccounts=friend_data["linkedAccounts"],
-            colorTheme=friend_data["colorTheme"],
-            preferredPlatforms=friend_data["preferredPlatforms"],
-        )
-        return friend_details
-
-    def search_friend_list(self, gamertag: str):
-        """
-        Search for a friend
-
-        Args:
-            gamertag (str): gamertag of specified user
-
-        Returns:
-            FRIEND_INFO_GAMERTAG: friend info.
-            Object attributes:
-            - GameDisplayPicRaw: str
-            - Gamerscore: str
-            - Gamertag: str
-            - AccountTier: str
-            - XboxOneRep: str
-            - RealName: str
-            - Bio: str
-            - TenureLevel: str
-            - Watermarks: str
-            - Location: str
-            - ShowUserAsAvatar: str
-        """
-        endpoint = self.url.search_friend_url(gamertag)
-        response = self._make_request(endpoint).json()
-        friends_data = response["profileUsers"][0]["settings"]
-        friend_data = {item['id']: item['value'] for item in friends_data}
-        friend_details = FRIEND_INFO_GAMERTAG(
-            GameDisplayPicRaw=friend_data["GameDisplayPicRaw"],
-            Gamerscore=friend_data["Gamerscore"],
-            Gamertag=friend_data["Gamertag"],
-            AccountTier=friend_data["AccountTier"],
-            XboxOneRep=friend_data["XboxOneRep"],
-            RealName=friend_data["RealName"],
-            Bio=friend_data["Bio"],
-            TenureLevel=friend_data["TenureLevel"],
-            Watermarks=friend_data["Watermarks"],
-            Location=friend_data["Location"],
-            ShowUserAsAvatar=friend_data["ShowUserAsAvatar"],
-        )
-        return friend_details
-
-    def get_gamepass_all_games(self):
-        """
-        Get all games available on Game Pass
-
-        Returns:
-            list: gamepass games.
-        """
-        endpoint = self.url.gamepass_all_url()
-        response = self._make_request(endpoint).json()[1:]
-        id_list = [item['id'] for item in response]
-        return id_list
-
-    def get_gamepass_pc_games(self):
-        """
-        Get all games available on Game Pass for PC
-
-        Returns:
-            list: Game Pass PC games.
-        """
-        endpoint = self.url.gamepass_pc_url()
-        response = self._make_request(endpoint).json()[1:]
-        id_list = [item['id'] for item in response]
-        return id_list
-
-    def get_gamepass_eaplay_games(self):
-        """
-        Get all games available on EA Play
-
-        Returns:
-            list: EA Play games.
-        """
-        endpoint = self.url.gamepass_eaplay_url()
-        response = self._make_request(endpoint).json()[1:]
-        id_list = [item['id'] for item in response]
-        return id_list
-
-    def get_gamepass_nocontroller_games(self):
-        """
-        Get all games available on Game Pass that don't require a controller
-
-        Returns:
-            list: Game Pass games that don't require a controller.
-        """
-        endpoint = self.url.gamepass_nocontroller_url()
-        response = self._make_request(endpoint).json()[1:]
-        id_list = [item['id'] for item in response]
-        return id_list
-
-    def get_new_marketplace_games(self):
-        """
-        Get all new games available on the marketplace
-
-        Returns:
-            list: new marketplace games.
-        """
-        endpoint = self.url.marketplace_new_url()
-        response = self._make_request(endpoint).json()
-        games_list = response["Products"]
-        return games_list
-
-    def get_toppaid_marketplace_games(self):
-        """
-        Get all top paid games available on the marketplace
-
-        Returns:
-            list: top paid marketplace games.
-        """
-        endpoint = self.url.marketplace_toppaid_url()
-        response = self._make_request(endpoint).json()
-        games_list = response["Products"]
-        return games_list
-
-    def get_bestrated_marketplace_games(self):
-        """
-        Get all best rated games available on the marketplace
-
-        Returns:
-            list: best rated marketplace games.
-        """
-        endpoint = self.url.marketplace_bestrated_url()
-        response = self._make_request(endpoint).json()
-        games_list = response["Products"]
-        return games_list
-
-    def get_comingcoon_marketplace_games(self):
-        """
-        Get all coming soon games available on the marketplace
-
-        Returns:
-            list: coming soon marketplace games.
-        """
-        endpoint = self.url.marketplace_comingsoon_url()
-        response = self._make_request(endpoint).json()
-        games_list = response["Products"]
-        return games_list
-
-    def get_deals_marketplace_games(self):
-        """
-        Get all deals available on the marketplace
-
-        Returns:
-            list: deals marketplace games.
-        """
-        endpoint = self.url.marketplace_deals_url()
-        response = self._make_request(endpoint).json()
-        games_list = response["Products"]
-        return games_list
-
-    def get_topfree_marketplace_games(self):
-        """
-        Get all top free games available on the marketplace
-
-        Returns:
-            list: top free marketplace games.
-        """
-        endpoint = self.url.marketplace_topfree_url()
-        response = self._make_request(endpoint).json()
-        games_list = response["Products"]
-        return games_list
-
-    def get_mostplayed_marketplace_games(self):
-        """
-        Get all most played games available on the marketplace
-
-        Returns:
-            list: most played marketplace games.
-        """
-        endpoint = self.url.marketplace_mostplayed_url()
-        response = self._make_request(endpoint).json()
-        games_list = response["Products"]
-        return games_list
-
-    def search_marketplace_game(self, titleId):
-        """
-        Search for a game on the marketplace
-
-        Args:
-            titleId (str): titleId of specified game
-
-        Returns:
-            list: marketplace games.
-        """
-        endpoint = self.url.marketplace_searchgame_url(titleId=titleId)
-        response = self._make_request(endpoint).json()
-        games_list = response["Products"]
-        return games_list
-
-    def get_player_summary(self, xuid: str):
-        """
-        Get player summary
-
-        Args:
-            xuid (str): xuid of specified user
-
-        Returns:
-            PLAYER_SUMMARY: player summary.
-            Object attributes:
-            - xuid: str
-            - isFavorite: bool
-            - isFollowingCaller: bool
-            - isFollowedByCaller: bool
-            - isIdentityShared: bool
-            - addedDateTimeUtc: str
-            - displayName: str
-            - realName: str
-            - displayPicRaw: str
-            - useAvatar: bool
-            - gamertag: str
-            - gamerScore: str
-            - xboxOneRep: str
-            - presenceState: str
-            - presenceText: str
-            - presenceDevices: list
-            - isBroadcasting: bool
-            - isCloaked: bool
-            - isQuarantined: bool
-            - suggestion: str
-            - recommendation: str
-            - titleHistory: list
-            - multiplayerSummary: dict
-            - recentPlayer: list
-            - follower: list
-            - preferredColor: dict
-            - presenceDetails: dict
-            - titlePresence: dict
-            - titleSummaries: list
-            - presenceTitleIds: list
-            - detail: dict
-            - communityManagerTitles: list
-            - socialManager: str
-            - broadcast: str
-            - tournamentSummary: dict
-            - avatar: str
-        """
-        endpoint = self.url.player_summary_url(xuid=xuid)
-        response = self._make_request(endpoint).json()
-        user_data = response['people'][0]
-        player_summary = PLAYER_SUMMARY(
-            xuid=user_data["xuid"],
-            isFavorite=user_data["isFavorite"],
-            isFollowingCaller=user_data['isFollowingCaller'],
-            isFollowedByCaller=user_data['isFollowedByCaller'],
-            isIdentityShared=user_data['isIdentityShared'],
-            addedDateTimeUtc=user_data['addedDateTimeUtc'],
-            displayName=user_data['displayName'],
-            realName=user_data['realName'],
-            displayPicRaw=user_data['displayPicRaw'],
-            useAvatar=user_data['useAvatar'],
-            gamertag=user_data['gamertag'],
-            gamerScore=user_data['gamerScore'],
-            xboxOneRep=user_data['xboxOneRep'],
-            presenceState=user_data['presenceState'],
-            presenceText=user_data['presenceText'],
-            presenceDevices=user_data['presenceDevices'],
-            isBroadcasting=user_data['isBroadcasting'],
-            isCloaked=user_data['isCloaked'],
-            isQuarantined=user_data['isQuarantined'],
-            suggestion=user_data['suggestion'],
-            recommendation=user_data['recommendation'],
-            titleHistory=user_data['titleHistory'],
-            multiplayerSummary=user_data['multiplayerSummary'],
-            recentPlayer=user_data['recentPlayer'],
-            follower=user_data['follower'],
-            preferredColor=user_data['preferredColor'],
-            presenceDetails=user_data['presenceDetails'],
-            titlePresence=user_data['titlePresence'],
-            titleSummaries=user_data['titleSummaries'],
-            presenceTitleIds=user_data['presenceTitleIds'],
-            detail=user_data['detail'],
-            communityManagerTitles=user_data['communityManagerTitles'],
-            socialManager=user_data['socialManager'],
-            broadcast=user_data['broadcast'],
-            tournamentSummary=user_data['tournamentSummary'],
-            avatar=user_data['avatar'],
-        )
-        return player_summary
-
-    def get_player_title_history(self, xuid: str):
-        """
-        Get player title history
-
-        Args:
-            xuid (str): xuid of specified user
-
-        Returns:
-            list: player title history.
-        """
-        endpoint = self.url.player_titleHistory_url(xuid=xuid)
-        response = self._make_request(endpoint).json()
-        titie_history = response['titles']
-        return titie_history
-
-    def get_session_details(self, sessionName: str):
-        """
-        Get session details
-
-        Args:
-            sessionName (str): name of specified session
-
-        Returns:
-            dict: session details.
-        """
-        endpoint = self.url.session_details_url(sessionName=sessionName)
-        response = self._make_request(endpoint).json()
-        session_details = response
-        return session_details
-
-    def get_group_summary(self, groupId):
-        """
-        Get group summary
-
-        Args:
-            groupId (str): groupId of specified group
-
-        Returns:
-            dict: group summary.
-        """
-        endpoint = self.url.group_summary_url(groupId=groupId)
-        response = self._make_request(endpoint).json()
-        group_summary = response
-        return group_summary
-
-    def get_group_messages(self, groupId: str):
-        """
-        Get group messages
-
-        Args:
-            groupId (str): groupId of specified group
-
-        Returns:
-            list: group messages.
-        """
-        endpoint = self.url.group_messages_url(groupId=groupId)
-        response = self._make_request(endpoint).json()
-        group_messages = response["messages"]
-        return group_messages
+import requests
+
+from .URLs import URLs
+from .classes.ACCOUNT_INFO_GAMERTAG import ACCOUNT_INFO_GAMERTAG
+from .classes.ACCOUNT_INFO_XUID import ACCOUNT_INFO_XUID
+from .classes.CLUB_DETAILS import CLUB_DETAILS
+from .classes.FRIEND_INFO_GAMERTAG import FRIEND_INFO_GAMERTAG
+from .classes.PLAYER_SUMMARY import PLAYER_SUMMARY
+from .classes.XUID_PRESENCE import XUID_PRESENCE
+
+
+class XPA:
+    def __init__(self, api_key):
+        self.api_key = api_key
+        self.url = URLs()
+
+    def _make_request(self, endpoint):
+        headers = {'x-authorization': self.api_key}
+        return requests.get(endpoint, headers=headers)
+
+    def _find_setting_by_id(self, settings, setting_id):
+        for setting in settings:
+            if setting['id'] == setting_id:
+                return setting['value']
+        return None
+
+    def get_account_info_xuid(self, xuid: str) -> ACCOUNT_INFO_XUID:
+        """Get someone's profile information
+
+        Args:
+            xuid (str): xuid of specified user.
+
+        Returns:
+            ACCOUNT_INFO_XUID: user account info.
+            
+            Object attributes:
+            - GameDisplayPicRaw: str
+            - Gamerscore: str
+            - Gamertag: str
+            - AccountTier: str
+            - XboxOneRep: str
+            - PreferredColor: str
+            - RealName: str
+            - Bio: str
+            - Location: str
+        """
+        endpoint = self.url.account_xuid_url(xuid)
+        response = self._make_request(endpoint).json()
+        user_data = response['profileUsers'][0]['settings']
+        account_info = ACCOUNT_INFO_XUID(
+            GameDisplayPicRaw=self._find_setting_by_id(user_data, 'GameDisplayPicRaw'),
+            Gamerscore=self._find_setting_by_id(user_data, 'Gamerscore'),
+            Gamertag=self._find_setting_by_id(user_data, 'Gamertag'),
+            AccountTier=self._find_setting_by_id(user_data, 'AccountTier'),
+            XboxOneRep=self._find_setting_by_id(user_data, 'XboxOneRep'),
+            PreferredColor=self._find_setting_by_id(user_data, 'PreferredColor'),
+            RealName=self._find_setting_by_id(user_data, 'RealName'),
+            Bio=self._find_setting_by_id(user_data, 'Bio'),
+            Location=self._find_setting_by_id(user_data, 'Location')
+        )
+        return account_info
+
+    def get_account_info_gamertag(self, gamertag: str) -> ACCOUNT_INFO_GAMERTAG:
+        """
+        Get someone's profile information
+
+        Args:
+            gamertag (str): gamertag of specified user
+
+        Returns:
+            ACCOUNT_INFO_GAMERTAG: user account info.
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
+        """
+        endpoint = self.url.search_gamertag_url(gamertag)
+        response = self._make_request(endpoint).json()
+        user_data = response['people'][0]
+        account_info = ACCOUNT_INFO_GAMERTAG(
+            xuid=user_data["xuid"],
+            displayName=user_data["displayName"],
+            realName=user_data["realName"],
+            displayPicRaw=user_data["displayPicRaw"],
+            showUserAsAvatar=user_data["showUserAsAvatar"],
+            gamertag=user_data["gamertag"],
+            gamerScore=user_data["gamerScore"],
+            modernGamertag=user_data["modernGamertag"],
+            modernGamertagSuffix=user_data["modernGamertagSuffix"],
+            uniqueModernGamertag=user_data["uniqueModernGamertag"],
+            xboxOneRep=user_data["xboxOneRep"],
+            presenceState=user_data["presenceState"],
+            presenceText=user_data["presenceText"],
+            presenceDevices=user_data["presenceDevices"],
+            isBroadcasting=user_data["isBroadcasting"],
+            isCloaked=user_data["isCloaked"],
+            isQuarantined=user_data["isQuarantined"],
+            isXbox360Gamerpic=user_data["isXbox360Gamerpic"],
+            lastSeenDateTimeUtc=user_data["lastSeenDateTimeUtc"],
+            preferredColor=user_data["preferredColor"],
+            presenceDetails=user_data["presenceDetails"],
+            titlePresence=user_data["titlePresence"],
+            titleSummaries=user_data["titleSummaries"],
+            accountTier=user_data["detail"]["accountTier"],
+            bio=user_data["detail"]["bio"],
+            isVerified=user_data["detail"]["isVerified"],
+            location=user_data["detail"]["location"],
+            tenure=user_data["detail"]["tenure"],
+            watermarks=user_data["detail"]["watermarks"],
+            blocked=user_data["detail"]["blocked"],
+            mute=user_data["detail"]["mute"],
+            followerCount=user_data["detail"]["followerCount"],
+            followingCount=user_data["detail"]["followingCount"],
+            hasGamePass=user_data["detail"]["hasGamePass"],
+            socialManager=user_data["socialManager"],
+            broadcast=user_data["broadcast"],
+            avatar=user_data["avatar"],
+            linkedAccounts=user_data["linkedAccounts"],
+            colorTheme=user_data["colorTheme"],
+            preferredPlatforms=user_data["preferredPlatforms"],
+        )
+        return account_info
+
+    def get_presence(self, xuid: str) -> XUID_PRESENCE:
+        """
+        Get user presence information
+
+        Args:
+            xuid (str): xuid of specified user
+
+        Returns:
+            XUID_PRESENCE: user presence info.
+            Object attributes:
+            - state: str
+            - last_seen_device_type: str
+            - last_seen_title_id: str
+            - last_seen_title_name: str
+            - last_seen_timestamp: str
+        """
+        endpoint = self.url.xuid_presence_url(xuid)
+        response = self._make_request(endpoint).json()
+        user_data = response[0]
+        presence = XUID_PRESENCE(
+            state=user_data["state"],
+            last_seen_device_type=user_data["lastSeen"]["deviceType"],
+            last_seen_title_id=user_data["lastSeen"]["titleId"],
+            last_seen_title_name=user_data["lastSeen"]["titleName"],
+            last_seen_timestamp=user_data["lastSeen"]["timestamp"]
+        )
+        return presence
+
+    def get_user_achievements(self, xuid: str):
+        """
+        Get user achievements
+
+        Args:
+            xuid (str): xuid of specified user
+
+        Returns:
+            list: user achievements.
+        """
+        endpoint = self.url.achievements_xuid_url(xuid)
+        response = self._make_request(endpoint).json()
+        user_data = response['titles']
+        return user_data
+
+    def get_title_achievements(self, xuid: str, titleId: str):
+        """
+        Get user achievements for a specific title
+
+        Args:
+            xuid (str): xuid of specified user
+            titleId (str): titleId of specified title
+
+        Returns:
+            list: user achievements for the specified title.
+        """
+        endpoint = self.url.title_achievements_xuid_url(xuid, titleId)
+        response = self._make_request(endpoint).json()
+        user_data = response["achievements"]
+        return user_data
+
+    def get_title360_achievements(self, xuid: str, titleId: str):
+        """
+        Get user achievements for a specific title
+
+        Args:
+            xuid (str): xuid of specified user
+            titleId (str): titleId of specified title
+
+        Returns:
+            list: user achievements for the specified title.
+        """
+        endpoint = self.url.title360_achievements_xuid_url(xuid, titleId)
+        response = self._make_request(endpoint).json()
+        user_data = response["achievements"]
+        return user_data
+
+    def get_player360_achievements(self, xuid: str, titleId: str):
+        """
+        Get user achievements for a specific title
+
+        Args:
+            xuid (str): xuid of specified user
+            titleId (str): titleId of specified title
+
+        Returns:
+            list: user achievements for the specified title.
+        """
+        endpoint = self.url.player360_achievements_xuid_url(xuid, titleId)
+        response = self._make_request(endpoint).json()
+        user_data = response["achievements"]
+        return user_data
+
+    def get_club_details(self, clubId: str) -> CLUB_DETAILS:
+        """
+        Get club details
+
+        Args:
+            clubId (str): clubId of specified club
+
+        Returns:
+            CLUB_DETAILS: club details.
+            Object attributes:
+            - identificator: str
+            - clubType: str
+            - creationDateUtc: str
+            - settings: list
+            - followersCount: int
+            - membersCount: int
+            - moderatorsCount: int
+            - recommendedCount: int
+            - requestedToJoinCount: int
+            - clubPresenceCount: int
+            - clubPresenceTodayCount: int
+            - clubPresenceInGameCount: int
+            - roster: list
+            - targetRoles: list
+            - recommendation: list
+            - clubPresence: list
+            - state: str
+            - suspendedUntilUtc: str
+            - reportCount: int
+            - reportedItemsCount: int
+            - maxMembersPerClub: int
+            - ownerXuid: str
+            - founderXuid: str
+            - description: str
+            - rules: str
+            - name: str
+            - shortName: str
+            - isSearchable: bool
+            - isRecommendable: bool
+            - requestToJoinEnabled: bool
+            - openJoinEnabled: bool
+            - leaveEnabled: bool
+            - transferOwnershipEnabled: bool
+            - matureContentEnabled: bool
+            - watchClubTitlesOnly: bool
+            - displayImageUrl: str
+            - backgroundImageUrl: str
+            - preferredLocale: str
+            - tags: list
+            - associatedTitles: list
+            - primaryColor: str
+            - secondaryColor: str
+            - tertiaryColor: str
+        """
+        endpoint = self.url.club_details_url(clubId)
+        response = self._make_request(endpoint).json()
+        club_data = response["clubs"][0]
+        club_details = CLUB_DETAILS(
+            identificator=club_data["id"],
+            clubType=club_data["clubType"],
+            creationDateUtc=club_data["creationDateUtc"],
+            settings=club_data["settings"],
+            followersCount=club_data["followersCount"],
+            membersCount=club_data["membersCount"],
+            moderatorsCount=club_data["moderatorsCount"],
+            recommendedCount=club_data["recommendedCount"],
+            requestedToJoinCount=club_data["requestedToJoinCount"],
+            clubPresenceCount=club_data["clubPresenceCount"],
+            clubPresenceTodayCount=club_data["clubPresenceTodayCount"],
+            clubPresenceInGameCount=club_data["clubPresenceInGameCount"],
+            roster=club_data["roster"],
+            targetRoles=club_data["targetRoles"],
+            recommendation=club_data["recommendation"],
+            clubPresence=club_data["clubPresence"],
+            state=club_data["state"],
+            suspendedUntilUtc=club_data["suspendedUntilUtc"],
+            reportCount=club_data["reportCount"],
+            reportedItemsCount=club_data["reportedItemsCount"],
+            maxMembersPerClub=club_data["maxMembersPerClub"],
+            ownerXuid=club_data["ownerXuid"],
+            founderXuid=club_data["founderXuid"],
+            description=club_data["profile"]["description"]["value"],
+            rules=club_data["profile"]["rules"]["value"],
+            name=club_data["profile"]["name"]["value"],
+            shortName=club_data["profile"]["shortName"]["value"],
+            isSearchable=club_data["profile"]["isSearchable"]["value"],
+            isRecommendable=club_data["profile"]["isRecommendable"]["value"],
+            requestToJoinEnabled=club_data["profile"]["requestToJoinEnabled"]["value"],
+            openJoinEnabled=club_data["profile"]["openJoinEnabled"]["value"],
+            leaveEnabled=club_data["profile"]["leaveEnabled"]["value"],
+            transferOwnershipEnabled=club_data["profile"]["transferOwnershipEnabled"]["value"],
+            matureContentEnabled=club_data["profile"]["matureContentEnabled"]["value"],
+            watchClubTitlesOnly=club_data["profile"]["watchClubTitlesOnly"]["value"],
+            displayImageUrl=club_data["profile"]["displayImageUrl"]["value"],
+            backgroundImageUrl=club_data["profile"]["backgroundImageUrl"]["value"],
+            preferredLocale=club_data["profile"]["preferredLocale"]["value"],
+            tags=club_data["profile"]["tags"]["value"],
+            associatedTitles=club_data["profile"]["associatedTitles"]["value"],
+            primaryColor=club_data["profile"]["primaryColor"]["value"],
+            secondaryColor=club_data["profile"]["secondaryColor"]["value"],
+            tertiaryColor=club_data["profile"]["tertiaryColor"]["value"]
+        )
+        return club_details
+
+    def get_friends_xuid(self, xuid: str) -> ACCOUNT_INFO_GAMERTAG:
+        """
+        Get user friends
+
+        Args:
+            xuid (str): xuid of specified user
+
+        Returns:
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
+        """
+        endpoint = self.url.friends_xuid_url(xuid)
+        response = self._make_request(endpoint).json()
+        friend_data = response['people'][0]
+        friend_details = ACCOUNT_INFO_GAMERTAG(
+            xuid=friend_data["xuid"],
+            displayName=friend_data["displayName"],
+            realName=friend_data["realName"],
+            displayPicRaw=friend_data["displayPicRaw"],
+            showUserAsAvatar=friend_data["showUserAsAvatar"],
+            gamertag=friend_data["gamertag"],
+            gamerScore=friend_data["gamerScore"],
+            modernGamertag=friend_data["modernGamertag"],
+            modernGamertagSuffix=friend_data["modernGamertagSuffix"],
+            uniqueModernGamertag=friend_data["uniqueModernGamertag"],
+            xboxOneRep=friend_data["xboxOneRep"],
+            presenceState=friend_data["presenceState"],
+            presenceText=friend_data["presenceText"],
+            presenceDevices=friend_data["presenceDevices"],
+            isBroadcasting=friend_data["isBroadcasting"],
+            isCloaked=friend_data["isCloaked"],
+            isQuarantined=friend_data["isQuarantined"],
+            isXbox360Gamerpic=friend_data["isXbox360Gamerpic"],
+            lastSeenDateTimeUtc=friend_data["lastSeenDateTimeUtc"],
+            preferredColor=friend_data["preferredColor"],
+            presenceDetails=friend_data["presenceDetails"],
+            titlePresence=friend_data["titlePresence"],
+            titleSummaries=friend_data["titleSummaries"],
+            accountTier=friend_data["detail"]["accountTier"],
+            bio=friend_data["detail"]["bio"],
+            isVerified=friend_data["detail"]["isVerified"],
+            location=friend_data["detail"]["location"],
+            tenure=friend_data["detail"]["tenure"],
+            watermarks=friend_data["detail"]["watermarks"],
+            blocked=friend_data["detail"]["blocked"],
+            mute=friend_data["detail"]["mute"],
+            followerCount=friend_data["detail"]["followerCount"],
+            followingCount=friend_data["detail"]["followingCount"],
+            hasGamePass=friend_data["detail"]["hasGamePass"],
+            socialManager=friend_data["socialManager"],
+            broadcast=friend_data["broadcast"],
+            avatar=friend_data["avatar"],
+            linkedAccounts=friend_data["linkedAccounts"],
+            colorTheme=friend_data["colorTheme"],
+            preferredPlatforms=friend_data["preferredPlatforms"],
+        )
+        return friend_details
+
+    def search_friend_list(self, gamertag: str) -> FRIEND_INFO_GAMERTAG:
+        """
+        Search for a friend
+
+        Args:
+            gamertag (str): gamertag of specified user
+
+        Returns:
+            FRIEND_INFO_GAMERTAG: friend info.
+            Object attributes:
+            - GameDisplayPicRaw: str
+            - Gamerscore: str
+            - Gamertag: str
+            - AccountTier: str
+            - XboxOneRep: str
+            - RealName: str
+            - Bio: str
+            - TenureLevel: str
+            - Watermarks: str
+            - Location: str
+            - ShowUserAsAvatar: str
+        """
+        endpoint = self.url.search_friend_url(gamertag)
+        response = self._make_request(endpoint).json()
+        friends_data = response["profileUsers"][0]["settings"]
+        friend_data = {item['id']: item['value'] for item in friends_data}
+        friend_details = FRIEND_INFO_GAMERTAG(
+            GameDisplayPicRaw=friend_data["GameDisplayPicRaw"],
+            Gamerscore=friend_data["Gamerscore"],
+            Gamertag=friend_data["Gamertag"],
+            AccountTier=friend_data["AccountTier"],
+            XboxOneRep=friend_data["XboxOneRep"],
+            RealName=friend_data["RealName"],
+            Bio=friend_data["Bio"],
+            TenureLevel=friend_data["TenureLevel"],
+            Watermarks=friend_data["Watermarks"],
+            Location=friend_data["Location"],
+            ShowUserAsAvatar=friend_data["ShowUserAsAvatar"],
+        )
+        return friend_details
+
+    def get_gamepass_all_games(self):
+        """
+        Get all games available on Game Pass
+
+        Returns:
+            list: gamepass games.
+        """
+        endpoint = self.url.gamepass_all_url()
+        response = self._make_request(endpoint).json()[1:]
+        id_list = [item['id'] for item in response]
+        return id_list
+
+    def get_gamepass_pc_games(self):
+        """
+        Get all games available on Game Pass for PC
+
+        Returns:
+            list: Game Pass PC games.
+        """
+        endpoint = self.url.gamepass_pc_url()
+        response = self._make_request(endpoint).json()[1:]
+        id_list = [item['id'] for item in response]
+        return id_list
+
+    def get_gamepass_eaplay_games(self):
+        """
+        Get all games available on EA Play
+
+        Returns:
+            list: EA Play games.
+        """
+        endpoint = self.url.gamepass_eaplay_url()
+        response = self._make_request(endpoint).json()[1:]
+        id_list = [item['id'] for item in response]
+        return id_list
+
+    def get_gamepass_nocontroller_games(self):
+        """
+        Get all games available on Game Pass that don't require a controller
+
+        Returns:
+            list: Game Pass games that don't require a controller.
+        """
+        endpoint = self.url.gamepass_nocontroller_url()
+        response = self._make_request(endpoint).json()[1:]
+        id_list = [item['id'] for item in response]
+        return id_list
+
+    def get_new_marketplace_games(self):
+        """
+        Get all new games available on the marketplace
+
+        Returns:
+            list: new marketplace games.
+        """
+        endpoint = self.url.marketplace_new_url()
+        response = self._make_request(endpoint).json()
+        games_list = response["Products"]
+        return games_list
+
+    def get_toppaid_marketplace_games(self):
+        """
+        Get all top paid games available on the marketplace
+
+        Returns:
+            list: top paid marketplace games.
+        """
+        endpoint = self.url.marketplace_toppaid_url()
+        response = self._make_request(endpoint).json()
+        games_list = response["Products"]
+        return games_list
+
+    def get_bestrated_marketplace_games(self):
+        """
+        Get all best rated games available on the marketplace
+
+        Returns:
+            list: best rated marketplace games.
+        """
+        endpoint = self.url.marketplace_bestrated_url()
+        response = self._make_request(endpoint).json()
+        games_list = response["Products"]
+        return games_list
+
+    def get_comingcoon_marketplace_games(self):
+        """
+        Get all coming soon games available on the marketplace
+
+        Returns:
+            list: coming soon marketplace games.
+        """
+        endpoint = self.url.marketplace_comingsoon_url()
+        response = self._make_request(endpoint).json()
+        games_list = response["Products"]
+        return games_list
+
+    def get_deals_marketplace_games(self):
+        """
+        Get all deals available on the marketplace
+
+        Returns:
+            list: deals marketplace games.
+        """
+        endpoint = self.url.marketplace_deals_url()
+        response = self._make_request(endpoint).json()
+        games_list = response["Products"]
+        return games_list
+
+    def get_topfree_marketplace_games(self):
+        """
+        Get all top free games available on the marketplace
+
+        Returns:
+            list: top free marketplace games.
+        """
+        endpoint = self.url.marketplace_topfree_url()
+        response = self._make_request(endpoint).json()
+        games_list = response["Products"]
+        return games_list
+
+    def get_mostplayed_marketplace_games(self):
+        """
+        Get all most played games available on the marketplace
+
+        Returns:
+            list: most played marketplace games.
+        """
+        endpoint = self.url.marketplace_mostplayed_url()
+        response = self._make_request(endpoint).json()
+        games_list = response["Products"]
+        return games_list
+
+    def search_marketplace_game(self, titleId):
+        """
+        Search for a game on the marketplace
+
+        Args:
+            titleId (str): titleId of specified game
+
+        Returns:
+            list: marketplace games.
+        """
+        endpoint = self.url.marketplace_searchgame_url(titleId=titleId)
+        response = self._make_request(endpoint).json()
+        games_list = response["Products"]
+        return games_list
+
+    def get_player_summary(self, xuid: str) -> PLAYER_SUMMARY:
+        """
+        Get player summary
+
+        Args:
+            xuid (str): xuid of specified user
+
+        Returns:
+            PLAYER_SUMMARY: player summary.
+            Object attributes:
+            - xuid: str
+            - isFavorite: bool
+            - isFollowingCaller: bool
+            - isFollowedByCaller: bool
+            - isIdentityShared: bool
+            - addedDateTimeUtc: str
+            - displayName: str
+            - realName: str
+            - displayPicRaw: str
+            - useAvatar: bool
+            - gamertag: str
+            - gamerScore: str
+            - xboxOneRep: str
+            - presenceState: str
+            - presenceText: str
+            - presenceDevices: list
+            - isBroadcasting: bool
+            - isCloaked: bool
+            - isQuarantined: bool
+            - suggestion: str
+            - recommendation: str
+            - titleHistory: list
+            - multiplayerSummary: dict
+            - recentPlayer: list
+            - follower: list
+            - preferredColor: dict
+            - presenceDetails: dict
+            - titlePresence: dict
+            - titleSummaries: list
+            - presenceTitleIds: list
+            - detail: dict
+            - communityManagerTitles: list
+            - socialManager: str
+            - broadcast: str
+            - tournamentSummary: dict
+            - avatar: str
+        """
+        endpoint = self.url.player_summary_url(xuid=xuid)
+        response = self._make_request(endpoint).json()
+        user_data = response['people'][0]
+        player_summary = PLAYER_SUMMARY(
+            xuid=user_data["xuid"],
+            isFavorite=user_data["isFavorite"],
+            isFollowingCaller=user_data['isFollowingCaller'],
+            isFollowedByCaller=user_data['isFollowedByCaller'],
+            isIdentityShared=user_data['isIdentityShared'],
+            addedDateTimeUtc=user_data['addedDateTimeUtc'],
+            displayName=user_data['displayName'],
+            realName=user_data['realName'],
+            displayPicRaw=user_data['displayPicRaw'],
+            useAvatar=user_data['useAvatar'],
+            gamertag=user_data['gamertag'],
+            gamerScore=user_data['gamerScore'],
+            xboxOneRep=user_data['xboxOneRep'],
+            presenceState=user_data['presenceState'],
+            presenceText=user_data['presenceText'],
+            presenceDevices=user_data['presenceDevices'],
+            isBroadcasting=user_data['isBroadcasting'],
+            isCloaked=user_data['isCloaked'],
+            isQuarantined=user_data['isQuarantined'],
+            suggestion=user_data['suggestion'],
+            recommendation=user_data['recommendation'],
+            titleHistory=user_data['titleHistory'],
+            multiplayerSummary=user_data['multiplayerSummary'],
+            recentPlayer=user_data['recentPlayer'],
+            follower=user_data['follower'],
+            preferredColor=user_data['preferredColor'],
+            presenceDetails=user_data['presenceDetails'],
+            titlePresence=user_data['titlePresence'],
+            titleSummaries=user_data['titleSummaries'],
+            presenceTitleIds=user_data['presenceTitleIds'],
+            detail=user_data['detail'],
+            communityManagerTitles=user_data['communityManagerTitles'],
+            socialManager=user_data['socialManager'],
+            broadcast=user_data['broadcast'],
+            tournamentSummary=user_data['tournamentSummary'],
+            avatar=user_data['avatar'],
+        )
+        return player_summary
+
+    def get_player_title_history(self, xuid: str):
+        """
+        Get player title history
+
+        Args:
+            xuid (str): xuid of specified user
+
+        Returns:
+            list: player title history.
+        """
+        endpoint = self.url.player_titleHistory_url(xuid=xuid)
+        response = self._make_request(endpoint).json()
+        titie_history = response['titles']
+        return titie_history
+
+    def get_session_details(self, sessionName: str):
+        """
+        Get session details
+
+        Args:
+            sessionName (str): name of specified session
+
+        Returns:
+            dict: session details.
+        """
+        endpoint = self.url.session_details_url(sessionName=sessionName)
+        response = self._make_request(endpoint).json()
+        session_details = response
+        return session_details
+
+    def get_group_summary(self, groupId):
+        """
+        Get group summary
+
+        Args:
+            groupId (str): groupId of specified group
+
+        Returns:
+            dict: group summary.
+        """
+        endpoint = self.url.group_summary_url(groupId=groupId)
+        response = self._make_request(endpoint).json()
+        group_summary = response
+        return group_summary
+
+    def get_group_messages(self, groupId: str):
+        """
+        Get group messages
+
+        Args:
+            groupId (str): groupId of specified group
+
+        Returns:
+            list: group messages.
+        """
+        endpoint = self.url.group_messages_url(groupId=groupId)
+        response = self._make_request(endpoint).json()
+        group_messages = response["messages"]
+        return group_messages
```

