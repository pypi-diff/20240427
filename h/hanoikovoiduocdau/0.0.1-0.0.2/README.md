# Comparing `tmp/hanoikovoiduocdau-0.0.1.tar.gz` & `tmp/hanoikovoiduocdau-0.0.2.tar.gz`

## Comparing `hanoikovoiduocdau-0.0.1.tar` & `hanoikovoiduocdau-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.1/src/hanoikovoidcdau/__init__.py
--rw-r--r--   0        0        0    87348 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.1/src/hanoikovoidcdau/data.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.1/src/hanoikovoidcdau/standardize.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.1/tests/main.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.1/LICENSE
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.1/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/src/hanoikovoidcdau/__init__.py
+-rw-r--r--   0        0        0    87256 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/src/hanoikovoidcdau/data.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/src/hanoikovoidcdau/standardize.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/tests/main.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/LICENSE
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/PKG-INFO
```

### Comparing `hanoikovoiduocdau-0.0.1/src/hanoikovoidcdau/data.py` & `hanoikovoiduocdau-0.0.2/src/hanoikovoidcdau/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -235,15 +235,15 @@
                 "Đường Yên Nghĩa",
                 "Đường Yên Phúc",
                 "Đường Yết Kiêu"
             ]
         },
         {
             "date": "2024-04-27 00:07:43",
-            "district": "Hoàng Mai",
+            "name": "Hoàng Mai",
             "wards": [
                 "Đại Kim",
                 "Định Công",
                 "Giải Phóng",
                 "Giáp Bát",
                 "Hoàng Liệt",
                 "Hoàng Văn Thụ",
@@ -345,15 +345,15 @@
                 "Đường Vũ Tông Phan",
                 "Đường Xóm 5",
                 "Yên Duyên",
                 "Đường Yên Sở"
             ]
         },
         {
-            "district": "Cầu Giấy",
+            "name": "Cầu Giấy",
             "wards": [
                 "Cầu Giấy",
                 "Dịch Vọng",
                 "Dịch Vọng Hậu",
                 "Mai Dịch",
                 "Mễ Trì",
                 "Mỹ Đình",
@@ -478,15 +478,15 @@
                 "Đường Xuân Thủy",
                 "Đường Xuân Thủy, Phường Dịch Vọng Hậu",
                 "Đường Yên Hòa"
             ]
         },
         {
             "date": "2024-04-27 00:07:44",
-            "district": "Long Biên",
+            "name": "Long Biên",
             "wards": [
                 "Bồ Đề",
                 "Cự Khối",
                 "Đức Giang",
                 "Gia Huy",
                 "Gia Lâm",
                 "Gia Thuỵ",
@@ -626,15 +626,15 @@
                 "Đường Việt Hưng",
                 "Đường Vũ Xuân Thiều",
                 "Phố Xuân Đỗ"
             ]
         },
         {
             "date": "2024-04-27 00:07:44",
-            "district": "Thường Tín",
+            "name": "Thường Tín",
             "wards": [
                 "Dũng Tiến",
                 "Duyên Thái",
                 "Hà Hồi",
                 "Hiền Giang",
                 "Hòa Bình",
                 "Liên Phương",
@@ -671,15 +671,15 @@
                 "Đường Tỉnh lộ 71",
                 "Đường Tỉnh lộ 73",
                 "Đường Trần Phú"
             ]
         },
         {
             "date": "2024-04-27 00:07:45",
-            "district": "Bắc Từ Liêm",
+            "name": "Bắc Từ Liêm",
             "wards": [
                 "Cổ Nhuế",
                 "Đông Ngạc",
                 "Đức Thắng",
                 "Liên Mạc",
                 "Minh Khai",
                 "Phú Diễn",
@@ -737,15 +737,15 @@
                 "Đường Văn Trì",
                 "Đường Xuân Đỉnh",
                 "Đường Yên Nội"
             ]
         },
         {
             "date": "2024-04-27 00:07:45",
-            "district": "Hai Bà Trưng",
+            "name": "Hai Bà Trưng",
             "wards": [
                 "Bạch Đằng",
                 "Bách Khoa",
                 "Bạch Mai",
                 "Bùi Thị Xuân",
                 "Cầu Dền",
                 "Cửa Nam",
@@ -907,15 +907,15 @@
                 "Phố Yên Bái 2",
                 "Phố Yên Lạc",
                 "Phố Yết Kiêu"
             ]
         },
         {
             "date": "2024-04-27 00:07:45",
-            "district": "Mỹ Đức",
+            "name": "Mỹ Đức",
             "wards": [],
             "streets": [
                 "Đường Cầu Ái Nàng",
                 "Đường Đại Nghĩa",
                 "Đường 74",
                 "Đường Bờ Sông",
                 "Đường Nghĩa Ái",
@@ -925,15 +925,15 @@
                 "Đường Tỉnh lộ 419",
                 "Đường Tỉnh lộ 424",
                 "Phố Văn Giang"
             ]
         },
         {
             "date": "2024-04-27 00:07:45",
-            "district": "Sơn Tây",
+            "name": "Sơn Tây",
             "wards": [
                 "Cổ Đông",
                 "Đường Lâm",
                 "Lê Lợi",
                 "Ngô Quyền",
                 "Phú Thịnh",
                 "Quang Trung",
@@ -987,15 +987,15 @@
                 "Đường Trưng Vương",
                 "Đường Tùng Thiện",
                 "Đường Vạn An"
             ]
         },
         {
             "date": "2024-04-27 00:07:46",
-            "district": "Đông Anh",
+            "name": "Đông Anh",
             "wards": [
                 "Cổ Dương -Tiên Dương",
                 "Thị Trấn Bần Yên Nhân",
                 "Thị trấn Đông Anh",
                 "Xã Bắc Hồng",
                 "Xã Cổ Loa",
                 "Xã Đại Mạch",
@@ -1077,15 +1077,15 @@
                 "Đường Võ Nguyên Giáp",
                 "Đường Xóm Đông",
                 "Đường Xuân Canh"
             ]
         },
         {
             "date": "2024-04-27 00:07:46",
-            "district": "Đan Phượng",
+            "name": "Đan Phượng",
             "wards": [
                 "Hạ Mỗ",
                 "Hồng Hà",
                 "Liên Hà",
                 "Liên Hồng",
                 "Tân Hội",
                 "Tân Lập",
@@ -1111,15 +1111,15 @@
                 "Đường Thượng Mỗ",
                 "Đường Tình Yêu",
                 "Đường Trung Thọ Dương"
             ]
         },
         {
             "date": "2024-04-27 00:07:46",
-            "district": "Thanh Oai",
+            "name": "Thanh Oai",
             "wards": [
                 "Bình Minh",
                 "Cao Viên",
                 "Cự Khê",
                 "Hồng Dương",
                 "Tam Hưng",
                 "Thanh Mai",
@@ -1128,15 +1128,15 @@
                 "Thị trấn Kim Bài",
                 "TT Kim Bài"
             ],
             "streets": []
         },
         {
             "date": "2024-04-27 00:07:46",
-            "district": "Đống Đa",
+            "name": "Đống Đa",
             "wards": [
                 "Bách Khoa",
                 "Cát Linh",
                 "Cửa Nam",
                 "Điện Biên",
                 "Đống Đa",
                 "Đồng Tâm",
@@ -1280,15 +1280,15 @@
                 "Xã Đàn 2",
                 "Phố Y Miếu",
                 "Đường Yên Lãng"
             ]
         },
         {
             "date": "2024-04-27 00:07:47",
-            "district": "Chương Mỹ",
+            "name": "Chương Mỹ",
             "wards": [],
             "streets": [
                 "Đường Cấn Hữu",
                 "Đường Chi Nê-Tinh Mỹ",
                 "Đường Đìa Chiến Lược",
                 "Đường Đồng Lệ",
                 "Đường Mới Yên Cốc",
@@ -1312,15 +1312,15 @@
                 "Đường Trung Hòa-Trường Yên",
                 "Đường Viết Tuấn",
                 "Đường Yên Sơn"
             ]
         },
         {
             "date": "2024-04-27 00:07:47",
-            "district": "Hoàn Kiếm",
+            "name": "Hoàn Kiếm",
             "wards": [
                 "Chương Dương",
                 "Chương Dương Độ",
                 "Cửa Đông",
                 "Cửa Nam",
                 "Đồng Xuân",
                 "Hai Bà Trưng",
@@ -1554,15 +1554,15 @@
                 "Đường Vọng Hà",
                 "Đường Yên Thái",
                 "Phố Yết Kiêu"
             ]
         },
         {
             "date": "2024-04-27 00:07:47",
-            "district": "Hoài Đức",
+            "name": "Hoài Đức",
             "wards": [
                 "Thị trấn Trạm Trôi",
                 "An Khánh",
                 "Đắc Sở",
                 "Di Trạch",
                 "Đông La",
                 "Đức Thượng",
@@ -1606,15 +1606,15 @@
                 "Đường Trãi",
                 "Đường Yên Sở",
                 "Đường Yên Sở-Sơn Đồng"
             ]
         },
         {
             "date": "2024-04-27 00:07:47",
-            "district": "Ba Đình",
+            "name": "Ba Đình",
             "wards": [
                 "An Dương",
                 "Ba Đình",
                 "Cách Bi",
                 "Cát Linh",
                 "Cống Vị",
                 "Cửa Đông",
@@ -1761,15 +1761,15 @@
                 "Phố Yên Ninh",
                 "Đường Yên Phụ",
                 "Phố Yên Thế"
             ]
         },
         {
             "date": "2024-04-27 00:07:48",
-            "district": "Thạch Thất",
+            "name": "Thạch Thất",
             "wards": [],
             "streets": [
                 "Phố Bãi Cháy",
                 "Đường Bãi Dài",
                 "Đường Bình Sơn",
                 "Đường Chàng Sơn",
                 "Phố Chợ Bò",
@@ -1804,15 +1804,15 @@
                 "Đường Xanh Villas Khu đô thị Xanh Villas",
                 "Đường Xóm Chùa",
                 "Đường Yên Bình"
             ]
         },
         {
             "date": "2024-04-27 00:07:48",
-            "district": "Nam Từ Liêm",
+            "name": "Nam Từ Liêm",
             "wards": [
                 "Cầu Diễn",
                 "Đại Mỗ",
                 "Mễ Trì",
                 "Mỹ Đình",
                 "Mỹ Đình 2",
                 "Phú Đô",
@@ -1907,15 +1907,15 @@
                 "Đường Vườn Cam",
                 "Xuân Phương",
                 "Đường Yên Hòa Đại Mỗ"
             ]
         },
         {
             "date": "2024-04-27 00:07:49",
-            "district": "Ba Vì",
+            "name": "Ba Vì",
             "wards": [
                 "Cam Thượng",
                 "Châu Sơn",
                 "Chu Minh",
                 "Đông Quang",
                 "Khai Quang",
                 "Minh Châu",
@@ -1935,15 +1935,15 @@
                 "Mê Linh",
                 "Đường Quốc lộ 32",
                 "Đường Vật Lại",
             ]
         },
         {
             "date": "2024-04-27 00:07:49",
-            "district": "Thanh Trì",
+            "name": "Thanh Trì",
             "wards": [
                 "Phường Hữu Hòa",
                 "Thanh Liệt",
                 "Thị trấn Văn Điển",
                 "Xã Đại Áng",
                 "Xã Đông Mỹ",
                 "Xã Duyên Hà",
@@ -1996,15 +1996,15 @@
                 "Đường Tựu Liệt",
                 "Đường Vĩnh Ninh",
                 "Đường Vĩnh Thịnh"
             ]
         },
         {
             "date": "2024-04-27 00:07:49",
-            "district": "Quốc Oai",
+            "name": "Quốc Oai",
             "wards": [
                 "Đồng Quang",
                 "Đông Yên",
                 "Hòa Thạch",
                 "Phú Cát",
                 "Quang Trung",
                 "Thạch Thán",
@@ -2017,15 +2017,15 @@
                 "Đường Quốc Oai",
                 "Đường Tỉnh lộ 419",
                 "Trại Vàng"
             ]
         },
         {
             "date": "2024-04-27 00:07:50",
-            "district": "Tây Hồ",
+            "name": "Tây Hồ",
             "wards": [
                 "Bưởi",
                 "Nhật Tân",
                 "Phú Thượng",
                 "Phúc Xá",
                 "Phường Trúc Bạch",
                 "Quảng An",
@@ -2086,15 +2086,15 @@
                 "Đường Xuân La",
                 "Yên Hoa",
                 "Đường Yên Phụ"
             ]
         },
         {
             "date": "2024-04-27 00:07:50",
-            "district": "Thanh Xuân",
+            "name": "Thanh Xuân",
             "wards": [
                 "Định Công",
                 "Đồng Tâm",
                 "Giáp Bát",
                 "Hạ Đình",
                 "Hà Đông",
                 "Hoàng Liệt",
```

### Comparing `hanoikovoiduocdau-0.0.1/src/hanoikovoidcdau/standardize.py` & `hanoikovoiduocdau-0.0.2/src/hanoikovoidcdau/standardize.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,48 +22,43 @@
             all_wards.append(ward)
     return all_wards
 
 
 def get_all_district(standard_data):
     all_districts = []
     for district in standard_data["district"]:
-        for d in district["name"]:
-            all_districts.append(d)
+        all_districts.append(district["name"])
+
+    print(all_districts)
     return all_districts
 
 
 def find_closest_match(input_street, standard_data):
     closest_match = difflib.get_close_matches(input_street, standard_data)
     if closest_match:
         return closest_match[0]
 
     return input_street
 
 
 def standardize_street_name(street: str) -> str:
-    street = street.strip()
-    street = street.replace(" ", "")
     street = remove_keywords(useless_street_keywords, street)
     all_streets = get_all_streets(data)
     ans = find_closest_match(street, all_streets)
     return ans
 
 
 def standardize_ward_name(ward: str) -> str:
-    ward = ward.strip()
-    ward = ward.replace(" ", "")
     ward = remove_keywords(useless_ward_keywords, ward)
     all_wards = get_all_wards(data)
     ans = find_closest_match(ward, all_wards)
     return ans
 
 
 def standardize_district_name(district: str) -> str:
-    district = district.strip()
-    district = district.replace(" ", "")
     all_districts = get_all_district(data)
     ans = find_closest_match(district, all_districts)
     return ans
 
 
 def remove_keywords(useless_keywords: list, street: str) -> str:
     for keyword in useless_keywords:
```

### Comparing `hanoikovoiduocdau-0.0.1/LICENSE` & `hanoikovoiduocdau-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hanoikovoiduocdau-0.0.1/pyproject.toml` & `hanoikovoiduocdau-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/hanoikovoidcdau"]
 
 [project]
 name = "hanoikovoiduocdau"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "betty2310", email = "huynhduongsh1@gmail.com" }]
 description = "A package for standardize Hanoi's address"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

