# Comparing `tmp/sharded_google_photos-0.2.2.tar.gz` & `tmp/sharded_google_photos-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharded_google_photos-0.2.2.tar", max compression
+gzip compressed data, was "sharded_google_photos-0.2.3.tar", max compression
```

## Comparing `sharded_google_photos-0.2.2.tar` & `sharded_google_photos-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0    35149 2024-03-18 17:48:51.353682 sharded_google_photos-0.2.2/LICENSE
--rw-r--r--   0        0        0     4911 2024-04-12 00:24:04.266588 sharded_google_photos-0.2.2/README.md
--rw-r--r--   0        0        0      780 2024-04-12 00:24:08.844577 sharded_google_photos-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      464 2024-04-11 21:04:01.535822 sharded_google_photos-0.2.2/sharded_google_photos/backup/diffs_splitter.py
--rw-r--r--   0        0        0     9209 2024-04-12 00:24:04.267735 sharded_google_photos-0.2.2/sharded_google_photos/backup/gphotos_backup.py
--rw-r--r--   0        0        0      551 2024-03-27 17:57:15.555272 sharded_google_photos-0.2.2/sharded_google_photos/backup/gphotos_uploader.py
--rw-r--r--   0        0        0     2782 2024-04-12 00:24:04.268961 sharded_google_photos-0.2.2/sharded_google_photos/backup/media_item_repository.py
--rw-r--r--   0        0        0     2841 2024-03-27 17:57:15.558065 sharded_google_photos-0.2.2/sharded_google_photos/backup/shared_album_repository.py
--rw-r--r--   0        0        0     2193 2024-03-27 17:57:15.559288 sharded_google_photos-0.2.2/sharded_google_photos/cleanup/gphotos_cleaner.py
--rw-r--r--   0        0        0     6453 2024-04-12 00:24:04.271074 sharded_google_photos-0.2.2/sharded_google_photos/shared/gphotos_album_client.py
--rw-r--r--   0        0        0     4306 2024-04-11 20:37:57.786024 sharded_google_photos-0.2.2/sharded_google_photos/shared/gphotos_client.py
--rw-r--r--   0        0        0     9122 2024-04-12 00:24:04.272729 sharded_google_photos-0.2.2/sharded_google_photos/shared/gphotos_mediaitem_client.py
--rw-r--r--   0        0        0     1721 2024-03-27 17:57:15.565065 sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_album_client.py
--rw-r--r--   0        0        0     1540 2024-03-27 17:57:15.566785 sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_client.py
--rw-r--r--   0        0        0     1197 2024-03-27 17:57:15.567903 sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_mediaitem_client.py
--rw-r--r--   0        0        0     9185 2024-03-27 17:57:15.569275 sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_repository.py
--rw-r--r--   0        0        0      616 2024-03-29 18:32:42.115559 sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/mocked_saved_credentials_file.py
--rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 sharded_google_photos-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-18 17:48:51.353682 sharded_google_photos-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5106 2024-04-27 07:22:31.291936 sharded_google_photos-0.2.3/README.md
+-rw-r--r--   0        0        0      835 2024-04-27 07:24:15.894733 sharded_google_photos-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1600 2024-04-26 23:16:52.824355 sharded_google_photos-0.2.3/sharded_google_photos/backup/add_new_metadata.py
+-rw-r--r--   0        0        0     8966 2024-04-26 23:16:52.825254 sharded_google_photos-0.2.3/sharded_google_photos/backup/gphotos_backup.py
+-rw-r--r--   0        0        0      573 2024-04-26 23:16:52.826109 sharded_google_photos-0.2.3/sharded_google_photos/backup/gphotos_uploader.py
+-rw-r--r--   0        0        0      626 2024-04-26 23:16:52.826756 sharded_google_photos-0.2.3/sharded_google_photos/backup/group_diffs_with_metadata.py
+-rw-r--r--   0        0        0     2834 2024-04-26 23:16:52.827502 sharded_google_photos-0.2.3/sharded_google_photos/backup/media_item_repository.py
+-rw-r--r--   0        0        0      481 2024-04-26 23:16:52.828144 sharded_google_photos-0.2.3/sharded_google_photos/backup/models.py
+-rw-r--r--   0        0        0     2917 2024-04-26 23:16:52.828907 sharded_google_photos-0.2.3/sharded_google_photos/backup/shared_album_repository.py
+-rw-r--r--   0        0        0     2318 2024-04-26 23:16:52.829900 sharded_google_photos-0.2.3/sharded_google_photos/cleanup/gphotos_cleaner.py
+-rw-r--r--   0        0        0     6241 2024-04-17 07:18:04.621703 sharded_google_photos-0.2.3/sharded_google_photos/shared/gphotos_album_client.py
+-rw-r--r--   0        0        0     4290 2024-04-17 07:18:04.622619 sharded_google_photos-0.2.3/sharded_google_photos/shared/gphotos_client.py
+-rw-r--r--   0        0        0     9327 2024-04-26 23:16:52.831109 sharded_google_photos-0.2.3/sharded_google_photos/shared/gphotos_mediaitem_client.py
+-rw-r--r--   0        0        0     1721 2024-03-27 17:57:15.565065 sharded_google_photos-0.2.3/sharded_google_photos/shared/testing/fake_gphotos_album_client.py
+-rw-r--r--   0        0        0     1540 2024-04-12 16:43:18.984897 sharded_google_photos-0.2.3/sharded_google_photos/shared/testing/fake_gphotos_client.py
+-rw-r--r--   0        0        0     1197 2024-03-27 17:57:15.567903 sharded_google_photos-0.2.3/sharded_google_photos/shared/testing/fake_gphotos_mediaitem_client.py
+-rw-r--r--   0        0        0     9185 2024-03-27 17:57:15.569275 sharded_google_photos-0.2.3/sharded_google_photos/shared/testing/fake_gphotos_repository.py
+-rw-r--r--   0        0        0      616 2024-03-29 18:32:42.115559 sharded_google_photos-0.2.3/sharded_google_photos/shared/testing/mocked_saved_credentials_file.py
+-rw-r--r--   0        0        0     5789 1970-01-01 00:00:00.000000 sharded_google_photos-0.2.3/PKG-INFO
```

### Comparing `sharded_google_photos-0.2.2/LICENSE` & `sharded_google_photos-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.2/README.md` & `sharded_google_photos-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # Sharded-Google-Photos
 
 ## Description
 
-Running out of space in your Google Photos account? Wish you can upload an unlimited number of photos on Google Photos? Now you can! With this Python library, you can upload your photos to multiple Google Photo Accounts and then share those albums to your main Google Photos account. That way, you get to see all of your photos on one main Google Photos account.
+Running out of space in your Google Photos account? Wish you can upload your photos to multiple Google Accounts? Now you can! With this Python library, you can upload your photos to multiple Google Photo Accounts and then share those albums to your main Google Photos account. That way, you get to see all of your photos on one main Google Photos account.
+
+## Getting Started
 
 It works like this:
 
-1. Let's say you have three Google Accounts. Create an OAuth2 to interact with Google Photos and Google Drive.
+1. Let's say you have three Google Accounts. Follow [this doc](docs/create_client_id.md) to create your own OAuth2 Google Client ID to interact with Google Photos and Google Drive.
 
 2. Install `libmagic`
 
 3. Install the package by running `pip install sharded-google-photos`.
 
 4. Import the following code in your `main.py` app:
 
     ```python
     from sharded_google_photos.backup.gphotos_backup import GPhotosBackup
     from sharded_google_photos.shared.gphotos_client import GPhotosClient
 
     clients = [
-        GPhotosClient(creds_file = "credentials-1.json", client_secret="client_secret.json"),
-        GPhotosClient(creds_file = "credentials-2.json", client_secret="client_secret.json"),
-        GPhotosClient(creds_file = "credentials-3.json", client_secret="client_secret.json"),
+        GPhotosClient(name="bob@gmail.com", creds_file = "credentials-1.json", client_secret="client_secret.json"),
+        GPhotosClient(name="alice@gmail.com", creds_file = "credentials-2.json", client_secret="client_secret.json"),
+        GPhotosClient(name="jerry@gmail.com", creds_file = "credentials-3.json", client_secret="client_secret.json"),
     ]
     for client in clients:
         client.authenticate()
 
     backup_client = GPhotosBackup(clients)
     ```
 
+    Run this script and follow the instructions from the cli.
+
 5. To upload four photos from two folders, run the following:
 
     ```python
     new_album_uris = backup_client.backup(
         [
             { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg" },
             { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/2.jpg" },
@@ -105,15 +109,15 @@
     ```bash
     poetry run python sharded_google_photos/main.py
     ```
 
 4. To lint your code, run:
 
     ```bash
-    poetry run flake8 && poetry run black sharded_google_photos/
+    poetry run flake8 && poetry run black .
     ```
 
 5. To run tests and code coverage, run:
 
     ```bash
     poetry run coverage run -m pytest && poetry run coverage report -m
     ```
```

### Comparing `sharded_google_photos-0.2.2/pyproject.toml` & `sharded_google_photos-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 [tool.poetry]
 name = "sharded-google-photos"
-version = "0.2.2"
+version = "0.2.3"
 description = "A tool to shard photos across multiple Google Photo accounts"
 authors = ["Emilio K <e.kartonoe@gmail.com>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 google-api-python-client = "^2.122.0"
 google-auth-oauthlib = "^1.2.0"
 backoff = "^2.2.1"
 python-magic = "^0.4.27"
+tqdm = "^4.66.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 pytest = "^8.1.1"
 flake8 = "^7.0.0"
 flake8-bugbear = "^24.2.6"
 coverage = "^7.4.4"
 pytest-mock = "^3.12.0"
 requests-mock = "^1.11.0"
+freezegun = "^1.4.0"
+mypy = "^1.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 omit = [".*", "*/site-packages/*"]
```

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/backup/gphotos_backup.py` & `sharded_google_photos-0.2.3/sharded_google_photos/backup/gphotos_backup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import os
 import logging
 
 from sharded_google_photos.shared.gphotos_client import GPhotosClient
 
-from .diffs_splitter import diffs_splitter
+from .group_diffs_with_metadata import group_diffs_with_metadata
 from .shared_album_repository import SharedAlbumRepository
 from .media_item_repository import MediaItemRepository
 from .gphotos_uploader import GPhotosUploader
+from .add_new_metadata import add_new_metadata
+from .models import Diffs, DiffsWithMetadata
 
 logger = logging.getLogger(__name__)
 
 
 class NoAvailableSpaceInExistingAlbumException(Exception):
     """Exception raised when there is no space in an existing album"""
 
@@ -21,32 +22,36 @@
         self.album_title = album_title
 
 
 class GPhotosBackup:
     def __init__(self, gphoto_clients: list[GPhotosClient]):
         self.gphoto_clients = gphoto_clients
 
-    def backup(self, diffs):
+    def backup(self, diffs: Diffs):
         # Insert new metadata in the diffs
-        new_diffs = self.add_new_metadata(diffs)
+        new_diffs = add_new_metadata(diffs)
         logger.debug("Step 1: Add new metadata to the diff")
 
         # Split the diff based on the album title
-        chunked_new_diffs = diffs_splitter(new_diffs)
+        chunked_new_diffs = group_diffs_with_metadata(new_diffs)
         logger.debug("Step 2: Split the diff")
 
         # Find all the albums in all accounts with an index to which account
         shared_album_repository = SharedAlbumRepository(self.gphoto_clients)
         shared_album_repository.setup()
         logger.debug("Step 3: Found existing shared albums")
 
-        assigned_albums = self.get_album_assignment_for_chunked_diffs(
+        assigned_albums = self.__get_album_assignment_for_chunked_diffs(
             shared_album_repository, chunked_new_diffs
         )
         logger.debug("Step 4: Assigned albums to diffs")
+        for album_title in chunked_new_diffs:
+            client_idx = assigned_albums[album_title]["client_idx"]
+            client = self.gphoto_clients[client_idx]
+            logger.debug(f"{album_title} -> {client_idx}")
 
         # Handle each folder one by one
         for album_title in chunked_new_diffs:
             album = assigned_albums[album_title]["album"]
             client = self.gphoto_clients[assigned_albums[album_title]["client_idx"]]
 
             # Find the existing photos that are in that album
@@ -78,72 +83,54 @@
                 file_names=[a["file_name"] for a in added_diffs],
             )
             logger.debug(
                 f"Step 7: Uploaded {len(upload_tokens)} photos to {album_title}"
             )
 
             # Attach them to gphotos album in chunks of 50
-            self.add_uploaded_photos_safely(media_item_repository, upload_tokens)
+            self.__add_uploaded_photos_safely(media_item_repository, upload_tokens)
             logger.debug(f"Step 8: Added uploaded photos to {album_title}")
 
+            logger.debug("Step 9: Added hash to each image")
+
             # Rename the album if it's currently empty
             if media_item_repository.get_num_media_items() == 0:
                 new_album_name = f"To delete/{album['title']}"
                 new_album = shared_album_repository.rename_album(
                     album["id"], new_album_name
                 )
-                logger.debug(f"Step 9: Renamed empty album {album_title} to be deleted")
+                logger.debug(f"Step 10: Marked empty album {album_title} to be deleted")
 
                 self.gphoto_clients[new_album["client_idx"]].albums().unshare_album(
                     new_album["id"]
                 )
-                logger.debug(f"Step 10: Unshared empty album {album_title}")
+                logger.debug(f"Step 11: Unshared empty album {album_title}")
 
         # Get a list of all the new albums made and its urls
         new_shared_album_urls = [
             assigned_album["album"]["shareInfo"]["shareableUrl"]
             for assigned_album in assigned_albums.values()
             if assigned_album["is_new_album"]
         ]
         return new_shared_album_urls
 
-    def add_new_metadata(self, diffs):
-        new_diffs = []
-        for diff in diffs:
-            rel_path = diff["path"]
-            abs_path = os.path.abspath(rel_path)
-            album_title = os.path.dirname(rel_path)
-            if album_title[:2] == "./":
-                album_title = album_title[2:]
-
-            new_diffs.append(
-                {
-                    "modifier": diff["modifier"],
-                    "album_title": album_title,
-                    "file_name": os.path.basename(abs_path),
-                    "abs_path": abs_path,
-                    "file_size_in_bytes": os.stat(abs_path).st_size,
-                }
-            )
-        return new_diffs
-
-    def get_album_assignment_for_chunked_diffs(
+    def __get_album_assignment_for_chunked_diffs(
         self, shared_album_repository, chunked_new_diffs
     ):
         results = {}
-        space_remaining = [self.get_remaining_storage(c) for c in self.gphoto_clients]
+        space_remaining = [self.__get_remaining_storage(c) for c in self.gphoto_clients]
 
         logger.debug(f"Current space remaining: {space_remaining}")
 
         # Go through all of the albums that already exist
         for album_title in chunked_new_diffs:
             if not shared_album_repository.contains_album_title(album_title):
                 continue
 
-            space_needed = self.get_new_storage_needed(
+            space_needed = self.__get_new_storage_needed(
                 chunked_new_diffs[album_title].get("+", [])
             )
 
             album = shared_album_repository.get_album_from_title(album_title)
             client_idx = album["client_idx"]
 
             if space_remaining[client_idx] - space_needed <= 0:
@@ -162,18 +149,18 @@
 
         # Go through all the albums that do not exist yet
         for album_title in chunked_new_diffs:
             if shared_album_repository.contains_album_title(album_title):
                 continue
 
             add_diffs = chunked_new_diffs[album_title].get("+", [])
-            space_needed = self.get_new_storage_needed(add_diffs)
+            space_needed = self.__get_new_storage_needed(add_diffs)
 
             # Get the best client to allocate to
-            best_client_idx = self.find_best_client_for_new_album(
+            best_client_idx = self.__find_best_client_for_new_album(
                 space_remaining, space_needed
             )
 
             if best_client_idx is None:
                 raise Exception(f"Can't find space to create new album {album_title}")
 
             client_idx = best_client_idx
@@ -196,24 +183,24 @@
                 results[album_title]["client_idx"], album_title
             )
 
         logger.debug("Created new albums")
 
         return results
 
-    def get_new_storage_needed(self, diffs):
+    def __get_new_storage_needed(self, diffs: DiffsWithMetadata):
         return sum([diff["file_size_in_bytes"] for diff in diffs])
 
-    def get_remaining_storage(self, gphoto_client):
+    def __get_remaining_storage(self, gphoto_client):
         storage_quota = gphoto_client.get_storage_quota()
         max_limit = int(storage_quota["limit"])
         usage = int(storage_quota["usage"])
         return max_limit - usage
 
-    def find_best_client_for_new_album(self, space_remaining, space_needed):
+    def __find_best_client_for_new_album(self, space_remaining, space_needed):
         max_remaining_space = float("-inf")
         best_client_idx = None
 
         for client_idx in range(len(self.gphoto_clients)):
             remaining_space = space_remaining[client_idx]
 
             if space_needed > remaining_space:
@@ -224,15 +211,15 @@
 
             if max_remaining_space < remaining_space:
                 max_remaining_space = remaining_space
                 best_client_idx = client_idx
 
         return best_client_idx
 
-    def add_uploaded_photos_safely(self, media_item_repository, upload_tokens):
+    def __add_uploaded_photos_safely(self, media_item_repository, upload_tokens):
         MAX_UPLOAD_TOKEN_LENGTH_PER_CALL = 50
 
         for i in range(0, len(upload_tokens), MAX_UPLOAD_TOKEN_LENGTH_PER_CALL):
             chunked_upload_tokens = upload_tokens[
                 i : i + MAX_UPLOAD_TOKEN_LENGTH_PER_CALL
             ]
             media_item_repository.add_uploaded_photos(chunked_upload_tokens)
```

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/backup/gphotos_uploader.py` & `sharded_google_photos-0.2.3/sharded_google_photos/backup/gphotos_uploader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from sharded_google_photos.shared.gphotos_client import GPhotosClient
 
 
 class GPhotosUploader:
     def __init__(self, gphoto_client: GPhotosClient):
         self.gphoto_client = gphoto_client
 
-    def upload_photos(self, file_paths, file_names):
+    def upload_photos(self, file_paths: list[str], file_names: list[str]):
         upload_tokens = []
 
         for file_path, file_name in zip(file_paths, file_names):
             upload_token = self.gphoto_client.media_items().upload_photo_in_chunks(
                 file_path, file_name
             )
             upload_tokens.append(upload_token)
```

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/backup/media_item_repository.py` & `sharded_google_photos-0.2.3/sharded_google_photos/backup/media_item_repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,78 +3,78 @@
 from sharded_google_photos.shared.gphotos_client import GPhotosClient
 
 logger = logging.getLogger(__name__)
 
 
 class MediaItemRepository:
     def __init__(self, album_id: str, gphoto_client: GPhotosClient):
-        self.album_id = album_id
-        self.gphoto_client = gphoto_client
+        self.__album_id = album_id
+        self.__gphoto_client = gphoto_client
 
-        self.media_id_to_obj = {}
-        self.file_name_to_media_ids = {}
+        self.__media_id_to_obj = {}
+        self.__file_name_to_media_ids = {}
 
     def setup(self):
-        self.media_id_to_obj = {}
-        self.file_name_to_media_ids = {}
+        self.__media_id_to_obj = {}
+        self.__file_name_to_media_ids = {}
 
-        media_items = self.gphoto_client.media_items().search_for_media_items(
-            album_id=self.album_id
+        media_items = self.__gphoto_client.media_items().search_for_media_items(
+            album_id=self.__album_id
         )
 
         for media_item in media_items:
             file_name = media_item["filename"]
             media_id = media_item["id"]
 
-            self.file_name_to_media_ids[file_name] = media_item["id"]
-            self.media_id_to_obj[media_id] = media_item
+            self.__file_name_to_media_ids[file_name] = media_item["id"]
+            self.__media_id_to_obj[media_id] = media_item
 
     def contains_file_name(self, file_name):
-        return file_name in self.file_name_to_media_ids
+        return file_name in self.__file_name_to_media_ids
 
     def get_media_item_from_file_name(self, file_name):
-        if file_name not in self.file_name_to_media_ids:
+        if file_name not in self.__file_name_to_media_ids:
             raise Exception(f"Media item {file_name} not found")
 
-        media_id = self.file_name_to_media_ids[file_name]
-        return self.media_id_to_obj[media_id]
+        media_id = self.__file_name_to_media_ids[file_name]
+        return self.__media_id_to_obj[media_id]
 
     def get_num_media_items(self):
-        return len(self.media_id_to_obj)
+        return len(self.__media_id_to_obj)
 
     def remove_media_items(self, media_ids):
         MAX_REMOVE_ITEMS_LENGTH_PER_CALL = 50
 
         if len(media_ids) == 0:
             return
 
         for media_id in media_ids:
-            if media_id not in self.media_id_to_obj:
+            if media_id not in self.__media_id_to_obj:
                 raise Exception("Media item is not found")
 
-            media_item = self.media_id_to_obj[media_id]
-            del self.media_id_to_obj[media_id]
-            del self.file_name_to_media_ids[media_item["filename"]]
+            media_item = self.__media_id_to_obj[media_id]
+            del self.__media_id_to_obj[media_id]
+            del self.__file_name_to_media_ids[media_item["filename"]]
 
         for i in range(0, len(media_ids), MAX_REMOVE_ITEMS_LENGTH_PER_CALL):
             chunked_media_ids = media_ids[i : i + MAX_REMOVE_ITEMS_LENGTH_PER_CALL]
-            self.gphoto_client.albums().remove_photos_from_album(
-                self.album_id, chunked_media_ids
+            self.__gphoto_client.albums().remove_photos_from_album(
+                self.__album_id, chunked_media_ids
             )
 
-        logger.debug(f"Media items removed from album {self.album_id}: {media_ids}")
+        logger.debug(f"Media items removed from album {self.__album_id}: {media_ids}")
 
     def add_uploaded_photos(self, upload_tokens):
         if len(upload_tokens) == 0:
             logger.debug("No uploaded tokens to add")
             return
 
-        results = self.gphoto_client.media_items().add_uploaded_photos_to_gphotos(
-            upload_tokens, self.album_id
+        results = self.__gphoto_client.media_items().add_uploaded_photos_to_gphotos(
+            upload_tokens, self.__album_id
         )
         media_items = [obj["mediaItem"] for obj in results["newMediaItemResults"]]
 
         for media_item in media_items:
-            self.media_id_to_obj[media_item["id"]] = media_item
-            self.file_name_to_media_ids[media_item["filename"]] = media_item["id"]
+            self.__media_id_to_obj[media_item["id"]] = media_item
+            self.__file_name_to_media_ids[media_item["filename"]] = media_item["id"]
 
         logger.debug(f"Added new media items: {media_items}")
```

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/backup/shared_album_repository.py` & `sharded_google_photos-0.2.3/sharded_google_photos/backup/shared_album_repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,79 +3,81 @@
 from sharded_google_photos.shared.gphotos_client import GPhotosClient
 
 logger = logging.getLogger(__name__)
 
 
 class SharedAlbumRepository:
     def __init__(self, gphoto_clients: list[GPhotosClient]):
-        self.gphoto_clients = gphoto_clients
+        self.__gphoto_clients = gphoto_clients
 
-        self.album_id_to_album = {}
-        self.album_title_to_album_id = {}
+        self.__album_id_to_album = {}
+        self.__album_title_to_album_id = {}
 
     def setup(self):
-        self.album_id_to_album = {}
-        self.album_title_to_album_id = {}
+        self.__album_id_to_album = {}
+        self.__album_title_to_album_id = {}
 
-        for client_idx in range(len(self.gphoto_clients)):
+        for client_idx in range(len(self.__gphoto_clients)):
             client_albums = (
-                self.gphoto_clients[client_idx].albums().list_shared_albums()
+                self.__gphoto_clients[client_idx].albums().list_shared_albums()
             )
 
             for client_album_idx in range(len(client_albums)):
                 album = client_albums[client_album_idx]
                 album["client_idx"] = client_idx
 
                 album_title = album["title"]
                 album_id = album["id"]
 
-                self.album_id_to_album[album_id] = album
-                self.album_title_to_album_id[album_title] = album_id
+                self.__album_id_to_album[album_id] = album
+                self.__album_title_to_album_id[album_title] = album_id
 
     def contains_album_title(self, title):
-        return title in self.album_title_to_album_id
+        return title in self.__album_title_to_album_id
 
     def get_album_from_title(self, title):
-        if title not in self.album_title_to_album_id:
+        if title not in self.__album_title_to_album_id:
             raise Exception(f"Album {title} does not exist")
 
-        album_id = self.album_title_to_album_id[title]
-        return self.album_id_to_album[album_id]
+        album_id = self.__album_title_to_album_id[title]
+        return self.__album_id_to_album[album_id]
 
     def create_shared_album(self, client_idx, title):
-        if title in self.album_title_to_album_id:
+        if title in self.__album_title_to_album_id:
             raise Exception(f"Album {title} already exists")
 
-        new_album = self.gphoto_clients[client_idx].albums().create_album(title)
+        new_album = self.__gphoto_clients[client_idx].albums().create_album(title)
         new_album["client_idx"] = client_idx
 
         new_album_id = new_album["id"]
-        share_info = self.gphoto_clients[client_idx].albums().share_album(new_album_id)
+        share_info = (
+            self.__gphoto_clients[client_idx].albums().share_album(new_album_id)
+        )
         new_album["shareInfo"] = share_info["shareInfo"]
 
-        self.album_id_to_album[new_album_id] = new_album
-        self.album_title_to_album_id[title] = new_album_id
+        self.__album_id_to_album[new_album_id] = new_album
+        self.__album_title_to_album_id[title] = new_album_id
         return new_album
 
     def rename_album(self, album_id, new_title):
-        if album_id not in self.album_id_to_album:
+        if album_id not in self.__album_id_to_album:
             raise Exception(f"Album {album_id} does not exist")
 
-        if new_title in self.album_title_to_album_id:
+        if new_title in self.__album_title_to_album_id:
             raise Exception(f"Album with name {new_title} already exists")
 
-        old_album = self.album_id_to_album[album_id]
+        old_album = self.__album_id_to_album[album_id]
         old_title = old_album["title"]
         client_idx = old_album["client_idx"]
 
         new_album = (
-            self.gphoto_clients[client_idx].albums().update_album(album_id, new_title)
+            self.__gphoto_clients[client_idx].albums().update_album(album_id, new_title)
         )
         new_album["client_idx"] = client_idx
 
-        del self.album_id_to_album[album_id]
-        del self.album_title_to_album_id[old_title]
+        del self.__album_id_to_album[album_id]
+        del self.__album_title_to_album_id[old_title]
 
-        self.album_id_to_album[new_album["id"]] = new_album
-        self.album_title_to_album_id[new_album["title"]] = new_album["id"]
+        self.__album_id_to_album[new_album["id"]] = new_album
+        self.__album_title_to_album_id[new_album["title"]] = new_album["id"]
 
         return new_album
```

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/cleanup/gphotos_cleaner.py` & `sharded_google_photos-0.2.3/sharded_google_photos/cleanup/gphotos_cleaner.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,53 +3,55 @@
 from sharded_google_photos.shared.gphotos_client import GPhotosClient
 
 logger = logging.getLogger(__name__)
 
 
 class GPhotosCleaner:
     def __init__(self, gphoto_client: GPhotosClient):
-        self.gphoto_client = gphoto_client
+        self._gphoto_client = gphoto_client
 
     def mark_unalbumed_photos_to_trash(self):
-        # Find the trash account
-        logger.debug(
-            "Step 1: Find the trash albums in all accounts, and if not, create one"
-        )
+        """Finds all of the photos that are not in an album, and puts it in a
+        dedicated "Trash" album to be deleted by the user manually.
+        """
+
+        # Find the trash album
+        logger.debug("Step 1: Find the trash album, and if not, create one")
         trash_album = None
-        for album in self.gphoto_client.albums().list_albums():
+        for album in self._gphoto_client.albums().list_albums():
             if album["title"] == "Trash":
                 trash_album = album
 
         if trash_album is None:
             logger.debug("No trash album found. Creating new trash album")
-            trash_album = self.gphoto_client.albums().create_album("Trash")
+            trash_album = self._gphoto_client.albums().create_album("Trash")
 
         logger.debug(f"Trash album: {trash_album}")
 
         # Find all of the media item ids in all shared albums
         logger.debug("Step 2: Find all media item ids in shared albums")
         media_item_ids_in_albums = set()
-        for shared_album in self.gphoto_client.albums().list_shared_albums():
+        for shared_album in self._gphoto_client.albums().list_shared_albums():
             shared_album_id = shared_album["id"]
-            for media_items in self.gphoto_client.media_items().search_for_media_items(
+            for media_items in self._gphoto_client.media_items().search_for_media_items(
                 shared_album_id
             ):
                 media_item_ids_in_albums.add(media_items["id"])
 
         logger.debug(f"Media item ids in albums: {media_item_ids_in_albums}")
 
         # Go through all of the media items, and if they are not in albums, move it to trash
         logger.debug(
             "Step 3: Find all media item ids not in a shared album, and trash them"
         )
         media_item_ids_to_trash = []
-        for media_item in self.gphoto_client.media_items().search_for_media_items():
+        for media_item in self._gphoto_client.media_items().search_for_media_items():
             media_item_id = media_item["id"]
             if media_item_id not in media_item_ids_in_albums:
                 media_item_ids_to_trash.append(media_item_id)
 
         if len(media_item_ids_to_trash) > 0:
-            self.gphoto_client.albums().add_photos_to_album(
+            self._gphoto_client.albums().add_photos_to_album(
                 trash_album["id"], media_item_ids_to_trash
             )
 
         logger.debug(f"Media item ids moved to trash: {media_item_ids_to_trash}")
```

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/shared/gphotos_album_client.py` & `sharded_google_photos-0.2.3/sharded_google_photos/shared/gphotos_album_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 import json
 import logging
 import backoff
 from requests.exceptions import RequestException
 
 from google.auth.transport.requests import AuthorizedSession
-from google.auth.transport import DEFAULT_RETRYABLE_STATUS_CODES
 
 logger = logging.getLogger(__name__)
 
 
-def fatal_code(e):
-    return e.response.status_code not in DEFAULT_RETRYABLE_STATUS_CODES
-
-
 class GPhotosAlbumClient:
     def __init__(self, session: AuthorizedSession):
         self._session = session
 
     def list_shared_albums(self, exclude_non_app_created_data: bool = False):
         logger.debug("Listing albums")
 
@@ -35,15 +30,15 @@
             if "nextPageToken" in res_body:
                 cur_page_token = res_body["nextPageToken"]
             else:
                 break
 
         return albums
 
-    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def _list_shared_albums_in_pages(
         self, page_token: str | None, exclude_non_app_created_data: bool
     ):
         uri = "https://photoslibrary.googleapis.com/v1/sharedAlbums"
         params = {
             "pageToken": page_token,
             "excludeNonAppCreatedData": exclude_non_app_created_data,
@@ -71,39 +66,40 @@
             if "nextPageToken" in res_json:
                 cur_page_token = res_json["nextPageToken"]
             else:
                 break
 
         return albums
 
-    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def _list_albums_in_pages(
         self, page_token: str | None, exclude_non_app_created_data: bool
     ):
         uri = "https://photoslibrary.googleapis.com/v1/albums"
         params = {
             "pageToken": page_token,
             "excludeNonAppCreatedData": exclude_non_app_created_data,
         }
         res = self._session.get(uri, params=params)
         res.raise_for_status()
+
         return res.json()
 
-    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def create_album(self, album_name: str):
         logger.debug(f"Creating album {album_name}")
 
         request_body = json.dumps({"album": {"title": album_name}})
         uri = "https://photoslibrary.googleapis.com/v1/albums"
         res = self._session.post(uri, request_body)
         res.raise_for_status()
 
         return res.json()
 
-    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def update_album(
         self, album_id: str, new_title: str = None, new_cover_media_item_id: str = None
     ):
         uri = f"https://photoslibrary.googleapis.com/v1/albums/{album_id}"
 
         if new_title is not None and new_cover_media_item_id is not None:
             uri += "?updateMask=title&updateMask=coverPhotoMediaItemId"
@@ -114,23 +110,22 @@
 
         request = {"title": new_title, "coverPhotoMediaItemId": new_cover_media_item_id}
         res = self._session.patch(uri, json.dumps(request))
         res.raise_for_status()
 
         return res.json()
 
-    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def share_album(
         self,
         album_id: str,
         is_collaborative: bool = False,
         is_commentable: bool = False,
     ):
         logger.debug(f"Sharing album {album_id}")
-
         request_body = json.dumps(
             {
                 "sharedAlbumOptions": {
                     "isCollaborative": is_collaborative,
                     "isCommentable": is_commentable,
                 }
             }
@@ -139,47 +134,47 @@
             album_id
         )
         res = self._session.post(uri, request_body)
         res.raise_for_status()
 
         return res.json()
 
-    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def join_album(self, share_token: str):
         logger.debug(f"Joining shared album {share_token}")
 
         request_body = json.dumps({"shareToken": share_token})
         uri = "https://photoslibrary.googleapis.com/v1/sharedAlbums:join"
         res = self._session.post(uri, request_body)
         res.raise_for_status()
 
         return res.json()
 
-    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def unshare_album(self, album_id: str):
         logger.debug(f"Unsharing shared album {album_id}")
 
         uri = "https://photoslibrary.googleapis.com/v1/albums/{0}:unshare".format(
             album_id
         )
         res = self._session.post(uri)
         res.raise_for_status()
 
-    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def add_photos_to_album(self, album_id: str, media_item_ids: list[str]):
         logger.debug(f"Add photos to album {album_id} {media_item_ids}")
 
         request_body = json.dumps({"mediaItemIds": media_item_ids})
         uri = "https://photoslibrary.googleapis.com/v1/albums/{0}:batchAddMediaItems".format(
             album_id
         )
         res = self._session.post(uri, request_body)
         res.raise_for_status()
 
-    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def remove_photos_from_album(self, album_id: str, media_item_ids: list[str]):
         logger.debug(f"Removing photos from album {album_id} {media_item_ids}")
 
         request_body = json.dumps({"mediaItemIds": media_item_ids})
         uri = "https://photoslibrary.googleapis.com/v1/albums/{0}:batchRemoveMediaItems".format(
             album_id
         )
```

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/shared/gphotos_client.py` & `sharded_google_photos-0.2.3/sharded_google_photos/shared/gphotos_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
 import logging
+import backoff
+from requests.exceptions import RequestException
 
 from google.oauth2.credentials import Credentials
 from google.auth.transport.requests import AuthorizedSession
 from google_auth_oauthlib.flow import InstalledAppFlow
 
 from sharded_google_photos.shared.gphotos_album_client import GPhotosAlbumClient
 from sharded_google_photos.shared.gphotos_mediaitem_client import GPhotosMediaItemClient
@@ -97,24 +99,21 @@
             authorization_prompt_message=f"For {self.name}, please visit this URL: {{url}}",
             success_message="The auth flow is complete; you may close this window.",
             open_browser=False,
         )
 
         return iaflow.credentials
 
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def get_storage_quota(self):
         params = {"fields": "storageQuota"}
         uri = "https://www.googleapis.com/drive/v3/about"
-        response = self.session.get(uri, params=params)
+        res = self.session.get(uri, params=params)
+        res.raise_for_status()
 
-        if response.status_code != 200:
-            raise Exception(
-                f"Failed to get storage quota: {response.status_code} {response.content}"
-            )
-
-        return response.json()["storageQuota"]
+        return res.json()["storageQuota"]
 
     def albums(self):
         return self._albums_client
 
     def media_items(self):
         return self._media_items_client
```

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/shared/gphotos_mediaitem_client.py` & `sharded_google_photos-0.2.3/sharded_google_photos/shared/gphotos_mediaitem_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 import os
 import backoff
 import magic
-from requests.exceptions import RequestException, HTTPError
+from requests.exceptions import HTTPError, RequestException
 
 from google.auth.transport.requests import AuthorizedSession
 from google.auth.transport import DEFAULT_RETRYABLE_STATUS_CODES
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_RETRYABLE_ERROR_CODES_FOR_UPLOADED_PHOTOS = set(
@@ -49,15 +49,15 @@
         super().__init__(message)
 
 
 class GPhotosMediaItemClient:
     def __init__(self, session: AuthorizedSession):
         self._session = session
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def add_uploaded_photos_to_gphotos(
         self, upload_tokens: list[str], album_id: str = None
     ):
         logger.debug(f"Add uploaded photos {upload_tokens} to album {album_id}")
 
         create_body = json.dumps(
             {
@@ -120,15 +120,15 @@
             if "nextPageToken" in res_body:
                 page_token = res_body["nextPageToken"]
             else:
                 break
 
         return media_items
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def _search_media_items_in_pages(
         self,
         album_id: str | None,
         filters: object | None,
         order_by: object | None,
         page_token: str | None,
     ):
@@ -142,15 +142,15 @@
                     "pageToken": page_token,
                 }
             ),
         )
         res.raise_for_status()
         return res
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def upload_photo(self, photo_file_path: str, file_name: str):
         logger.debug(f"Uploading photo {photo_file_path}")
 
         photo_file = open(photo_file_path, mode="rb")
         photo_bytes = photo_file.read()
 
         self._session.headers["Content-type"] = "application/octet-stream"
@@ -160,32 +160,37 @@
         res = self._session.post(
             "https://photoslibrary.googleapis.com/v1/uploads", photo_bytes
         )
         res.raise_for_status()
 
         return res.content.decode()
 
-    @backoff.on_exception(backoff.expo, (IllegalStateException))
-    def upload_photo_in_chunks(self, photo_file_path: str, file_name: str):
+    @backoff.on_exception(backoff.expo, (IllegalStateException), max_time=60)
+    def upload_photo_in_chunks(
+        self,
+        photo_file_path: str,
+        file_name: str,
+    ):
         upload_token = None
         mime_type = self._get_mime_type(photo_file_path)
         file_size_in_bytes = os.stat(photo_file_path).st_size
 
         logger.debug(
-            f"Uploading in chunks with mime_type {mime_type} and file size {file_size_in_bytes}"
+            f"Uploading {photo_file_path} in chunks ({mime_type}, {file_size_in_bytes} bytes)"
         )
 
         res_1 = self._initialize_chunked_upload(
             mime_type, file_name, file_size_in_bytes
         )
         upload_url = res_1.headers["X-Goog-Upload-URL"]
         chunk_size = int(res_1.headers["X-Goog-Upload-Chunk-Granularity"])
 
         logger.debug(f"Obtained upload url and chunk size: {upload_url} {chunk_size}")
 
+        num_bytes_uploaded = 0
         with open(photo_file_path, "rb") as file_obj:
             cur_offset = 0
             chunk = file_obj.read(chunk_size)
             while chunk:
                 chunk_read = len(chunk)
                 next_chunk = file_obj.read(chunk_size)
 
@@ -214,24 +219,26 @@
 
                     logger.debug(f"Adjusted seek to {size_received}")
                     file_obj.seek(size_received, 0)
                     cur_offset = size_received
                     next_chunk = file_obj.read(chunk_size)
                 else:
                     cur_offset += chunk_read
+                    num_bytes_uploaded += chunk_read
 
                 if is_last_chunk:
                     upload_token = res_2.content.decode()
 
                 chunk = next_chunk
 
         logger.debug(f"Chunk uploading finished: {photo_file_path}")
+
         return upload_token
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def _initialize_chunked_upload(
         self, mime_type: str, file_name: str, file_size_in_bytes: int
     ):
         self._session.headers["Content-Length"] = "0"
         self._session.headers["X-Goog-Upload-Command"] = "start"
         self._session.headers["X-Goog-Upload-Content-Type"] = mime_type
         self._session.headers["X-Goog-Upload-Protocol"] = "resumable"
@@ -239,29 +246,29 @@
         self._session.headers["X-Goog-Upload-Raw-Size"] = str(file_size_in_bytes)
 
         res = self._session.post("https://photoslibrary.googleapis.com/v1/uploads")
         res.raise_for_status()
 
         return res
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def _upload_photo_chunk(
         self, upload_url: str, cur_offset: int, chunk: bytes, is_last_chunk: bool
     ):
         upload_cmd = "upload, finalize" if is_last_chunk else "upload"
         self._session.headers["X-Goog-Upload-Command"] = upload_cmd
         self._session.headers["X-Goog-Upload-Offset"] = str(cur_offset)
 
         res = self._session.post(upload_url, chunk)
         if res.status_code in DEFAULT_RETRYABLE_STATUS_CODES:
             res.raise_for_status()
 
         return res
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), max_time=60)
     def _query_chunked_upload(self, upload_url):
         self._session.headers["Content-Length"] = "0"
         self._session.headers["X-Goog-Upload-Command"] = "query"
 
         res = self._session.post(upload_url)
         res.raise_for_status()
```

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_album_client.py` & `sharded_google_photos-0.2.3/sharded_google_photos/shared/testing/fake_gphotos_album_client.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_client.py` & `sharded_google_photos-0.2.3/sharded_google_photos/shared/testing/fake_gphotos_client.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_mediaitem_client.py` & `sharded_google_photos-0.2.3/sharded_google_photos/shared/testing/fake_gphotos_mediaitem_client.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_repository.py` & `sharded_google_photos-0.2.3/sharded_google_photos/shared/testing/fake_gphotos_repository.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/mocked_saved_credentials_file.py` & `sharded_google_photos-0.2.3/sharded_google_photos/shared/testing/mocked_saved_credentials_file.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.2/PKG-INFO` & `sharded_google_photos-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 Metadata-Version: 2.1
 Name: sharded-google-photos
-Version: 0.2.2
+Version: 0.2.3
 Summary: A tool to shard photos across multiple Google Photo accounts
 License: GNU General Public License v3.0
 Author: Emilio K
 Author-email: e.kartonoe@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: google-api-python-client (>=2.122.0,<3.0.0)
 Requires-Dist: google-auth-oauthlib (>=1.2.0,<2.0.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Sharded-Google-Photos
 
 ## Description
 
-Running out of space in your Google Photos account? Wish you can upload an unlimited number of photos on Google Photos? Now you can! With this Python library, you can upload your photos to multiple Google Photo Accounts and then share those albums to your main Google Photos account. That way, you get to see all of your photos on one main Google Photos account.
+Running out of space in your Google Photos account? Wish you can upload your photos to multiple Google Accounts? Now you can! With this Python library, you can upload your photos to multiple Google Photo Accounts and then share those albums to your main Google Photos account. That way, you get to see all of your photos on one main Google Photos account.
+
+## Getting Started
 
 It works like this:
 
-1. Let's say you have three Google Accounts. Create an OAuth2 to interact with Google Photos and Google Drive.
+1. Let's say you have three Google Accounts. Follow [this doc](docs/create_client_id.md) to create your own OAuth2 Google Client ID to interact with Google Photos and Google Drive.
 
 2. Install `libmagic`
 
 3. Install the package by running `pip install sharded-google-photos`.
 
 4. Import the following code in your `main.py` app:
 
     ```python
     from sharded_google_photos.backup.gphotos_backup import GPhotosBackup
     from sharded_google_photos.shared.gphotos_client import GPhotosClient
 
     clients = [
-        GPhotosClient(creds_file = "credentials-1.json", client_secret="client_secret.json"),
-        GPhotosClient(creds_file = "credentials-2.json", client_secret="client_secret.json"),
-        GPhotosClient(creds_file = "credentials-3.json", client_secret="client_secret.json"),
+        GPhotosClient(name="bob@gmail.com", creds_file = "credentials-1.json", client_secret="client_secret.json"),
+        GPhotosClient(name="alice@gmail.com", creds_file = "credentials-2.json", client_secret="client_secret.json"),
+        GPhotosClient(name="jerry@gmail.com", creds_file = "credentials-3.json", client_secret="client_secret.json"),
     ]
     for client in clients:
         client.authenticate()
 
     backup_client = GPhotosBackup(clients)
     ```
 
+    Run this script and follow the instructions from the cli.
+
 5. To upload four photos from two folders, run the following:
 
     ```python
     new_album_uris = backup_client.backup(
         [
             { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg" },
             { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/2.jpg" },
@@ -122,15 +127,15 @@
     ```bash
     poetry run python sharded_google_photos/main.py
     ```
 
 4. To lint your code, run:
 
     ```bash
-    poetry run flake8 && poetry run black sharded_google_photos/
+    poetry run flake8 && poetry run black .
     ```
 
 5. To run tests and code coverage, run:
 
     ```bash
     poetry run coverage run -m pytest && poetry run coverage report -m
     ```
```

