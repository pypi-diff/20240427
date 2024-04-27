# Comparing `tmp/bitcoin_safe-0.6.0a0.tar.gz` & `tmp/bitcoin_safe-0.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin_safe-0.6.0a0.tar", max compression
+gzip compressed data, was "bitcoin_safe-0.6.0a1.tar", max compression
```

## Comparing `bitcoin_safe-0.6.0a0.tar` & `bitcoin_safe-0.6.0a1.tar`

### file list

```diff
@@ -1,260 +1,260 @@
--rw-r--r--   0        0        0      644 2024-03-20 13:56:51.549261 bitcoin_safe-0.6.0a0/LICENSE
--rw-r--r--   0        0        0     4247 2024-04-26 05:59:33.675300 bitcoin_safe-0.6.0a0/README.md
--rw-r--r--   0        0        0       24 2024-04-24 13:50:36.396043 bitcoin_safe-0.6.0a0/bitcoin_safe/__init__.py
--rw-r--r--   0        0        0     1456 2024-04-24 16:26:26.615316 bitcoin_safe-0.6.0a0/bitcoin_safe/__main__.py
--rw-r--r--   0        0        0     6932 2024-04-26 06:09:53.626565 bitcoin_safe-0.6.0a0/bitcoin_safe/config.py
--rw-r--r--   0        0        0     2999 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a0/bitcoin_safe/descriptors.py
--rw-r--r--   0        0        0     1306 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a0/bitcoin_safe/device_export.py
--rw-r--r--   0        0        0     4976 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a0/bitcoin_safe/dynamic_lib_load.py
--rw-r--r--   0        0        0     1305 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a0/bitcoin_safe/execute_config.py
--rw-r--r--   0        0        0     2141 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a0/bitcoin_safe/fx.py
--rw-r--r--   0        0        0        0 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/__init__.py
--rw-r--r--   0        0        0    12417 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/explainer0.ui
--rw-r--r--   0        0        0    12419 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/explainer1.ui
--rw-r--r--   0        0        0   122131 2023-12-08 19:45:37.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/2of3backup.svg
--rw-r--r--   0        0        0      687 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/add.png
--rw-r--r--   0        0        0     1349 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/android_electrum_icon_background.png
--rw-r--r--   0        0        0     8928 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/bitcoin-testnet.png
--rw-r--r--   0        0        0     3075 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/bug.png
--rw-r--r--   0        0        0     1096 2023-12-14 15:09:14.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/camera.svg
--rw-r--r--   0        0        0      687 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/camera_dark.png
--rw-r--r--   0        0        0     1304 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/camera_white.png
--rw-r--r--   0        0        0    54212 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/checkmark.png
--rw-r--r--   0        0        0     1044 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/chevron-right.png
--rw-r--r--   0        0        0     1146 2024-02-05 10:38:12.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/clip.svg
--rw-r--r--   0        0        0     7607 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/clock1.png
--rw-r--r--   0        0        0     8512 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/clock2.png
--rw-r--r--   0        0        0     7229 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/clock3.png
--rw-r--r--   0        0        0     7522 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/clock4.png
--rw-r--r--   0        0        0    10074 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/clock5.png
--rw-r--r--   0        0        0     3521 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/closebutton.png
--rw-r--r--   0        0        0     3812 2024-02-03 12:39:12.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/cloud-sync.svg
--rw-r--r--   0        0        0    14573 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/cloud_no.png
--rw-r--r--   0        0        0     8329 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/cloud_yes.png
--rw-r--r--   0        0        0     8070 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard-dice.svg
--rw-r--r--   0        0        0    17195 2024-01-28 12:33:26.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard-generate24.png
--rw-r--r--   0        0        0     4229 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard-only.svg
--rw-r--r--   0        0        0    14288 2024-01-28 09:08:54.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard-register-multisig-decriptor.png
--rw-r--r--   0        0        0    14316 2024-02-28 10:15:29.171933 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard-view-seed.png
--rw-r--r--   0        0        0    14353 2024-01-28 09:08:09.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard-wallet-export.png
--rw-r--r--   0        0        0     5283 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard.png
--rw-r--r--   0        0        0     4274 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard.svg
--rw-r--r--   0        0        0     5242 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard_unpaired.png
--rw-r--r--   0        0        0     3566 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard_unpaired.svg
--rw-r--r--   0        0        0    54212 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/confirmed.png
--rw-r--r--   0        0        0     4153 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/confirmed.svg
--rw-r--r--   0        0        0     5113 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/confirmed_bw.png
--rw-r--r--   0        0        0     2111 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/copy.png
--rw-r--r--   0        0        0      880 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/copy_bw.png
--rw-r--r--   0        0        0      453 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/delete.png
--rw-r--r--   0        0        0    65286 2023-12-24 11:19:00.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/descriptor-backup.svg
--rw-r--r--   0        0        0    18399 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/descriptor.svg
--rw-r--r--   0        0        0    20662 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/descriptor3.svg
--rw-r--r--   0        0        0     1863 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/dice.svg
--rw-r--r--   0        0        0   249404 2024-02-26 10:25:07.531743 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/distribute-multisig.svg
--rw-r--r--   0        0        0   293552 2024-02-26 10:27:16.318444 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/distribute-multisigsig-export.svgz
--rw-r--r--   0        0        0    45895 2024-02-26 10:08:52.867612 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/distribute-singlesig-export.svgz
--rw-r--r--   0        0        0    83484 2024-02-26 10:07:04.773452 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/distribute-singlesig.svg
--rw-r--r--   0        0        0     2970 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/download.png
--rw-r--r--   0        0        0     2225 2024-02-26 10:06:33.612835 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/earth.svg
--rw-r--r--   0        0        0     2510 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/electrumb.png
--rw-r--r--   0        0        0    28522 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/expired.png
--rw-r--r--   0        0        0     2910 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/eye1.png
--rw-r--r--   0        0        0     4779 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/file.png
--rw-r--r--   0        0        0     5938 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/globe.png
--rw-r--r--   0        0        0      240 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/hamburger.png
--rw-r--r--   0        0        0     1276 2023-07-07 19:42:34.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/history.svg
--rw-r--r--   0        0        0     1771 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/info.png
--rw-r--r--   0        0        0    15433 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/kangaroo.png
--rw-r--r--   0        0        0     1230 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/keep-quiet-icon.svg
--rw-r--r--   0        0        0    15398 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/key-gray.png
--rw-r--r--   0        0        0      988 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/key-hole-icon.svg
--rw-r--r--   0        0        0     5428 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/key.png
--rw-r--r--   0        0        0    23125 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/link.png
--rw-r--r--   0        0        0     1674 2023-12-14 18:36:51.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/loader-icon.svg
--rw-r--r--   0        0        0    40380 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/lock.png
--rw-r--r--   0        0        0    12125 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/lock.svg
--rw-r--r--   0        0        0     4400 2023-07-06 09:39:13.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/logo.svg
--rw-r--r--   0        0        0     4548 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/mail_icon.png
--rw-r--r--   0        0        0      997 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/menu_vertical.png
--rw-r--r--   0        0        0     5565 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/menu_vertical_white.png
--rw-r--r--   0        0        0      199 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/microphone.png
--rw-r--r--   0        0        0     3031 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/network.png
--rw-r--r--   0        0        0     1117 2023-07-06 11:00:16.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/no-photography-icon.svg
--rw-r--r--   0        0        0    10364 2023-07-06 11:57:23.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/no-typing-icon.svg
--rw-r--r--   0        0        0      463 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/offline_tx.png
--rw-r--r--   0        0        0     1309 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/paste.png
--rw-r--r--   0        0        0     2173 2023-07-01 09:19:26.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/pdf-file.svg
--rw-r--r--   0        0        0     1641 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/pen.png
--rw-r--r--   0        0        0     1238 2023-12-14 15:42:01.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/pen.svg
--rw-r--r--   0        0        0     1519 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/picture_in_picture.png
--rw-r--r--   0        0        0    58005 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/preferences.png
--rw-r--r--   0        0        0    27175 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/preferences.svg
--rw-r--r--   0        0        0     3177 2023-12-14 18:20:48.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/print.svg
--rw-r--r--   0        0        0     1200 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/qr-code.svg
--rw-r--r--   0        0        0      314 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/qrcode.png
--rw-r--r--   0        0        0      380 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/qrcode_white.png
--rw-r--r--   0        0        0     2555 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/question.png
--rw-r--r--   0        0        0     1929 2023-07-07 20:04:30.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/receive.svg
--rw-r--r--   0        0        0     1426 2023-06-30 17:44:30.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/reset-update.svg
--rw-r--r--   0        0        0      272 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/revealer.png
--rw-r--r--   0        0        0     1965 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/revealer_c.png
--rw-r--r--   0        0        0     1860 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/right-arrow.svg
--rw-r--r--   0        0        0     3869 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/rocket.png
--rw-r--r--   0        0        0      946 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/save.png
--rw-r--r--   0        0        0     1261 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/sd-card.svg
--rw-r--r--   0        0        0    38276 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/seal.png
--rw-r--r--   0        0        0    17829 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/seed-plate-large.svg
--rw-r--r--   0        0        0    24206 2023-07-01 06:31:12.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/seed-plate.svg
--rw-r--r--   0        0        0    10322 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/seed.png
--rw-r--r--   0        0        0      820 2024-01-03 16:14:13.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/send.svg
--rw-r--r--   0        0        0     3325 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/share.png
--rw-r--r--   0        0        0      392 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/speaker.png
--rw-r--r--   0        0        0    71068 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_connected.png
--rw-r--r--   0        0        0     6593 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_connected.svg
--rw-r--r--   0        0        0    62949 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_connected_fork.png
--rw-r--r--   0        0        0    69081 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_connected_proxy.png
--rw-r--r--   0        0        0     6593 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_connected_proxy.svg
--rw-r--r--   0        0        0    60879 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_connected_proxy_fork.png
--rw-r--r--   0        0        0    66105 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_disconnected.png
--rw-r--r--   0        0        0    10522 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_disconnected.svg
--rw-r--r--   0        0        0    74851 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_lagging.png
--rw-r--r--   0        0        0     6595 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_lagging.svg
--rw-r--r--   0        0        0    63949 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_lagging_fork.png
--rw-r--r--   0        0        0    81206 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_waiting.png
--rw-r--r--   0        0        0    17633 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_waiting.svg
--rw-r--r--   0        0        0      886 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/tab_addresses.png
--rw-r--r--   0        0        0     1592 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/tab_coins.png
--rw-r--r--   0        0        0      824 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/tab_console.png
--rw-r--r--   0        0        0     1446 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/tab_contacts.png
--rw-r--r--   0        0        0     1873 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/tab_receive.png
--rw-r--r--   0        0        0     2712 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/tor_logo.png
--rw-r--r--   0        0        0     3532 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/unconfirmed.png
--rw-r--r--   0        0        0     5499 2024-01-03 16:09:47.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/unconfirmed.svg
--rw-r--r--   0        0        0     6118 2024-01-03 16:13:32.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/unconfirmed_child.svg
--rw-r--r--   0        0        0     1256 2023-06-30 17:26:47.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/undo-arrow.svg
--rw-r--r--   0        0        0    45956 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/unlock.png
--rw-r--r--   0        0        0    19461 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/unlock.svg
--rw-r--r--   0        0        0    23805 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/unpaid.png
--rw-r--r--   0        0        0     1580 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/update.png
--rwxr-xr-x   0        0        0     4485 2023-12-13 10:35:24.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/usb-stick-dice.svg
--rwxr-xr-x   0        0        0     1537 2023-12-13 10:35:40.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/usb-stick.svg
--rw-r--r--   0        0        0     1203 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/usb.svg
--rw-r--r--   0        0        0     3144 2024-02-26 09:16:36.816540 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/vault.svg
--rw-r--r--   0        0        0      824 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/wallet.png
--rw-r--r--   0        0        0     4839 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/warning.png
--rw-r--r--   0        0        0    11786 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/zoom.png
--rw-r--r--   0        0        0    57378 2024-04-25 19:36:30.568801 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_ar_AE.qm
--rw-r--r--   0        0        0    83650 2024-04-25 19:36:30.524800 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_ar_AE.ts
--rw-r--r--   0        0        0    64114 2024-04-25 19:36:30.580802 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_es_ES.qm
--rw-r--r--   0        0        0    78563 2024-04-25 19:36:28.976764 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_es_ES.ts
--rw-r--r--   0        0        0    60174 2024-04-25 19:36:30.572801 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_hi_IN.qm
--rw-r--r--   0        0        0    95901 2024-04-25 19:36:29.612779 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_hi_IN.ts
--rw-r--r--   0        0        0    48866 2024-04-25 19:36:30.576801 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_ja_JP.qm
--rw-r--r--   0        0        0    82623 2024-04-25 19:36:30.224793 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_ja_JP.ts
--rw-r--r--   0        0        0    63502 2024-04-25 19:36:30.580802 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_pt_PT.qm
--rw-r--r--   0        0        0    78432 2024-04-25 19:36:29.920786 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_pt_PT.ts
--rw-r--r--   0        0        0    64616 2024-04-25 19:36:30.564801 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_ru_RU.qm
--rw-r--r--   0        0        0    90820 2024-04-25 19:36:29.292771 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_ru_RU.ts
--rw-r--r--   0        0        0    43656 2024-04-25 19:36:30.568801 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_zh_CN.qm
--rw-r--r--   0        0        0    74932 2024-04-25 19:36:28.656756 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_zh_CN.ts
--rw-r--r--   0        0        0     8711 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/new_wallet_design.ui
--rw-r--r--   0        0        0        0 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/__init__.py
--rw-r--r--   0        0        0     6670 2024-04-26 06:09:53.642566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/about_dialog.py
--rw-r--r--   0        0        0     6031 2024-04-26 06:09:53.638566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/address_dialog.py
--rw-r--r--   0        0        0    25684 2024-04-26 06:09:53.638566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/address_list.py
--rw-r--r--   0        0        0     3192 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/bitcoin_quick_receive.py
--rw-r--r--   0        0        0    15674 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/block_buttons.py
--rw-r--r--   0        0        0     2842 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/block_change_signals.py
--rw-r--r--   0        0        0    13654 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/buttonedit.py
--rw-r--r--   0        0        0     4474 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/category_list.py
--rw-r--r--   0        0        0     2570 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/controlled_groupbox.py
--rw-r--r--   0        0        0     6474 2024-04-26 06:09:53.642566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/custom_edits.py
--rw-r--r--   0        0        0     4345 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/data_tab_widget.py
--rw-r--r--   0        0        0     4434 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/debug_widget.py
--rw-r--r--   0        0        0    17557 2024-04-26 06:09:53.638566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/descriptor_ui.py
--rw-r--r--   0        0        0     6808 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/dialog_import.py
--rw-r--r--   0        0        0     9559 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/dialogs.py
--rw-r--r--   0        0        0     5471 2024-04-26 06:09:53.658566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/downloader.py
--rw-r--r--   0        0        0     5479 2024-04-26 06:09:53.658566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/expandable_widget.py
--rw-r--r--   0        0        0    14760 2024-04-26 06:09:53.658566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/export_data.py
--rw-r--r--   0        0        0    13013 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/fee_group.py
--rw-r--r--   0        0        0    27430 2024-04-27 07:03:44.978069 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/hist_list.py
--rw-r--r--   0        0        0     3080 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/html_delegate.py
--rw-r--r--   0        0        0     1918 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/invisible_scroll_area.py
--rw-r--r--   0        0        0    22871 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/keystore_ui.py
--rw-r--r--   0        0        0     7813 2024-04-26 06:09:53.658566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/keystore_uis.py
--rw-r--r--   0        0        0     5154 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/label_syncer.py
--rw-r--r--   0        0        0     6664 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/language_chooser.py
--rw-r--r--   0        0        0    46762 2024-04-27 07:03:45.602082 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/main.py
--rw-r--r--   0        0        0    33789 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/my_treeview.py
--rw-r--r--   0        0        0     4284 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/mytabwidget.py
--rw-r--r--   0        0        0     4255 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nLockTimePicker.py
--rw-r--r--   0        0        0       20 2024-02-23 06:55:23.224482 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/network_settings/__init__.py
--rw-r--r--   0        0        0     1455 2024-04-12 11:53:22.023574 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/network_settings/__main__.py
--rw-r--r--   0        0        0    26160 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/network_settings/main.py
--rw-r--r--   0        0        0     9023 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/new_wallet_welcome_screen.py
--rw-r--r--   0        0        0        0 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/__init__.py
--rw-r--r--   0        0        0     2931 2024-04-12 15:30:48.598519 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/__main__.py
--rw-r--r--   0        0        0        0 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/connected_devices/__init__.py
--rw-r--r--   0        0        0      813 2024-04-12 15:28:39.016484 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/connected_devices/__main__.py
--rw-r--r--   0        0        0    11239 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/connected_devices/chat_gui.py
--rw-r--r--   0        0        0     1146 2024-02-05 10:38:12.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/connected_devices/clip.svg
--rw-r--r--   0        0        0    15019 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/connected_devices/connected_devices.py
--rw-r--r--   0        0        0    38797 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/nostr.py
--rw-r--r--   0        0        0    17776 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/nostr_sync.py
--rw-r--r--   0        0        0     5435 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/notification_bar.py
--rw-r--r--   0        0        0     2396 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/notification_bar_regtest.py
--rw-r--r--   0        0        0    11187 2024-04-26 06:09:53.638566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/plot.py
--rw-r--r--   0        0        0        0 2024-02-22 10:28:40.561281 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/qr_components/__init__.py
--rw-r--r--   0        0        0      900 2024-02-08 13:19:31.445074 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/qr_components/__main__.py
--rw-r--r--   0        0        0    14098 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/qr_components/image_widget.py
--rw-r--r--   0        0        0     3680 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/qr_components/qr.py
--rw-r--r--   0        0        0     6437 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/qr_components/quick_receive.py
--rw-r--r--   0        0        0    30721 2024-04-27 07:03:45.006070 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/qt_wallet.py
--rw-r--r--   0        0        0    16090 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/recipients.py
--rw-r--r--   0        0        0    17071 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/search_tree_view.py
--rw-r--r--   0        0        0     4318 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/slider.py
--rw-r--r--   0        0        0     2755 2024-04-26 06:09:53.658566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/spinbox.py
--rw-r--r--   0        0        0     5194 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/spinning_button.py
--rw-r--r--   0        0        0    34891 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/step_progress_bar.py
--rw-r--r--   0        0        0     7647 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/sync_tab.py
--rw-r--r--   0        0        0     3470 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/synced_tab_widget.py
--rw-r--r--   0        0        0       20 2024-02-22 10:31:13.688337 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/taglist/__init__.py
--rw-r--r--   0        0        0      830 2024-02-14 11:17:43.657660 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/taglist/__main__.py
--rw-r--r--   0        0        0    24952 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/taglist/main.py
--rw-r--r--   0        0        0    44448 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/tutorial.py
--rw-r--r--   0        0        0     5332 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/tutorial_screenshots.py
--rw-r--r--   0        0        0     7504 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/tx_signing_steps.py
--rw-r--r--   0        0        0    53353 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/ui_tx.py
--rw-r--r--   0        0        0     8358 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/update_notification_bar.py
--rw-r--r--   0        0        0    23920 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/util.py
--rw-r--r--   0        0        0    17572 2024-04-26 06:09:53.658566 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/utxo_list.py
--rw-r--r--   0        0        0     4206 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/send.ui
--rw-r--r--   0        0        0    11975 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/settings.ui
--rw-r--r--   0        0        0     1713 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/gui/sign_tx.ui
--rw-r--r--   0        0        0     1941 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a0/bitcoin_safe/html.py
--rw-r--r--   0        0        0     1560 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a0/bitcoin_safe/i18n.py
--rw-r--r--   0        0        0     7834 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a0/bitcoin_safe/keystore.py
--rw-r--r--   0        0        0    13025 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a0/bitcoin_safe/labels.py
--rw-r--r--   0        0        0     3124 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a0/bitcoin_safe/logging_handlers.py
--rw-r--r--   0        0        0     3611 2024-04-26 06:09:53.626565 bitcoin_safe-0.6.0a0/bitcoin_safe/logging_setup.py
--rw-r--r--   0        0        0     3877 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a0/bitcoin_safe/main.ui
--rw-r--r--   0        0        0     9155 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a0/bitcoin_safe/mempool.py
--rw-r--r--   0        0        0    12920 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a0/bitcoin_safe/network_config.py
--rw-r--r--   0        0        0    12221 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a0/bitcoin_safe/pdfrecovery.py
--rw-r--r--   0        0        0    17559 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a0/bitcoin_safe/psbt_util.py
--rw-r--r--   0        0        0    11408 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a0/bitcoin_safe/pythonbdk_types.py
--rw-r--r--   0        0        0     2417 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a0/bitcoin_safe/rpc.py
--rw-r--r--   0        0        0     6686 2024-04-27 07:03:44.266054 bitcoin_safe-0.6.0a0/bitcoin_safe/signals.py
--rw-r--r--   0        0        0    23647 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a0/bitcoin_safe/signature_manager.py
--rw-r--r--   0        0        0    12555 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a0/bitcoin_safe/signer.py
--rwxr-xr-x   0        0        0     3106 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a0/bitcoin_safe/simple_mailer.py
--rw-r--r--   0        0        0     9495 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a0/bitcoin_safe/storage.py
--rw-r--r--   0        0        0     7053 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a0/bitcoin_safe/threading_manager.py
--rw-r--r--   0        0        0     5944 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a0/bitcoin_safe/tx.py
--rw-r--r--   0        0        0     1700 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a0/bitcoin_safe/tx_util.py
--rw-r--r--   0        0        0    23909 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a0/bitcoin_safe/util.py
--rw-r--r--   0        0        0    65937 2024-04-26 06:09:53.626565 bitcoin_safe-0.6.0a0/bitcoin_safe/wallet.py
--rw-r--r--   0        0        0     5761 2024-04-27 08:01:25.905279 bitcoin_safe-0.6.0a0/pyproject.toml
--rw-r--r--   0        0        0     5584 1970-01-01 00:00:00.000000 bitcoin_safe-0.6.0a0/PKG-INFO
+-rw-r--r--   0        0        0      644 2024-03-20 13:56:51.549261 bitcoin_safe-0.6.0a1/LICENSE
+-rw-r--r--   0        0        0     4530 2024-04-27 08:33:29.931397 bitcoin_safe-0.6.0a1/README.md
+-rw-r--r--   0        0        0       24 2024-04-27 10:11:06.893561 bitcoin_safe-0.6.0a1/bitcoin_safe/__init__.py
+-rw-r--r--   0        0        0     1456 2024-04-24 16:26:26.615316 bitcoin_safe-0.6.0a1/bitcoin_safe/__main__.py
+-rw-r--r--   0        0        0     6932 2024-04-26 06:09:53.626565 bitcoin_safe-0.6.0a1/bitcoin_safe/config.py
+-rw-r--r--   0        0        0     2999 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a1/bitcoin_safe/descriptors.py
+-rw-r--r--   0        0        0     1306 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a1/bitcoin_safe/device_export.py
+-rw-r--r--   0        0        0     4976 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a1/bitcoin_safe/dynamic_lib_load.py
+-rw-r--r--   0        0        0     1305 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a1/bitcoin_safe/execute_config.py
+-rw-r--r--   0        0        0     2141 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a1/bitcoin_safe/fx.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/__init__.py
+-rw-r--r--   0        0        0    12417 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/explainer0.ui
+-rw-r--r--   0        0        0    12419 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/explainer1.ui
+-rw-r--r--   0        0        0   122131 2023-12-08 19:45:37.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/2of3backup.svg
+-rw-r--r--   0        0        0      687 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/add.png
+-rw-r--r--   0        0        0     1349 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/android_electrum_icon_background.png
+-rw-r--r--   0        0        0     8928 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/bitcoin-testnet.png
+-rw-r--r--   0        0        0     3075 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/bug.png
+-rw-r--r--   0        0        0     1096 2023-12-14 15:09:14.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/camera.svg
+-rw-r--r--   0        0        0      687 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/camera_dark.png
+-rw-r--r--   0        0        0     1304 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/camera_white.png
+-rw-r--r--   0        0        0    54212 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/checkmark.png
+-rw-r--r--   0        0        0     1044 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/chevron-right.png
+-rw-r--r--   0        0        0     1146 2024-02-05 10:38:12.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/clip.svg
+-rw-r--r--   0        0        0     7607 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/clock1.png
+-rw-r--r--   0        0        0     8512 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/clock2.png
+-rw-r--r--   0        0        0     7229 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/clock3.png
+-rw-r--r--   0        0        0     7522 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/clock4.png
+-rw-r--r--   0        0        0    10074 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/clock5.png
+-rw-r--r--   0        0        0     3521 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/closebutton.png
+-rw-r--r--   0        0        0     3812 2024-02-03 12:39:12.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/cloud-sync.svg
+-rw-r--r--   0        0        0    14573 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/cloud_no.png
+-rw-r--r--   0        0        0     8329 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/cloud_yes.png
+-rw-r--r--   0        0        0     8070 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard-dice.svg
+-rw-r--r--   0        0        0    17195 2024-01-28 12:33:26.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard-generate24.png
+-rw-r--r--   0        0        0     4229 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard-only.svg
+-rw-r--r--   0        0        0    14288 2024-01-28 09:08:54.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard-register-multisig-decriptor.png
+-rw-r--r--   0        0        0    14316 2024-02-28 10:15:29.171933 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard-view-seed.png
+-rw-r--r--   0        0        0    14353 2024-01-28 09:08:09.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard-wallet-export.png
+-rw-r--r--   0        0        0     5283 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard.png
+-rw-r--r--   0        0        0     4274 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard.svg
+-rw-r--r--   0        0        0     5242 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard_unpaired.png
+-rw-r--r--   0        0        0     3566 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard_unpaired.svg
+-rw-r--r--   0        0        0    54212 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/confirmed.png
+-rw-r--r--   0        0        0     4153 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/confirmed.svg
+-rw-r--r--   0        0        0     5113 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/confirmed_bw.png
+-rw-r--r--   0        0        0     2111 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/copy.png
+-rw-r--r--   0        0        0      880 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/copy_bw.png
+-rw-r--r--   0        0        0      453 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/delete.png
+-rw-r--r--   0        0        0    65286 2023-12-24 11:19:00.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/descriptor-backup.svg
+-rw-r--r--   0        0        0    18399 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/descriptor.svg
+-rw-r--r--   0        0        0    20662 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/descriptor3.svg
+-rw-r--r--   0        0        0     1863 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/dice.svg
+-rw-r--r--   0        0        0   249404 2024-02-26 10:25:07.531743 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/distribute-multisig.svg
+-rw-r--r--   0        0        0   293552 2024-02-26 10:27:16.318444 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/distribute-multisigsig-export.svgz
+-rw-r--r--   0        0        0    45895 2024-02-26 10:08:52.867612 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/distribute-singlesig-export.svgz
+-rw-r--r--   0        0        0    83484 2024-02-26 10:07:04.773452 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/distribute-singlesig.svg
+-rw-r--r--   0        0        0     2970 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/download.png
+-rw-r--r--   0        0        0     2225 2024-02-26 10:06:33.612835 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/earth.svg
+-rw-r--r--   0        0        0     2510 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/electrumb.png
+-rw-r--r--   0        0        0    28522 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/expired.png
+-rw-r--r--   0        0        0     2910 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/eye1.png
+-rw-r--r--   0        0        0     4779 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/file.png
+-rw-r--r--   0        0        0     5938 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/globe.png
+-rw-r--r--   0        0        0      240 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/hamburger.png
+-rw-r--r--   0        0        0     1276 2023-07-07 19:42:34.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/history.svg
+-rw-r--r--   0        0        0     1771 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/info.png
+-rw-r--r--   0        0        0    15433 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/kangaroo.png
+-rw-r--r--   0        0        0     1230 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/keep-quiet-icon.svg
+-rw-r--r--   0        0        0    15398 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/key-gray.png
+-rw-r--r--   0        0        0      988 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/key-hole-icon.svg
+-rw-r--r--   0        0        0     5428 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/key.png
+-rw-r--r--   0        0        0    23125 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/link.png
+-rw-r--r--   0        0        0     1674 2023-12-14 18:36:51.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/loader-icon.svg
+-rw-r--r--   0        0        0    40380 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/lock.png
+-rw-r--r--   0        0        0    12125 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/lock.svg
+-rw-r--r--   0        0        0     4400 2023-07-06 09:39:13.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/logo.svg
+-rw-r--r--   0        0        0     4548 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/mail_icon.png
+-rw-r--r--   0        0        0      997 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/menu_vertical.png
+-rw-r--r--   0        0        0     5565 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/menu_vertical_white.png
+-rw-r--r--   0        0        0      199 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/microphone.png
+-rw-r--r--   0        0        0     3031 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/network.png
+-rw-r--r--   0        0        0     1117 2023-07-06 11:00:16.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/no-photography-icon.svg
+-rw-r--r--   0        0        0    10364 2023-07-06 11:57:23.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/no-typing-icon.svg
+-rw-r--r--   0        0        0      463 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/offline_tx.png
+-rw-r--r--   0        0        0     1309 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/paste.png
+-rw-r--r--   0        0        0     2173 2023-07-01 09:19:26.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/pdf-file.svg
+-rw-r--r--   0        0        0     1641 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/pen.png
+-rw-r--r--   0        0        0     1238 2023-12-14 15:42:01.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/pen.svg
+-rw-r--r--   0        0        0     1519 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/picture_in_picture.png
+-rw-r--r--   0        0        0    58005 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/preferences.png
+-rw-r--r--   0        0        0    27175 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/preferences.svg
+-rw-r--r--   0        0        0     3177 2023-12-14 18:20:48.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/print.svg
+-rw-r--r--   0        0        0     1200 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/qr-code.svg
+-rw-r--r--   0        0        0      314 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/qrcode.png
+-rw-r--r--   0        0        0      380 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/qrcode_white.png
+-rw-r--r--   0        0        0     2555 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/question.png
+-rw-r--r--   0        0        0     1929 2023-07-07 20:04:30.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/receive.svg
+-rw-r--r--   0        0        0     1426 2023-06-30 17:44:30.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/reset-update.svg
+-rw-r--r--   0        0        0      272 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/revealer.png
+-rw-r--r--   0        0        0     1965 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/revealer_c.png
+-rw-r--r--   0        0        0     1860 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/right-arrow.svg
+-rw-r--r--   0        0        0     3869 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/rocket.png
+-rw-r--r--   0        0        0      946 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/save.png
+-rw-r--r--   0        0        0     1261 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/sd-card.svg
+-rw-r--r--   0        0        0    38276 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/seal.png
+-rw-r--r--   0        0        0    17829 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/seed-plate-large.svg
+-rw-r--r--   0        0        0    24206 2023-07-01 06:31:12.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/seed-plate.svg
+-rw-r--r--   0        0        0    10322 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/seed.png
+-rw-r--r--   0        0        0      820 2024-01-03 16:14:13.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/send.svg
+-rw-r--r--   0        0        0     3325 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/share.png
+-rw-r--r--   0        0        0      392 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/speaker.png
+-rw-r--r--   0        0        0    71068 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_connected.png
+-rw-r--r--   0        0        0     6593 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_connected.svg
+-rw-r--r--   0        0        0    62949 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_connected_fork.png
+-rw-r--r--   0        0        0    69081 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_connected_proxy.png
+-rw-r--r--   0        0        0     6593 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_connected_proxy.svg
+-rw-r--r--   0        0        0    60879 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_connected_proxy_fork.png
+-rw-r--r--   0        0        0    66105 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_disconnected.png
+-rw-r--r--   0        0        0    10522 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_disconnected.svg
+-rw-r--r--   0        0        0    74851 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_lagging.png
+-rw-r--r--   0        0        0     6595 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_lagging.svg
+-rw-r--r--   0        0        0    63949 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_lagging_fork.png
+-rw-r--r--   0        0        0    81206 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_waiting.png
+-rw-r--r--   0        0        0    17633 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_waiting.svg
+-rw-r--r--   0        0        0      886 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/tab_addresses.png
+-rw-r--r--   0        0        0     1592 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/tab_coins.png
+-rw-r--r--   0        0        0      824 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/tab_console.png
+-rw-r--r--   0        0        0     1446 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/tab_contacts.png
+-rw-r--r--   0        0        0     1873 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/tab_receive.png
+-rw-r--r--   0        0        0     2712 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/tor_logo.png
+-rw-r--r--   0        0        0     3532 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/unconfirmed.png
+-rw-r--r--   0        0        0     5499 2024-01-03 16:09:47.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/unconfirmed.svg
+-rw-r--r--   0        0        0     6118 2024-01-03 16:13:32.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/unconfirmed_child.svg
+-rw-r--r--   0        0        0     1256 2023-06-30 17:26:47.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/undo-arrow.svg
+-rw-r--r--   0        0        0    45956 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/unlock.png
+-rw-r--r--   0        0        0    19461 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/unlock.svg
+-rw-r--r--   0        0        0    23805 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/unpaid.png
+-rw-r--r--   0        0        0     1580 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/update.png
+-rwxr-xr-x   0        0        0     4485 2023-12-13 10:35:24.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/usb-stick-dice.svg
+-rwxr-xr-x   0        0        0     1537 2023-12-13 10:35:40.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/usb-stick.svg
+-rw-r--r--   0        0        0     1203 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/usb.svg
+-rw-r--r--   0        0        0     3144 2024-02-26 09:16:36.816540 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/vault.svg
+-rw-r--r--   0        0        0      824 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/wallet.png
+-rw-r--r--   0        0        0     4839 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/warning.png
+-rw-r--r--   0        0        0    11786 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/zoom.png
+-rw-r--r--   0        0        0    57378 2024-04-25 19:36:30.568801 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_ar_AE.qm
+-rw-r--r--   0        0        0    83650 2024-04-25 19:36:30.524800 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_ar_AE.ts
+-rw-r--r--   0        0        0    64114 2024-04-25 19:36:30.580802 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_es_ES.qm
+-rw-r--r--   0        0        0    78563 2024-04-25 19:36:28.976764 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_es_ES.ts
+-rw-r--r--   0        0        0    60174 2024-04-25 19:36:30.572801 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_hi_IN.qm
+-rw-r--r--   0        0        0    95901 2024-04-25 19:36:29.612779 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_hi_IN.ts
+-rw-r--r--   0        0        0    48866 2024-04-25 19:36:30.576801 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_ja_JP.qm
+-rw-r--r--   0        0        0    82623 2024-04-25 19:36:30.224793 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_ja_JP.ts
+-rw-r--r--   0        0        0    63502 2024-04-25 19:36:30.580802 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_pt_PT.qm
+-rw-r--r--   0        0        0    78432 2024-04-25 19:36:29.920786 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_pt_PT.ts
+-rw-r--r--   0        0        0    64616 2024-04-25 19:36:30.564801 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_ru_RU.qm
+-rw-r--r--   0        0        0    90820 2024-04-25 19:36:29.292771 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_ru_RU.ts
+-rw-r--r--   0        0        0    43656 2024-04-25 19:36:30.568801 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_zh_CN.qm
+-rw-r--r--   0        0        0    74932 2024-04-25 19:36:28.656756 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_zh_CN.ts
+-rw-r--r--   0        0        0     8711 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/new_wallet_design.ui
+-rw-r--r--   0        0        0        0 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/__init__.py
+-rw-r--r--   0        0        0     6670 2024-04-26 06:09:53.642566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/about_dialog.py
+-rw-r--r--   0        0        0     6031 2024-04-26 06:09:53.638566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/address_dialog.py
+-rw-r--r--   0        0        0    25684 2024-04-26 06:09:53.638566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/address_list.py
+-rw-r--r--   0        0        0     3192 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/bitcoin_quick_receive.py
+-rw-r--r--   0        0        0    15674 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/block_buttons.py
+-rw-r--r--   0        0        0     2842 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/block_change_signals.py
+-rw-r--r--   0        0        0    13654 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/buttonedit.py
+-rw-r--r--   0        0        0     4474 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/category_list.py
+-rw-r--r--   0        0        0     2570 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/controlled_groupbox.py
+-rw-r--r--   0        0        0     6474 2024-04-26 06:09:53.642566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/custom_edits.py
+-rw-r--r--   0        0        0     4345 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/data_tab_widget.py
+-rw-r--r--   0        0        0     4434 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/debug_widget.py
+-rw-r--r--   0        0        0    17557 2024-04-26 06:09:53.638566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/descriptor_ui.py
+-rw-r--r--   0        0        0     6808 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/dialog_import.py
+-rw-r--r--   0        0        0     9559 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/dialogs.py
+-rw-r--r--   0        0        0     5471 2024-04-26 06:09:53.658566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/downloader.py
+-rw-r--r--   0        0        0     5479 2024-04-26 06:09:53.658566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/expandable_widget.py
+-rw-r--r--   0        0        0    14760 2024-04-26 06:09:53.658566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/export_data.py
+-rw-r--r--   0        0        0    13013 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/fee_group.py
+-rw-r--r--   0        0        0    27430 2024-04-27 07:03:44.978069 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/hist_list.py
+-rw-r--r--   0        0        0     3080 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/html_delegate.py
+-rw-r--r--   0        0        0     1918 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/invisible_scroll_area.py
+-rw-r--r--   0        0        0    22871 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/keystore_ui.py
+-rw-r--r--   0        0        0     7813 2024-04-26 06:09:53.658566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/keystore_uis.py
+-rw-r--r--   0        0        0     5154 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/label_syncer.py
+-rw-r--r--   0        0        0     6664 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/language_chooser.py
+-rw-r--r--   0        0        0    46762 2024-04-27 07:03:45.602082 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/main.py
+-rw-r--r--   0        0        0    33789 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/my_treeview.py
+-rw-r--r--   0        0        0     4284 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/mytabwidget.py
+-rw-r--r--   0        0        0     4255 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nLockTimePicker.py
+-rw-r--r--   0        0        0       20 2024-02-23 06:55:23.224482 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/network_settings/__init__.py
+-rw-r--r--   0        0        0     1455 2024-04-12 11:53:22.023574 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/network_settings/__main__.py
+-rw-r--r--   0        0        0    26160 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/network_settings/main.py
+-rw-r--r--   0        0        0     9023 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/new_wallet_welcome_screen.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/__init__.py
+-rw-r--r--   0        0        0     2931 2024-04-12 15:30:48.598519 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/connected_devices/__init__.py
+-rw-r--r--   0        0        0      813 2024-04-12 15:28:39.016484 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/connected_devices/__main__.py
+-rw-r--r--   0        0        0    11239 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/connected_devices/chat_gui.py
+-rw-r--r--   0        0        0     1146 2024-02-05 10:38:12.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/connected_devices/clip.svg
+-rw-r--r--   0        0        0    15019 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/connected_devices/connected_devices.py
+-rw-r--r--   0        0        0    38797 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/nostr.py
+-rw-r--r--   0        0        0    17776 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/nostr_sync.py
+-rw-r--r--   0        0        0     5435 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/notification_bar.py
+-rw-r--r--   0        0        0     2396 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/notification_bar_regtest.py
+-rw-r--r--   0        0        0    11187 2024-04-26 06:09:53.638566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/plot.py
+-rw-r--r--   0        0        0        0 2024-02-22 10:28:40.561281 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/qr_components/__init__.py
+-rw-r--r--   0        0        0      900 2024-02-08 13:19:31.445074 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/qr_components/__main__.py
+-rw-r--r--   0        0        0    14098 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/qr_components/image_widget.py
+-rw-r--r--   0        0        0     3680 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/qr_components/qr.py
+-rw-r--r--   0        0        0     6437 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/qr_components/quick_receive.py
+-rw-r--r--   0        0        0    30721 2024-04-27 07:03:45.006070 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/qt_wallet.py
+-rw-r--r--   0        0        0    16090 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/recipients.py
+-rw-r--r--   0        0        0    17071 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/search_tree_view.py
+-rw-r--r--   0        0        0     4318 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/slider.py
+-rw-r--r--   0        0        0     2755 2024-04-26 06:09:53.658566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/spinbox.py
+-rw-r--r--   0        0        0     5194 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/spinning_button.py
+-rw-r--r--   0        0        0    34891 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/step_progress_bar.py
+-rw-r--r--   0        0        0     7647 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/sync_tab.py
+-rw-r--r--   0        0        0     3470 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/synced_tab_widget.py
+-rw-r--r--   0        0        0       20 2024-02-22 10:31:13.688337 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/taglist/__init__.py
+-rw-r--r--   0        0        0      830 2024-02-14 11:17:43.657660 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/taglist/__main__.py
+-rw-r--r--   0        0        0    24952 2024-04-26 06:09:53.662566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/taglist/main.py
+-rw-r--r--   0        0        0    44448 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/tutorial.py
+-rw-r--r--   0        0        0     5332 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/tutorial_screenshots.py
+-rw-r--r--   0        0        0     7504 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/tx_signing_steps.py
+-rw-r--r--   0        0        0    53353 2024-04-26 06:09:53.650566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/ui_tx.py
+-rw-r--r--   0        0        0     8358 2024-04-26 06:09:53.654566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/update_notification_bar.py
+-rw-r--r--   0        0        0    23920 2024-04-26 06:09:53.646566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/util.py
+-rw-r--r--   0        0        0    17572 2024-04-26 06:09:53.658566 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/utxo_list.py
+-rw-r--r--   0        0        0     4206 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/send.ui
+-rw-r--r--   0        0        0    11975 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/settings.ui
+-rw-r--r--   0        0        0     1713 2023-06-25 13:54:16.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/gui/sign_tx.ui
+-rw-r--r--   0        0        0     1941 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a1/bitcoin_safe/html.py
+-rw-r--r--   0        0        0     1560 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a1/bitcoin_safe/i18n.py
+-rw-r--r--   0        0        0     7834 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a1/bitcoin_safe/keystore.py
+-rw-r--r--   0        0        0    13025 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a1/bitcoin_safe/labels.py
+-rw-r--r--   0        0        0     3124 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a1/bitcoin_safe/logging_handlers.py
+-rw-r--r--   0        0        0     3611 2024-04-26 06:09:53.626565 bitcoin_safe-0.6.0a1/bitcoin_safe/logging_setup.py
+-rw-r--r--   0        0        0     3877 2023-06-25 13:54:04.000000 bitcoin_safe-0.6.0a1/bitcoin_safe/main.ui
+-rw-r--r--   0        0        0     9155 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a1/bitcoin_safe/mempool.py
+-rw-r--r--   0        0        0    12920 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a1/bitcoin_safe/network_config.py
+-rw-r--r--   0        0        0    12221 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a1/bitcoin_safe/pdfrecovery.py
+-rw-r--r--   0        0        0    17559 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a1/bitcoin_safe/psbt_util.py
+-rw-r--r--   0        0        0    11408 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a1/bitcoin_safe/pythonbdk_types.py
+-rw-r--r--   0        0        0     2417 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a1/bitcoin_safe/rpc.py
+-rw-r--r--   0        0        0     6686 2024-04-27 07:03:44.266054 bitcoin_safe-0.6.0a1/bitcoin_safe/signals.py
+-rw-r--r--   0        0        0    23647 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a1/bitcoin_safe/signature_manager.py
+-rw-r--r--   0        0        0    12555 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a1/bitcoin_safe/signer.py
+-rwxr-xr-x   0        0        0     3106 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a1/bitcoin_safe/simple_mailer.py
+-rw-r--r--   0        0        0     9495 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a1/bitcoin_safe/storage.py
+-rw-r--r--   0        0        0     7261 2024-04-27 10:22:55.252857 bitcoin_safe-0.6.0a1/bitcoin_safe/threading_manager.py
+-rw-r--r--   0        0        0     5944 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a1/bitcoin_safe/tx.py
+-rw-r--r--   0        0        0     1700 2024-04-26 06:09:53.630566 bitcoin_safe-0.6.0a1/bitcoin_safe/tx_util.py
+-rw-r--r--   0        0        0    23909 2024-04-26 06:09:53.634565 bitcoin_safe-0.6.0a1/bitcoin_safe/util.py
+-rw-r--r--   0        0        0    65937 2024-04-26 06:09:53.626565 bitcoin_safe-0.6.0a1/bitcoin_safe/wallet.py
+-rw-r--r--   0        0        0     5761 2024-04-27 08:01:25.905279 bitcoin_safe-0.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0     5867 1970-01-01 00:00:00.000000 bitcoin_safe-0.6.0a1/PKG-INFO
```

### Comparing `bitcoin_safe-0.6.0a0/LICENSE` & `bitcoin_safe-0.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/README.md` & `bitcoin_safe-0.6.0a1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -138,7 +138,30 @@
 nigiri rpc generatetoaddress 1 bcrt1qgsnt3d4sny4w4zd5zl9x6jufc5rankqmgphyms9vz0ds73q4xfms655y4c # mine blocks
 
 # or use the internal faucet
 nigiri faucet bcrt1qgsnt3d4sny4w4zd5zl9x6jufc5rankqmgphyms9vz0ds73q4xfms655y4c 0.01
 ```
 
 * 
+
+
+
+
+## Installation from PyPi
+
+### Ubuntu, Debian, Windows
+
+- Install `poetry` and run `bitcoin_safe`
+  
+  ```sh
+  pip install bitcoin-safe
+  python -m bitcoin_safe
+  ```
+
+### Mac
+
+- Run `bitcoin_safe`
+  
+  ```sh
+  python3 -m pip install bitcoin-safe
+  python3 -m bitcoin_safe
+  ```
```

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/__main__.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/__main__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/config.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/config.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/descriptors.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/descriptors.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/device_export.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/device_export.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/dynamic_lib_load.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/dynamic_lib_load.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/execute_config.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/execute_config.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/fx.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/fx.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/explainer0.ui` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/explainer0.ui`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/explainer1.ui` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/explainer1.ui`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/2of3backup.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/2of3backup.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/add.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/add.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/android_electrum_icon_background.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/android_electrum_icon_background.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/bitcoin-testnet.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/bitcoin-testnet.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/bug.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/bug.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/camera.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/camera.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/camera_dark.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/camera_dark.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/camera_white.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/camera_white.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/checkmark.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/checkmark.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/chevron-right.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/chevron-right.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/clip.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/clip.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/clock1.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/clock1.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/clock2.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/clock2.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/clock3.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/clock3.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/clock4.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/clock4.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/clock5.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/clock5.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/closebutton.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/closebutton.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/cloud-sync.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/cloud-sync.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/cloud_no.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/cloud_no.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/cloud_yes.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/cloud_yes.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard-dice.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard-dice.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard-generate24.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard-generate24.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard-only.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard-only.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard-register-multisig-decriptor.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard-register-multisig-decriptor.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard-view-seed.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard-view-seed.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard-wallet-export.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard-wallet-export.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard_unpaired.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard_unpaired.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/coldcard_unpaired.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/coldcard_unpaired.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/confirmed.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/confirmed.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/confirmed.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/confirmed.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/confirmed_bw.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/confirmed_bw.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/copy.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/copy.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/copy_bw.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/copy_bw.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/descriptor-backup.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/descriptor-backup.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/descriptor.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/descriptor.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/descriptor3.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/descriptor3.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/dice.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/dice.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/distribute-multisig.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/distribute-multisig.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/distribute-multisigsig-export.svgz` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/distribute-multisigsig-export.svgz`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/distribute-singlesig-export.svgz` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/distribute-singlesig-export.svgz`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/distribute-singlesig.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/distribute-singlesig.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/download.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/download.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/earth.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/earth.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/electrumb.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/electrumb.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/expired.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/expired.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/eye1.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/eye1.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/file.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/file.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/globe.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/globe.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/history.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/history.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/info.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/info.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/kangaroo.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/kangaroo.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/keep-quiet-icon.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/keep-quiet-icon.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/key-gray.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/key-gray.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/key-hole-icon.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/key-hole-icon.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/key.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/key.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/link.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/link.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/loader-icon.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/loader-icon.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/lock.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/lock.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/lock.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/lock.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/logo.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/logo.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/mail_icon.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/mail_icon.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/menu_vertical.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/menu_vertical.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/menu_vertical_white.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/menu_vertical_white.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/network.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/network.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/no-photography-icon.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/no-photography-icon.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/no-typing-icon.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/no-typing-icon.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/paste.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/paste.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/pdf-file.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/pdf-file.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/pen.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/pen.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/pen.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/pen.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/picture_in_picture.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/picture_in_picture.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/preferences.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/preferences.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/preferences.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/preferences.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/print.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/print.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/qr-code.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/qr-code.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/question.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/question.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/receive.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/receive.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/reset-update.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/reset-update.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/revealer_c.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/revealer_c.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/right-arrow.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/right-arrow.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/rocket.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/rocket.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/save.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/save.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/sd-card.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/sd-card.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/seal.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/seal.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/seed-plate-large.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/seed-plate-large.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/seed-plate.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/seed-plate.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/seed.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/seed.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/send.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/send.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/share.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/share.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_connected.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_connected.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_connected.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_connected.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_connected_fork.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_connected_fork.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_connected_proxy.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_connected_proxy.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_connected_proxy.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_connected_proxy.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_connected_proxy_fork.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_connected_proxy_fork.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_disconnected.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_disconnected.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_disconnected.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_disconnected.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_lagging.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_lagging.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_lagging.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_lagging.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_lagging_fork.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_lagging_fork.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_waiting.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_waiting.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/status_waiting.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/status_waiting.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/tab_addresses.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/tab_addresses.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/tab_coins.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/tab_coins.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/tab_console.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/tab_console.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/tab_contacts.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/tab_contacts.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/tab_receive.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/tab_receive.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/tor_logo.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/tor_logo.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/unconfirmed.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/unconfirmed.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/unconfirmed.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/unconfirmed.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/unconfirmed_child.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/unconfirmed_child.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/undo-arrow.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/undo-arrow.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/unlock.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/unlock.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/unlock.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/unlock.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/unpaid.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/unpaid.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/update.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/update.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/usb-stick-dice.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/usb-stick-dice.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/usb-stick.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/usb-stick.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/usb.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/usb.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/vault.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/vault.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/wallet.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/wallet.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/warning.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/warning.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/icons/zoom.png` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_ar_AE.qm` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_ar_AE.qm`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_ar_AE.ts` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_ar_AE.ts`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_es_ES.qm` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_es_ES.qm`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_es_ES.ts` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_es_ES.ts`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_hi_IN.qm` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_hi_IN.qm`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_hi_IN.ts` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_hi_IN.ts`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_ja_JP.qm` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_ja_JP.qm`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_ja_JP.ts` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_ja_JP.ts`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_pt_PT.qm` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_pt_PT.qm`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_pt_PT.ts` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_pt_PT.ts`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_ru_RU.qm` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_ru_RU.qm`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_ru_RU.ts` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_ru_RU.ts`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_zh_CN.qm` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_zh_CN.qm`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/locales/app_zh_CN.ts` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/locales/app_zh_CN.ts`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/new_wallet_design.ui` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/new_wallet_design.ui`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/about_dialog.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/about_dialog.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/address_dialog.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/address_dialog.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/address_list.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/address_list.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/bitcoin_quick_receive.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/bitcoin_quick_receive.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/block_buttons.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/block_buttons.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/block_change_signals.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/block_change_signals.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/buttonedit.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/buttonedit.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/category_list.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/category_list.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/controlled_groupbox.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/controlled_groupbox.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/custom_edits.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/custom_edits.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/data_tab_widget.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/data_tab_widget.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/debug_widget.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/debug_widget.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/descriptor_ui.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/descriptor_ui.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/dialog_import.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/dialog_import.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/dialogs.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/dialogs.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/downloader.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/downloader.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/expandable_widget.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/expandable_widget.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/export_data.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/export_data.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/fee_group.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/fee_group.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/hist_list.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/hist_list.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/html_delegate.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/html_delegate.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/invisible_scroll_area.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/invisible_scroll_area.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/keystore_ui.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/keystore_ui.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/keystore_uis.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/keystore_uis.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/label_syncer.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/label_syncer.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/language_chooser.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/language_chooser.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/main.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/main.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/my_treeview.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/my_treeview.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/mytabwidget.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/mytabwidget.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nLockTimePicker.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nLockTimePicker.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/network_settings/__main__.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/network_settings/__main__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/network_settings/main.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/network_settings/main.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/new_wallet_welcome_screen.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/new_wallet_welcome_screen.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/__main__.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/connected_devices/__main__.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/connected_devices/__main__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/connected_devices/chat_gui.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/connected_devices/chat_gui.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/connected_devices/clip.svg` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/connected_devices/clip.svg`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/connected_devices/connected_devices.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/connected_devices/connected_devices.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/nostr.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/nostr.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/nostr_sync/nostr_sync.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/nostr_sync/nostr_sync.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/notification_bar.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/notification_bar.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/notification_bar_regtest.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/notification_bar_regtest.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/plot.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/plot.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/qr_components/__main__.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/qr_components/__main__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/qr_components/image_widget.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/qr_components/image_widget.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/qr_components/qr.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/qr_components/qr.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/qr_components/quick_receive.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/qr_components/quick_receive.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/qt_wallet.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/qt_wallet.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/recipients.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/recipients.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/search_tree_view.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/search_tree_view.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/slider.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/slider.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/spinbox.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/spinbox.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/spinning_button.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/spinning_button.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/step_progress_bar.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/step_progress_bar.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/sync_tab.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/sync_tab.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/synced_tab_widget.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/synced_tab_widget.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/taglist/__main__.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/taglist/__main__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/taglist/main.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/taglist/main.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/tutorial.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/tutorial.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/tutorial_screenshots.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/tutorial_screenshots.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/tx_signing_steps.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/tx_signing_steps.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/ui_tx.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/ui_tx.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/update_notification_bar.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/update_notification_bar.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/util.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/util.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/qt/utxo_list.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/qt/utxo_list.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/send.ui` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/send.ui`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/settings.ui` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/settings.ui`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/gui/sign_tx.ui` & `bitcoin_safe-0.6.0a1/bitcoin_safe/gui/sign_tx.ui`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/html.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/html.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/i18n.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/i18n.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/keystore.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/keystore.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/labels.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/labels.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/logging_handlers.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/logging_handlers.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/logging_setup.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/logging_setup.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/main.ui` & `bitcoin_safe-0.6.0a1/bitcoin_safe/main.ui`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/mempool.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/mempool.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/network_config.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/network_config.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/pdfrecovery.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/pdfrecovery.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/psbt_util.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/psbt_util.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/pythonbdk_types.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/pythonbdk_types.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/rpc.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/rpc.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/signals.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/signals.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/signature_manager.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/signature_manager.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/signer.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/signer.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/simple_mailer.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/simple_mailer.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/storage.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/storage.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/threading_manager.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/threading_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -140,14 +140,15 @@
         if self.worker and self.worker.task.cancel:
             logger.debug(f"Stopping {self.thread_name}.")
             self.worker.task.cancel()
         self.my_quit()
 
     def my_quit(self):
         self.quit()
+        self.wait()
         self.signals_min.signal_stop_threat.emit(self)
 
 
 class NoThread:
     "This is great for debugging purposes"
 
     def __init__(self, *args, **kwargs):
@@ -184,23 +185,27 @@
 
         self.signals_min.signal_add_threat.connect(self._append)
         self.signals_min.signal_stop_threat.connect(self._remove)
 
     def _append(self, thread: TaskThread):
         with self.lock:
             self.threads.append(thread)
-            logger.debug(f"Appended thread {thread}, Number of threads = {len(self.threads)}")
+            logger.debug(
+                f"Appended thread {thread.thread_name}, Number of threads = {len(self.threads)} {[thread.thread_name for thread in   self.threads]}"
+            )
             assert thread in self.threads
 
     def _remove(self, thread: TaskThread):
         with self.lock:
             if thread in self.threads:
                 self.threads.remove(thread)
                 thread.deleteLater()
-            logger.debug(f"Removed thread {thread}, Number of threads = {len(self.threads)}")
+            logger.debug(
+                f"Removed thread {thread.thread_name}, Number of threads = {len(self.threads)} {[thread.thread_name for thread in   self.threads]}"
+            )
 
     def stop_and_wait_all(self, timeout=10):
         # Wait for all threads to finish
         logger.warning(f"unfinished Threads {list(self.threads)}")
         for thread in list(self.threads):
             if thread.isRunning():
                 thread.stop()
```

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/tx.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/tx.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/tx_util.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/tx_util.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/util.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/util.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/bitcoin_safe/wallet.py` & `bitcoin_safe-0.6.0a1/bitcoin_safe/wallet.py`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/pyproject.toml` & `bitcoin_safe-0.6.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bitcoin_safe-0.6.0a0/PKG-INFO` & `bitcoin_safe-0.6.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoin-safe
-Version: 0.6.0a0
+Version: 0.6.0a1
 Summary: Long-term Bitcoin savings made Easy
 Home-page: https://github.com/andreasgriffin/bitcoin-safe
 License: GPL-3.0
 Author: andreasgriffin
 Author-email: andreasgriffin@proton.me
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -175,7 +175,30 @@
 
 # or use the internal faucet
 nigiri faucet bcrt1qgsnt3d4sny4w4zd5zl9x6jufc5rankqmgphyms9vz0ds73q4xfms655y4c 0.01
 ```
 
 * 
 
+
+
+
+## Installation from PyPi
+
+### Ubuntu, Debian, Windows
+
+- Install `poetry` and run `bitcoin_safe`
+  
+  ```sh
+  pip install bitcoin-safe
+  python -m bitcoin_safe
+  ```
+
+### Mac
+
+- Run `bitcoin_safe`
+  
+  ```sh
+  python3 -m pip install bitcoin-safe
+  python3 -m bitcoin_safe
+  ```
+
```

