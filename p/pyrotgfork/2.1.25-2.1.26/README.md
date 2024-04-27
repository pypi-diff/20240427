# Comparing `tmp/pyrotgfork-2.1.25.tar.gz` & `tmp/pyrotgfork-2.1.26.tar.gz`

## Comparing `pyrotgfork-2.1.25.tar` & `pyrotgfork-2.1.26.tar`

### file list

```diff
@@ -1,474 +1,503 @@
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/__init__.py
--rw-r--r--   0        0        0    46382 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/client.py
--rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/dispatcher.py
--rw-r--r--   0        0        0   208021 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/emoji.py
--rw-r--r--   0        0        0    16314 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/file_id.py
--rw-r--r--   0        0        0    28452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/filters.py
--rw-r--r--   0        0        0    61915 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/mime_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/py.typed
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/sync.py
--rw-r--r--   0        0        0    17420 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/utils.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/connection/__init__.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/connection/connection.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/connection/transport/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/crypto/__init__.py
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/crypto/aes.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/crypto/mtproto.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/crypto/prime.py
--rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/crypto/rsa.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/accent_color.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/auto_name.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/chat_action.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/chat_event_action.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/chat_member_status.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/chat_type.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/client_platform.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/message_entity_type.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/message_media_type.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/message_service_type.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/messages_filter.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/next_code_type.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/parse_mode.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/poll_type.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/profile_color.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/sent_code_type.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/enums/user_status.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/errors/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/errors/rpc_error.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/__init__.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/handler.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/message_handler.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/message_reaction_count_updated_handler.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/message_reaction_updated_handler.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/poll_handler.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/handlers/user_status_handler.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/__init__.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/advanced/save_file.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/check_password.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/connect.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/initialize.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/log_out.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/send_code.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/auth/terminate.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/__init__.py
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/send_game.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/bots/set_game_score.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/business/__init__.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/business/get_business_connection.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chat_topics/__init__.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chat_topics/close_forum_topic.py
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chat_topics/create_forum_topic.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chat_topics/delete_forum_topic.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chat_topics/edit_forum_topic.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chat_topics/get_forum_topic.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chat_topics/get_forum_topics.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chat_topics/hide_forum_topic.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chat_topics/reopen_forum_topic.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chat_topics/unhide_forum_topic.py
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/__init__.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/create_group.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/get_created_chats.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_ttl.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/chats/unpin_chat_message.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/contacts/import_contacts.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_message_reaction_count_updated.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_message_reaction_updated.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/decorators/on_user_status.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/invite_links/revoke_chat_invite_link.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/__init__.py
--rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/download_media.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/search_global.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_document.py
--rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_location.py
--rw-r--r--   0        0        0    22833 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_message.py
--rw-r--r--   0        0        0    12533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0        0        0    15141 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_video.py
--rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/set_reaction.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/messages/vote_poll.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/password/__init__.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/password/remove_cloud_password.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/stickers/get_stickers.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/__init__.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/block_user.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/get_me.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/get_users.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/set_birthdate.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/set_personal_chat.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/set_username.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/users/update_profile.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/utilities/compose.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/utilities/idle.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/utilities/restart.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/utilities/run.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/utilities/start.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/utilities/stop.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/parser/__init__.py
--rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/parser/html.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/parser/markdown.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/parser/parser.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/parser/utils.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/__init__.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/__init__.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/future_salt.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/future_salts.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/list.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/message.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/msg_container.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/tl_object.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/session/__init__.py
--rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/session/auth.py
--rw-r--r--   0        0        0    14294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/session/session.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/session/internals/__init__.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/session/internals/data_center.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/session/internals/msg_id.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/session/internals/seq_no.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/storage/__init__.py
--rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/storage/aio_sqlite_storage.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/storage/file_storage.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/storage/memory_storage.py
--rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/storage/storage.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/list.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/object.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/update.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/authorization/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/authorization/terms_of_service.py
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0        0        0    14613 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/web_app_info.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/business/__init__.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/business/business_connection.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/business/business_intro.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/business/business_location.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/business/business_opening_hours.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/business/business_opening_hours_interval.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/chat_topics/__init__.py
--rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/chat_topics/forum_topic.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/chat_topics/forum_topic_closed.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/chat_topics/forum_topic_created.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/chat_topics/forum_topic_edited.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/chat_topics/forum_topic_reopened.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/chat_topics/general_forum_topic_hidden.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/chat_topics/general_forum_topic_unhidden.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_voice.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_media/__init__.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_media/input_media.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_media/input_phone_contact.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_media/link_preview_options.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0        0        0    13513 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_message_content/external_reply_info.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/input_message_content/reply_parameters.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/message_origin/__init__.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/message_origin/message_import_info.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/message_origin/message_origin.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/message_origin/message_origin_channel.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/message_origin/message_origin_chat.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/message_origin/message_origin_hidden_user.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/message_origin/message_origin_user.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/chat_boost_added.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/gift_code.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/gifted_premium.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/giveaway.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/giveaway_completed.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/giveaway_winners.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0        0        0   190251 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/message_reaction_count_updated.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/message_reaction_updated.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/story.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/birthdate.py
--rw-r--r--   0        0        0    46491 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_color.py
--rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_shared.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0        0        0    18356 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/users_shared.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/video_chat_participants_invited.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/COPYING
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/COPYING.lesser
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/NOTICE
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/README.md
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/hatch_build.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/pyproject.toml
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 pyrotgfork-2.1.25/PKG-INFO
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/__init__.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/api/__init__.py
+-rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/api/compiler.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/api/source/auth_key.tl
+-rw-r--r--   0        0        0   207740 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/api/source/main_api.tl
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/api/source/sys_msgs.tl
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/api/template/combinator.txt
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/api/template/type.txt
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/__init__.py
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/compiler.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/sort.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0        0        0    34482 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/template/class.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/compiler/errors/template/sub_class.txt
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/__init__.py
+-rw-r--r--   0        0        0    46382 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/client.py
+-rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/dispatcher.py
+-rw-r--r--   0        0        0   208021 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/emoji.py
+-rw-r--r--   0        0        0    16314 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/file_id.py
+-rw-r--r--   0        0        0    28542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/filters.py
+-rw-r--r--   0        0        0    61915 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/mime_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/py.typed
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/sync.py
+-rw-r--r--   0        0        0    17454 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/utils.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/connection/__init__.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/connection/connection.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/connection/transport/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/crypto/__init__.py
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/crypto/aes.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/crypto/mtproto.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/crypto/prime.py
+-rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/crypto/rsa.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/accent_color.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/auto_name.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/chat_action.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/chat_type.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/client_platform.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/message_media_type.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/message_service_type.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/messages_filter.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/next_code_type.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/parse_mode.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/poll_type.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/profile_color.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/enums/user_status.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/errors/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/errors/rpc_error.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/__init__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/handler.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/message_handler.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/message_reaction_count_updated_handler.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/message_reaction_updated_handler.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/handlers/user_status_handler.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/__init__.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/advanced/save_file.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/connect.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/auth/terminate.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/get_bot_info_description.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/get_bot_info_short_description.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/get_bot_name.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/set_bot_info_description.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/set_bot_info_short_description.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/set_bot_name.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/bots/set_game_score.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/business/__init__.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/business/get_business_connection.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chat_topics/__init__.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chat_topics/close_forum_topic.py
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chat_topics/create_forum_topic.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chat_topics/delete_forum_topic.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chat_topics/edit_forum_topic.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chat_topics/get_forum_topic.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chat_topics/get_forum_topics.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chat_topics/hide_forum_topic.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chat_topics/reopen_forum_topic.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chat_topics/unhide_forum_topic.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/get_created_chats.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/search_chats.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_ttl.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/chats/unpin_chat_message.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/contacts/import_contacts.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_message_reaction_count_updated.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_message_reaction_updated.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/decorators/on_user_status.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/edit_cached_media.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0        0        0    22833 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0        0        0    12533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0        0        0    15141 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/set_reaction.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/messages/vote_poll.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/password/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/password/remove_cloud_password.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/stickers/get_stickers.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/__init__.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/block_user.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/get_me.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/get_users.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/set_birthdate.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/set_personal_chat.py
+-rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/set_username.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/users/update_profile.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/utilities/run.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/utilities/start.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/parser/__init__.py
+-rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/parser/html.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/parser/markdown.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/parser/parser.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/parser/utils.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/__init__.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/__init__.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/list.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/message.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/msg_container.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/tl_object.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/session/__init__.py
+-rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/session/auth.py
+-rw-r--r--   0        0        0    14294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/session/session.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/session/internals/__init__.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/session/internals/data_center.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/storage/__init__.py
+-rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/storage/aio_sqlite_storage.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/storage/file_storage.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/storage/memory_storage.py
+-rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/storage/storage.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/list.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/object.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/update.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/authorization/terms_of_service.py
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0        0        0    14613 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/web_app_info.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/business/__init__.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/business/business_connection.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/business/business_intro.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/business/business_location.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/business/business_opening_hours.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/business/business_opening_hours_interval.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/chat_topics/__init__.py
+-rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/chat_topics/forum_topic.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/chat_topics/forum_topic_closed.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/chat_topics/forum_topic_created.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/chat_topics/forum_topic_edited.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/chat_topics/forum_topic_reopened.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/chat_topics/general_forum_topic_hidden.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/chat_topics/general_forum_topic_unhidden.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_voice.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_media/input_phone_contact.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_media/link_preview_options.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0        0        0    13513 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_message_content/external_reply_info.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/input_message_content/reply_parameters.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/message_origin/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/message_origin/message_import_info.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/message_origin/message_origin.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/message_origin/message_origin_channel.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/message_origin/message_origin_chat.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/message_origin/message_origin_hidden_user.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/message_origin/message_origin_user.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/chat_boost_added.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/gift_code.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/gifted_premium.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/giveaway.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/giveaway_completed.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/giveaway_winners.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0        0        0   192723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/message_reaction_count_updated.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/message_reaction_updated.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/story.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/birthdate.py
+-rw-r--r--   0        0        0    46488 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_color.py
+-rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_shared.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0        0        0    18356 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/users_shared.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/video_chat_participants_invited.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/COPYING
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/COPYING.lesser
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/NOTICE
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/README.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/hatch_build.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/pyproject.toml
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 pyrotgfork-2.1.26/PKG-INFO
```

### Comparing `pyrotgfork-2.1.25/pyrogram/__init__.py` & `pyrotgfork-2.1.26/pyrogram/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "2.1.25"
+__version__ = "2.1.26"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `pyrotgfork-2.1.25/pyrogram/client.py` & `pyrotgfork-2.1.26/pyrogram/client.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/dispatcher.py` & `pyrotgfork-2.1.26/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/emoji.py` & `pyrotgfork-2.1.26/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/file_id.py` & `pyrotgfork-2.1.26/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/filters.py` & `pyrotgfork-2.1.26/pyrogram/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 
 
 # endregion
 
 
 # region forwarded_filter
 async def forwarded_filter(_, __, m: Message) -> bool:
-    return bool(m.forward_date)
+    return bool(m.forward_origin)
 
 
 forwarded = create(forwarded_filter)
 """Filter messages that are forwarded."""
 
 
 # endregion
@@ -813,16 +813,19 @@
 
 
 # endregion
 
 
 # region linked_channel_filter
 async def linked_channel_filter(_, __, m: Message) -> bool:
-    return bool(m.forward_from_chat and not m.from_user)
-
+    return bool(
+        m.forward_origin and
+        m.forward_origin.type == "channel" and
+        m.forward_origin.chat == m.sender_chat
+    )
 
 linked_channel: Filter = create(linked_channel_filter)
 """Filter messages that are automatically forwarded from the linked channel to the group chat."""
 
 
 # endregion
```

### Comparing `pyrotgfork-2.1.25/pyrogram/mime_types.py` & `pyrotgfork-2.1.26/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/sync.py` & `pyrotgfork-2.1.26/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/utils.py` & `pyrotgfork-2.1.26/pyrogram/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,17 +502,17 @@
             quote,
             quote_parse_mode,
             quote_entities
         )).values()
         reply_to.quote_text = message
         reply_to.quote_entities = entities
     if reply_parameters.chat_id:
-        reply_to.reply_to_peer_id = await client.resolve_peer(chat_id)
+        reply_to.reply_to_peer_id = await client.resolve_peer(reply_parameters.chat_id)
     if reply_parameters.quote_position:
-        reply_to.quote_offset = quote_position
+        reply_to.quote_offset = reply_parameters.quote_position
     return reply_to
 
 
 def is_plain_domain(url):
     # https://github.com/tdlib/td/blob/d963044/td/telegram/MessageEntity.cpp#L1778
     return (
         url.find('/') >= len(url) and
```

### Comparing `pyrotgfork-2.1.25/pyrogram/connection/__init__.py` & `pyrotgfork-2.1.26/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/connection/connection.py` & `pyrotgfork-2.1.26/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/connection/transport/__init__.py` & `pyrotgfork-2.1.26/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/__init__.py` & `pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/tcp.py` & `pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/tcp_abridged.py` & `pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/tcp_full.py` & `pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `pyrotgfork-2.1.26/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/crypto/__init__.py` & `pyrotgfork-2.1.26/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/crypto/aes.py` & `pyrotgfork-2.1.26/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/crypto/mtproto.py` & `pyrotgfork-2.1.26/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/crypto/prime.py` & `pyrotgfork-2.1.26/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/crypto/rsa.py` & `pyrotgfork-2.1.26/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/__init__.py` & `pyrotgfork-2.1.26/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/accent_color.py` & `pyrotgfork-2.1.26/pyrogram/enums/accent_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/auto_name.py` & `pyrotgfork-2.1.26/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/chat_action.py` & `pyrotgfork-2.1.26/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/chat_event_action.py` & `pyrotgfork-2.1.26/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/chat_member_status.py` & `pyrotgfork-2.1.26/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/chat_members_filter.py` & `pyrotgfork-2.1.26/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/chat_type.py` & `pyrotgfork-2.1.26/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/client_platform.py` & `pyrotgfork-2.1.26/pyrogram/enums/client_platform.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/message_entity_type.py` & `pyrotgfork-2.1.26/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/message_media_type.py` & `pyrotgfork-2.1.26/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/message_service_type.py` & `pyrotgfork-2.1.26/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/messages_filter.py` & `pyrotgfork-2.1.26/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/next_code_type.py` & `pyrotgfork-2.1.26/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/parse_mode.py` & `pyrotgfork-2.1.26/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/poll_type.py` & `pyrotgfork-2.1.26/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/profile_color.py` & `pyrotgfork-2.1.26/pyrogram/enums/profile_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/sent_code_type.py` & `pyrotgfork-2.1.26/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/enums/user_status.py` & `pyrotgfork-2.1.26/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/errors/__init__.py` & `pyrotgfork-2.1.26/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/errors/rpc_error.py` & `pyrotgfork-2.1.26/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/__init__.py` & `pyrotgfork-2.1.26/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/callback_query_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/chat_join_request_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/chat_member_updated_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/chosen_inline_result_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/deleted_messages_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/disconnect_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/edited_message_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/inline_query_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/message_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/message_reaction_count_updated_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/message_reaction_count_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/message_reaction_updated_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/message_reaction_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/poll_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/raw_update_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/handlers/user_status_handler.py` & `pyrotgfork-2.1.26/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/advanced/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/advanced/invoke.py` & `pyrotgfork-2.1.26/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/advanced/resolve_peer.py` & `pyrotgfork-2.1.26/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/advanced/save_file.py` & `pyrotgfork-2.1.26/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/accept_terms_of_service.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/check_password.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/connect.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/disconnect.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/get_password_hint.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/initialize.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/log_out.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/recover_password.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/resend_code.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/send_code.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/send_recovery_code.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/sign_in.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/sign_in_bot.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/sign_up.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/auth/terminate.py` & `pyrotgfork-2.1.26/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/answer_callback_query.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/answer_inline_query.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/answer_web_app_query.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/delete_bot_commands.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/get_bot_commands.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/get_bot_default_privileges.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/get_chat_menu_button.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/get_game_high_scores.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/get_inline_bot_results.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/request_callback_answer.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/send_game.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/send_inline_bot_result.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/set_bot_commands.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/set_bot_default_privileges.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/set_chat_menu_button.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/bots/set_game_score.py` & `pyrotgfork-2.1.26/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/business/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/business/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/business/get_business_connection.py` & `pyrotgfork-2.1.26/pyrogram/methods/business/get_business_connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chat_topics/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/chat_topics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chat_topics/close_forum_topic.py` & `pyrotgfork-2.1.26/pyrogram/methods/chat_topics/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chat_topics/create_forum_topic.py` & `pyrotgfork-2.1.26/pyrogram/methods/chat_topics/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chat_topics/delete_forum_topic.py` & `pyrotgfork-2.1.26/pyrogram/methods/chat_topics/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chat_topics/edit_forum_topic.py` & `pyrotgfork-2.1.26/pyrogram/methods/chat_topics/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chat_topics/get_forum_topic.py` & `pyrotgfork-2.1.26/pyrogram/methods/chat_topics/get_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py` & `pyrotgfork-2.1.26/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chat_topics/get_forum_topics.py` & `pyrotgfork-2.1.26/pyrogram/methods/chat_topics/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chat_topics/hide_forum_topic.py` & `pyrotgfork-2.1.26/pyrogram/methods/chat_topics/hide_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chat_topics/reopen_forum_topic.py` & `pyrotgfork-2.1.26/pyrogram/methods/chat_topics/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chat_topics/unhide_forum_topic.py` & `pyrotgfork-2.1.26/pyrogram/methods/chat_topics/unhide_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from .get_send_as_chats import GetSendAsChats
 from .join_chat import JoinChat
 from .leave_chat import LeaveChat
 from .mark_chat_unread import MarkChatUnread
 from .pin_chat_message import PinChatMessage
 from .promote_chat_member import PromoteChatMember
 from .restrict_chat_member import RestrictChatMember
+from .search_chats import SearchChats
 from .set_administrator_title import SetAdministratorTitle
 from .set_chat_description import SetChatDescription
 from .set_chat_permissions import SetChatPermissions
 from .set_chat_photo import SetChatPhoto
 from .set_chat_protected_content import SetChatProtectedContent
 from .set_chat_title import SetChatTitle
 from .set_chat_ttl import SetChatTTL
@@ -62,14 +63,15 @@
 class Chats(
     GetChat,
     LeaveChat,
     JoinChat,
     BanChatMember,
     UnbanChatMember,
     RestrictChatMember,
+    SearchChats,
     PromoteChatMember,
     GetChatMembers,
     GetChatMember,
     SetChatPhoto,
     DeleteChatPhoto,
     SetChatTitle,
     SetChatDescription,
```

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/add_chat_members.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/archive_chats.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/ban_chat_member.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/create_channel.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/create_group.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/create_supergroup.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/delete_channel.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/delete_chat_photo.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/delete_supergroup.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/delete_user_history.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/get_chat.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/get_chat_event_log.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/get_chat_member.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/get_chat_members.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/get_chat_members_count.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/get_chat_online_count.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/get_created_chats.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/get_created_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/get_dialogs.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/get_dialogs_count.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/get_nearby_chats.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/get_send_as_chats.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/join_chat.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/leave_chat.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/mark_chat_unread.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/pin_chat_message.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/promote_chat_member.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/restrict_chat_member.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/set_administrator_title.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_description.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_permissions.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_photo.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_protected_content.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_title.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_ttl.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_ttl.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/set_chat_username.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/set_send_as_chat.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/set_slow_mode.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/unarchive_chats.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/unban_chat_member.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/unpin_all_chat_messages.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/chats/unpin_chat_message.py` & `pyrotgfork-2.1.26/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/contacts/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/contacts/add_contact.py` & `pyrotgfork-2.1.26/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/contacts/delete_contacts.py` & `pyrotgfork-2.1.26/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/contacts/get_contacts.py` & `pyrotgfork-2.1.26/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/contacts/get_contacts_count.py` & `pyrotgfork-2.1.26/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/contacts/import_contacts.py` & `pyrotgfork-2.1.26/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_callback_query.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_chat_join_request.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_chat_member_updated.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_chosen_inline_result.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_deleted_messages.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_disconnect.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_edited_message.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_inline_query.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_message.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_message_reaction_count_updated.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_message_reaction_updated.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_poll.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_raw_update.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/decorators/on_user_status.py` & `pyrotgfork-2.1.26/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/approve_chat_join_request.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/create_chat_invite_link.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/decline_chat_join_request.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/export_chat_invite_link.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_invite_link.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/get_chat_join_requests.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `pyrotgfork-2.1.26/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from .copy_media_group import CopyMediaGroup
 from .copy_message import CopyMessage
 from .delete_messages import DeleteMessages
 from .download_media import DownloadMedia
+from .edit_cached_media import EditCachedMedia
 from .edit_inline_caption import EditInlineCaption
 from .edit_inline_media import EditInlineMedia
 from .edit_inline_reply_markup import EditInlineReplyMarkup
 from .edit_inline_text import EditInlineText
 from .edit_message_caption import EditMessageCaption
 from .edit_message_media import EditMessageMedia
 from .edit_message_reply_markup import EditMessageReplyMarkup
@@ -69,14 +70,15 @@
 
 
 class Messages(
     CopyMediaGroup,
     CopyMessage,
     DeleteMessages,
     DownloadMedia,
+    EditCachedMedia,
     EditInlineCaption,
     EditInlineMedia,
     EditInlineReplyMarkup,
     EditInlineText,
     EditMessageCaption,
     EditMessageMedia,
     EditMessageReplyMarkup,
```

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/copy_media_group.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/copy_message.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/delete_messages.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/download_media.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/edit_inline_caption.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/edit_inline_media.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/edit_inline_media.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             actual_media = raw.types.InputMediaPhoto(
                 id=raw.types.InputPhoto(
                     id=uploaded_media.photo.id,
                     access_hash=uploaded_media.photo.access_hash,
                     file_reference=uploaded_media.photo.file_reference
                 ),
                 spoiler=getattr(media, "has_spoiler", None)
-            ) if isinstance(media, types.InputMediaPhoto) else raw.types.InputMediaDocument(
+            ) if isinstance(uploaded_media, raw.types.MessageMediaPhoto) else raw.types.InputMediaDocument(
                 id=raw.types.InputDocument(
                     id=uploaded_media.document.id,
                     access_hash=uploaded_media.document.access_hash,
                     file_reference=uploaded_media.document.file_reference
                 ),
                 spoiler=getattr(media, "has_spoiler", None)
             )
```

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/edit_inline_reply_markup.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/edit_inline_text.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/edit_message_caption.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/edit_message_media.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/edit_message_reply_markup.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/edit_message_text.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/forward_messages.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/get_chat_history.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/get_chat_history_count.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/get_discussion_message.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/get_discussion_replies.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/get_discussion_replies_count.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/get_media_group.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/get_messages.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/inline_session.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/read_chat_history.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/retract_vote.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/search_global.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/search_global_count.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/search_messages.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/search_messages_count.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_animation.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_audio.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_cached_media.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_chat_action.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_contact.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_dice.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_document.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_location.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_media_group.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_message.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_photo.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_poll.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_poll.py`

 * *Files 8% similar despite different names*

```diff
@@ -162,24 +162,45 @@
         )).values()
 
         reply_to = await utils._get_reply_message_parameters(
             self,
             message_thread_id,
             reply_parameters
         )
+
+        # TODO: wait for BOT API update?
+        question, question_entities = (await utils.parse_text_entities(self, question, None, None)).values()
+        if not question_entities:
+            question_entities = []
+
+        answers = []
+        for i, answer_ in enumerate(options):
+            answer, answer_entities = (await utils.parse_text_entities(self, answer_, None, None)).values()
+            if not answer_entities:
+                answer_entities = []
+            answers.append(
+                raw.types.PollAnswer(
+                    text=raw.types.TextWithEntities(
+                        text=answer,
+                        entities=answer_entities
+                    ),
+                    option=bytes([i])
+                )
+            )
+
         rpc = raw.functions.messages.SendMedia(
             peer=await self.resolve_peer(chat_id),
             media=raw.types.InputMediaPoll(
                 poll=raw.types.Poll(
                     id=self.rnd_id(),
-                    question=question,
-                    answers=[
-                        raw.types.PollAnswer(text=text, option=bytes([i]))
-                        for i, text in enumerate(options)
-                    ],
+                    question=raw.types.TextWithEntities(
+                        text=question,
+                        entities=question_entities
+                    ),
+                    answers=answers,
                     closed=is_closed,
                     public_voters=not is_anonymous,
                     multiple_choice=allows_multiple_answers,
                     quiz=type == enums.PollType.QUIZ or False,
                     close_period=open_period,
                     close_date=utils.datetime_to_timestamp(close_date)
                 ),
```

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_sticker.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_venue.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_video.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_video_note.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/send_voice.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/set_reaction.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/set_reaction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/stop_poll.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/stream_media.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/messages/vote_poll.py` & `pyrotgfork-2.1.26/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/password/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/password/change_cloud_password.py` & `pyrotgfork-2.1.26/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/password/enable_cloud_password.py` & `pyrotgfork-2.1.26/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/password/remove_cloud_password.py` & `pyrotgfork-2.1.26/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/stickers/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/stickers/get_stickers.py` & `pyrotgfork-2.1.26/pyrogram/methods/stickers/get_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/block_user.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/delete_profile_photos.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/get_chat_photos.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/get_chat_photos_count.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/get_common_chats.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/get_default_emoji_statuses.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/get_me.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/get_users.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/set_birthdate.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/set_birthdate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/set_emoji_status.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/set_personal_chat.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/set_personal_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/set_profile_photo.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/set_profile_photo.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 
         The ``photo`` and ``video`` arguments are mutually exclusive.
         Pass either one as named argument (see examples below).
 
         .. note::
 
             This method only works for Users.
-            Bots profile photos must be set using BotFather.
 
         .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             photo (``str`` | ``BinaryIO``, *optional*):
                 Profile photo to set.
                 Pass a file path as string to upload a new photo that exists on your local machine or
```

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/set_username.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/unblock_user.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/users/update_profile.py` & `pyrotgfork-2.1.26/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/utilities/__init__.py` & `pyrotgfork-2.1.26/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/utilities/add_handler.py` & `pyrotgfork-2.1.26/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/utilities/compose.py` & `pyrotgfork-2.1.26/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/utilities/export_session_string.py` & `pyrotgfork-2.1.26/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/utilities/idle.py` & `pyrotgfork-2.1.26/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/utilities/remove_handler.py` & `pyrotgfork-2.1.26/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/utilities/restart.py` & `pyrotgfork-2.1.26/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/utilities/run.py` & `pyrotgfork-2.1.26/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/utilities/start.py` & `pyrotgfork-2.1.26/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/utilities/stop.py` & `pyrotgfork-2.1.26/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/methods/utilities/stop_transmission.py` & `pyrotgfork-2.1.26/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/parser/__init__.py` & `pyrotgfork-2.1.26/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/parser/html.py` & `pyrotgfork-2.1.26/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/parser/markdown.py` & `pyrotgfork-2.1.26/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/parser/parser.py` & `pyrotgfork-2.1.26/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/parser/utils.py` & `pyrotgfork-2.1.26/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/__init__.py` & `pyrotgfork-2.1.26/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/__init__.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/future_salt.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/future_salts.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/gzip_packed.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/list.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/message.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/msg_container.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/tl_object.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/primitives/__init__.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/primitives/bool.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/primitives/bytes.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/primitives/double.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/primitives/int.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/primitives/string.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/raw/core/primitives/vector.py` & `pyrotgfork-2.1.26/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/session/__init__.py` & `pyrotgfork-2.1.26/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/session/auth.py` & `pyrotgfork-2.1.26/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/session/session.py` & `pyrotgfork-2.1.26/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/session/internals/__init__.py` & `pyrotgfork-2.1.26/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/session/internals/data_center.py` & `pyrotgfork-2.1.26/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/session/internals/msg_factory.py` & `pyrotgfork-2.1.26/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/session/internals/msg_id.py` & `pyrotgfork-2.1.26/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/session/internals/seq_no.py` & `pyrotgfork-2.1.26/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/storage/__init__.py` & `pyrotgfork-2.1.26/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/storage/aio_sqlite_storage.py` & `pyrotgfork-2.1.26/pyrogram/storage/aio_sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/storage/file_storage.py` & `pyrotgfork-2.1.26/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/storage/memory_storage.py` & `pyrotgfork-2.1.26/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/storage/sqlite_storage.py` & `pyrotgfork-2.1.26/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/storage/storage.py` & `pyrotgfork-2.1.26/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/__init__.py` & `pyrotgfork-2.1.26/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/list.py` & `pyrotgfork-2.1.26/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/object.py` & `pyrotgfork-2.1.26/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/update.py` & `pyrotgfork-2.1.26/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/authorization/__init__.py` & `pyrotgfork-2.1.26/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/authorization/sent_code.py` & `pyrotgfork-2.1.26/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/authorization/terms_of_service.py` & `pyrotgfork-2.1.26/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/__init__.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/callback_game.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/callback_query.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/force_reply.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/game_high_score.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/login_url.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/menu_button.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/bots_and_keyboards/web_app_info.py` & `pyrotgfork-2.1.26/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/business/__init__.py` & `pyrotgfork-2.1.26/pyrogram/types/business/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/business/business_connection.py` & `pyrotgfork-2.1.26/pyrogram/types/business/business_connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/business/business_intro.py` & `pyrotgfork-2.1.26/pyrogram/types/business/business_intro.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/business/business_location.py` & `pyrotgfork-2.1.26/pyrogram/types/business/business_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/business/business_opening_hours.py` & `pyrotgfork-2.1.26/pyrogram/types/business/business_opening_hours.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/business/business_opening_hours_interval.py` & `pyrotgfork-2.1.26/pyrogram/types/business/business_opening_hours_interval.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/chat_topics/__init__.py` & `pyrotgfork-2.1.26/pyrogram/types/chat_topics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/chat_topics/forum_topic.py` & `pyrotgfork-2.1.26/pyrogram/types/chat_topics/forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/chat_topics/forum_topic_closed.py` & `pyrotgfork-2.1.26/pyrogram/types/chat_topics/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/chat_topics/forum_topic_created.py` & `pyrotgfork-2.1.26/pyrogram/types/chat_topics/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/chat_topics/forum_topic_edited.py` & `pyrotgfork-2.1.26/pyrogram/types/chat_topics/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/chat_topics/forum_topic_reopened.py` & `pyrotgfork-2.1.26/pyrogram/types/chat_topics/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/chat_topics/general_forum_topic_hidden.py` & `pyrotgfork-2.1.26/pyrogram/types/chat_topics/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/chat_topics/general_forum_topic_unhidden.py` & `pyrotgfork-2.1.26/pyrogram/types/chat_topics/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/__init__.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/chosen_inline_result.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_animation.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_article.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_audio.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_contact.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_document.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_location.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_photo.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_venue.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_video.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/inline_mode/inline_query_result_voice.py` & `pyrotgfork-2.1.26/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_media/__init__.py` & `pyrotgfork-2.1.26/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_media/input_media.py` & `pyrotgfork-2.1.26/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_media/input_media_animation.py` & `pyrotgfork-2.1.26/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_media/input_media_audio.py` & `pyrotgfork-2.1.26/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_media/input_media_document.py` & `pyrotgfork-2.1.26/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_media/input_media_photo.py` & `pyrotgfork-2.1.26/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_media/input_media_video.py` & `pyrotgfork-2.1.26/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_media/input_phone_contact.py` & `pyrotgfork-2.1.26/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_media/link_preview_options.py` & `pyrotgfork-2.1.26/pyrogram/types/input_media/link_preview_options.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_message_content/__init__.py` & `pyrotgfork-2.1.26/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_message_content/external_reply_info.py` & `pyrotgfork-2.1.26/pyrogram/types/input_message_content/external_reply_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_message_content/input_message_content.py` & `pyrotgfork-2.1.26/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_message_content/input_text_message_content.py` & `pyrotgfork-2.1.26/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/input_message_content/reply_parameters.py` & `pyrotgfork-2.1.26/pyrogram/types/input_message_content/reply_parameters.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/message_origin/__init__.py` & `pyrotgfork-2.1.26/pyrogram/types/message_origin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/message_origin/message_import_info.py` & `pyrotgfork-2.1.26/pyrogram/types/message_origin/message_import_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/message_origin/message_origin.py` & `pyrotgfork-2.1.26/pyrogram/types/message_origin/message_origin.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/message_origin/message_origin_channel.py` & `pyrotgfork-2.1.26/pyrogram/types/message_origin/message_origin_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/message_origin/message_origin_chat.py` & `pyrotgfork-2.1.26/pyrogram/types/message_origin/message_origin_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/message_origin/message_origin_hidden_user.py` & `pyrotgfork-2.1.26/pyrogram/types/message_origin/message_origin_hidden_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/message_origin/message_origin_user.py` & `pyrotgfork-2.1.26/pyrogram/types/message_origin/message_origin_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/__init__.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/animation.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/audio.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/chat_boost_added.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/chat_boost_added.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/contact.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/dice.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/document.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/game.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/gift_code.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/gift_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/gifted_premium.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/gifted_premium.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/giveaway.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/giveaway.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/giveaway_completed.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/giveaway_completed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/giveaway_winners.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/giveaway_winners.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/location.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/message.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -9740,2152 +9740,2307 @@
 000260b0: 6368 6174 5f69 643d 7365 6c66 2e63 6861  chat_id=self.cha
 000260c0: 742e 6964 2c0a 2020 2020 2020 2020 2020  t.id,.          
 000260d0: 2020 6d65 7373 6167 655f 6964 3d73 656c    message_id=sel
 000260e0: 662e 6964 2c0a 2020 2020 2020 2020 2020  f.id,.          
 000260f0: 2020 7265 706c 795f 6d61 726b 7570 3d72    reply_markup=r
 00026100: 6570 6c79 5f6d 6172 6b75 700a 2020 2020  eply_markup.    
 00026110: 2020 2020 290a 0a20 2020 2061 7379 6e63      )..    async
-00026120: 2064 6566 2066 6f72 7761 7264 280a 2020   def forward(.  
-00026130: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00026140: 2020 2020 6368 6174 5f69 643a 2055 6e69      chat_id: Uni
-00026150: 6f6e 5b69 6e74 2c20 7374 725d 2c0a 2020  on[int, str],.  
-00026160: 2020 2020 2020 6d65 7373 6167 655f 7468        message_th
-00026170: 7265 6164 5f69 643a 2069 6e74 203d 204e  read_id: int = N
-00026180: 6f6e 652c 0a20 2020 2020 2020 2064 6973  one,.        dis
-00026190: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-000261a0: 6e3a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  n: bool = None,.
-000261b0: 2020 2020 2020 2020 7072 6f74 6563 745f          protect_
-000261c0: 636f 6e74 656e 743a 2062 6f6f 6c20 3d20  content: bool = 
-000261d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6472  None,.        dr
-000261e0: 6f70 5f61 7574 686f 723a 2062 6f6f 6c20  op_author: bool 
-000261f0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00026200: 6472 6f70 5f6d 6564 6961 5f63 6170 7469  drop_media_capti
-00026210: 6f6e 733a 2062 6f6f 6c20 3d20 4e6f 6e65  ons: bool = None
-00026220: 2c0a 2020 2020 2020 2020 7363 6865 6475  ,.        schedu
-00026230: 6c65 5f64 6174 653a 2064 6174 6574 696d  le_date: datetim
-00026240: 6520 3d20 4e6f 6e65 0a20 2020 2029 202d  e = None.    ) -
-00026250: 3e20 556e 696f 6e5b 2274 7970 6573 2e4d  > Union["types.M
-00026260: 6573 7361 6765 222c 204c 6973 745b 2274  essage", List["t
-00026270: 7970 6573 2e4d 6573 7361 6765 225d 5d3a  ypes.Message"]]:
-00026280: 0a20 2020 2020 2020 2022 2222 426f 756e  .        """Boun
-00026290: 6420 6d65 7468 6f64 202a 666f 7277 6172  d method *forwar
-000262a0: 642a 206f 6620 3a6f 626a 3a60 7e70 7972  d* of :obj:`~pyr
-000262b0: 6f67 7261 6d2e 7479 7065 732e 4d65 7373  ogram.types.Mess
-000262c0: 6167 6560 2e0a 0a20 2020 2020 2020 2055  age`...        U
-000262d0: 7365 2061 7320 6120 7368 6f72 7463 7574  se as a shortcut
-000262e0: 2066 6f72 3a0a 0a20 2020 2020 2020 202e   for:..        .
-000262f0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
-00026300: 7974 686f 6e0a 0a20 2020 2020 2020 2020  ython..         
-00026310: 2020 2061 7761 6974 2063 6c69 656e 742e     await client.
-00026320: 666f 7277 6172 645f 6d65 7373 6167 6573  forward_messages
-00026330: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00026340: 2020 6368 6174 5f69 643d 6368 6174 5f69    chat_id=chat_i
-00026350: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00026360: 2020 2066 726f 6d5f 6368 6174 5f69 643d     from_chat_id=
-00026370: 6d65 7373 6167 652e 6368 6174 2e69 642c  message.chat.id,
-00026380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026390: 206d 6573 7361 6765 5f69 6473 3d6d 6573   message_ids=mes
-000263a0: 7361 6765 2e69 640a 2020 2020 2020 2020  sage.id.        
-000263b0: 2020 2020 290a 0a20 2020 2020 2020 2045      )..        E
-000263c0: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
-000263d0: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
-000263e0: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
-000263f0: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00026400: 7420 6d65 7373 6167 652e 666f 7277 6172  t message.forwar
-00026410: 6428 6368 6174 5f69 6429 0a0a 2020 2020  d(chat_id)..    
-00026420: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
-00026430: 2020 2020 2020 2020 2020 2020 6368 6174              chat
-00026440: 5f69 6420 2860 6069 6e74 6060 207c 2060  _id (``int`` | `
-00026450: 6073 7472 6060 293a 0a20 2020 2020 2020  `str``):.       
-00026460: 2020 2020 2020 2020 2055 6e69 7175 6520           Unique 
-00026470: 6964 656e 7469 6669 6572 2028 696e 7429  identifier (int)
-00026480: 206f 7220 7573 6572 6e61 6d65 2028 7374   or username (st
-00026490: 7229 206f 6620 7468 6520 7461 7267 6574  r) of the target
-000264a0: 2063 6861 742e 0a20 2020 2020 2020 2020   chat..         
-000264b0: 2020 2020 2020 2046 6f72 2079 6f75 7220         For your 
-000264c0: 7065 7273 6f6e 616c 2063 6c6f 7564 2028  personal cloud (
-000264d0: 5361 7665 6420 4d65 7373 6167 6573 2920  Saved Messages) 
-000264e0: 796f 7520 6361 6e20 7369 6d70 6c79 2075  you can simply u
-000264f0: 7365 2022 6d65 2220 6f72 2022 7365 6c66  se "me" or "self
-00026500: 222e 0a20 2020 2020 2020 2020 2020 2020  "..             
-00026510: 2020 2046 6f72 2061 2063 6f6e 7461 6374     For a contact
-00026520: 2074 6861 7420 6578 6973 7473 2069 6e20   that exists in 
-00026530: 796f 7572 2054 656c 6567 7261 6d20 6164  your Telegram ad
-00026540: 6472 6573 7320 626f 6f6b 2079 6f75 2063  dress book you c
-00026550: 616e 2075 7365 2068 6973 2070 686f 6e65  an use his phone
-00026560: 206e 756d 6265 7220 2873 7472 292e 0a0a   number (str)...
-00026570: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00026580: 6167 655f 7468 7265 6164 5f69 6420 2860  age_thread_id (`
-00026590: 6069 6e74 6060 2c20 2a6f 7074 696f 6e61  `int``, *optiona
-000265a0: 6c2a 293a 0a20 2020 2020 2020 2020 2020  l*):.           
-000265b0: 2020 2020 2055 6e69 7175 6520 6964 656e       Unique iden
-000265c0: 7469 6669 6572 2066 6f72 2074 6865 2074  tifier for the t
-000265d0: 6172 6765 7420 6d65 7373 6167 6520 7468  arget message th
-000265e0: 7265 6164 2028 746f 7069 6329 206f 6620  read (topic) of 
-000265f0: 7468 6520 666f 7275 6d3b 2066 6f72 2066  the forum; for f
-00026600: 6f72 756d 2073 7570 6572 6772 6f75 7073  orum supergroups
-00026610: 206f 6e6c 790a 0a20 2020 2020 2020 2020   only..         
-00026620: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
-00026630: 6963 6174 696f 6e20 2860 6062 6f6f 6c60  ication (``bool`
-00026640: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
+00026120: 2064 6566 2065 6469 745f 6361 6368 6564   def edit_cached
+00026130: 5f6d 6564 6961 280a 2020 2020 2020 2020  _media(.        
+00026140: 6669 6c65 5f69 643a 2073 7472 2c0a 2020  file_id: str,.  
+00026150: 2020 2020 2020 6361 7074 696f 6e3a 2073        caption: s
+00026160: 7472 203d 2022 222c 0a20 2020 2020 2020  tr = "",.       
+00026170: 2070 6172 7365 5f6d 6f64 653a 204f 7074   parse_mode: Opt
+00026180: 696f 6e61 6c5b 2265 6e75 6d73 2e50 6172  ional["enums.Par
+00026190: 7365 4d6f 6465 225d 203d 204e 6f6e 652c  seMode"] = None,
+000261a0: 0a20 2020 2020 2020 2063 6170 7469 6f6e  .        caption
+000261b0: 5f65 6e74 6974 6965 733a 204c 6973 745b  _entities: List[
+000261c0: 2274 7970 6573 2e4d 6573 7361 6765 456e  "types.MessageEn
+000261d0: 7469 7479 225d 203d 204e 6f6e 652c 0a20  tity"] = None,. 
+000261e0: 2020 2020 2020 2073 6368 6564 756c 655f         schedule_
+000261f0: 6461 7465 3a20 6461 7465 7469 6d65 203d  date: datetime =
+00026200: 204e 6f6e 652c 0a20 2020 2020 2020 2068   None,.        h
+00026210: 6173 5f73 706f 696c 6572 3a20 626f 6f6c  as_spoiler: bool
+00026220: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00026230: 2072 6570 6c79 5f6d 6172 6b75 703a 2022   reply_markup: "
+00026240: 7479 7065 732e 496e 6c69 6e65 4b65 7962  types.InlineKeyb
+00026250: 6f61 7264 4d61 726b 7570 2220 3d20 4e6f  oardMarkup" = No
+00026260: 6e65 0a20 2020 2029 202d 3e20 224d 6573  ne.    ) -> "Mes
+00026270: 7361 6765 223a 0a20 2020 2020 2020 2022  sage":.        "
+00026280: 2222 4564 6974 2061 206d 6564 6961 2073  ""Edit a media s
+00026290: 746f 7265 6420 6f6e 2074 6865 2054 656c  tored on the Tel
+000262a0: 6567 7261 6d20 7365 7276 6572 7320 7573  egram servers us
+000262b0: 696e 6720 6120 6669 6c65 5f69 642e 0a0a  ing a file_id...
+000262c0: 2020 2020 2020 2020 5468 6973 2063 6f6e          This con
+000262d0: 7665 6e69 656e 6365 206d 6574 686f 6420  venience method 
+000262e0: 776f 726b 7320 7769 7468 2061 6e79 2076  works with any v
+000262f0: 616c 6964 2066 696c 655f 6964 206f 6e6c  alid file_id onl
+00026300: 792e 0a20 2020 2020 2020 2049 7420 646f  y..        It do
+00026310: 6573 2074 6865 2073 616d 6520 6173 2063  es the same as c
+00026320: 616c 6c69 6e67 2074 6865 2072 656c 6576  alling the relev
+00026330: 616e 7420 6d65 7468 6f64 2066 6f72 2065  ant method for e
+00026340: 6469 7469 6e67 206d 6564 6961 2075 7369  diting media usi
+00026350: 6e67 2061 2066 696c 655f 6964 2c20 7468  ng a file_id, th
+00026360: 7573 2073 6176 696e 6720 796f 7520 6672  us saving you fr
+00026370: 6f6d 2074 6865 0a20 2020 2020 2020 2068  om the.        h
+00026380: 6173 736c 6520 6f66 2075 7369 6e67 2074  assle of using t
+00026390: 6865 2063 6f72 7265 6374 203a 6f62 6a3a  he correct :obj:
+000263a0: 607e 7079 726f 6772 616d 2e74 7970 6573  `~pyrogram.types
+000263b0: 2e49 6e70 7574 4d65 6469 6160 2066 6f72  .InputMedia` for
+000263c0: 2074 6865 206d 6564 6961 2074 6865 2066   the media the f
+000263d0: 696c 655f 6964 2069 7320 706f 696e 7469  ile_id is pointi
+000263e0: 6e67 2074 6f2e 0a0a 2020 2020 2020 2020  ng to...        
+000263f0: 2e2e 2069 6e63 6c75 6465 3a3a 202f 5f69  .. include:: /_i
+00026400: 6e63 6c75 6465 732f 7573 6162 6c65 2d62  ncludes/usable-b
+00026410: 792f 7573 6572 732d 626f 7473 2e72 7374  y/users-bots.rst
+00026420: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00026430: 7465 7273 3a0a 2020 2020 2020 2020 2020  ters:.          
+00026440: 2020 6669 6c65 5f69 6420 2860 6073 7472    file_id (``str
+00026450: 6060 293a 0a20 2020 2020 2020 2020 2020  ``):.           
+00026460: 2020 2020 204d 6564 6961 2074 6f20 7365       Media to se
+00026470: 6e64 2e0a 2020 2020 2020 2020 2020 2020  nd..            
+00026480: 2020 2020 5061 7373 2061 2066 696c 655f      Pass a file_
+00026490: 6964 2061 7320 7374 7269 6e67 2074 6f20  id as string to 
+000264a0: 7365 6e64 2061 206d 6564 6961 2074 6861  send a media tha
+000264b0: 7420 6578 6973 7473 206f 6e20 7468 6520  t exists on the 
+000264c0: 5465 6c65 6772 616d 2073 6572 7665 7273  Telegram servers
+000264d0: 2e0a 0a20 2020 2020 2020 2020 2020 2063  ...            c
+000264e0: 6170 7469 6f6e 2028 6060 7374 7260 602c  aption (``str``,
+000264f0: 202a 6f70 7469 6f6e 616c 2a29 3a0a 2020   *optional*):.  
+00026500: 2020 2020 2020 2020 2020 2020 2020 4d65                Me
+00026510: 6469 6120 6361 7074 696f 6e2c 2030 2d31  dia caption, 0-1
+00026520: 3032 3420 6368 6172 6163 7465 7273 2e0a  024 characters..
+00026530: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+00026540: 7365 5f6d 6f64 6520 283a 6f62 6a3a 607e  se_mode (:obj:`~
+00026550: 7079 726f 6772 616d 2e65 6e75 6d73 2e50  pyrogram.enums.P
+00026560: 6172 7365 4d6f 6465 602c 202a 6f70 7469  arseMode`, *opti
+00026570: 6f6e 616c 2a29 3a0a 2020 2020 2020 2020  onal*):.        
+00026580: 2020 2020 2020 2020 4279 2064 6566 6175          By defau
+00026590: 6c74 2c20 7465 7874 7320 6172 6520 7061  lt, texts are pa
+000265a0: 7273 6564 2075 7369 6e67 2062 6f74 6820  rsed using both 
+000265b0: 4d61 726b 646f 776e 2061 6e64 2048 544d  Markdown and HTM
+000265c0: 4c20 7374 796c 6573 2e0a 2020 2020 2020  L styles..      
+000265d0: 2020 2020 2020 2020 2020 596f 7520 6361            You ca
+000265e0: 6e20 636f 6d62 696e 6520 626f 7468 2073  n combine both s
+000265f0: 796e 7461 7865 7320 746f 6765 7468 6572  yntaxes together
+00026600: 2e0a 0a20 2020 2020 2020 2020 2020 2063  ...            c
+00026610: 6170 7469 6f6e 5f65 6e74 6974 6965 7320  aption_entities 
+00026620: 284c 6973 7420 6f66 203a 6f62 6a3a 607e  (List of :obj:`~
+00026630: 7079 726f 6772 616d 2e74 7970 6573 2e4d  pyrogram.types.M
+00026640: 6573 7361 6765 456e 7469 7479 6029 3a0a  essageEntity`):.
 00026650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026660: 5365 6e64 7320 7468 6520 6d65 7373 6167  Sends the messag
-00026670: 6520 7369 6c65 6e74 6c79 2e0a 2020 2020  e silently..    
-00026680: 2020 2020 2020 2020 2020 2020 5573 6572              User
-00026690: 7320 7769 6c6c 2072 6563 6569 7665 2061  s will receive a
-000266a0: 206e 6f74 6966 6963 6174 696f 6e20 7769   notification wi
-000266b0: 7468 206e 6f20 736f 756e 642e 0a0a 2020  th no sound...  
-000266c0: 2020 2020 2020 2020 2020 7072 6f74 6563            protec
-000266d0: 745f 636f 6e74 656e 7420 2860 6062 6f6f  t_content (``boo
-000266e0: 6c60 602c 202a 6f70 7469 6f6e 616c 2a29  l``, *optional*)
-000266f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00026700: 2020 5072 6f74 6563 7473 2074 6865 2063    Protects the c
-00026710: 6f6e 7465 6e74 7320 6f66 2074 6865 2073  ontents of the s
-00026720: 656e 7420 6d65 7373 6167 6520 6672 6f6d  ent message from
-00026730: 2066 6f72 7761 7264 696e 6720 616e 6420   forwarding and 
-00026740: 7361 7669 6e67 2e0a 0a20 2020 2020 2020  saving...       
-00026750: 2020 2020 2064 726f 705f 6175 7468 6f72       drop_author
-00026760: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
-00026770: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
-00026780: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
-00026790: 2074 6f20 666f 7277 6172 6420 6d65 7373   to forward mess
-000267a0: 6167 6573 2077 6974 686f 7574 2071 756f  ages without quo
-000267b0: 7469 6e67 2074 6865 206f 7269 6769 6e61  ting the origina
-000267c0: 6c20 6175 7468 6f72 2e0a 0a20 2020 2020  l author...     
-000267d0: 2020 2020 2020 2064 726f 705f 6d65 6469         drop_medi
-000267e0: 615f 6361 7074 696f 6e73 2028 6060 626f  a_captions (``bo
-000267f0: 6f6c 6060 2c20 2a6f 7074 696f 6e61 6c2a  ol``, *optional*
-00026800: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00026810: 2020 2057 6865 7468 6572 2074 6f20 7374     Whether to st
-00026820: 7269 7020 6361 7074 696f 6e73 2066 726f  rip captions fro
-00026830: 6d20 6d65 6469 612e 0a0a 2020 2020 2020  m media...      
-00026840: 2020 2020 2020 7363 6865 6475 6c65 5f64        schedule_d
-00026850: 6174 6520 283a 7079 3a6f 626a 3a60 7e64  ate (:py:obj:`~d
-00026860: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
-00026870: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
-00026880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026890: 4461 7465 2077 6865 6e20 7468 6520 6d65  Date when the me
-000268a0: 7373 6167 6520 7769 6c6c 2062 6520 6175  ssage will be au
-000268b0: 746f 6d61 7469 6361 6c6c 7920 7365 6e74  tomatically sent
-000268c0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000268d0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-000268e0: 4f6e 2073 7563 6365 7373 2c20 7468 6520  On success, the 
-000268f0: 666f 7277 6172 6465 6420 4d65 7373 6167  forwarded Messag
-00026900: 6520 6973 2072 6574 7572 6e65 642e 0a0a  e is returned...
-00026910: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
-00026920: 2020 2020 2020 2020 2020 2020 5250 4345              RPCE
-00026930: 7272 6f72 3a20 496e 2063 6173 6520 6f66  rror: In case of
-00026940: 2061 2054 656c 6567 7261 6d20 5250 4320   a Telegram RPC 
-00026950: 6572 726f 722e 0a20 2020 2020 2020 2022  error..        "
-00026960: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00026970: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
-00026980: 6965 6e74 2e66 6f72 7761 7264 5f6d 6573  ient.forward_mes
-00026990: 7361 6765 7328 0a20 2020 2020 2020 2020  sages(.         
-000269a0: 2020 2066 726f 6d5f 6368 6174 5f69 643d     from_chat_id=
-000269b0: 7365 6c66 2e63 6861 742e 6964 2c0a 2020  self.chat.id,.  
-000269c0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-000269d0: 655f 6964 733d 7365 6c66 2e69 642c 0a20  e_ids=self.id,. 
-000269e0: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-000269f0: 6964 3d63 6861 745f 6964 2c0a 2020 2020  id=chat_id,.    
-00026a00: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
-00026a10: 7468 7265 6164 5f69 643d 6d65 7373 6167  thread_id=messag
-00026a20: 655f 7468 7265 6164 5f69 642c 0a20 2020  e_thread_id,.   
-00026a30: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
-00026a40: 5f6e 6f74 6966 6963 6174 696f 6e3d 6469  _notification=di
-00026a50: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
-00026a60: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-00026a70: 7072 6f74 6563 745f 636f 6e74 656e 743d  protect_content=
-00026a80: 7072 6f74 6563 745f 636f 6e74 656e 742c  protect_content,
-00026a90: 0a20 2020 2020 2020 2020 2020 2064 726f  .            dro
-00026aa0: 705f 6175 7468 6f72 3d64 726f 705f 6175  p_author=drop_au
-00026ab0: 7468 6f72 2c0a 2020 2020 2020 2020 2020  thor,.          
-00026ac0: 2020 6472 6f70 5f6d 6564 6961 5f63 6170    drop_media_cap
-00026ad0: 7469 6f6e 733d 6472 6f70 5f6d 6564 6961  tions=drop_media
-00026ae0: 5f63 6170 7469 6f6e 732c 0a20 2020 2020  _captions,.     
-00026af0: 2020 2020 2020 2073 6368 6564 756c 655f         schedule_
-00026b00: 6461 7465 3d73 6368 6564 756c 655f 6461  date=schedule_da
-00026b10: 7465 0a20 2020 2020 2020 2029 0a0a 2020  te.        )..  
-00026b20: 2020 6173 796e 6320 6465 6620 636f 7079    async def copy
-00026b30: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00026b40: 2020 2020 2020 2020 6368 6174 5f69 643a          chat_id:
-00026b50: 2055 6e69 6f6e 5b69 6e74 2c20 7374 725d   Union[int, str]
-00026b60: 2c0a 2020 2020 2020 2020 6361 7074 696f  ,.        captio
-00026b70: 6e3a 2073 7472 203d 204e 6f6e 652c 0a20  n: str = None,. 
-00026b80: 2020 2020 2020 2070 6172 7365 5f6d 6f64         parse_mod
-00026b90: 653a 204f 7074 696f 6e61 6c5b 2265 6e75  e: Optional["enu
-00026ba0: 6d73 2e50 6172 7365 4d6f 6465 225d 203d  ms.ParseMode"] =
-00026bb0: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
-00026bc0: 6170 7469 6f6e 5f65 6e74 6974 6965 733a  aption_entities:
-00026bd0: 204c 6973 745b 2274 7970 6573 2e4d 6573   List["types.Mes
-00026be0: 7361 6765 456e 7469 7479 225d 203d 204e  sageEntity"] = N
-00026bf0: 6f6e 652c 0a20 2020 2020 2020 2064 6973  one,.        dis
-00026c00: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-00026c10: 6e3a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  n: bool = None,.
-00026c20: 2020 2020 2020 2020 7265 706c 795f 7061          reply_pa
-00026c30: 7261 6d65 7465 7273 3a20 2274 7970 6573  rameters: "types
-00026c40: 2e52 6570 6c79 5061 7261 6d65 7465 7273  .ReplyParameters
-00026c50: 2220 3d20 4e6f 6e65 2c0a 2020 2020 2020  " = None,.      
-00026c60: 2020 7265 706c 795f 6d61 726b 7570 3a20    reply_markup: 
-00026c70: 556e 696f 6e5b 0a20 2020 2020 2020 2020  Union[.         
-00026c80: 2020 2022 7479 7065 732e 496e 6c69 6e65     "types.Inline
-00026c90: 4b65 7962 6f61 7264 4d61 726b 7570 222c  KeyboardMarkup",
-00026ca0: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-00026cb0: 7065 732e 5265 706c 794b 6579 626f 6172  pes.ReplyKeyboar
-00026cc0: 644d 6172 6b75 7022 2c0a 2020 2020 2020  dMarkup",.      
-00026cd0: 2020 2020 2020 2274 7970 6573 2e52 6570        "types.Rep
-00026ce0: 6c79 4b65 7962 6f61 7264 5265 6d6f 7665  lyKeyboardRemove
-00026cf0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00026d00: 7479 7065 732e 466f 7263 6552 6570 6c79  types.ForceReply
-00026d10: 220a 2020 2020 2020 2020 5d20 3d20 6f62  ".        ] = ob
-00026d20: 6a65 6374 2c0a 2020 2020 2020 2020 7265  ject,.        re
-00026d30: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00026d40: 643a 2069 6e74 203d 204e 6f6e 652c 0a20  d: int = None,. 
-00026d50: 2020 2020 2020 2073 6368 6564 756c 655f         schedule_
-00026d60: 6461 7465 3a20 6461 7465 7469 6d65 203d  date: datetime =
-00026d70: 204e 6f6e 650a 2020 2020 2920 2d3e 2055   None.    ) -> U
-00026d80: 6e69 6f6e 5b22 7479 7065 732e 4d65 7373  nion["types.Mess
-00026d90: 6167 6522 2c20 4c69 7374 5b22 7479 7065  age", List["type
-00026da0: 732e 4d65 7373 6167 6522 5d5d 3a0a 2020  s.Message"]]:.  
-00026db0: 2020 2020 2020 2222 2242 6f75 6e64 206d        """Bound m
-00026dc0: 6574 686f 6420 2a63 6f70 792a 206f 6620  ethod *copy* of 
-00026dd0: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
-00026de0: 7479 7065 732e 4d65 7373 6167 6560 2e0a  types.Message`..
-00026df0: 0a20 2020 2020 2020 2055 7365 2061 7320  .        Use as 
-00026e00: 6120 7368 6f72 7463 7574 2066 6f72 3a0a  a shortcut for:.
-00026e10: 0a20 2020 2020 2020 202e 2e20 636f 6465  .        .. code
-00026e20: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-00026e30: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-00026e40: 6974 2063 6c69 656e 742e 636f 7079 5f6d  it client.copy_m
-00026e50: 6573 7361 6765 280a 2020 2020 2020 2020  essage(.        
-00026e60: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
-00026e70: 6368 6174 5f69 642c 0a20 2020 2020 2020  chat_id,.       
-00026e80: 2020 2020 2020 2020 2066 726f 6d5f 6368           from_ch
-00026e90: 6174 5f69 643d 6d65 7373 6167 652e 6368  at_id=message.ch
-00026ea0: 6174 2e69 642c 0a20 2020 2020 2020 2020  at.id,.         
-00026eb0: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
-00026ec0: 643d 6d65 7373 6167 652e 6964 0a20 2020  d=message.id.   
-00026ed0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00026ee0: 2020 2020 4578 616d 706c 653a 0a20 2020      Example:.   
-00026ef0: 2020 2020 2020 2020 202e 2e20 636f 6465           .. code
-00026f00: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-00026f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026f20: 2061 7761 6974 206d 6573 7361 6765 2e63   await message.c
-00026f30: 6f70 7928 6368 6174 5f69 6429 0a0a 2020  opy(chat_id)..  
-00026f40: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00026f50: 3a0a 2020 2020 2020 2020 2020 2020 6368  :.            ch
-00026f60: 6174 5f69 6420 2860 6069 6e74 6060 207c  at_id (``int`` |
-00026f70: 2060 6073 7472 6060 293a 0a20 2020 2020   ``str``):.     
-00026f80: 2020 2020 2020 2020 2020 2055 6e69 7175             Uniqu
-00026f90: 6520 6964 656e 7469 6669 6572 2028 696e  e identifier (in
-00026fa0: 7429 206f 7220 7573 6572 6e61 6d65 2028  t) or username (
-00026fb0: 7374 7229 206f 6620 7468 6520 7461 7267  str) of the targ
-00026fc0: 6574 2063 6861 742e 0a20 2020 2020 2020  et chat..       
-00026fd0: 2020 2020 2020 2020 2046 6f72 2079 6f75           For you
-00026fe0: 7220 7065 7273 6f6e 616c 2063 6c6f 7564  r personal cloud
-00026ff0: 2028 5361 7665 6420 4d65 7373 6167 6573   (Saved Messages
-00027000: 2920 796f 7520 6361 6e20 7369 6d70 6c79  ) you can simply
-00027010: 2075 7365 2022 6d65 2220 6f72 2022 7365   use "me" or "se
-00027020: 6c66 222e 0a20 2020 2020 2020 2020 2020  lf"..           
-00027030: 2020 2020 2046 6f72 2061 2063 6f6e 7461       For a conta
-00027040: 6374 2074 6861 7420 6578 6973 7473 2069  ct that exists i
-00027050: 6e20 796f 7572 2054 656c 6567 7261 6d20  n your Telegram 
-00027060: 6164 6472 6573 7320 626f 6f6b 2079 6f75  address book you
-00027070: 2063 616e 2075 7365 2068 6973 2070 686f   can use his pho
-00027080: 6e65 206e 756d 6265 7220 2873 7472 292e  ne number (str).
-00027090: 0a0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
-000270a0: 7074 696f 6e20 2860 6073 7472 696e 6760  ption (``string`
-000270b0: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
-000270c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000270d0: 4e65 7720 6361 7074 696f 6e20 666f 7220  New caption for 
-000270e0: 6d65 6469 612c 2030 2d31 3032 3420 6368  media, 0-1024 ch
-000270f0: 6172 6163 7465 7273 2061 6674 6572 2065  aracters after e
-00027100: 6e74 6974 6965 7320 7061 7273 696e 672e  ntities parsing.
-00027110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00027120: 2049 6620 6e6f 7420 7370 6563 6966 6965   If not specifie
-00027130: 642c 2074 6865 206f 7269 6769 6e61 6c20  d, the original 
-00027140: 6361 7074 696f 6e20 6973 206b 6570 742e  caption is kept.
-00027150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00027160: 2050 6173 7320 2222 2028 656d 7074 7920   Pass "" (empty 
-00027170: 7374 7269 6e67 2920 746f 2072 656d 6f76  string) to remov
-00027180: 6520 7468 6520 6361 7074 696f 6e2e 0a0a  e the caption...
-00027190: 2020 2020 2020 2020 2020 2020 7061 7273              pars
-000271a0: 655f 6d6f 6465 2028 3a6f 626a 3a60 7e70  e_mode (:obj:`~p
-000271b0: 7972 6f67 7261 6d2e 656e 756d 732e 5061  yrogram.enums.Pa
-000271c0: 7273 654d 6f64 6560 2c20 2a6f 7074 696f  rseMode`, *optio
-000271d0: 6e61 6c2a 293a 0a20 2020 2020 2020 2020  nal*):.         
-000271e0: 2020 2020 2020 2042 7920 6465 6661 756c         By defaul
-000271f0: 742c 2074 6578 7473 2061 7265 2070 6172  t, texts are par
-00027200: 7365 6420 7573 696e 6720 626f 7468 204d  sed using both M
-00027210: 6172 6b64 6f77 6e20 616e 6420 4854 4d4c  arkdown and HTML
-00027220: 2073 7479 6c65 732e 0a20 2020 2020 2020   styles..       
-00027230: 2020 2020 2020 2020 2059 6f75 2063 616e           You can
-00027240: 2063 6f6d 6269 6e65 2062 6f74 6820 7379   combine both sy
-00027250: 6e74 6178 6573 2074 6f67 6574 6865 722e  ntaxes together.
-00027260: 0a0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
-00027270: 7074 696f 6e5f 656e 7469 7469 6573 2028  ption_entities (
-00027280: 4c69 7374 206f 6620 3a6f 626a 3a60 7e70  List of :obj:`~p
-00027290: 7972 6f67 7261 6d2e 7479 7065 732e 4d65  yrogram.types.Me
-000272a0: 7373 6167 6545 6e74 6974 7960 293a 0a20  ssageEntity`):. 
-000272b0: 2020 2020 2020 2020 2020 2020 2020 204c                 L
-000272c0: 6973 7420 6f66 2073 7065 6369 616c 2065  ist of special e
-000272d0: 6e74 6974 6965 7320 7468 6174 2061 7070  ntities that app
-000272e0: 6561 7220 696e 2074 6865 206e 6577 2063  ear in the new c
-000272f0: 6170 7469 6f6e 2c20 7768 6963 6820 6361  aption, which ca
-00027300: 6e20 6265 2073 7065 6369 6669 6564 2069  n be specified i
-00027310: 6e73 7465 6164 206f 6620 2a70 6172 7365  nstead of *parse
-00027320: 5f6d 6f64 652a 2e0a 0a20 2020 2020 2020  _mode*...       
-00027330: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
-00027340: 6966 6963 6174 696f 6e20 2860 6062 6f6f  ification (``boo
-00027350: 6c60 602c 202a 6f70 7469 6f6e 616c 2a29  l``, *optional*)
-00027360: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00027370: 2020 5365 6e64 7320 7468 6520 6d65 7373    Sends the mess
-00027380: 6167 6520 7369 6c65 6e74 6c79 2e0a 2020  age silently..  
-00027390: 2020 2020 2020 2020 2020 2020 2020 5573                Us
-000273a0: 6572 7320 7769 6c6c 2072 6563 6569 7665  ers will receive
-000273b0: 2061 206e 6f74 6966 6963 6174 696f 6e20   a notification 
-000273c0: 7769 7468 206e 6f20 736f 756e 642e 0a0a  with no sound...
-000273d0: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-000273e0: 795f 7061 7261 6d65 7465 7273 2028 3a6f  y_parameters (:o
-000273f0: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
-00027400: 7065 732e 5265 706c 7950 6172 616d 6574  pes.ReplyParamet
-00027410: 6572 7360 2c20 2a6f 7074 696f 6e61 6c2a  ers`, *optional*
-00027420: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00027430: 2020 2044 6573 6372 6970 7469 6f6e 206f     Description o
-00027440: 6620 7468 6520 6d65 7373 6167 6520 746f  f the message to
-00027450: 2072 6570 6c79 2074 6f0a 0a20 2020 2020   reply to..     
-00027460: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
-00027470: 6b75 7020 283a 6f62 6a3a 607e 7079 726f  kup (:obj:`~pyro
-00027480: 6772 616d 2e74 7970 6573 2e49 6e6c 696e  gram.types.Inlin
-00027490: 654b 6579 626f 6172 644d 6172 6b75 7060  eKeyboardMarkup`
-000274a0: 207c 203a 6f62 6a3a 607e 7079 726f 6772   | :obj:`~pyrogr
-000274b0: 616d 2e74 7970 6573 2e52 6570 6c79 4b65  am.types.ReplyKe
-000274c0: 7962 6f61 7264 4d61 726b 7570 6020 7c20  yboardMarkup` | 
-000274d0: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
-000274e0: 7479 7065 732e 5265 706c 794b 6579 626f  types.ReplyKeybo
-000274f0: 6172 6452 656d 6f76 6560 207c 203a 6f62  ardRemove` | :ob
-00027500: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
-00027510: 6573 2e46 6f72 6365 5265 706c 7960 2c20  es.ForceReply`, 
-00027520: 2a6f 7074 696f 6e61 6c2a 293a 0a20 2020  *optional*):.   
-00027530: 2020 2020 2020 2020 2020 2020 2041 6464               Add
-00027540: 6974 696f 6e61 6c20 696e 7465 7266 6163  itional interfac
-00027550: 6520 6f70 7469 6f6e 732e 2041 6e20 6f62  e options. An ob
-00027560: 6a65 6374 2066 6f72 2061 6e20 696e 6c69  ject for an inli
-00027570: 6e65 206b 6579 626f 6172 642c 2063 7573  ne keyboard, cus
-00027580: 746f 6d20 7265 706c 7920 6b65 7962 6f61  tom reply keyboa
-00027590: 7264 2c0a 2020 2020 2020 2020 2020 2020  rd,.            
-000275a0: 2020 2020 696e 7374 7275 6374 696f 6e73      instructions
-000275b0: 2074 6f20 7265 6d6f 7665 2072 6570 6c79   to remove reply
-000275c0: 206b 6579 626f 6172 6420 6f72 2074 6f20   keyboard or to 
-000275d0: 666f 7263 6520 6120 7265 706c 7920 6672  force a reply fr
-000275e0: 6f6d 2074 6865 2075 7365 722e 0a20 2020  om the user..   
-000275f0: 2020 2020 2020 2020 2020 2020 2049 6620               If 
-00027600: 6e6f 7420 7370 6563 6966 6965 642c 2074  not specified, t
-00027610: 6865 206f 7269 6769 6e61 6c20 7265 706c  he original repl
-00027620: 7920 6d61 726b 7570 2069 7320 6b65 7074  y markup is kept
-00027630: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00027640: 2020 5061 7373 204e 6f6e 6520 746f 2072    Pass None to r
-00027650: 656d 6f76 6520 7468 6520 7265 706c 7920  emove the reply 
-00027660: 6d61 726b 7570 2e0a 0a20 2020 2020 2020  markup...       
-00027670: 2020 2020 2073 6368 6564 756c 655f 6461       schedule_da
-00027680: 7465 2028 3a70 793a 6f62 6a3a 607e 6461  te (:py:obj:`~da
-00027690: 7465 7469 6d65 2e64 6174 6574 696d 6560  tetime.datetime`
-000276a0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
-000276b0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-000276c0: 6174 6520 7768 656e 2074 6865 206d 6573  ate when the mes
-000276d0: 7361 6765 2077 696c 6c20 6265 2061 7574  sage will be aut
-000276e0: 6f6d 6174 6963 616c 6c79 2073 656e 742e  omatically sent.
-000276f0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00027700: 733a 0a20 2020 2020 2020 2020 2020 203a  s:.            :
-00027710: 6f62 6a3a 607e 7079 726f 6772 616d 2e74  obj:`~pyrogram.t
-00027720: 7970 6573 2e4d 6573 7361 6765 603a 204f  ypes.Message`: O
-00027730: 6e20 7375 6363 6573 732c 2074 6865 2063  n success, the c
-00027740: 6f70 6965 6420 6d65 7373 6167 6520 6973  opied message is
-00027750: 2072 6574 7572 6e65 642e 0a0a 2020 2020   returned...    
-00027760: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-00027770: 2020 2020 2020 2020 5250 4345 7272 6f72          RPCError
-00027780: 3a20 496e 2063 6173 6520 6f66 2061 2054  : In case of a T
-00027790: 656c 6567 7261 6d20 5250 4320 6572 726f  elegram RPC erro
-000277a0: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
-000277b0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-000277c0: 6572 7669 6365 3a0a 2020 2020 2020 2020  ervice:.        
-000277d0: 2020 2020 6c6f 672e 7761 726e 696e 6728      log.warning(
-000277e0: 2253 6572 7669 6365 206d 6573 7361 6765  "Service message
-000277f0: 7320 6361 6e6e 6f74 2062 6520 636f 7069  s cannot be copi
-00027800: 6564 2e20 6368 6174 5f69 643a 2025 732c  ed. chat_id: %s,
-00027810: 206d 6573 7361 6765 5f69 643a 2025 7322   message_id: %s"
-00027820: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00027830: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00027840: 6861 742e 6964 2c20 7365 6c66 2e69 6429  hat.id, self.id)
-00027850: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
-00027860: 6c66 2e67 616d 6520 616e 6420 6e6f 7420  lf.game and not 
-00027870: 7365 6c66 2e5f 636c 6965 6e74 2e6d 652e  self._client.me.
-00027880: 6973 5f62 6f74 3a0a 2020 2020 2020 2020  is_bot:.        
-00027890: 2020 2020 6c6f 672e 7761 726e 696e 6728      log.warning(
-000278a0: 2255 7365 7273 2063 616e 6e6f 7420 7365  "Users cannot se
-000278b0: 6e64 206d 6573 7361 6765 7320 7769 7468  nd messages with
-000278c0: 2047 616d 6520 6d65 6469 6120 7479 7065   Game media type
-000278d0: 2e20 6368 6174 5f69 643a 2025 732c 206d  . chat_id: %s, m
-000278e0: 6573 7361 6765 5f69 643a 2025 7322 2c0a  essage_id: %s",.
-000278f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027900: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-00027910: 742e 6964 2c20 7365 6c66 2e69 6429 0a20  t.id, self.id). 
-00027920: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-00027930: 2e65 6d70 7479 3a0a 2020 2020 2020 2020  .empty:.        
-00027940: 2020 2020 6c6f 672e 7761 726e 696e 6728      log.warning(
-00027950: 2245 6d70 7479 206d 6573 7361 6765 7320  "Empty messages 
-00027960: 6361 6e6e 6f74 2062 6520 636f 7069 6564  cannot be copied
-00027970: 2e22 290a 2020 2020 2020 2020 656c 6966  .").        elif
-00027980: 2073 656c 662e 7465 7874 3a0a 2020 2020   self.text:.    
-00027990: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-000279a0: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
-000279b0: 742e 7365 6e64 5f6d 6573 7361 6765 280a  t.send_message(.
-000279c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000279d0: 6368 6174 5f69 643d 6368 6174 5f69 642c  chat_id=chat_id,
-000279e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000279f0: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
-00027a00: 6964 3d73 656c 662e 6d65 7373 6167 655f  id=self.message_
-00027a10: 7468 7265 6164 5f69 642c 0a20 2020 2020  thread_id,.     
-00027a20: 2020 2020 2020 2020 2020 2062 7573 696e             busin
-00027a30: 6573 735f 636f 6e6e 6563 7469 6f6e 5f69  ess_connection_i
-00027a40: 643d 7365 6c66 2e62 7573 696e 6573 735f  d=self.business_
-00027a50: 636f 6e6e 6563 7469 6f6e 5f69 642c 0a20  connection_id,. 
-00027a60: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00027a70: 6578 743d 7365 6c66 2e74 6578 742c 0a20  ext=self.text,. 
-00027a80: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00027a90: 6172 7365 5f6d 6f64 653d 656e 756d 732e  arse_mode=enums.
-00027aa0: 5061 7273 654d 6f64 652e 4449 5341 424c  ParseMode.DISABL
-00027ab0: 4544 2c0a 2020 2020 2020 2020 2020 2020  ED,.            
-00027ac0: 2020 2020 656e 7469 7469 6573 3d73 656c      entities=sel
-00027ad0: 662e 656e 7469 7469 6573 2c0a 2020 2020  f.entities,.    
-00027ae0: 2020 2020 2020 2020 2020 2020 6c69 6e6b              link
-00027af0: 5f70 7265 7669 6577 5f6f 7074 696f 6e73  _preview_options
-00027b00: 3d73 656c 662e 6c69 6e6b 5f70 7265 7669  =self.link_previ
-00027b10: 6577 5f6f 7074 696f 6e73 2c0a 2020 2020  ew_options,.    
-00027b20: 2020 2020 2020 2020 2020 2020 6469 7361              disa
-00027b30: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00027b40: 3d64 6973 6162 6c65 5f6e 6f74 6966 6963  =disable_notific
-00027b50: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
-00027b60: 2020 2020 2020 2070 726f 7465 6374 5f63         protect_c
-00027b70: 6f6e 7465 6e74 3d73 656c 662e 6861 735f  ontent=self.has_
-00027b80: 7072 6f74 6563 7465 645f 636f 6e74 656e  protected_conten
-00027b90: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00027ba0: 2020 2072 6570 6c79 5f70 6172 616d 6574     reply_paramet
-00027bb0: 6572 733d 7265 706c 795f 7061 7261 6d65  ers=reply_parame
-00027bc0: 7465 7273 2c0a 2020 2020 2020 2020 2020  ters,.          
-00027bd0: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
-00027be0: 7570 3d73 656c 662e 7265 706c 795f 6d61  up=self.reply_ma
-00027bf0: 726b 7570 2069 6620 7265 706c 795f 6d61  rkup if reply_ma
-00027c00: 726b 7570 2069 7320 6f62 6a65 6374 2065  rkup is object e
-00027c10: 6c73 6520 7265 706c 795f 6d61 726b 7570  lse reply_markup
-00027c20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00027c30: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
-00027c40: 6765 5f69 643d 7265 706c 795f 746f 5f6d  ge_id=reply_to_m
-00027c50: 6573 7361 6765 5f69 642c 0a20 2020 2020  essage_id,.     
-00027c60: 2020 2020 2020 2020 2020 2073 6368 6564             sched
-00027c70: 756c 655f 6461 7465 3d73 6368 6564 756c  ule_date=schedul
-00027c80: 655f 6461 7465 0a20 2020 2020 2020 2020  e_date.         
-00027c90: 2020 2029 0a20 2020 2020 2020 2065 6c69     ).        eli
-00027ca0: 6620 7365 6c66 2e6d 6564 6961 3a0a 2020  f self.media:.  
-00027cb0: 2020 2020 2020 2020 2020 7365 6e64 5f6d            send_m
-00027cc0: 6564 6961 203d 2070 6172 7469 616c 280a  edia = partial(.
-00027cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027ce0: 7365 6c66 2e5f 636c 6965 6e74 2e73 656e  self._client.sen
-00027cf0: 645f 6361 6368 6564 5f6d 6564 6961 2c0a  d_cached_media,.
-00027d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027d10: 6368 6174 5f69 643d 6368 6174 5f69 642c  chat_id=chat_id,
-00027d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00027d30: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-00027d40: 6174 696f 6e3d 6469 7361 626c 655f 6e6f  ation=disable_no
-00027d50: 7469 6669 6361 7469 6f6e 2c0a 2020 2020  tification,.    
-00027d60: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-00027d70: 795f 7061 7261 6d65 7465 7273 3d72 6570  y_parameters=rep
-00027d80: 6c79 5f70 6172 616d 6574 6572 732c 0a20  ly_parameters,. 
-00027d90: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00027da0: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
-00027db0: 3d73 656c 662e 6d65 7373 6167 655f 7468  =self.message_th
-00027dc0: 7265 6164 5f69 642c 0a20 2020 2020 2020  read_id,.       
-00027dd0: 2020 2020 2020 2020 2062 7573 696e 6573           busines
-00027de0: 735f 636f 6e6e 6563 7469 6f6e 5f69 643d  s_connection_id=
-00027df0: 7365 6c66 2e62 7573 696e 6573 735f 636f  self.business_co
-00027e00: 6e6e 6563 7469 6f6e 5f69 642c 0a20 2020  nnection_id,.   
-00027e10: 2020 2020 2020 2020 2020 2020 2073 6368               sch
-00027e20: 6564 756c 655f 6461 7465 3d73 6368 6564  edule_date=sched
-00027e30: 756c 655f 6461 7465 2c0a 2020 2020 2020  ule_date,.      
-00027e40: 2020 2020 2020 2020 2020 7072 6f74 6563            protec
-00027e50: 745f 636f 6e74 656e 743d 7365 6c66 2e68  t_content=self.h
-00027e60: 6173 5f70 726f 7465 6374 6564 5f63 6f6e  as_protected_con
-00027e70: 7465 6e74 2c0a 2020 2020 2020 2020 2020  tent,.          
-00027e80: 2020 2020 2020 6861 735f 7370 6f69 6c65        has_spoile
-00027e90: 723d 7365 6c66 2e68 6173 5f6d 6564 6961  r=self.has_media
-00027ea0: 5f73 706f 696c 6572 2c0a 2020 2020 2020  _spoiler,.      
-00027eb0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
-00027ec0: 746f 5f6d 6573 7361 6765 5f69 643d 7265  to_message_id=re
-00027ed0: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00027ee0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00027ef0: 2020 2072 6570 6c79 5f6d 6172 6b75 703d     reply_markup=
-00027f00: 7365 6c66 2e72 6570 6c79 5f6d 6172 6b75  self.reply_marku
-00027f10: 7020 6966 2072 6570 6c79 5f6d 6172 6b75  p if reply_marku
-00027f20: 7020 6973 206f 626a 6563 7420 656c 7365  p is object else
-00027f30: 2072 6570 6c79 5f6d 6172 6b75 700a 2020   reply_markup.  
-00027f40: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00027f50: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00027f60: 2e70 686f 746f 3a0a 2020 2020 2020 2020  .photo:.        
-00027f70: 2020 2020 2020 2020 6669 6c65 5f69 6420          file_id 
-00027f80: 3d20 7365 6c66 2e70 686f 746f 2e66 696c  = self.photo.fil
-00027f90: 655f 6964 0a20 2020 2020 2020 2020 2020  e_id.           
-00027fa0: 2065 6c69 6620 7365 6c66 2e61 7564 696f   elif self.audio
-00027fb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00027fc0: 2020 6669 6c65 5f69 6420 3d20 7365 6c66    file_id = self
-00027fd0: 2e61 7564 696f 2e66 696c 655f 6964 0a20  .audio.file_id. 
-00027fe0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00027ff0: 7365 6c66 2e64 6f63 756d 656e 743a 0a20  self.document:. 
-00028000: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00028010: 696c 655f 6964 203d 2073 656c 662e 646f  ile_id = self.do
-00028020: 6375 6d65 6e74 2e66 696c 655f 6964 0a20  cument.file_id. 
-00028030: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00028040: 7365 6c66 2e76 6964 656f 3a0a 2020 2020  self.video:.    
-00028050: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00028060: 5f69 6420 3d20 7365 6c66 2e76 6964 656f  _id = self.video
-00028070: 2e66 696c 655f 6964 0a20 2020 2020 2020  .file_id.       
-00028080: 2020 2020 2065 6c69 6620 7365 6c66 2e61       elif self.a
-00028090: 6e69 6d61 7469 6f6e 3a0a 2020 2020 2020  nimation:.      
-000280a0: 2020 2020 2020 2020 2020 6669 6c65 5f69            file_i
-000280b0: 6420 3d20 7365 6c66 2e61 6e69 6d61 7469  d = self.animati
-000280c0: 6f6e 2e66 696c 655f 6964 0a20 2020 2020  on.file_id.     
-000280d0: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-000280e0: 2e76 6f69 6365 3a0a 2020 2020 2020 2020  .voice:.        
-000280f0: 2020 2020 2020 2020 6669 6c65 5f69 6420          file_id 
-00028100: 3d20 7365 6c66 2e76 6f69 6365 2e66 696c  = self.voice.fil
-00028110: 655f 6964 0a20 2020 2020 2020 2020 2020  e_id.           
-00028120: 2065 6c69 6620 7365 6c66 2e73 7469 636b   elif self.stick
-00028130: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-00028140: 2020 2020 6669 6c65 5f69 6420 3d20 7365      file_id = se
-00028150: 6c66 2e73 7469 636b 6572 2e66 696c 655f  lf.sticker.file_
-00028160: 6964 0a20 2020 2020 2020 2020 2020 2065  id.            e
-00028170: 6c69 6620 7365 6c66 2e76 6964 656f 5f6e  lif self.video_n
-00028180: 6f74 653a 0a20 2020 2020 2020 2020 2020  ote:.           
-00028190: 2020 2020 2066 696c 655f 6964 203d 2073       file_id = s
-000281a0: 656c 662e 7669 6465 6f5f 6e6f 7465 2e66  elf.video_note.f
-000281b0: 696c 655f 6964 0a20 2020 2020 2020 2020  ile_id.         
-000281c0: 2020 2065 6c69 6620 7365 6c66 2e63 6f6e     elif self.con
-000281d0: 7461 6374 3a0a 2020 2020 2020 2020 2020  tact:.          
-000281e0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-000281f0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-00028200: 7365 6e64 5f63 6f6e 7461 6374 280a 2020  send_contact(.  
-00028210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028220: 2020 6368 6174 5f69 642c 0a20 2020 2020    chat_id,.     
-00028230: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00028240: 686f 6e65 5f6e 756d 6265 723d 7365 6c66  hone_number=self
-00028250: 2e63 6f6e 7461 6374 2e70 686f 6e65 5f6e  .contact.phone_n
-00028260: 756d 6265 722c 0a20 2020 2020 2020 2020  umber,.         
-00028270: 2020 2020 2020 2020 2020 2066 6972 7374             first
-00028280: 5f6e 616d 653d 7365 6c66 2e63 6f6e 7461  _name=self.conta
-00028290: 6374 2e66 6972 7374 5f6e 616d 652c 0a20  ct.first_name,. 
+00026660: 4c69 7374 206f 6620 7370 6563 6961 6c20  List of special 
+00026670: 656e 7469 7469 6573 2074 6861 7420 6170  entities that ap
+00026680: 7065 6172 2069 6e20 7468 6520 6361 7074  pear in the capt
+00026690: 696f 6e2c 2077 6869 6368 2063 616e 2062  ion, which can b
+000266a0: 6520 7370 6563 6966 6965 6420 696e 7374  e specified inst
+000266b0: 6561 6420 6f66 202a 7061 7273 655f 6d6f  ead of *parse_mo
+000266c0: 6465 2a2e 0a0a 2020 2020 2020 2020 2020  de*...          
+000266d0: 2020 7363 6865 6475 6c65 5f64 6174 6520    schedule_date 
+000266e0: 283a 7079 3a6f 626a 3a60 7e64 6174 6574  (:py:obj:`~datet
+000266f0: 696d 652e 6461 7465 7469 6d65 602c 202a  ime.datetime`, *
+00026700: 6f70 7469 6f6e 616c 2a29 3a0a 2020 2020  optional*):.    
+00026710: 2020 2020 2020 2020 2020 2020 4461 7465              Date
+00026720: 2077 6865 6e20 7468 6520 6d65 7373 6167   when the messag
+00026730: 6520 7769 6c6c 2062 6520 6175 746f 6d61  e will be automa
+00026740: 7469 6361 6c6c 7920 7365 6e74 2e0a 0a20  tically sent... 
+00026750: 2020 2020 2020 2020 2020 2068 6173 5f73             has_s
+00026760: 706f 696c 6572 2028 6060 626f 6f6c 6060  poiler (``bool``
+00026770: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
+00026780: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00026790: 7275 652c 2069 6620 7468 6520 6d65 7373  rue, if the mess
+000267a0: 6167 6520 6d65 6469 6120 6973 2063 6f76  age media is cov
+000267b0: 6572 6564 2062 7920 6120 7370 6f69 6c65  ered by a spoile
+000267c0: 7220 616e 696d 6174 696f 6e2e 0a0a 2020  r animation...  
+000267d0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+000267e0: 6d61 726b 7570 2028 3a6f 626a 3a60 7e70  markup (:obj:`~p
+000267f0: 7972 6f67 7261 6d2e 7479 7065 732e 496e  yrogram.types.In
+00026800: 6c69 6e65 4b65 7962 6f61 7264 4d61 726b  lineKeyboardMark
+00026810: 7570 602c 202a 6f70 7469 6f6e 616c 2a29  up`, *optional*)
+00026820: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00026830: 2020 416e 2049 6e6c 696e 654b 6579 626f    An InlineKeybo
+00026840: 6172 644d 6172 6b75 7020 6f62 6a65 6374  ardMarkup object
+00026850: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00026860: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00026870: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
+00026880: 7479 7065 732e 4d65 7373 6167 6560 3a20  types.Message`: 
+00026890: 4f6e 2073 7563 6365 7373 2c20 7468 6520  On success, the 
+000268a0: 6564 6974 6564 206d 6564 6961 206d 6573  edited media mes
+000268b0: 7361 6765 2069 7320 7265 7475 726e 6564  sage is returned
+000268c0: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+000268d0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+000268e0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+000268f0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+00026900: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
+00026910: 7373 6167 652e 6564 6974 5f63 6163 6865  ssage.edit_cache
+00026920: 645f 6d65 6469 6128 6669 6c65 5f69 6429  d_media(file_id)
+00026930: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00026940: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+00026950: 7420 7365 6c66 2e5f 636c 6965 6e74 2e65  t self._client.e
+00026960: 6469 745f 6361 6368 6564 5f6d 6564 6961  dit_cached_media
+00026970: 280a 2020 2020 2020 2020 2020 2020 6368  (.            ch
+00026980: 6174 5f69 643d 7365 6c66 2e63 6861 742e  at_id=self.chat.
+00026990: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+000269a0: 6d65 7373 6167 655f 6964 3d73 656c 662e  message_id=self.
+000269b0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+000269c0: 6669 6c65 5f69 643d 6669 6c65 5f69 642c  file_id=file_id,
+000269d0: 0a20 2020 2020 2020 2020 2020 2063 6170  .            cap
+000269e0: 7469 6f6e 3d63 6170 7469 6f6e 2c0a 2020  tion=caption,.  
+000269f0: 2020 2020 2020 2020 2020 7061 7273 655f            parse_
+00026a00: 6d6f 6465 3d70 6172 7365 5f6d 6f64 652c  mode=parse_mode,
+00026a10: 0a20 2020 2020 2020 2020 2020 2063 6170  .            cap
+00026a20: 7469 6f6e 5f65 6e74 6974 6965 733d 6361  tion_entities=ca
+00026a30: 7074 696f 6e5f 656e 7469 7469 6573 2c0a  ption_entities,.
+00026a40: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+00026a50: 6475 6c65 5f64 6174 653d 7363 6865 6475  dule_date=schedu
+00026a60: 6c65 5f64 6174 652c 0a20 2020 2020 2020  le_date,.       
+00026a70: 2020 2020 2068 6173 5f73 706f 696c 6572       has_spoiler
+00026a80: 3d68 6173 5f73 706f 696c 6572 2c0a 2020  =has_spoiler,.  
+00026a90: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+00026aa0: 6d61 726b 7570 3d72 6570 6c79 5f6d 6172  markup=reply_mar
+00026ab0: 6b75 700a 2020 2020 2020 2020 290a 0a20  kup.        ).. 
+00026ac0: 2020 2061 7379 6e63 2064 6566 2066 6f72     async def for
+00026ad0: 7761 7264 280a 2020 2020 2020 2020 7365  ward(.        se
+00026ae0: 6c66 2c0a 2020 2020 2020 2020 6368 6174  lf,.        chat
+00026af0: 5f69 643a 2055 6e69 6f6e 5b69 6e74 2c20  _id: Union[int, 
+00026b00: 7374 725d 2c0a 2020 2020 2020 2020 6d65  str],.        me
+00026b10: 7373 6167 655f 7468 7265 6164 5f69 643a  ssage_thread_id:
+00026b20: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+00026b30: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
+00026b40: 6966 6963 6174 696f 6e3a 2062 6f6f 6c20  ification: bool 
+00026b50: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00026b60: 7072 6f74 6563 745f 636f 6e74 656e 743a  protect_content:
+00026b70: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
+00026b80: 2020 2020 2020 6472 6f70 5f61 7574 686f        drop_autho
+00026b90: 723a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  r: bool = None,.
+00026ba0: 2020 2020 2020 2020 6472 6f70 5f6d 6564          drop_med
+00026bb0: 6961 5f63 6170 7469 6f6e 733a 2062 6f6f  ia_captions: boo
+00026bc0: 6c20 3d20 4e6f 6e65 2c0a 2020 2020 2020  l = None,.      
+00026bd0: 2020 7363 6865 6475 6c65 5f64 6174 653a    schedule_date:
+00026be0: 2064 6174 6574 696d 6520 3d20 4e6f 6e65   datetime = None
+00026bf0: 0a20 2020 2029 202d 3e20 556e 696f 6e5b  .    ) -> Union[
+00026c00: 2274 7970 6573 2e4d 6573 7361 6765 222c  "types.Message",
+00026c10: 204c 6973 745b 2274 7970 6573 2e4d 6573   List["types.Mes
+00026c20: 7361 6765 225d 5d3a 0a20 2020 2020 2020  sage"]]:.       
+00026c30: 2022 2222 426f 756e 6420 6d65 7468 6f64   """Bound method
+00026c40: 202a 666f 7277 6172 642a 206f 6620 3a6f   *forward* of :o
+00026c50: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
+00026c60: 7065 732e 4d65 7373 6167 6560 2e0a 0a20  pes.Message`... 
+00026c70: 2020 2020 2020 2055 7365 2061 7320 6120         Use as a 
+00026c80: 7368 6f72 7463 7574 2066 6f72 3a0a 0a20  shortcut for:.. 
+00026c90: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+00026ca0: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+00026cb0: 2020 2020 2020 2020 2020 2061 7761 6974             await
+00026cc0: 2063 6c69 656e 742e 666f 7277 6172 645f   client.forward_
+00026cd0: 6d65 7373 6167 6573 280a 2020 2020 2020  messages(.      
+00026ce0: 2020 2020 2020 2020 2020 6368 6174 5f69            chat_i
+00026cf0: 643d 6368 6174 5f69 642c 0a20 2020 2020  d=chat_id,.     
+00026d00: 2020 2020 2020 2020 2020 2066 726f 6d5f             from_
+00026d10: 6368 6174 5f69 643d 6d65 7373 6167 652e  chat_id=message.
+00026d20: 6368 6174 2e69 642c 0a20 2020 2020 2020  chat.id,.       
+00026d30: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00026d40: 5f69 6473 3d6d 6573 7361 6765 2e69 640a  _ids=message.id.
+00026d50: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00026d60: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
+00026d70: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
+00026d80: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+00026d90: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+00026da0: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
+00026db0: 652e 666f 7277 6172 6428 6368 6174 5f69  e.forward(chat_i
+00026dc0: 6429 0a0a 2020 2020 2020 2020 5061 7261  d)..        Para
+00026dd0: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
+00026de0: 2020 2020 6368 6174 5f69 6420 2860 6069      chat_id (``i
+00026df0: 6e74 6060 207c 2060 6073 7472 6060 293a  nt`` | ``str``):
+00026e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026e10: 2055 6e69 7175 6520 6964 656e 7469 6669   Unique identifi
+00026e20: 6572 2028 696e 7429 206f 7220 7573 6572  er (int) or user
+00026e30: 6e61 6d65 2028 7374 7229 206f 6620 7468  name (str) of th
+00026e40: 6520 7461 7267 6574 2063 6861 742e 0a20  e target chat.. 
+00026e50: 2020 2020 2020 2020 2020 2020 2020 2046                 F
+00026e60: 6f72 2079 6f75 7220 7065 7273 6f6e 616c  or your personal
+00026e70: 2063 6c6f 7564 2028 5361 7665 6420 4d65   cloud (Saved Me
+00026e80: 7373 6167 6573 2920 796f 7520 6361 6e20  ssages) you can 
+00026e90: 7369 6d70 6c79 2075 7365 2022 6d65 2220  simply use "me" 
+00026ea0: 6f72 2022 7365 6c66 222e 0a20 2020 2020  or "self"..     
+00026eb0: 2020 2020 2020 2020 2020 2046 6f72 2061             For a
+00026ec0: 2063 6f6e 7461 6374 2074 6861 7420 6578   contact that ex
+00026ed0: 6973 7473 2069 6e20 796f 7572 2054 656c  ists in your Tel
+00026ee0: 6567 7261 6d20 6164 6472 6573 7320 626f  egram address bo
+00026ef0: 6f6b 2079 6f75 2063 616e 2075 7365 2068  ok you can use h
+00026f00: 6973 2070 686f 6e65 206e 756d 6265 7220  is phone number 
+00026f10: 2873 7472 292e 0a0a 2020 2020 2020 2020  (str)...        
+00026f20: 2020 2020 6d65 7373 6167 655f 7468 7265      message_thre
+00026f30: 6164 5f69 6420 2860 6069 6e74 6060 2c20  ad_id (``int``, 
+00026f40: 2a6f 7074 696f 6e61 6c2a 293a 0a20 2020  *optional*):.   
+00026f50: 2020 2020 2020 2020 2020 2020 2055 6e69               Uni
+00026f60: 7175 6520 6964 656e 7469 6669 6572 2066  que identifier f
+00026f70: 6f72 2074 6865 2074 6172 6765 7420 6d65  or the target me
+00026f80: 7373 6167 6520 7468 7265 6164 2028 746f  ssage thread (to
+00026f90: 7069 6329 206f 6620 7468 6520 666f 7275  pic) of the foru
+00026fa0: 6d3b 2066 6f72 2066 6f72 756d 2073 7570  m; for forum sup
+00026fb0: 6572 6772 6f75 7073 206f 6e6c 790a 0a20  ergroups only.. 
+00026fc0: 2020 2020 2020 2020 2020 2064 6973 6162             disab
+00026fd0: 6c65 5f6e 6f74 6966 6963 6174 696f 6e20  le_notification 
+00026fe0: 2860 6062 6f6f 6c60 602c 202a 6f70 7469  (``bool``, *opti
+00026ff0: 6f6e 616c 2a29 3a0a 2020 2020 2020 2020  onal*):.        
+00027000: 2020 2020 2020 2020 5365 6e64 7320 7468          Sends th
+00027010: 6520 6d65 7373 6167 6520 7369 6c65 6e74  e message silent
+00027020: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
+00027030: 2020 2020 5573 6572 7320 7769 6c6c 2072      Users will r
+00027040: 6563 6569 7665 2061 206e 6f74 6966 6963  eceive a notific
+00027050: 6174 696f 6e20 7769 7468 206e 6f20 736f  ation with no so
+00027060: 756e 642e 0a0a 2020 2020 2020 2020 2020  und...          
+00027070: 2020 7072 6f74 6563 745f 636f 6e74 656e    protect_conten
+00027080: 7420 2860 6062 6f6f 6c60 602c 202a 6f70  t (``bool``, *op
+00027090: 7469 6f6e 616c 2a29 3a0a 2020 2020 2020  tional*):.      
+000270a0: 2020 2020 2020 2020 2020 5072 6f74 6563            Protec
+000270b0: 7473 2074 6865 2063 6f6e 7465 6e74 7320  ts the contents 
+000270c0: 6f66 2074 6865 2073 656e 7420 6d65 7373  of the sent mess
+000270d0: 6167 6520 6672 6f6d 2066 6f72 7761 7264  age from forward
+000270e0: 696e 6720 616e 6420 7361 7669 6e67 2e0a  ing and saving..
+000270f0: 0a20 2020 2020 2020 2020 2020 2064 726f  .            dro
+00027100: 705f 6175 7468 6f72 2028 6060 626f 6f6c  p_author (``bool
+00027110: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
+00027120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027130: 2057 6865 7468 6572 2074 6f20 666f 7277   Whether to forw
+00027140: 6172 6420 6d65 7373 6167 6573 2077 6974  ard messages wit
+00027150: 686f 7574 2071 756f 7469 6e67 2074 6865  hout quoting the
+00027160: 206f 7269 6769 6e61 6c20 6175 7468 6f72   original author
+00027170: 2e0a 0a20 2020 2020 2020 2020 2020 2064  ...            d
+00027180: 726f 705f 6d65 6469 615f 6361 7074 696f  rop_media_captio
+00027190: 6e73 2028 6060 626f 6f6c 6060 2c20 2a6f  ns (``bool``, *o
+000271a0: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
+000271b0: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+000271c0: 6572 2074 6f20 7374 7269 7020 6361 7074  er to strip capt
+000271d0: 696f 6e73 2066 726f 6d20 6d65 6469 612e  ions from media.
+000271e0: 0a0a 2020 2020 2020 2020 2020 2020 7363  ..            sc
+000271f0: 6865 6475 6c65 5f64 6174 6520 283a 7079  hedule_date (:py
+00027200: 3a6f 626a 3a60 7e64 6174 6574 696d 652e  :obj:`~datetime.
+00027210: 6461 7465 7469 6d65 602c 202a 6f70 7469  datetime`, *opti
+00027220: 6f6e 616c 2a29 3a0a 2020 2020 2020 2020  onal*):.        
+00027230: 2020 2020 2020 2020 4461 7465 2077 6865          Date whe
+00027240: 6e20 7468 6520 6d65 7373 6167 6520 7769  n the message wi
+00027250: 6c6c 2062 6520 6175 746f 6d61 7469 6361  ll be automatica
+00027260: 6c6c 7920 7365 6e74 2e0a 0a20 2020 2020  lly sent...     
+00027270: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00027280: 2020 2020 2020 2020 4f6e 2073 7563 6365          On succe
+00027290: 7373 2c20 7468 6520 666f 7277 6172 6465  ss, the forwarde
+000272a0: 6420 4d65 7373 6167 6520 6973 2072 6574  d Message is ret
+000272b0: 7572 6e65 642e 0a0a 2020 2020 2020 2020  urned...        
+000272c0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+000272d0: 2020 2020 5250 4345 7272 6f72 3a20 496e      RPCError: In
+000272e0: 2063 6173 6520 6f66 2061 2054 656c 6567   case of a Teleg
+000272f0: 7261 6d20 5250 4320 6572 726f 722e 0a20  ram RPC error.. 
+00027300: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00027310: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+00027320: 7365 6c66 2e5f 636c 6965 6e74 2e66 6f72  self._client.for
+00027330: 7761 7264 5f6d 6573 7361 6765 7328 0a20  ward_messages(. 
+00027340: 2020 2020 2020 2020 2020 2066 726f 6d5f             from_
+00027350: 6368 6174 5f69 643d 7365 6c66 2e63 6861  chat_id=self.cha
+00027360: 742e 6964 2c0a 2020 2020 2020 2020 2020  t.id,.          
+00027370: 2020 6d65 7373 6167 655f 6964 733d 7365    message_ids=se
+00027380: 6c66 2e69 642c 0a20 2020 2020 2020 2020  lf.id,.         
+00027390: 2020 2063 6861 745f 6964 3d63 6861 745f     chat_id=chat_
+000273a0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+000273b0: 6d65 7373 6167 655f 7468 7265 6164 5f69  message_thread_i
+000273c0: 643d 6d65 7373 6167 655f 7468 7265 6164  d=message_thread
+000273d0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+000273e0: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
+000273f0: 6174 696f 6e3d 6469 7361 626c 655f 6e6f  ation=disable_no
+00027400: 7469 6669 6361 7469 6f6e 2c0a 2020 2020  tification,.    
+00027410: 2020 2020 2020 2020 7072 6f74 6563 745f          protect_
+00027420: 636f 6e74 656e 743d 7072 6f74 6563 745f  content=protect_
+00027430: 636f 6e74 656e 742c 0a20 2020 2020 2020  content,.       
+00027440: 2020 2020 2064 726f 705f 6175 7468 6f72       drop_author
+00027450: 3d64 726f 705f 6175 7468 6f72 2c0a 2020  =drop_author,.  
+00027460: 2020 2020 2020 2020 2020 6472 6f70 5f6d            drop_m
+00027470: 6564 6961 5f63 6170 7469 6f6e 733d 6472  edia_captions=dr
+00027480: 6f70 5f6d 6564 6961 5f63 6170 7469 6f6e  op_media_caption
+00027490: 732c 0a20 2020 2020 2020 2020 2020 2073  s,.            s
+000274a0: 6368 6564 756c 655f 6461 7465 3d73 6368  chedule_date=sch
+000274b0: 6564 756c 655f 6461 7465 0a20 2020 2020  edule_date.     
+000274c0: 2020 2029 0a0a 2020 2020 6173 796e 6320     )..    async 
+000274d0: 6465 6620 636f 7079 280a 2020 2020 2020  def copy(.      
+000274e0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000274f0: 6368 6174 5f69 643a 2055 6e69 6f6e 5b69  chat_id: Union[i
+00027500: 6e74 2c20 7374 725d 2c0a 2020 2020 2020  nt, str],.      
+00027510: 2020 6361 7074 696f 6e3a 2073 7472 203d    caption: str =
+00027520: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
+00027530: 6172 7365 5f6d 6f64 653a 204f 7074 696f  arse_mode: Optio
+00027540: 6e61 6c5b 2265 6e75 6d73 2e50 6172 7365  nal["enums.Parse
+00027550: 4d6f 6465 225d 203d 204e 6f6e 652c 0a20  Mode"] = None,. 
+00027560: 2020 2020 2020 2063 6170 7469 6f6e 5f65         caption_e
+00027570: 6e74 6974 6965 733a 204c 6973 745b 2274  ntities: List["t
+00027580: 7970 6573 2e4d 6573 7361 6765 456e 7469  ypes.MessageEnti
+00027590: 7479 225d 203d 204e 6f6e 652c 0a20 2020  ty"] = None,.   
+000275a0: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
+000275b0: 6966 6963 6174 696f 6e3a 2062 6f6f 6c20  ification: bool 
+000275c0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000275d0: 7265 706c 795f 7061 7261 6d65 7465 7273  reply_parameters
+000275e0: 3a20 2274 7970 6573 2e52 6570 6c79 5061  : "types.ReplyPa
+000275f0: 7261 6d65 7465 7273 2220 3d20 4e6f 6e65  rameters" = None
+00027600: 2c0a 2020 2020 2020 2020 7265 706c 795f  ,.        reply_
+00027610: 6d61 726b 7570 3a20 556e 696f 6e5b 0a20  markup: Union[. 
+00027620: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00027630: 732e 496e 6c69 6e65 4b65 7962 6f61 7264  s.InlineKeyboard
+00027640: 4d61 726b 7570 222c 0a20 2020 2020 2020  Markup",.       
+00027650: 2020 2020 2022 7479 7065 732e 5265 706c       "types.Repl
+00027660: 794b 6579 626f 6172 644d 6172 6b75 7022  yKeyboardMarkup"
+00027670: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+00027680: 7970 6573 2e52 6570 6c79 4b65 7962 6f61  ypes.ReplyKeyboa
+00027690: 7264 5265 6d6f 7665 222c 0a20 2020 2020  rdRemove",.     
+000276a0: 2020 2020 2020 2022 7479 7065 732e 466f         "types.Fo
+000276b0: 7263 6552 6570 6c79 220a 2020 2020 2020  rceReply".      
+000276c0: 2020 5d20 3d20 6f62 6a65 6374 2c0a 2020    ] = object,.  
+000276d0: 2020 2020 2020 7265 706c 795f 746f 5f6d        reply_to_m
+000276e0: 6573 7361 6765 5f69 643a 2069 6e74 203d  essage_id: int =
+000276f0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+00027700: 6368 6564 756c 655f 6461 7465 3a20 6461  chedule_date: da
+00027710: 7465 7469 6d65 203d 204e 6f6e 650a 2020  tetime = None.  
+00027720: 2020 2920 2d3e 2055 6e69 6f6e 5b22 7479    ) -> Union["ty
+00027730: 7065 732e 4d65 7373 6167 6522 2c20 4c69  pes.Message", Li
+00027740: 7374 5b22 7479 7065 732e 4d65 7373 6167  st["types.Messag
+00027750: 6522 5d5d 3a0a 2020 2020 2020 2020 2222  e"]]:.        ""
+00027760: 2242 6f75 6e64 206d 6574 686f 6420 2a63  "Bound method *c
+00027770: 6f70 792a 206f 6620 3a6f 626a 3a60 7e70  opy* of :obj:`~p
+00027780: 7972 6f67 7261 6d2e 7479 7065 732e 4d65  yrogram.types.Me
+00027790: 7373 6167 6560 2e0a 0a20 2020 2020 2020  ssage`...       
+000277a0: 2055 7365 2061 7320 6120 7368 6f72 7463   Use as a shortc
+000277b0: 7574 2066 6f72 3a0a 0a20 2020 2020 2020  ut for:..       
+000277c0: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+000277d0: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+000277e0: 2020 2020 2061 7761 6974 2063 6c69 656e       await clien
+000277f0: 742e 636f 7079 5f6d 6573 7361 6765 280a  t.copy_message(.
+00027800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027810: 6368 6174 5f69 643d 6368 6174 5f69 642c  chat_id=chat_id,
+00027820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027830: 2066 726f 6d5f 6368 6174 5f69 643d 6d65   from_chat_id=me
+00027840: 7373 6167 652e 6368 6174 2e69 642c 0a20  ssage.chat.id,. 
+00027850: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00027860: 6573 7361 6765 5f69 643d 6d65 7373 6167  essage_id=messag
+00027870: 652e 6964 0a20 2020 2020 2020 2020 2020  e.id.           
+00027880: 2029 0a0a 2020 2020 2020 2020 4578 616d   )..        Exam
+00027890: 706c 653a 0a20 2020 2020 2020 2020 2020  ple:.           
+000278a0: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+000278b0: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+000278c0: 2020 2020 2020 2020 2061 7761 6974 206d           await m
+000278d0: 6573 7361 6765 2e63 6f70 7928 6368 6174  essage.copy(chat
+000278e0: 5f69 6429 0a0a 2020 2020 2020 2020 5061  _id)..        Pa
+000278f0: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
+00027900: 2020 2020 2020 6368 6174 5f69 6420 2860        chat_id (`
+00027910: 6069 6e74 6060 207c 2060 6073 7472 6060  `int`` | ``str``
+00027920: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00027930: 2020 2055 6e69 7175 6520 6964 656e 7469     Unique identi
+00027940: 6669 6572 2028 696e 7429 206f 7220 7573  fier (int) or us
+00027950: 6572 6e61 6d65 2028 7374 7229 206f 6620  ername (str) of 
+00027960: 7468 6520 7461 7267 6574 2063 6861 742e  the target chat.
+00027970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027980: 2046 6f72 2079 6f75 7220 7065 7273 6f6e   For your person
+00027990: 616c 2063 6c6f 7564 2028 5361 7665 6420  al cloud (Saved 
+000279a0: 4d65 7373 6167 6573 2920 796f 7520 6361  Messages) you ca
+000279b0: 6e20 7369 6d70 6c79 2075 7365 2022 6d65  n simply use "me
+000279c0: 2220 6f72 2022 7365 6c66 222e 0a20 2020  " or "self"..   
+000279d0: 2020 2020 2020 2020 2020 2020 2046 6f72               For
+000279e0: 2061 2063 6f6e 7461 6374 2074 6861 7420   a contact that 
+000279f0: 6578 6973 7473 2069 6e20 796f 7572 2054  exists in your T
+00027a00: 656c 6567 7261 6d20 6164 6472 6573 7320  elegram address 
+00027a10: 626f 6f6b 2079 6f75 2063 616e 2075 7365  book you can use
+00027a20: 2068 6973 2070 686f 6e65 206e 756d 6265   his phone numbe
+00027a30: 7220 2873 7472 292e 0a0a 2020 2020 2020  r (str)...      
+00027a40: 2020 2020 2020 6361 7074 696f 6e20 2860        caption (`
+00027a50: 6073 7472 696e 6760 602c 202a 6f70 7469  `string``, *opti
+00027a60: 6f6e 616c 2a29 3a0a 2020 2020 2020 2020  onal*):.        
+00027a70: 2020 2020 2020 2020 4e65 7720 6361 7074          New capt
+00027a80: 696f 6e20 666f 7220 6d65 6469 612c 2030  ion for media, 0
+00027a90: 2d31 3032 3420 6368 6172 6163 7465 7273  -1024 characters
+00027aa0: 2061 6674 6572 2065 6e74 6974 6965 7320   after entities 
+00027ab0: 7061 7273 696e 672e 0a20 2020 2020 2020  parsing..       
+00027ac0: 2020 2020 2020 2020 2049 6620 6e6f 7420           If not 
+00027ad0: 7370 6563 6966 6965 642c 2074 6865 206f  specified, the o
+00027ae0: 7269 6769 6e61 6c20 6361 7074 696f 6e20  riginal caption 
+00027af0: 6973 206b 6570 742e 0a20 2020 2020 2020  is kept..       
+00027b00: 2020 2020 2020 2020 2050 6173 7320 2222           Pass ""
+00027b10: 2028 656d 7074 7920 7374 7269 6e67 2920   (empty string) 
+00027b20: 746f 2072 656d 6f76 6520 7468 6520 6361  to remove the ca
+00027b30: 7074 696f 6e2e 0a0a 2020 2020 2020 2020  ption...        
+00027b40: 2020 2020 7061 7273 655f 6d6f 6465 2028      parse_mode (
+00027b50: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
+00027b60: 656e 756d 732e 5061 7273 654d 6f64 6560  enums.ParseMode`
+00027b70: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
+00027b80: 2020 2020 2020 2020 2020 2020 2020 2042                 B
+00027b90: 7920 6465 6661 756c 742c 2074 6578 7473  y default, texts
+00027ba0: 2061 7265 2070 6172 7365 6420 7573 696e   are parsed usin
+00027bb0: 6720 626f 7468 204d 6172 6b64 6f77 6e20  g both Markdown 
+00027bc0: 616e 6420 4854 4d4c 2073 7479 6c65 732e  and HTML styles.
+00027bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027be0: 2059 6f75 2063 616e 2063 6f6d 6269 6e65   You can combine
+00027bf0: 2062 6f74 6820 7379 6e74 6178 6573 2074   both syntaxes t
+00027c00: 6f67 6574 6865 722e 0a0a 2020 2020 2020  ogether...      
+00027c10: 2020 2020 2020 6361 7074 696f 6e5f 656e        caption_en
+00027c20: 7469 7469 6573 2028 4c69 7374 206f 6620  tities (List of 
+00027c30: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
+00027c40: 7479 7065 732e 4d65 7373 6167 6545 6e74  types.MessageEnt
+00027c50: 6974 7960 293a 0a20 2020 2020 2020 2020  ity`):.         
+00027c60: 2020 2020 2020 204c 6973 7420 6f66 2073         List of s
+00027c70: 7065 6369 616c 2065 6e74 6974 6965 7320  pecial entities 
+00027c80: 7468 6174 2061 7070 6561 7220 696e 2074  that appear in t
+00027c90: 6865 206e 6577 2063 6170 7469 6f6e 2c20  he new caption, 
+00027ca0: 7768 6963 6820 6361 6e20 6265 2073 7065  which can be spe
+00027cb0: 6369 6669 6564 2069 6e73 7465 6164 206f  cified instead o
+00027cc0: 6620 2a70 6172 7365 5f6d 6f64 652a 2e0a  f *parse_mode*..
+00027cd0: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00027ce0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00027cf0: 6e20 2860 6062 6f6f 6c60 602c 202a 6f70  n (``bool``, *op
+00027d00: 7469 6f6e 616c 2a29 3a0a 2020 2020 2020  tional*):.      
+00027d10: 2020 2020 2020 2020 2020 5365 6e64 7320            Sends 
+00027d20: 7468 6520 6d65 7373 6167 6520 7369 6c65  the message sile
+00027d30: 6e74 6c79 2e0a 2020 2020 2020 2020 2020  ntly..          
+00027d40: 2020 2020 2020 5573 6572 7320 7769 6c6c        Users will
+00027d50: 2072 6563 6569 7665 2061 206e 6f74 6966   receive a notif
+00027d60: 6963 6174 696f 6e20 7769 7468 206e 6f20  ication with no 
+00027d70: 736f 756e 642e 0a0a 2020 2020 2020 2020  sound...        
+00027d80: 2020 2020 7265 706c 795f 7061 7261 6d65      reply_parame
+00027d90: 7465 7273 2028 3a6f 626a 3a60 7e70 7972  ters (:obj:`~pyr
+00027da0: 6f67 7261 6d2e 7479 7065 732e 5265 706c  ogram.types.Repl
+00027db0: 7950 6172 616d 6574 6572 7360 2c20 2a6f  yParameters`, *o
+00027dc0: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
+00027dd0: 2020 2020 2020 2020 2020 2044 6573 6372             Descr
+00027de0: 6970 7469 6f6e 206f 6620 7468 6520 6d65  iption of the me
+00027df0: 7373 6167 6520 746f 2072 6570 6c79 2074  ssage to reply t
+00027e00: 6f0a 0a20 2020 2020 2020 2020 2020 2072  o..            r
+00027e10: 6570 6c79 5f6d 6172 6b75 7020 283a 6f62  eply_markup (:ob
+00027e20: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
+00027e30: 6573 2e49 6e6c 696e 654b 6579 626f 6172  es.InlineKeyboar
+00027e40: 644d 6172 6b75 7060 207c 203a 6f62 6a3a  dMarkup` | :obj:
+00027e50: 607e 7079 726f 6772 616d 2e74 7970 6573  `~pyrogram.types
+00027e60: 2e52 6570 6c79 4b65 7962 6f61 7264 4d61  .ReplyKeyboardMa
+00027e70: 726b 7570 6020 7c20 3a6f 626a 3a60 7e70  rkup` | :obj:`~p
+00027e80: 7972 6f67 7261 6d2e 7479 7065 732e 5265  yrogram.types.Re
+00027e90: 706c 794b 6579 626f 6172 6452 656d 6f76  plyKeyboardRemov
+00027ea0: 6560 207c 203a 6f62 6a3a 607e 7079 726f  e` | :obj:`~pyro
+00027eb0: 6772 616d 2e74 7970 6573 2e46 6f72 6365  gram.types.Force
+00027ec0: 5265 706c 7960 2c20 2a6f 7074 696f 6e61  Reply`, *optiona
+00027ed0: 6c2a 293a 0a20 2020 2020 2020 2020 2020  l*):.           
+00027ee0: 2020 2020 2041 6464 6974 696f 6e61 6c20       Additional 
+00027ef0: 696e 7465 7266 6163 6520 6f70 7469 6f6e  interface option
+00027f00: 732e 2041 6e20 6f62 6a65 6374 2066 6f72  s. An object for
+00027f10: 2061 6e20 696e 6c69 6e65 206b 6579 626f   an inline keybo
+00027f20: 6172 642c 2063 7573 746f 6d20 7265 706c  ard, custom repl
+00027f30: 7920 6b65 7962 6f61 7264 2c0a 2020 2020  y keyboard,.    
+00027f40: 2020 2020 2020 2020 2020 2020 696e 7374              inst
+00027f50: 7275 6374 696f 6e73 2074 6f20 7265 6d6f  ructions to remo
+00027f60: 7665 2072 6570 6c79 206b 6579 626f 6172  ve reply keyboar
+00027f70: 6420 6f72 2074 6f20 666f 7263 6520 6120  d or to force a 
+00027f80: 7265 706c 7920 6672 6f6d 2074 6865 2075  reply from the u
+00027f90: 7365 722e 0a20 2020 2020 2020 2020 2020  ser..           
+00027fa0: 2020 2020 2049 6620 6e6f 7420 7370 6563       If not spec
+00027fb0: 6966 6965 642c 2074 6865 206f 7269 6769  ified, the origi
+00027fc0: 6e61 6c20 7265 706c 7920 6d61 726b 7570  nal reply markup
+00027fd0: 2069 7320 6b65 7074 2e0a 2020 2020 2020   is kept..      
+00027fe0: 2020 2020 2020 2020 2020 5061 7373 204e            Pass N
+00027ff0: 6f6e 6520 746f 2072 656d 6f76 6520 7468  one to remove th
+00028000: 6520 7265 706c 7920 6d61 726b 7570 2e0a  e reply markup..
+00028010: 0a20 2020 2020 2020 2020 2020 2073 6368  .            sch
+00028020: 6564 756c 655f 6461 7465 2028 3a70 793a  edule_date (:py:
+00028030: 6f62 6a3a 607e 6461 7465 7469 6d65 2e64  obj:`~datetime.d
+00028040: 6174 6574 696d 6560 2c20 2a6f 7074 696f  atetime`, *optio
+00028050: 6e61 6c2a 293a 0a20 2020 2020 2020 2020  nal*):.         
+00028060: 2020 2020 2020 2044 6174 6520 7768 656e         Date when
+00028070: 2074 6865 206d 6573 7361 6765 2077 696c   the message wil
+00028080: 6c20 6265 2061 7574 6f6d 6174 6963 616c  l be automatical
+00028090: 6c79 2073 656e 742e 0a0a 2020 2020 2020  ly sent...      
+000280a0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+000280b0: 2020 2020 2020 203a 6f62 6a3a 607e 7079         :obj:`~py
+000280c0: 726f 6772 616d 2e74 7970 6573 2e4d 6573  rogram.types.Mes
+000280d0: 7361 6765 603a 204f 6e20 7375 6363 6573  sage`: On succes
+000280e0: 732c 2074 6865 2063 6f70 6965 6420 6d65  s, the copied me
+000280f0: 7373 6167 6520 6973 2072 6574 7572 6e65  ssage is returne
+00028100: 642e 0a0a 2020 2020 2020 2020 5261 6973  d...        Rais
+00028110: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00028120: 5250 4345 7272 6f72 3a20 496e 2063 6173  RPCError: In cas
+00028130: 6520 6f66 2061 2054 656c 6567 7261 6d20  e of a Telegram 
+00028140: 5250 4320 6572 726f 722e 0a20 2020 2020  RPC error..     
+00028150: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00028160: 6620 7365 6c66 2e73 6572 7669 6365 3a0a  f self.service:.
+00028170: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
+00028180: 7761 726e 696e 6728 2253 6572 7669 6365  warning("Service
+00028190: 206d 6573 7361 6765 7320 6361 6e6e 6f74   messages cannot
+000281a0: 2062 6520 636f 7069 6564 2e20 6368 6174   be copied. chat
+000281b0: 5f69 643a 2025 732c 206d 6573 7361 6765  _id: %s, message
+000281c0: 5f69 643a 2025 7322 2c0a 2020 2020 2020  _id: %s",.      
+000281d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000281e0: 2020 7365 6c66 2e63 6861 742e 6964 2c20    self.chat.id, 
+000281f0: 7365 6c66 2e69 6429 0a20 2020 2020 2020  self.id).       
+00028200: 2065 6c69 6620 7365 6c66 2e67 616d 6520   elif self.game 
+00028210: 616e 6420 6e6f 7420 7365 6c66 2e5f 636c  and not self._cl
+00028220: 6965 6e74 2e6d 652e 6973 5f62 6f74 3a0a  ient.me.is_bot:.
+00028230: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
+00028240: 7761 726e 696e 6728 2255 7365 7273 2063  warning("Users c
+00028250: 616e 6e6f 7420 7365 6e64 206d 6573 7361  annot send messa
+00028260: 6765 7320 7769 7468 2047 616d 6520 6d65  ges with Game me
+00028270: 6469 6120 7479 7065 2e20 6368 6174 5f69  dia type. chat_i
+00028280: 643a 2025 732c 206d 6573 7361 6765 5f69  d: %s, message_i
+00028290: 643a 2025 7322 2c0a 2020 2020 2020 2020  d: %s",.        
 000282a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000282b0: 2020 206c 6173 745f 6e61 6d65 3d73 656c     last_name=sel
-000282c0: 662e 636f 6e74 6163 742e 6c61 7374 5f6e  f.contact.last_n
-000282d0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-000282e0: 2020 2020 2020 2020 2076 6361 7264 3d73           vcard=s
-000282f0: 656c 662e 636f 6e74 6163 742e 7663 6172  elf.contact.vcar
-00028300: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00028310: 2020 2020 2020 2064 6973 6162 6c65 5f6e         disable_n
-00028320: 6f74 6966 6963 6174 696f 6e3d 6469 7361  otification=disa
-00028330: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00028340: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00028350: 2020 2020 2020 7265 706c 795f 7061 7261        reply_para
-00028360: 6d65 7465 7273 3d72 6570 6c79 5f70 6172  meters=reply_par
-00028370: 616d 6574 6572 732c 0a20 2020 2020 2020  ameters,.       
-00028380: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-00028390: 7361 6765 5f74 6872 6561 645f 6964 3d73  sage_thread_id=s
-000283a0: 656c 662e 6d65 7373 6167 655f 7468 7265  elf.message_thre
-000283b0: 6164 5f69 642c 0a20 2020 2020 2020 2020  ad_id,.         
-000283c0: 2020 2020 2020 2020 2020 2062 7573 696e             busin
-000283d0: 6573 735f 636f 6e6e 6563 7469 6f6e 5f69  ess_connection_i
-000283e0: 643d 7365 6c66 2e62 7573 696e 6573 735f  d=self.business_
-000283f0: 636f 6e6e 6563 7469 6f6e 5f69 642c 0a20  connection_id,. 
-00028400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028410: 2020 2073 6368 6564 756c 655f 6461 7465     schedule_date
-00028420: 3d73 6368 6564 756c 655f 6461 7465 2c0a  =schedule_date,.
-00028430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028440: 2020 2020 7072 6f74 6563 745f 636f 6e74      protect_cont
-00028450: 656e 743d 7365 6c66 2e68 6173 5f70 726f  ent=self.has_pro
-00028460: 7465 6374 6564 5f63 6f6e 7465 6e74 2c0a  tected_content,.
-00028470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028480: 2020 2020 7265 706c 795f 746f 5f6d 6573      reply_to_mes
-00028490: 7361 6765 5f69 643d 7265 706c 795f 746f  sage_id=reply_to
-000284a0: 5f6d 6573 7361 6765 5f69 642c 0a20 2020  _message_id,.   
-000284b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000284c0: 2072 6570 6c79 5f6d 6172 6b75 703d 7265   reply_markup=re
-000284d0: 706c 795f 6d61 726b 7570 0a20 2020 2020  ply_markup.     
-000284e0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000284f0: 2020 2020 2020 2020 2065 6c69 6620 7365           elif se
-00028500: 6c66 2e6c 6f63 6174 696f 6e3a 0a20 2020  lf.location:.   
-00028510: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00028520: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
-00028530: 636c 6965 6e74 2e73 656e 645f 6c6f 6361  client.send_loca
-00028540: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-00028550: 2020 2020 2020 2020 2020 6368 6174 5f69            chat_i
-00028560: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00028570: 2020 2020 2020 206c 6174 6974 7564 653d         latitude=
-00028580: 7365 6c66 2e6c 6f63 6174 696f 6e2e 6c61  self.location.la
-00028590: 7469 7475 6465 2c0a 2020 2020 2020 2020  titude,.        
-000285a0: 2020 2020 2020 2020 2020 2020 6c6f 6e67              long
-000285b0: 6974 7564 653d 7365 6c66 2e6c 6f63 6174  itude=self.locat
-000285c0: 696f 6e2e 6c6f 6e67 6974 7564 652c 0a20  ion.longitude,. 
-000285d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000285e0: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
-000285f0: 6963 6174 696f 6e3d 6469 7361 626c 655f  ication=disable_
-00028600: 6e6f 7469 6669 6361 7469 6f6e 2c0a 2020  notification,.  
-00028610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028620: 2020 7265 706c 795f 7061 7261 6d65 7465    reply_paramete
-00028630: 7273 3d72 6570 6c79 5f70 6172 616d 6574  rs=reply_paramet
-00028640: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
-00028650: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00028660: 5f74 6872 6561 645f 6964 3d73 656c 662e  _thread_id=self.
-00028670: 6d65 7373 6167 655f 7468 7265 6164 5f69  message_thread_i
-00028680: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00028690: 2020 2020 2020 2062 7573 696e 6573 735f         business_
-000286a0: 636f 6e6e 6563 7469 6f6e 5f69 643d 7365  connection_id=se
-000286b0: 6c66 2e62 7573 696e 6573 735f 636f 6e6e  lf.business_conn
-000286c0: 6563 7469 6f6e 5f69 642c 0a20 2020 2020  ection_id,.     
-000286d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000286e0: 6368 6564 756c 655f 6461 7465 3d73 6368  chedule_date=sch
-000286f0: 6564 756c 655f 6461 7465 2c0a 2020 2020  edule_date,.    
-00028700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028710: 7072 6f74 6563 745f 636f 6e74 656e 743d  protect_content=
-00028720: 7365 6c66 2e68 6173 5f70 726f 7465 6374  self.has_protect
-00028730: 6564 5f63 6f6e 7465 6e74 2c0a 2020 2020  ed_content,.    
-00028740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028750: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-00028760: 5f69 643d 7265 706c 795f 746f 5f6d 6573  _id=reply_to_mes
-00028770: 7361 6765 5f69 642c 0a20 2020 2020 2020  sage_id,.       
-00028780: 2020 2020 2020 2020 2020 2020 2072 6570               rep
-00028790: 6c79 5f6d 6172 6b75 703d 7265 706c 795f  ly_markup=reply_
-000287a0: 6d61 726b 7570 0a20 2020 2020 2020 2020  markup.         
-000287b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000287c0: 2020 2020 2065 6c69 6620 7365 6c66 2e76       elif self.v
-000287d0: 656e 7565 3a0a 2020 2020 2020 2020 2020  enue:.          
-000287e0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-000287f0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-00028800: 7365 6e64 5f76 656e 7565 280a 2020 2020  send_venue(.    
-00028810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028820: 6368 6174 5f69 642c 0a20 2020 2020 2020  chat_id,.       
-00028830: 2020 2020 2020 2020 2020 2020 206c 6174               lat
-00028840: 6974 7564 653d 7365 6c66 2e76 656e 7565  itude=self.venue
-00028850: 2e6c 6f63 6174 696f 6e2e 6c61 7469 7475  .location.latitu
-00028860: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
-00028870: 2020 2020 2020 2020 6c6f 6e67 6974 7564          longitud
-00028880: 653d 7365 6c66 2e76 656e 7565 2e6c 6f63  e=self.venue.loc
-00028890: 6174 696f 6e2e 6c6f 6e67 6974 7564 652c  ation.longitude,
-000288a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000288b0: 2020 2020 2074 6974 6c65 3d73 656c 662e       title=self.
-000288c0: 7665 6e75 652e 7469 746c 652c 0a20 2020  venue.title,.   
-000288d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000288e0: 2061 6464 7265 7373 3d73 656c 662e 7665   address=self.ve
-000288f0: 6e75 652e 6164 6472 6573 732c 0a20 2020  nue.address,.   
-00028900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028910: 2066 6f75 7273 7175 6172 655f 6964 3d73   foursquare_id=s
-00028920: 656c 662e 7665 6e75 652e 666f 7572 7371  elf.venue.foursq
-00028930: 7561 7265 5f69 642c 0a20 2020 2020 2020  uare_id,.       
-00028940: 2020 2020 2020 2020 2020 2020 2066 6f75               fou
-00028950: 7273 7175 6172 655f 7479 7065 3d73 656c  rsquare_type=sel
-00028960: 662e 7665 6e75 652e 666f 7572 7371 7561  f.venue.foursqua
-00028970: 7265 5f74 7970 652c 0a20 2020 2020 2020  re_type,.       
-00028980: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00028990: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-000289a0: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
-000289b0: 6361 7469 6f6e 2c0a 2020 2020 2020 2020  cation,.        
-000289c0: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-000289d0: 795f 7061 7261 6d65 7465 7273 3d72 6570  y_parameters=rep
-000289e0: 6c79 5f70 6172 616d 6574 6572 732c 0a20  ly_parameters,. 
-000289f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028a00: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
-00028a10: 645f 6964 3d73 656c 662e 6d65 7373 6167  d_id=self.messag
-00028a20: 655f 7468 7265 6164 5f69 642c 0a20 2020  e_thread_id,.   
-00028a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028a40: 2062 7573 696e 6573 735f 636f 6e6e 6563   business_connec
-00028a50: 7469 6f6e 5f69 643d 7365 6c66 2e62 7573  tion_id=self.bus
-00028a60: 696e 6573 735f 636f 6e6e 6563 7469 6f6e  iness_connection
-00028a70: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-00028a80: 2020 2020 2020 2020 2073 6368 6564 756c           schedul
-00028a90: 655f 6461 7465 3d73 6368 6564 756c 655f  e_date=schedule_
-00028aa0: 6461 7465 2c0a 2020 2020 2020 2020 2020  date,.          
-00028ab0: 2020 2020 2020 2020 2020 7072 6f74 6563            protec
-00028ac0: 745f 636f 6e74 656e 743d 7365 6c66 2e68  t_content=self.h
-00028ad0: 6173 5f70 726f 7465 6374 6564 5f63 6f6e  as_protected_con
-00028ae0: 7465 6e74 2c0a 2020 2020 2020 2020 2020  tent,.          
-00028af0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
-00028b00: 746f 5f6d 6573 7361 6765 5f69 643d 7265  to_message_id=re
-00028b10: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00028b20: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00028b30: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
-00028b40: 6b75 703d 7265 706c 795f 6d61 726b 7570  kup=reply_markup
-00028b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028b60: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
-00028b70: 6c69 6620 7365 6c66 2e70 6f6c 6c3a 0a20  lif self.poll:. 
-00028b80: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00028b90: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-00028ba0: 2e5f 636c 6965 6e74 2e73 656e 645f 706f  ._client.send_po
-00028bb0: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
-00028bc0: 2020 2020 2020 2020 6368 6174 5f69 642c          chat_id,
-00028bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028be0: 2020 2020 2071 7565 7374 696f 6e3d 7365       question=se
-00028bf0: 6c66 2e70 6f6c 6c2e 7175 6573 7469 6f6e  lf.poll.question
-00028c00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00028c10: 2020 2020 2020 6f70 7469 6f6e 733d 5b6f        options=[o
-00028c20: 7074 2e74 6578 7420 666f 7220 6f70 7420  pt.text for opt 
-00028c30: 696e 2073 656c 662e 706f 6c6c 2e6f 7074  in self.poll.opt
-00028c40: 696f 6e73 5d2c 0a20 2020 2020 2020 2020  ions],.         
-00028c50: 2020 2020 2020 2020 2020 2069 735f 616e             is_an
-00028c60: 6f6e 796d 6f75 733d 7365 6c66 2e70 6f6c  onymous=self.pol
-00028c70: 6c2e 6973 5f61 6e6f 6e79 6d6f 7573 2c0a  l.is_anonymous,.
+000282b0: 7365 6c66 2e63 6861 742e 6964 2c20 7365  self.chat.id, se
+000282c0: 6c66 2e69 6429 0a20 2020 2020 2020 2065  lf.id).        e
+000282d0: 6c69 6620 7365 6c66 2e65 6d70 7479 3a0a  lif self.empty:.
+000282e0: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
+000282f0: 7761 726e 696e 6728 2245 6d70 7479 206d  warning("Empty m
+00028300: 6573 7361 6765 7320 6361 6e6e 6f74 2062  essages cannot b
+00028310: 6520 636f 7069 6564 2e22 290a 2020 2020  e copied.").    
+00028320: 2020 2020 656c 6966 2073 656c 662e 7465      elif self.te
+00028330: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+00028340: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+00028350: 662e 5f63 6c69 656e 742e 7365 6e64 5f6d  f._client.send_m
+00028360: 6573 7361 6765 280a 2020 2020 2020 2020  essage(.        
+00028370: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
+00028380: 6368 6174 5f69 642c 0a20 2020 2020 2020  chat_id,.       
+00028390: 2020 2020 2020 2020 206d 6573 7361 6765           message
+000283a0: 5f74 6872 6561 645f 6964 3d73 656c 662e  _thread_id=self.
+000283b0: 6d65 7373 6167 655f 7468 7265 6164 5f69  message_thread_i
+000283c0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+000283d0: 2020 2062 7573 696e 6573 735f 636f 6e6e     business_conn
+000283e0: 6563 7469 6f6e 5f69 643d 7365 6c66 2e62  ection_id=self.b
+000283f0: 7573 696e 6573 735f 636f 6e6e 6563 7469  usiness_connecti
+00028400: 6f6e 5f69 642c 0a20 2020 2020 2020 2020  on_id,.         
+00028410: 2020 2020 2020 2074 6578 743d 7365 6c66         text=self
+00028420: 2e74 6578 742c 0a20 2020 2020 2020 2020  .text,.         
+00028430: 2020 2020 2020 2070 6172 7365 5f6d 6f64         parse_mod
+00028440: 653d 656e 756d 732e 5061 7273 654d 6f64  e=enums.ParseMod
+00028450: 652e 4449 5341 424c 4544 2c0a 2020 2020  e.DISABLED,.    
+00028460: 2020 2020 2020 2020 2020 2020 656e 7469              enti
+00028470: 7469 6573 3d73 656c 662e 656e 7469 7469  ties=self.entiti
+00028480: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00028490: 2020 2020 6c69 6e6b 5f70 7265 7669 6577      link_preview
+000284a0: 5f6f 7074 696f 6e73 3d73 656c 662e 6c69  _options=self.li
+000284b0: 6e6b 5f70 7265 7669 6577 5f6f 7074 696f  nk_preview_optio
+000284c0: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+000284d0: 2020 2020 6469 7361 626c 655f 6e6f 7469      disable_noti
+000284e0: 6669 6361 7469 6f6e 3d64 6973 6162 6c65  fication=disable
+000284f0: 5f6e 6f74 6966 6963 6174 696f 6e2c 0a20  _notification,. 
+00028500: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00028510: 726f 7465 6374 5f63 6f6e 7465 6e74 3d73  rotect_content=s
+00028520: 656c 662e 6861 735f 7072 6f74 6563 7465  elf.has_protecte
+00028530: 645f 636f 6e74 656e 742c 0a20 2020 2020  d_content,.     
+00028540: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
+00028550: 5f70 6172 616d 6574 6572 733d 7265 706c  _parameters=repl
+00028560: 795f 7061 7261 6d65 7465 7273 2c0a 2020  y_parameters,.  
+00028570: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00028580: 706c 795f 6d61 726b 7570 3d73 656c 662e  ply_markup=self.
+00028590: 7265 706c 795f 6d61 726b 7570 2069 6620  reply_markup if 
+000285a0: 7265 706c 795f 6d61 726b 7570 2069 7320  reply_markup is 
+000285b0: 6f62 6a65 6374 2065 6c73 6520 7265 706c  object else repl
+000285c0: 795f 6d61 726b 7570 2c0a 2020 2020 2020  y_markup,.      
+000285d0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+000285e0: 746f 5f6d 6573 7361 6765 5f69 643d 7265  to_message_id=re
+000285f0: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
+00028600: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00028610: 2020 2073 6368 6564 756c 655f 6461 7465     schedule_date
+00028620: 3d73 6368 6564 756c 655f 6461 7465 0a20  =schedule_date. 
+00028630: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00028640: 2020 2020 2065 6c69 6620 7365 6c66 2e6d       elif self.m
+00028650: 6564 6961 3a0a 2020 2020 2020 2020 2020  edia:.          
+00028660: 2020 7365 6e64 5f6d 6564 6961 203d 2070    send_media = p
+00028670: 6172 7469 616c 280a 2020 2020 2020 2020  artial(.        
+00028680: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
+00028690: 6965 6e74 2e73 656e 645f 6361 6368 6564  ient.send_cached
+000286a0: 5f6d 6564 6961 2c0a 2020 2020 2020 2020  _media,.        
+000286b0: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
+000286c0: 6368 6174 5f69 642c 0a20 2020 2020 2020  chat_id,.       
+000286d0: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
+000286e0: 5f6e 6f74 6966 6963 6174 696f 6e3d 6469  _notification=di
+000286f0: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+00028700: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00028710: 2020 2020 7265 706c 795f 7061 7261 6d65      reply_parame
+00028720: 7465 7273 3d72 6570 6c79 5f70 6172 616d  ters=reply_param
+00028730: 6574 6572 732c 0a20 2020 2020 2020 2020  eters,.         
+00028740: 2020 2020 2020 206d 6573 7361 6765 5f74         message_t
+00028750: 6872 6561 645f 6964 3d73 656c 662e 6d65  hread_id=self.me
+00028760: 7373 6167 655f 7468 7265 6164 5f69 642c  ssage_thread_id,
+00028770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028780: 2062 7573 696e 6573 735f 636f 6e6e 6563   business_connec
+00028790: 7469 6f6e 5f69 643d 7365 6c66 2e62 7573  tion_id=self.bus
+000287a0: 696e 6573 735f 636f 6e6e 6563 7469 6f6e  iness_connection
+000287b0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+000287c0: 2020 2020 2073 6368 6564 756c 655f 6461       schedule_da
+000287d0: 7465 3d73 6368 6564 756c 655f 6461 7465  te=schedule_date
+000287e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000287f0: 2020 7072 6f74 6563 745f 636f 6e74 656e    protect_conten
+00028800: 743d 7365 6c66 2e68 6173 5f70 726f 7465  t=self.has_prote
+00028810: 6374 6564 5f63 6f6e 7465 6e74 2c0a 2020  cted_content,.  
+00028820: 2020 2020 2020 2020 2020 2020 2020 6861                ha
+00028830: 735f 7370 6f69 6c65 723d 7365 6c66 2e68  s_spoiler=self.h
+00028840: 6173 5f6d 6564 6961 5f73 706f 696c 6572  as_media_spoiler
+00028850: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00028860: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
+00028870: 6765 5f69 643d 7265 706c 795f 746f 5f6d  ge_id=reply_to_m
+00028880: 6573 7361 6765 5f69 642c 0a20 2020 2020  essage_id,.     
+00028890: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
+000288a0: 5f6d 6172 6b75 703d 7365 6c66 2e72 6570  _markup=self.rep
+000288b0: 6c79 5f6d 6172 6b75 7020 6966 2072 6570  ly_markup if rep
+000288c0: 6c79 5f6d 6172 6b75 7020 6973 206f 626a  ly_markup is obj
+000288d0: 6563 7420 656c 7365 2072 6570 6c79 5f6d  ect else reply_m
+000288e0: 6172 6b75 700a 2020 2020 2020 2020 2020  arkup.          
+000288f0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00028900: 2069 6620 7365 6c66 2e70 686f 746f 3a0a   if self.photo:.
+00028910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028920: 6669 6c65 5f69 6420 3d20 7365 6c66 2e70  file_id = self.p
+00028930: 686f 746f 2e66 696c 655f 6964 0a20 2020  hoto.file_id.   
+00028940: 2020 2020 2020 2020 2065 6c69 6620 7365           elif se
+00028950: 6c66 2e61 7564 696f 3a0a 2020 2020 2020  lf.audio:.      
+00028960: 2020 2020 2020 2020 2020 6669 6c65 5f69            file_i
+00028970: 6420 3d20 7365 6c66 2e61 7564 696f 2e66  d = self.audio.f
+00028980: 696c 655f 6964 0a20 2020 2020 2020 2020  ile_id.         
+00028990: 2020 2065 6c69 6620 7365 6c66 2e64 6f63     elif self.doc
+000289a0: 756d 656e 743a 0a20 2020 2020 2020 2020  ument:.         
+000289b0: 2020 2020 2020 2066 696c 655f 6964 203d         file_id =
+000289c0: 2073 656c 662e 646f 6375 6d65 6e74 2e66   self.document.f
+000289d0: 696c 655f 6964 0a20 2020 2020 2020 2020  ile_id.         
+000289e0: 2020 2065 6c69 6620 7365 6c66 2e76 6964     elif self.vid
+000289f0: 656f 3a0a 2020 2020 2020 2020 2020 2020  eo:.            
+00028a00: 2020 2020 6669 6c65 5f69 6420 3d20 7365      file_id = se
+00028a10: 6c66 2e76 6964 656f 2e66 696c 655f 6964  lf.video.file_id
+00028a20: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00028a30: 6620 7365 6c66 2e61 6e69 6d61 7469 6f6e  f self.animation
+00028a40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00028a50: 2020 6669 6c65 5f69 6420 3d20 7365 6c66    file_id = self
+00028a60: 2e61 6e69 6d61 7469 6f6e 2e66 696c 655f  .animation.file_
+00028a70: 6964 0a20 2020 2020 2020 2020 2020 2065  id.            e
+00028a80: 6c69 6620 7365 6c66 2e76 6f69 6365 3a0a  lif self.voice:.
+00028a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028aa0: 6669 6c65 5f69 6420 3d20 7365 6c66 2e76  file_id = self.v
+00028ab0: 6f69 6365 2e66 696c 655f 6964 0a20 2020  oice.file_id.   
+00028ac0: 2020 2020 2020 2020 2065 6c69 6620 7365           elif se
+00028ad0: 6c66 2e73 7469 636b 6572 3a0a 2020 2020  lf.sticker:.    
+00028ae0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00028af0: 5f69 6420 3d20 7365 6c66 2e73 7469 636b  _id = self.stick
+00028b00: 6572 2e66 696c 655f 6964 0a20 2020 2020  er.file_id.     
+00028b10: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+00028b20: 2e76 6964 656f 5f6e 6f74 653a 0a20 2020  .video_note:.   
+00028b30: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00028b40: 655f 6964 203d 2073 656c 662e 7669 6465  e_id = self.vide
+00028b50: 6f5f 6e6f 7465 2e66 696c 655f 6964 0a20  o_note.file_id. 
+00028b60: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00028b70: 7365 6c66 2e63 6f6e 7461 6374 3a0a 2020  self.contact:.  
+00028b80: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00028b90: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+00028ba0: 5f63 6c69 656e 742e 7365 6e64 5f63 6f6e  _client.send_con
+00028bb0: 7461 6374 280a 2020 2020 2020 2020 2020  tact(.          
+00028bc0: 2020 2020 2020 2020 2020 6368 6174 5f69            chat_i
+00028bd0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00028be0: 2020 2020 2020 2070 686f 6e65 5f6e 756d         phone_num
+00028bf0: 6265 723d 7365 6c66 2e63 6f6e 7461 6374  ber=self.contact
+00028c00: 2e70 686f 6e65 5f6e 756d 6265 722c 0a20  .phone_number,. 
+00028c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028c20: 2020 2066 6972 7374 5f6e 616d 653d 7365     first_name=se
+00028c30: 6c66 2e63 6f6e 7461 6374 2e66 6972 7374  lf.contact.first
+00028c40: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
+00028c50: 2020 2020 2020 2020 2020 206c 6173 745f             last_
+00028c60: 6e61 6d65 3d73 656c 662e 636f 6e74 6163  name=self.contac
+00028c70: 742e 6c61 7374 5f6e 616d 652c 0a20 2020  t.last_name,.   
 00028c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028c90: 2020 2020 7479 7065 3d73 656c 662e 706f      type=self.po
-00028ca0: 6c6c 2e74 7970 652c 0a20 2020 2020 2020  ll.type,.       
-00028cb0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00028cc0: 6f77 735f 6d75 6c74 6970 6c65 5f61 6e73  ows_multiple_ans
-00028cd0: 7765 7273 3d73 656c 662e 706f 6c6c 2e61  wers=self.poll.a
-00028ce0: 6c6c 6f77 735f 6d75 6c74 6970 6c65 5f61  llows_multiple_a
-00028cf0: 6e73 7765 7273 2c0a 2020 2020 2020 2020  nswers,.        
-00028d00: 2020 2020 2020 2020 2020 2020 636f 7272              corr
-00028d10: 6563 745f 6f70 7469 6f6e 5f69 643d 7365  ect_option_id=se
-00028d20: 6c66 2e70 6f6c 6c2e 636f 7272 6563 745f  lf.poll.correct_
-00028d30: 6f70 7469 6f6e 5f69 642c 0a20 2020 2020  option_id,.     
-00028d40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00028d50: 7870 6c61 6e61 7469 6f6e 3d73 656c 662e  xplanation=self.
-00028d60: 706f 6c6c 2e65 7870 6c61 6e61 7469 6f6e  poll.explanation
-00028d70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00028d80: 2020 2020 2020 6578 706c 616e 6174 696f        explanatio
-00028d90: 6e5f 656e 7469 7469 6573 3d73 656c 662e  n_entities=self.
-00028da0: 706f 6c6c 2e65 7870 6c61 6e61 7469 6f6e  poll.explanation
-00028db0: 5f65 6e74 6974 6965 732c 0a20 2020 2020  _entities,.     
-00028dc0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00028dd0: 7065 6e5f 7065 7269 6f64 3d73 656c 662e  pen_period=self.
-00028de0: 706f 6c6c 2e6f 7065 6e5f 7065 7269 6f64  poll.open_period
-00028df0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00028e00: 2020 2020 2020 636c 6f73 655f 6461 7465        close_date
-00028e10: 3d73 656c 662e 706f 6c6c 2e63 6c6f 7365  =self.poll.close
-00028e20: 5f64 6174 652c 0a20 2020 2020 2020 2020  _date,.         
-00028e30: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-00028e40: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3d  le_notification=
-00028e50: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-00028e60: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-00028e70: 2020 2020 2020 2020 2020 7072 6f74 6563            protec
-00028e80: 745f 636f 6e74 656e 743d 7365 6c66 2e68  t_content=self.h
-00028e90: 6173 5f70 726f 7465 6374 6564 5f63 6f6e  as_protected_con
-00028ea0: 7465 6e74 2c0a 2020 2020 2020 2020 2020  tent,.          
-00028eb0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
-00028ec0: 7061 7261 6d65 7465 7273 3d72 6570 6c79  parameters=reply
-00028ed0: 5f70 6172 616d 6574 6572 732c 0a20 2020  _parameters,.   
-00028ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028ef0: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
-00028f00: 6964 3d73 656c 662e 6d65 7373 6167 655f  id=self.message_
-00028f10: 7468 7265 6164 5f69 642c 0a20 2020 2020  thread_id,.     
-00028f20: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00028f30: 7573 696e 6573 735f 636f 6e6e 6563 7469  usiness_connecti
-00028f40: 6f6e 5f69 643d 7365 6c66 2e62 7573 696e  on_id=self.busin
-00028f50: 6573 735f 636f 6e6e 6563 7469 6f6e 5f69  ess_connection_i
-00028f60: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00028f70: 2020 2020 2020 2073 6368 6564 756c 655f         schedule_
-00028f80: 6461 7465 3d73 6368 6564 756c 655f 6461  date=schedule_da
-00028f90: 7465 2c0a 2020 2020 2020 2020 2020 2020  te,.            
-00028fa0: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
-00028fb0: 5f6d 6573 7361 6765 5f69 643d 7265 706c  _message_id=repl
-00028fc0: 795f 746f 5f6d 6573 7361 6765 5f69 642c  y_to_message_id,
-00028fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028fe0: 2020 2020 2072 6570 6c79 5f6d 6172 6b75       reply_marku
-00028ff0: 703d 7265 706c 795f 6d61 726b 7570 0a20  p=reply_markup. 
-00029000: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00029010: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00029020: 6620 7365 6c66 2e67 616d 653a 0a20 2020  f self.game:.   
-00029030: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00029040: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
-00029050: 636c 6965 6e74 2e73 656e 645f 6761 6d65  client.send_game
-00029060: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00029070: 2020 2020 2020 6368 6174 5f69 642c 0a20        chat_id,. 
-00029080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029090: 2020 2067 616d 655f 7368 6f72 745f 6e61     game_short_na
-000290a0: 6d65 3d73 656c 662e 6761 6d65 2e73 686f  me=self.game.sho
-000290b0: 7274 5f6e 616d 652c 0a20 2020 2020 2020  rt_name,.       
-000290c0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-000290d0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-000290e0: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
-000290f0: 6361 7469 6f6e 2c0a 2020 2020 2020 2020  cation,.        
-00029100: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-00029110: 6563 745f 636f 6e74 656e 743d 7365 6c66  ect_content=self
-00029120: 2e68 6173 5f70 726f 7465 6374 6564 5f63  .has_protected_c
-00029130: 6f6e 7465 6e74 2c0a 2020 2020 2020 2020  ontent,.        
-00029140: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00029150: 6167 655f 7468 7265 6164 5f69 643d 7365  age_thread_id=se
-00029160: 6c66 2e6d 6573 7361 6765 5f74 6872 6561  lf.message_threa
-00029170: 645f 6964 2c0a 2020 2020 2020 2020 2020  d_id,.          
-00029180: 2020 2020 2020 2020 2020 6275 7369 6e65            busine
-00029190: 7373 5f63 6f6e 6e65 6374 696f 6e5f 6964  ss_connection_id
-000291a0: 3d73 656c 662e 6275 7369 6e65 7373 5f63  =self.business_c
-000291b0: 6f6e 6e65 6374 696f 6e5f 6964 2c0a 2020  onnection_id,.  
-000291c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000291d0: 2020 7265 706c 795f 7061 7261 6d65 7465    reply_paramete
-000291e0: 7273 3d72 6570 6c79 5f70 6172 616d 6574  rs=reply_paramet
-000291f0: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
-00029200: 2020 2020 2020 2020 2072 6570 6c79 5f74           reply_t
-00029210: 6f5f 6d65 7373 6167 655f 6964 3d72 6570  o_message_id=rep
-00029220: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
-00029230: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00029240: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
-00029250: 7570 3d72 6570 6c79 5f6d 6172 6b75 700a  up=reply_markup.
-00029260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029270: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00029280: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00029290: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-000292a0: 7272 6f72 2822 556e 6b6e 6f77 6e20 6d65  rror("Unknown me
-000292b0: 6469 6120 7479 7065 2229 0a0a 2020 2020  dia type")..    
-000292c0: 2020 2020 2020 2020 6966 2063 6170 7469          if capti
-000292d0: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
-000292e0: 2020 2020 2020 2020 2020 2020 6361 7074              capt
-000292f0: 696f 6e20 3d20 7365 6c66 2e63 6170 7469  ion = self.capti
-00029300: 6f6e 206f 7220 2222 0a20 2020 2020 2020  on or "".       
-00029310: 2020 2020 2020 2020 2063 6170 7469 6f6e           caption
-00029320: 5f65 6e74 6974 6965 7320 3d20 7365 6c66  _entities = self
-00029330: 2e63 6170 7469 6f6e 5f65 6e74 6974 6965  .caption_entitie
-00029340: 730a 0a20 2020 2020 2020 2020 2020 2072  s..            r
-00029350: 6574 7572 6e20 6177 6169 7420 7365 6e64  eturn await send
-00029360: 5f6d 6564 6961 280a 2020 2020 2020 2020  _media(.        
-00029370: 2020 2020 2020 2020 6669 6c65 5f69 643d          file_id=
-00029380: 6669 6c65 5f69 642c 0a20 2020 2020 2020  file_id,.       
-00029390: 2020 2020 2020 2020 2063 6170 7469 6f6e           caption
-000293a0: 3d63 6170 7469 6f6e 2c0a 2020 2020 2020  =caption,.      
-000293b0: 2020 2020 2020 2020 2020 7061 7273 655f            parse_
-000293c0: 6d6f 6465 3d70 6172 7365 5f6d 6f64 652c  mode=parse_mode,
-000293d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000293e0: 2063 6170 7469 6f6e 5f65 6e74 6974 6965   caption_entitie
-000293f0: 733d 6361 7074 696f 6e5f 656e 7469 7469  s=caption_entiti
-00029400: 6573 0a20 2020 2020 2020 2020 2020 2029  es.            )
-00029410: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00029420: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00029430: 2056 616c 7565 4572 726f 7228 2243 616e   ValueError("Can
-00029440: 2774 2063 6f70 7920 7468 6973 206d 6573  't copy this mes
-00029450: 7361 6765 2229 0a0a 2020 2020 6173 796e  sage")..    asyn
-00029460: 6320 6465 6620 6465 6c65 7465 2873 656c  c def delete(sel
-00029470: 662c 2072 6576 6f6b 653a 2062 6f6f 6c20  f, revoke: bool 
-00029480: 3d20 5472 7565 293a 0a20 2020 2020 2020  = True):.       
-00029490: 2022 2222 426f 756e 6420 6d65 7468 6f64   """Bound method
-000294a0: 202a 6465 6c65 7465 2a20 6f66 203a 6f62   *delete* of :ob
-000294b0: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
-000294c0: 6573 2e4d 6573 7361 6765 602e 0a0a 2020  es.Message`...  
-000294d0: 2020 2020 2020 5573 6520 6173 2061 2073        Use as a s
-000294e0: 686f 7274 6375 7420 666f 723a 0a0a 2020  hortcut for:..  
-000294f0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
-00029500: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
-00029510: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-00029520: 636c 6965 6e74 2e64 656c 6574 655f 6d65  client.delete_me
-00029530: 7373 6167 6573 280a 2020 2020 2020 2020  ssages(.        
-00029540: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
-00029550: 6368 6174 5f69 642c 0a20 2020 2020 2020  chat_id,.       
-00029560: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00029570: 5f69 6473 3d6d 6573 7361 6765 2e69 640a  _ids=message.id.
-00029580: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00029590: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
-000295a0: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
-000295b0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-000295c0: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-000295d0: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
-000295e0: 652e 6465 6c65 7465 2829 0a0a 2020 2020  e.delete()..    
-000295f0: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
-00029600: 2020 2020 2020 2020 2020 2020 7265 766f              revo
-00029610: 6b65 2028 6060 626f 6f6c 6060 2c20 2a6f  ke (``bool``, *o
-00029620: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
-00029630: 2020 2020 2020 2020 2020 2044 656c 6574             Delet
-00029640: 6573 206d 6573 7361 6765 7320 6f6e 2062  es messages on b
-00029650: 6f74 6820 7061 7274 732e 0a20 2020 2020  oth parts..     
-00029660: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00029670: 6973 206f 6e6c 7920 666f 7220 7072 6976  is only for priv
-00029680: 6174 6520 636c 6f75 6420 6368 6174 7320  ate cloud chats 
-00029690: 616e 6420 6e6f 726d 616c 2067 726f 7570  and normal group
-000296a0: 732c 206d 6573 7361 6765 7320 6f6e 0a20  s, messages on. 
-000296b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000296c0: 6861 6e6e 656c 7320 616e 6420 7375 7065  hannels and supe
-000296d0: 7267 726f 7570 7320 6172 6520 616c 7761  rgroups are alwa
-000296e0: 7973 2072 6576 6f6b 6564 2028 692e 652e  ys revoked (i.e.
-000296f0: 3a20 6465 6c65 7465 6420 666f 7220 6576  : deleted for ev
-00029700: 6572 796f 6e65 292e 0a20 2020 2020 2020  eryone)..       
-00029710: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00029720: 7320 746f 2054 7275 652e 0a0a 2020 2020  s to True...    
-00029730: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00029740: 2020 2020 2020 2020 2060 6069 6e74 6060           ``int``
-00029750: 3a20 416d 6f75 6e74 206f 6620 6166 6665  : Amount of affe
-00029760: 6374 6564 206d 6573 7361 6765 730a 0a20  cted messages.. 
-00029770: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
-00029780: 2020 2020 2020 2020 2020 2052 5043 4572             RPCEr
-00029790: 726f 723a 2049 6e20 6361 7365 206f 6620  ror: In case of 
-000297a0: 6120 5465 6c65 6772 616d 2052 5043 2065  a Telegram RPC e
-000297b0: 7272 6f72 2e0a 2020 2020 2020 2020 2222  rror..        ""
-000297c0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-000297d0: 2061 7761 6974 2073 656c 662e 5f63 6c69   await self._cli
-000297e0: 656e 742e 6465 6c65 7465 5f6d 6573 7361  ent.delete_messa
-000297f0: 6765 7328 0a20 2020 2020 2020 2020 2020  ges(.           
-00029800: 2063 6861 745f 6964 3d73 656c 662e 6368   chat_id=self.ch
-00029810: 6174 2e69 642c 0a20 2020 2020 2020 2020  at.id,.         
-00029820: 2020 206d 6573 7361 6765 5f69 6473 3d73     message_ids=s
-00029830: 656c 662e 6964 2c0a 2020 2020 2020 2020  elf.id,.        
-00029840: 2020 2020 7265 766f 6b65 3d72 6576 6f6b      revoke=revok
-00029850: 652c 0a20 2020 2020 2020 2020 2020 2069  e,.            i
-00029860: 735f 7363 6865 6475 6c65 643d 7365 6c66  s_scheduled=self
-00029870: 2e73 6368 6564 756c 6564 0a20 2020 2020  .scheduled.     
-00029880: 2020 2029 0a0a 2020 2020 6173 796e 6320     )..    async 
-00029890: 6465 6620 636c 6963 6b28 0a20 2020 2020  def click(.     
-000298a0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000298b0: 2078 3a20 556e 696f 6e5b 696e 742c 2073   x: Union[int, s
-000298c0: 7472 5d20 3d20 302c 0a20 2020 2020 2020  tr] = 0,.       
-000298d0: 2079 3a20 696e 7420 3d20 4e6f 6e65 2c0a   y: int = None,.
-000298e0: 2020 2020 2020 2020 7175 6f74 653a 2062          quote: b
-000298f0: 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020 2020  ool = None,.    
-00029900: 2020 2020 7469 6d65 6f75 743a 2069 6e74      timeout: int
-00029910: 203d 2031 302c 0a20 2020 2020 2020 2072   = 10,.        r
-00029920: 6571 7565 7374 5f77 7269 7465 5f61 6363  equest_write_acc
-00029930: 6573 733a 2062 6f6f 6c20 3d20 5472 7565  ess: bool = True
-00029940: 2c0a 2020 2020 2020 2020 7061 7373 776f  ,.        passwo
-00029950: 7264 3a20 7374 7220 3d20 4e6f 6e65 0a20  rd: str = None. 
-00029960: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-00029970: 2242 6f75 6e64 206d 6574 686f 6420 2a63  "Bound method *c
-00029980: 6c69 636b 2a20 6f66 203a 6f62 6a3a 607e  lick* of :obj:`~
-00029990: 7079 726f 6772 616d 2e74 7970 6573 2e4d  pyrogram.types.M
-000299a0: 6573 7361 6765 602e 0a0a 2020 2020 2020  essage`...      
-000299b0: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
-000299c0: 6375 7420 666f 7220 636c 6963 6b69 6e67  cut for clicking
-000299d0: 2061 2062 7574 746f 6e20 6174 7461 6368   a button attach
-000299e0: 6564 2074 6f20 7468 6520 6d65 7373 6167  ed to the messag
-000299f0: 6520 696e 7374 6561 6420 6f66 3a0a 0a20  e instead of:.. 
-00029a00: 2020 2020 2020 202d 2043 6c69 636b 696e         - Clickin
-00029a10: 6720 696e 6c69 6e65 2062 7574 746f 6e73  g inline buttons
-00029a20: 3a0a 0a20 2020 2020 2020 202e 2e20 636f  :..        .. co
-00029a30: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
-00029a40: 6e0a 0a20 2020 2020 2020 2020 2020 2061  n..            a
-00029a50: 7761 6974 2063 6c69 656e 742e 7265 7175  wait client.requ
-00029a60: 6573 745f 6361 6c6c 6261 636b 5f61 6e73  est_callback_ans
-00029a70: 7765 7228 0a20 2020 2020 2020 2020 2020  wer(.           
-00029a80: 2020 2020 2063 6861 745f 6964 3d6d 6573       chat_id=mes
-00029a90: 7361 6765 2e63 6861 742e 6964 2c0a 2020  sage.chat.id,.  
-00029aa0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00029ab0: 7373 6167 655f 6964 3d6d 6573 7361 6765  ssage_id=message
-00029ac0: 2e69 642c 0a20 2020 2020 2020 2020 2020  .id,.           
-00029ad0: 2020 2020 2063 616c 6c62 6163 6b5f 6461       callback_da
-00029ae0: 7461 3d6d 6573 7361 6765 2e72 6570 6c79  ta=message.reply
-00029af0: 5f6d 6172 6b75 705b 695d 5b6a 5d2e 6361  _markup[i][j].ca
-00029b00: 6c6c 6261 636b 5f64 6174 610a 2020 2020  llback_data.    
-00029b10: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00029b20: 2020 202d 2043 6c69 636b 696e 6720 6e6f     - Clicking no
-00029b30: 726d 616c 2062 7574 746f 6e73 3a0a 0a20  rmal buttons:.. 
-00029b40: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
-00029b50: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
-00029b60: 2020 2020 2020 2020 2020 2061 7761 6974             await
-00029b70: 2063 6c69 656e 742e 7365 6e64 5f6d 6573   client.send_mes
-00029b80: 7361 6765 280a 2020 2020 2020 2020 2020  sage(.          
-00029b90: 2020 2020 2020 6368 6174 5f69 643d 6d65        chat_id=me
-00029ba0: 7373 6167 652e 6368 6174 2e69 642c 0a20  ssage.chat.id,. 
-00029bb0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00029bc0: 6578 743d 6d65 7373 6167 652e 7265 706c  ext=message.repl
-00029bd0: 795f 6d61 726b 7570 5b69 5d5b 6a5d 2e74  y_markup[i][j].t
-00029be0: 6578 740a 2020 2020 2020 2020 2020 2020  ext.            
-00029bf0: 290a 0a20 2020 2020 2020 2045 7861 6d70  )..        Examp
-00029c00: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-00029c10: 5468 6973 206d 6574 686f 6420 6361 6e20  This method can 
-00029c20: 6265 2075 7365 6420 696e 2074 6872 6565  be used in three
-00029c30: 2064 6966 6665 7265 6e74 2077 6179 733a   different ways:
-00029c40: 0a0a 2020 2020 2020 2020 2020 2020 312e  ..            1.
-00029c50: 2020 5061 7373 206f 6e65 2069 6e74 6567    Pass one integ
-00029c60: 6572 2061 7267 756d 656e 7420 6f6e 6c79  er argument only
-00029c70: 2028 652e 672e 3a20 6060 2e63 6c69 636b   (e.g.: ``.click
-00029c80: 2832 2960 602c 2074 6f20 636c 6963 6b20  (2)``, to click 
-00029c90: 6120 6275 7474 6f6e 2061 7420 696e 6465  a button at inde
-00029ca0: 7820 3229 2e0a 2020 2020 2020 2020 2020  x 2)..          
-00029cb0: 2020 2020 2020 4275 7474 6f6e 7320 6172        Buttons ar
-00029cc0: 6520 636f 756e 7465 6420 6c65 6674 2074  e counted left t
-00029cd0: 6f20 7269 6768 742c 2073 7461 7274 696e  o right, startin
-00029ce0: 6720 6672 6f6d 2074 6865 2074 6f70 2e0a  g from the top..
-00029cf0: 0a20 2020 2020 2020 2020 2020 2032 2e20  .            2. 
-00029d00: 2050 6173 7320 7477 6f20 696e 7465 6765   Pass two intege
-00029d10: 7220 6172 6775 6d65 6e74 7320 2865 2e67  r arguments (e.g
-00029d20: 2e3a 2060 602e 636c 6963 6b28 312c 2030  .: ``.click(1, 0
-00029d30: 2960 602c 2074 6f20 636c 6963 6b20 6120  )``, to click a 
-00029d40: 6275 7474 6f6e 2061 7420 706f 7369 7469  button at positi
-00029d50: 6f6e 2028 312c 2030 2929 2e0a 2020 2020  on (1, 0))..    
-00029d60: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00029d70: 6f72 6967 696e 2028 302c 2030 2920 6973  origin (0, 0) is
-00029d80: 2074 6f70 2d6c 6566 742e 0a0a 2020 2020   top-left...    
-00029d90: 2020 2020 2020 2020 332e 2020 5061 7373          3.  Pass
-00029da0: 206f 6e65 2073 7472 696e 6720 6172 6775   one string argu
-00029db0: 6d65 6e74 206f 6e6c 7920 2865 2e67 2e3a  ment only (e.g.:
-00029dc0: 2060 602e 636c 6963 6b28 2253 6574 7469   ``.click("Setti
-00029dd0: 6e67 7322 2960 602c 2074 6f20 636c 6963  ngs")``, to clic
-00029de0: 6b20 6120 6275 7474 6f6e 2062 7920 7573  k a button by us
-00029df0: 696e 6720 6974 7320 6c61 6265 6c29 2e0a  ing its label)..
-00029e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029e10: 4f6e 6c79 2074 6865 2066 6972 7374 206d  Only the first m
-00029e20: 6174 6368 696e 6720 6275 7474 6f6e 2077  atching button w
-00029e30: 696c 6c20 6265 2070 7265 7373 6564 2e0a  ill be pressed..
-00029e40: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00029e50: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
-00029e60: 2078 2028 6060 696e 7460 6020 7c20 6060   x (``int`` | ``
-00029e70: 7374 7260 6029 3a0a 2020 2020 2020 2020  str``):.        
-00029e80: 2020 2020 2020 2020 5573 6564 2061 7320          Used as 
-00029e90: 696e 7465 6765 7220 696e 6465 782c 2069  integer index, i
-00029ea0: 6e74 6567 6572 2061 6273 6369 7373 6120  nteger abscissa 
-00029eb0: 2869 6e20 7061 6972 2077 6974 6820 7929  (in pair with y)
-00029ec0: 206f 7220 6173 2073 7472 696e 6720 6c61   or as string la
-00029ed0: 6265 6c2e 0a20 2020 2020 2020 2020 2020  bel..           
-00029ee0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-00029ef0: 2030 2028 6669 7273 7420 6275 7474 6f6e   0 (first button
-00029f00: 292e 0a0a 2020 2020 2020 2020 2020 2020  )...            
-00029f10: 7920 2860 6069 6e74 6060 2c20 2a6f 7074  y (``int``, *opt
-00029f20: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
-00029f30: 2020 2020 2020 2020 2055 7365 6420 6173           Used as
-00029f40: 206f 7264 696e 6174 6520 6f6e 6c79 2028   ordinate only (
-00029f50: 696e 2070 6169 7220 7769 7468 2078 292e  in pair with x).
-00029f60: 0a0a 2020 2020 2020 2020 2020 2020 7175  ..            qu
-00029f70: 6f74 6520 2860 6062 6f6f 6c60 602c 202a  ote (``bool``, *
-00029f80: 6f70 7469 6f6e 616c 2a29 3a0a 2020 2020  optional*):.    
-00029f90: 2020 2020 2020 2020 2020 2020 5573 6566              Usef
-00029fa0: 756c 2066 6f72 206e 6f72 6d61 6c20 6275  ul for normal bu
-00029fb0: 7474 6f6e 7320 6f6e 6c79 2c20 7768 6572  ttons only, wher
-00029fc0: 6520 7072 6573 7369 6e67 2069 7420 7769  e pressing it wi
-00029fd0: 6c6c 2072 6573 756c 7420 696e 2061 206e  ll result in a n
-00029fe0: 6577 206d 6573 7361 6765 2073 656e 742e  ew message sent.
-00029ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a000: 2049 6620 6060 5472 7565 6060 2c20 7468   If ``True``, th
-0002a010: 6520 6d65 7373 6167 6520 7769 6c6c 2062  e message will b
-0002a020: 6520 7365 6e74 2061 7320 6120 7265 706c  e sent as a repl
-0002a030: 7920 746f 2074 6869 7320 6d65 7373 6167  y to this messag
-0002a040: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
-0002a050: 2020 2044 6566 6175 6c74 7320 746f 2060     Defaults to `
-0002a060: 6054 7275 6560 6020 696e 2067 726f 7570  `True`` in group
-0002a070: 2063 6861 7473 2061 6e64 2060 6046 616c   chats and ``Fal
-0002a080: 7365 6060 2069 6e20 7072 6976 6174 6520  se`` in private 
-0002a090: 6368 6174 732e 0a0a 2020 2020 2020 2020  chats...        
-0002a0a0: 2020 2020 7469 6d65 6f75 7420 2860 6069      timeout (``i
-0002a0b0: 6e74 6060 2c20 2a6f 7074 696f 6e61 6c2a  nt``, *optional*
-0002a0c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0002a0d0: 2020 2054 696d 656f 7574 2069 6e20 7365     Timeout in se
-0002a0e0: 636f 6e64 732e 0a0a 2020 2020 2020 2020  conds...        
-0002a0f0: 2020 2020 7265 7175 6573 745f 7772 6974      request_writ
-0002a100: 655f 6163 6365 7373 2028 6060 626f 6f6c  e_access (``bool
-0002a110: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
-0002a120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a130: 204f 6e6c 7920 7573 6564 2069 6e20 6361   Only used in ca
-0002a140: 7365 206f 6620 3a6f 626a 3a60 7e70 7972  se of :obj:`~pyr
-0002a150: 6f67 7261 6d2e 7479 7065 732e 4c6f 6769  ogram.types.Logi
-0002a160: 6e55 726c 6020 6275 7474 6f6e 2e0a 2020  nUrl` button..  
-0002a170: 2020 2020 2020 2020 2020 2020 2020 5472                Tr
-0002a180: 7565 2c20 6966 2074 6865 2062 6f74 2063  ue, if the bot c
-0002a190: 616e 2073 656e 6420 6d65 7373 6167 6573  an send messages
-0002a1a0: 2074 6f20 7468 6520 7573 6572 2e0a 2020   to the user..  
-0002a1b0: 2020 2020 2020 2020 2020 2020 2020 4465                De
-0002a1c0: 6661 756c 7473 2074 6f20 6060 5472 7565  faults to ``True
-0002a1d0: 6060 2e0a 0a20 2020 2020 2020 2020 2020  ``...           
-0002a1e0: 2070 6173 7377 6f72 6420 2860 6073 7472   password (``str
-0002a1f0: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
-0002a200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a210: 2057 6865 6e20 636c 6963 6b69 6e67 2063   When clicking c
-0002a220: 6572 7461 696e 2062 7574 746f 6e73 2028  ertain buttons (
-0002a230: 7375 6368 2061 7320 426f 7446 6174 6865  such as BotFathe
-0002a240: 7227 7320 636f 6e66 6972 6d61 7469 6f6e  r's confirmation
-0002a250: 2062 7574 746f 6e20 746f 2074 7261 6e73   button to trans
-0002a260: 6665 7220 6f77 6e65 7273 6869 7029 2c20  fer ownership), 
-0002a270: 6966 2079 6f75 7220 6163 636f 756e 7420  if your account 
-0002a280: 6861 7320 3246 4120 656e 6162 6c65 642c  has 2FA enabled,
-0002a290: 2079 6f75 206e 6565 6420 746f 2070 726f   you need to pro
-0002a2a0: 7669 6465 2079 6f75 7220 6163 636f 756e  vide your accoun
-0002a2b0: 7427 7320 7061 7373 776f 7264 2e20 0a20  t's password. . 
-0002a2c0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0002a2d0: 6865 2032 2d73 7465 7020 7665 7269 6669  he 2-step verifi
-0002a2e0: 6361 7469 6f6e 2070 6173 7377 6f72 6420  cation password 
-0002a2f0: 666f 7220 7468 6520 6375 7272 656e 7420  for the current 
-0002a300: 7573 6572 2e20 4f6e 6c79 2061 7070 6c69  user. Only appli
-0002a310: 6361 626c 652c 2069 6620 7468 6520 3a6f  cable, if the :o
-0002a320: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
-0002a330: 7065 732e 496e 6c69 6e65 4b65 7962 6f61  pes.InlineKeyboa
-0002a340: 7264 4275 7474 6f6e 6020 636f 6e74 6169  rdButton` contai
-0002a350: 6e73 2060 6063 616c 6c62 6163 6b5f 6461  ns ``callback_da
-0002a360: 7461 5f77 6974 685f 7061 7373 776f 7264  ta_with_password
-0002a370: 6060 2e0a 0a20 2020 2020 2020 2052 6574  ``...        Ret
-0002a380: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-0002a390: 2020 2d20 2020 5468 6520 7265 7375 6c74    -   The result
-0002a3a0: 206f 6620 3a6d 6574 683a 607e 7079 726f   of :meth:`~pyro
-0002a3b0: 6772 616d 2e43 6c69 656e 742e 7265 7175  gram.Client.requ
-0002a3c0: 6573 745f 6361 6c6c 6261 636b 5f61 6e73  est_callback_ans
-0002a3d0: 7765 7260 2069 6e20 6361 7365 206f 6620  wer` in case of 
-0002a3e0: 696e 6c69 6e65 2063 616c 6c62 6163 6b20  inline callback 
-0002a3f0: 6275 7474 6f6e 2063 6c69 636b 732e 0a20  button clicks.. 
-0002a400: 2020 2020 2020 2020 2020 202d 2020 2054             -   T
-0002a410: 6865 2072 6573 756c 7420 6f66 203a 6d65  he result of :me
-0002a420: 7468 3a60 7e4d 6573 7361 6765 2e72 6570  th:`~Message.rep
-0002a430: 6c79 2829 6020 696e 2063 6173 6520 6f66  ly()` in case of
-0002a440: 206e 6f72 6d61 6c20 6275 7474 6f6e 2063   normal button c
-0002a450: 6c69 636b 732e 0a20 2020 2020 2020 2020  licks..         
-0002a460: 2020 202d 2020 2041 2073 7472 696e 6720     -   A string 
-0002a470: 696e 2063 6173 6520 7468 6520 696e 6c69  in case the inli
-0002a480: 6e65 2062 7574 746f 6e20 6973 2061 2055  ne button is a U
-0002a490: 524c 2c20 6120 2a73 7769 7463 685f 696e  RL, a *switch_in
-0002a4a0: 6c69 6e65 5f71 7565 7279 2a20 6f72 2061  line_query* or a
-0002a4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a4c0: 202a 7377 6974 6368 5f69 6e6c 696e 655f   *switch_inline_
-0002a4d0: 7175 6572 795f 6375 7272 656e 745f 6368  query_current_ch
-0002a4e0: 6174 2a20 6275 7474 6f6e 2e0a 2020 2020  at* button..    
-0002a4f0: 2020 2020 2020 2020 2d20 2020 4120 7374          -   A st
-0002a500: 7269 6e67 2055 524c 2077 6974 6820 7468  ring URL with th
-0002a510: 6520 7573 6572 2064 6574 6169 6c73 2c20  e user details, 
-0002a520: 696e 2063 6173 6520 6f66 2061 204c 6f67  in case of a Log
-0002a530: 696e 5572 6c20 6275 7474 6f6e 2e0a 2020  inUrl button..  
-0002a540: 2020 2020 2020 2020 2020 2d20 2020 4120            -   A 
-0002a550: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
-0002a560: 7479 7065 732e 5377 6974 6368 496e 6c69  types.SwitchInli
-0002a570: 6e65 5175 6572 7943 686f 7365 6e43 6861  neQueryChosenCha
-0002a580: 7460 206f 626a 6563 7420 696e 2063 6173  t` object in cas
-0002a590: 6520 6f66 2061 2060 6073 7769 7463 685f  e of a ``switch_
-0002a5a0: 696e 6c69 6e65 5f71 7565 7279 5f63 686f  inline_query_cho
-0002a5b0: 7365 6e5f 6368 6174 6060 2e0a 2020 2020  sen_chat``..    
-0002a5c0: 2020 2020 2020 2020 2d20 2020 4120 3a6f          -   A :o
-0002a5d0: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
-0002a5e0: 7065 732e 5573 6572 6020 6f62 6a65 6374  pes.User` object
-0002a5f0: 2069 6e20 6361 7365 206f 6620 6120 6060   in case of a ``
-0002a600: 4b65 7962 6f61 7264 4275 7474 6f6e 5573  KeyboardButtonUs
-0002a610: 6572 5072 6f66 696c 6560 6020 6275 7474  erProfile`` butt
-0002a620: 6f6e 2e0a 0a20 2020 2020 2020 2052 6169  on...        Rai
-0002a630: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
-0002a640: 2052 5043 4572 726f 723a 2049 6e20 6361   RPCError: In ca
-0002a650: 7365 206f 6620 6120 5465 6c65 6772 616d  se of a Telegram
-0002a660: 2052 5043 2065 7272 6f72 2e0a 2020 2020   RPC error..    
-0002a670: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
-0002a680: 6f72 3a20 496e 2063 6173 6520 7468 6520  or: In case the 
-0002a690: 7072 6f76 6964 6564 2069 6e64 6578 206f  provided index o
-0002a6a0: 7220 706f 7369 7469 6f6e 2069 7320 6f75  r position is ou
-0002a6b0: 7420 6f66 2072 616e 6765 206f 7220 7468  t of range or th
-0002a6c0: 6520 6275 7474 6f6e 206c 6162 656c 2077  e button label w
-0002a6d0: 6173 206e 6f74 2066 6f75 6e64 2e0a 2020  as not found..  
-0002a6e0: 2020 2020 2020 2020 2020 5469 6d65 6f75            Timeou
-0002a6f0: 7445 7272 6f72 3a20 496e 2063 6173 652c  tError: In case,
-0002a700: 2061 6674 6572 2063 6c69 636b 696e 6720   after clicking 
-0002a710: 616e 2069 6e6c 696e 6520 6275 7474 6f6e  an inline button
-0002a720: 2c20 7468 6520 626f 7420 6661 696c 7320  , the bot fails 
-0002a730: 746f 2061 6e73 7765 7220 7769 7468 696e  to answer within
-0002a740: 2074 6865 2074 696d 656f 7574 2e0a 2020   the timeout..  
-0002a750: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-0002a760: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0002a770: 2873 656c 662e 7265 706c 795f 6d61 726b  (self.reply_mark
-0002a780: 7570 2c20 7479 7065 732e 5265 706c 794b  up, types.ReplyK
-0002a790: 6579 626f 6172 644d 6172 6b75 7029 3a0a  eyboardMarkup):.
-0002a7a0: 2020 2020 2020 2020 2020 2020 6b65 7962              keyb
-0002a7b0: 6f61 7264 203d 2073 656c 662e 7265 706c  oard = self.repl
-0002a7c0: 795f 6d61 726b 7570 2e6b 6579 626f 6172  y_markup.keyboar
-0002a7d0: 640a 2020 2020 2020 2020 2020 2020 6973  d.            is
-0002a7e0: 5f69 6e6c 696e 6520 3d20 4661 6c73 650a  _inline = False.
-0002a7f0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-0002a800: 6e73 7461 6e63 6528 7365 6c66 2e72 6570  nstance(self.rep
-0002a810: 6c79 5f6d 6172 6b75 702c 2074 7970 6573  ly_markup, types
-0002a820: 2e49 6e6c 696e 654b 6579 626f 6172 644d  .InlineKeyboardM
-0002a830: 6172 6b75 7029 3a0a 2020 2020 2020 2020  arkup):.        
-0002a840: 2020 2020 6b65 7962 6f61 7264 203d 2073      keyboard = s
-0002a850: 656c 662e 7265 706c 795f 6d61 726b 7570  elf.reply_markup
-0002a860: 2e69 6e6c 696e 655f 6b65 7962 6f61 7264  .inline_keyboard
-0002a870: 0a20 2020 2020 2020 2020 2020 2069 735f  .            is_
-0002a880: 696e 6c69 6e65 203d 2054 7275 650a 2020  inline = True.  
-0002a890: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0002a8a0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-0002a8b0: 6c75 6545 7272 6f72 2822 5468 6520 6d65  lueError("The me
-0002a8c0: 7373 6167 6520 646f 6573 6e27 7420 636f  ssage doesn't co
-0002a8d0: 6e74 6169 6e20 616e 7920 6b65 7962 6f61  ntain any keyboa
-0002a8e0: 7264 2229 0a0a 2020 2020 2020 2020 6966  rd")..        if
-0002a8f0: 2069 7369 6e73 7461 6e63 6528 782c 2069   isinstance(x, i
-0002a900: 6e74 2920 616e 6420 7920 6973 204e 6f6e  nt) and y is Non
-0002a910: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-0002a920: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0002a930: 2020 2020 6275 7474 6f6e 203d 205b 0a20      button = [. 
-0002a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a950: 2020 2062 7574 746f 6e0a 2020 2020 2020     button.      
-0002a960: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0002a970: 7220 726f 7720 696e 206b 6579 626f 6172  r row in keyboar
-0002a980: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-0002a990: 2020 2020 2020 666f 7220 6275 7474 6f6e        for button
-0002a9a0: 2069 6e20 726f 770a 2020 2020 2020 2020   in row.        
-0002a9b0: 2020 2020 2020 2020 5d5b 785d 0a20 2020          ][x].   
-0002a9c0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-0002a9d0: 496e 6465 7845 7272 6f72 3a0a 2020 2020  IndexError:.    
-0002a9e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0002a9f0: 6520 5661 6c75 6545 7272 6f72 2866 2254  e ValueError(f"T
-0002aa00: 6865 2062 7574 746f 6e20 6174 2069 6e64  he button at ind
-0002aa10: 6578 207b 787d 2064 6f65 736e 2774 2065  ex {x} doesn't e
-0002aa20: 7869 7374 2229 0a20 2020 2020 2020 2065  xist").        e
-0002aa30: 6c69 6620 6973 696e 7374 616e 6365 2878  lif isinstance(x
-0002aa40: 2c20 696e 7429 2061 6e64 2069 7369 6e73  , int) and isins
-0002aa50: 7461 6e63 6528 792c 2069 6e74 293a 0a20  tance(y, int):. 
-0002aa60: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0002aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002aa80: 6275 7474 6f6e 203d 206b 6579 626f 6172  button = keyboar
-0002aa90: 645b 795d 5b78 5d0a 2020 2020 2020 2020  d[y][x].        
-0002aaa0: 2020 2020 6578 6365 7074 2049 6e64 6578      except Index
-0002aab0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-0002aac0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-0002aad0: 7565 4572 726f 7228 6622 5468 6520 6275  ueError(f"The bu
-0002aae0: 7474 6f6e 2061 7420 706f 7369 7469 6f6e  tton at position
-0002aaf0: 2028 7b78 7d2c 207b 797d 2920 646f 6573   ({x}, {y}) does
-0002ab00: 6e27 7420 6578 6973 7422 290a 2020 2020  n't exist").    
-0002ab10: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-0002ab20: 6e63 6528 782c 2073 7472 2920 616e 6420  nce(x, str) and 
-0002ab30: 7920 6973 204e 6f6e 653a 0a20 2020 2020  y is None:.     
-0002ab40: 2020 2020 2020 206c 6162 656c 203d 2078         label = x
-0002ab50: 2e65 6e63 6f64 6528 2275 7466 2d31 3622  .encode("utf-16"
-0002ab60: 2c20 2273 7572 726f 6761 7465 7061 7373  , "surrogatepass
-0002ab70: 2229 2e64 6563 6f64 6528 2275 7466 2d31  ").decode("utf-1
-0002ab80: 3622 290a 0a20 2020 2020 2020 2020 2020  6")..           
-0002ab90: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0002aba0: 2020 2020 2020 6275 7474 6f6e 203d 205b        button = [
-0002abb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002abc0: 2020 2020 2062 7574 746f 6e0a 2020 2020       button.    
-0002abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002abe0: 666f 7220 726f 7720 696e 206b 6579 626f  for row in keybo
-0002abf0: 6172 640a 2020 2020 2020 2020 2020 2020  ard.            
-0002ac00: 2020 2020 2020 2020 666f 7220 6275 7474          for butt
-0002ac10: 6f6e 2069 6e20 726f 770a 2020 2020 2020  on in row.      
-0002ac20: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0002ac30: 206c 6162 656c 203d 3d20 6275 7474 6f6e   label == button
-0002ac40: 2e74 6578 740a 2020 2020 2020 2020 2020  .text.          
-0002ac50: 2020 2020 2020 5d5b 305d 0a20 2020 2020        ][0].     
-0002ac60: 2020 2020 2020 2065 7863 6570 7420 496e         except In
-0002ac70: 6465 7845 7272 6f72 3a0a 2020 2020 2020  dexError:.      
-0002ac80: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0002ac90: 5661 6c75 6545 7272 6f72 2866 2254 6865  ValueError(f"The
-0002aca0: 2062 7574 746f 6e20 7769 7468 206c 6162   button with lab
-0002acb0: 656c 2027 7b78 7d27 2064 6f65 736e 2774  el '{x}' doesn't
-0002acc0: 2065 7869 7374 7322 290a 2020 2020 2020   exists").      
-0002acd0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0002ace0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0002acf0: 7272 6f72 2822 496e 7661 6c69 6420 6172  rror("Invalid ar
-0002ad00: 6775 6d65 6e74 7322 290a 0a20 2020 2020  guments")..     
-0002ad10: 2020 2069 6620 6973 5f69 6e6c 696e 653a     if is_inline:
-0002ad20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0002ad30: 6275 7474 6f6e 2e63 616c 6c62 6163 6b5f  button.callback_
-0002ad40: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-0002ad50: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-0002ad60: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-0002ad70: 7265 7175 6573 745f 6361 6c6c 6261 636b  request_callback
-0002ad80: 5f61 6e73 7765 7228 0a20 2020 2020 2020  _answer(.       
-0002ad90: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-0002ada0: 745f 6964 3d73 656c 662e 6368 6174 2e69  t_id=self.chat.i
-0002adb0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-0002adc0: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
-0002add0: 643d 7365 6c66 2e69 642c 0a20 2020 2020  d=self.id,.     
-0002ade0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0002adf0: 616c 6c62 6163 6b5f 6461 7461 3d62 7574  allback_data=but
-0002ae00: 746f 6e2e 6361 6c6c 6261 636b 5f64 6174  ton.callback_dat
-0002ae10: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-0002ae20: 2020 2020 2020 2074 696d 656f 7574 3d74         timeout=t
-0002ae30: 696d 656f 7574 0a20 2020 2020 2020 2020  imeout.         
-0002ae40: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0002ae50: 2020 2020 2065 6c69 6620 6275 7474 6f6e       elif button
-0002ae60: 2e63 616c 6c62 6163 6b5f 6461 7461 5f77  .callback_data_w
-0002ae70: 6974 685f 7061 7373 776f 7264 3a0a 2020  ith_password:.  
-0002ae80: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0002ae90: 2070 6173 7377 6f72 6420 6973 204e 6f6e   password is Non
-0002aea0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0002aeb0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-0002aec0: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
-0002aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002aee0: 2022 496e 7661 6c69 6420 6172 6775 6d65   "Invalid argume
-0002aef0: 6e74 2070 6173 7365 6422 0a20 2020 2020  nt passed".     
-0002af00: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0002af10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002af20: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-0002af30: 6c66 2e5f 636c 6965 6e74 2e72 6571 7565  lf._client.reque
-0002af40: 7374 5f63 616c 6c62 6163 6b5f 616e 7377  st_callback_answ
-0002af50: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-0002af60: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
-0002af70: 7365 6c66 2e63 6861 742e 6964 2c0a 2020  self.chat.id,.  
-0002af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002af90: 2020 6d65 7373 6167 655f 6964 3d73 656c    message_id=sel
-0002afa0: 662e 6964 2c0a 2020 2020 2020 2020 2020  f.id,.          
-0002afb0: 2020 2020 2020 2020 2020 6361 6c6c 6261            callba
-0002afc0: 636b 5f64 6174 613d 6275 7474 6f6e 2e63  ck_data=button.c
-0002afd0: 616c 6c62 6163 6b5f 6461 7461 5f77 6974  allback_data_wit
-0002afe0: 685f 7061 7373 776f 7264 2c0a 2020 2020  h_password,.    
-0002aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b000: 7061 7373 776f 7264 3d70 6173 7377 6f72  password=passwor
-0002b010: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-0002b020: 2020 2020 2020 2074 696d 656f 7574 3d74         timeout=t
-0002b030: 696d 656f 7574 0a20 2020 2020 2020 2020  imeout.         
-0002b040: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0002b050: 2020 2020 2065 6c69 6620 6275 7474 6f6e       elif button
-0002b060: 2e75 726c 3a0a 2020 2020 2020 2020 2020  .url:.          
-0002b070: 2020 2020 2020 7265 7475 726e 2062 7574        return but
-0002b080: 746f 6e2e 7572 6c0a 2020 2020 2020 2020  ton.url.        
-0002b090: 2020 2020 656c 6966 2062 7574 746f 6e2e      elif button.
-0002b0a0: 6c6f 6769 6e5f 7572 6c3a 0a20 2020 2020  login_url:.     
-0002b0b0: 2020 2020 2020 2020 2020 2074 6c75 203d             tlu =
-0002b0c0: 2062 7574 746f 6e2e 6c6f 6769 6e5f 7572   button.login_ur
-0002b0d0: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
-0002b0e0: 2020 7269 6565 7020 3d20 6177 6169 7420    rieep = await 
-0002b0f0: 7365 6c66 2e5f 636c 6965 6e74 2e72 6573  self._client.res
-0002b100: 6f6c 7665 5f70 6565 7228 0a20 2020 2020  olve_peer(.     
-0002b110: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0002b120: 656c 662e 6368 6174 2e69 640a 2020 2020  elf.chat.id.    
-0002b130: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0002b140: 2020 2020 2020 2020 2020 2020 2020 6f6b                ok
-0002b150: 6475 6974 203d 2061 7761 6974 2073 656c  duit = await sel
-0002b160: 662e 5f63 6c69 656e 742e 696e 766f 6b65  f._client.invoke
-0002b170: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002b180: 2020 2020 2020 7261 772e 6675 6e63 7469        raw.functi
-0002b190: 6f6e 732e 6d65 7373 6167 6573 2e52 6571  ons.messages.Req
-0002b1a0: 7565 7374 5572 6c41 7574 6828 0a20 2020  uestUrlAuth(.   
-0002b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b1c0: 2020 2020 2070 6565 723d 7269 6565 702c       peer=rieep,
-0002b1d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b1e0: 2020 2020 2020 2020 206d 7367 5f69 643d           msg_id=
-0002b1f0: 7365 6c66 2e69 642c 0a20 2020 2020 2020  self.id,.       
-0002b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b210: 2062 7574 746f 6e5f 6964 3d74 6c75 2e62   button_id=tlu.b
-0002b220: 7574 746f 6e5f 6964 2c0a 2020 2020 2020  utton_id,.      
-0002b230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b240: 2020 7572 6c3d 746c 752e 7572 6c0a 2020    url=tlu.url.  
-0002b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b260: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0002b270: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0002b280: 2020 2020 2020 7469 7564 6b6f 203d 2061        tiudko = a
-0002b290: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
-0002b2a0: 742e 696e 766f 6b65 280a 2020 2020 2020  t.invoke(.      
-0002b2b0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0002b2c0: 772e 6675 6e63 7469 6f6e 732e 6d65 7373  w.functions.mess
-0002b2d0: 6167 6573 2e41 6363 6570 7455 726c 4175  ages.AcceptUrlAu
-0002b2e0: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
-0002b2f0: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-0002b300: 655f 616c 6c6f 7765 643d 7265 7175 6573  e_allowed=reques
-0002b310: 745f 7772 6974 655f 6163 6365 7373 2c0a  t_write_access,.
-0002b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b330: 2020 2020 2020 2020 7065 6572 3d72 6965          peer=rie
-0002b340: 6570 2c0a 2020 2020 2020 2020 2020 2020  ep,.            
-0002b350: 2020 2020 2020 2020 2020 2020 6d73 675f              msg_
-0002b360: 6964 3d73 656c 662e 6964 2c0a 2020 2020  id=self.id,.    
-0002b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b380: 2020 2020 6275 7474 6f6e 5f69 643d 746c      button_id=tl
-0002b390: 752e 6275 7474 6f6e 5f69 642c 0a20 2020  u.button_id,.   
-0002b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b3b0: 2020 2020 2075 726c 3d74 6c75 2e75 726c       url=tlu.url
-0002b3c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b3d0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0002b3e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0002b3f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0002b400: 7469 7564 6b6f 2e75 726c 0a20 2020 2020  tiudko.url.     
-0002b410: 2020 2020 2020 2065 6c69 6620 6275 7474         elif butt
-0002b420: 6f6e 2e77 6562 5f61 7070 3a0a 2020 2020  on.web_app:.    
-0002b430: 2020 2020 2020 2020 2020 2020 746c 7520              tlu 
-0002b440: 3d20 6275 7474 6f6e 2e77 6562 5f61 7070  = button.web_app
-0002b450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b460: 2077 6869 6368 626f 7463 6861 7420 3d20   whichbotchat = 
-0002b470: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002b480: 2020 2020 2020 7365 6c66 2e76 6961 5f62        self.via_b
-0002b490: 6f74 2061 6e64 0a20 2020 2020 2020 2020  ot and.         
-0002b4a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002b4b0: 7669 615f 626f 742e 6964 0a20 2020 2020  via_bot.id.     
-0002b4c0: 2020 2020 2020 2020 2020 2029 206f 7220             ) or 
-0002b4d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002b4e0: 2020 2020 2020 7365 6c66 2e66 726f 6d5f        self.from_
-0002b4f0: 7573 6572 2061 6e64 0a20 2020 2020 2020  user and.       
-0002b500: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0002b510: 662e 6672 6f6d 5f75 7365 722e 6973 5f62  f.from_user.is_b
-0002b520: 6f74 2061 6e64 0a20 2020 2020 2020 2020  ot and.         
-0002b530: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002b540: 6672 6f6d 5f75 7365 722e 6964 0a20 2020  from_user.id.   
-0002b550: 2020 2020 2020 2020 2020 2020 2029 206f               ) o
-0002b560: 7220 4e6f 6e65 0a20 2020 2020 2020 2020  r None.         
-0002b570: 2020 2020 2020 2069 6620 6e6f 7420 7768         if not wh
-0002b580: 6963 6862 6f74 6368 6174 3a0a 2020 2020  ichbotchat:.    
-0002b590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b5a0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0002b5b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002b5c0: 2020 2020 2020 2020 2020 2249 6e76 616c            "Inval
-0002b5d0: 6964 2043 6861 7442 6f74 5479 7065 220a  id ChatBotType".
-0002b5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b5f0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0002b600: 2020 2020 2020 7269 6565 7020 3d20 6177        rieep = aw
-0002b610: 6169 7420 7365 6c66 2e5f 636c 6965 6e74  ait self._client
-0002b620: 2e72 6573 6f6c 7665 5f70 6565 7228 0a20  .resolve_peer(. 
-0002b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b640: 2020 2073 656c 662e 6368 6174 2e69 640a     self.chat.id.
-0002b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b660: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002b670: 2020 6965 6570 7220 3d20 6177 6169 7420    ieepr = await 
-0002b680: 7365 6c66 2e5f 636c 6965 6e74 2e72 6573  self._client.res
-0002b690: 6f6c 7665 5f70 6565 7228 0a20 2020 2020  olve_peer(.     
-0002b6a0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0002b6b0: 6869 6368 626f 7463 6861 740a 2020 2020  hichbotchat.    
-0002b6c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0002b6d0: 2020 2020 2020 2020 2020 2020 2020 6f6b                ok
-0002b6e0: 6475 6974 203d 2061 7761 6974 2073 656c  duit = await sel
-0002b6f0: 662e 5f63 6c69 656e 742e 696e 766f 6b65  f._client.invoke
-0002b700: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002b710: 2020 2020 2020 7261 772e 6675 6e63 7469        raw.functi
-0002b720: 6f6e 732e 6d65 7373 6167 6573 2e52 6571  ons.messages.Req
-0002b730: 7565 7374 5765 6256 6965 7728 0a20 2020  uestWebView(.   
-0002b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b750: 2020 2020 2070 6565 723d 7269 6565 702c       peer=rieep,
-0002b760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b770: 2020 2020 2020 2020 2062 6f74 3d69 6565           bot=iee
-0002b780: 7072 2c0a 2020 2020 2020 2020 2020 2020  pr,.            
-0002b790: 2020 2020 2020 2020 2020 2020 7572 6c3d              url=
-0002b7a0: 746c 752e 7572 6c2c 0a20 2020 2020 2020  tlu.url,.       
-0002b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b7c0: 2070 6c61 7466 6f72 6d3d 7365 6c66 2e5f   platform=self._
-0002b7d0: 636c 6965 6e74 2e63 6c69 656e 745f 706c  client.client_pl
-0002b7e0: 6174 666f 726d 2e76 616c 7565 2c0a 2020  atform.value,.  
-0002b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b800: 2020 2020 2020 2320 544f 444f 0a20 2020        # TODO.   
-0002b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b820: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0002b830: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0002b840: 2020 2020 2072 6574 7572 6e20 6f6b 6475       return okdu
-0002b850: 6974 2e75 726c 0a20 2020 2020 2020 2020  it.url.         
-0002b860: 2020 2065 6c69 6620 6275 7474 6f6e 2e75     elif button.u
-0002b870: 7365 725f 6964 3a0a 2020 2020 2020 2020  ser_id:.        
-0002b880: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-0002b890: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
-0002b8a0: 742e 6765 745f 6368 6174 280a 2020 2020  t.get_chat(.    
-0002b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b8c0: 6275 7474 6f6e 2e75 7365 725f 6964 2c0a  button.user_id,.
-0002b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b8e0: 2020 2020 4661 6c73 650a 2020 2020 2020      False.      
-0002b8f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0002b900: 2020 2020 2020 2020 656c 6966 2062 7574          elif but
-0002b910: 746f 6e2e 7377 6974 6368 5f69 6e6c 696e  ton.switch_inlin
-0002b920: 655f 7175 6572 793a 0a20 2020 2020 2020  e_query:.       
-0002b930: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0002b940: 6275 7474 6f6e 2e73 7769 7463 685f 696e  button.switch_in
-0002b950: 6c69 6e65 5f71 7565 7279 0a20 2020 2020  line_query.     
-0002b960: 2020 2020 2020 2065 6c69 6620 6275 7474         elif butt
-0002b970: 6f6e 2e73 7769 7463 685f 696e 6c69 6e65  on.switch_inline
-0002b980: 5f71 7565 7279 5f63 7572 7265 6e74 5f63  _query_current_c
-0002b990: 6861 743a 0a20 2020 2020 2020 2020 2020  hat:.           
-0002b9a0: 2020 2020 2072 6574 7572 6e20 6275 7474       return butt
-0002b9b0: 6f6e 2e73 7769 7463 685f 696e 6c69 6e65  on.switch_inline
-0002b9c0: 5f71 7565 7279 5f63 7572 7265 6e74 5f63  _query_current_c
-0002b9d0: 6861 740a 2020 2020 2020 2020 2020 2020  hat.            
-0002b9e0: 656c 6966 2062 7574 746f 6e2e 7377 6974  elif button.swit
-0002b9f0: 6368 5f69 6e6c 696e 655f 7175 6572 795f  ch_inline_query_
-0002ba00: 6368 6f73 656e 5f63 6861 743a 0a20 2020  chosen_chat:.   
-0002ba10: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0002ba20: 7572 6e20 6275 7474 6f6e 2e73 7769 7463  urn button.switc
-0002ba30: 685f 696e 6c69 6e65 5f71 7565 7279 5f63  h_inline_query_c
-0002ba40: 686f 7365 6e5f 6368 6174 0a20 2020 2020  hosen_chat.     
-0002ba50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0002ba60: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0002ba70: 7365 2056 616c 7565 4572 726f 7228 2254  se ValueError("T
-0002ba80: 6869 7320 6275 7474 6f6e 2069 7320 6e6f  his button is no
-0002ba90: 7420 7375 7070 6f72 7465 6420 7965 7422  t supported yet"
-0002baa0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0002bab0: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-0002bac0: 7420 7365 6c66 2e72 6570 6c79 2874 6578  t self.reply(tex
-0002bad0: 743d 6275 7474 6f6e 2c20 7175 6f74 653d  t=button, quote=
-0002bae0: 7175 6f74 6529 0a0a 2020 2020 6173 796e  quote)..    asyn
-0002baf0: 6320 6465 6620 7265 6163 7428 0a20 2020  c def react(.   
-0002bb00: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0002bb10: 2020 2072 6561 6374 696f 6e3a 2055 6e69     reaction: Uni
-0002bb20: 6f6e 5b0a 2020 2020 2020 2020 2020 2020  on[.            
-0002bb30: 696e 742c 0a20 2020 2020 2020 2020 2020  int,.           
-0002bb40: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-0002bb50: 2020 4c69 7374 5b55 6e69 6f6e 5b69 6e74    List[Union[int
-0002bb60: 2c20 7374 722c 2022 7479 7065 732e 5265  , str, "types.Re
-0002bb70: 6163 7469 6f6e 5479 7065 225d 5d0a 2020  actionType"]].  
-0002bb80: 2020 2020 2020 5d20 3d20 4e6f 6e65 2c0a        ] = None,.
-0002bb90: 2020 2020 2020 2020 6973 5f62 6967 3a20          is_big: 
-0002bba0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-0002bbb0: 2020 2020 2020 6164 645f 746f 5f72 6563        add_to_rec
-0002bbc0: 656e 743a 2062 6f6f 6c20 3d20 5472 7565  ent: bool = True
-0002bbd0: 0a20 2020 2029 202d 3e20 2274 7970 6573  .    ) -> "types
-0002bbe0: 2e4d 6573 7361 6765 5265 6163 7469 6f6e  .MessageReaction
-0002bbf0: 7322 3a0a 2020 2020 2020 2020 2222 2242  s":.        """B
-0002bc00: 6f75 6e64 206d 6574 686f 6420 2a72 6561  ound method *rea
-0002bc10: 6374 2a20 6f66 203a 6f62 6a3a 607e 7079  ct* of :obj:`~py
-0002bc20: 726f 6772 616d 2e74 7970 6573 2e4d 6573  rogram.types.Mes
-0002bc30: 7361 6765 602e 0a0a 2020 2020 2020 2020  sage`...        
-0002bc40: 5573 6520 6173 2061 2073 686f 7274 6375  Use as a shortcu
-0002bc50: 7420 666f 723a 0a0a 2020 2020 2020 2020  t for:..        
-0002bc60: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-0002bc70: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
-0002bc80: 2020 2020 6177 6169 7420 636c 6965 6e74      await client
-0002bc90: 2e73 6574 5f72 6561 6374 696f 6e28 0a20  .set_reaction(. 
-0002bca0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0002bcb0: 6861 745f 6964 3d63 6861 745f 6964 2c0a  hat_id=chat_id,.
-0002bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bcd0: 6d65 7373 6167 655f 6964 3d6d 6573 7361  message_id=messa
-0002bce0: 6765 2e69 642c 0a20 2020 2020 2020 2020  ge.id,.         
-0002bcf0: 2020 2020 2020 2072 6561 6374 696f 6e3d         reaction=
-0002bd00: 5b52 6561 6374 696f 6e54 7970 6545 6d6f  [ReactionTypeEmo
-0002bd10: 6a69 2865 6d6f 6a69 3d22 f09f 918d 2229  ji(emoji="....")
-0002bd20: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
-0002bd30: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-0002bd40: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-0002bd50: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-0002bd60: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-0002bd70: 2020 2020 2020 2320 5365 6e64 2061 2072        # Send a r
-0002bd80: 6561 6374 696f 6e0a 2020 2020 2020 2020  eaction.        
-0002bd90: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
-0002bda0: 7373 6167 652e 7265 6163 7428 5b52 6561  ssage.react([Rea
-0002bdb0: 6374 696f 6e54 7970 6545 6d6f 6a69 2865  ctionTypeEmoji(e
-0002bdc0: 6d6f 6a69 3d22 f09f 918d 2229 5d29 0a0a  moji="....")])..
-0002bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bde0: 2320 5265 7472 6163 7420 6120 7265 6163  # Retract a reac
-0002bdf0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-0002be00: 2020 2020 2061 7761 6974 206d 6573 7361       await messa
-0002be10: 6765 2e72 6561 6374 2829 0a0a 2020 2020  ge.react()..    
-0002be20: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
-0002be30: 2020 2020 2020 2020 2020 2020 7265 6163              reac
-0002be40: 7469 6f6e 2028 6060 696e 7460 6020 7c20  tion (``int`` | 
-0002be50: 6060 7374 7260 6020 7c20 4c69 7374 206f  ``str`` | List o
-0002be60: 6620 6060 696e 7460 6020 4f52 2060 6073  f ``int`` OR ``s
-0002be70: 7472 6060 207c 204c 6973 7420 6f66 203a  tr`` | List of :
-0002be80: 6f62 6a3a 607e 7079 726f 6772 616d 2e74  obj:`~pyrogram.t
-0002be90: 7970 6573 2e52 6561 6374 696f 6e54 7970  ypes.ReactionTyp
-0002bea0: 6560 2c20 2a6f 7074 696f 6e61 6c2a 293a  e`, *optional*):
-0002beb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002bec0: 204e 6577 206c 6973 7420 6f66 2072 6561   New list of rea
-0002bed0: 6374 696f 6e20 7479 7065 7320 746f 2073  ction types to s
-0002bee0: 6574 206f 6e20 7468 6520 6d65 7373 6167  et on the messag
-0002bef0: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
-0002bf00: 2020 2050 6173 7320 4e6f 6e65 2061 7320     Pass None as 
-0002bf10: 656d 6f6a 6920 2864 6566 6175 6c74 2920  emoji (default) 
-0002bf20: 746f 2072 6574 7261 6374 2074 6865 2072  to retract the r
-0002bf30: 6561 6374 696f 6e2e 0a0a 2020 2020 2020  eaction...      
-0002bf40: 2020 2020 2020 6973 5f62 6967 2028 6060        is_big (``
-0002bf50: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
-0002bf60: 6c2a 293a 0a20 2020 2020 2020 2020 2020  l*):.           
-0002bf70: 2020 2020 2050 6173 7320 5472 7565 2074       Pass True t
-0002bf80: 6f20 7365 7420 7468 6520 7265 6163 7469  o set the reacti
-0002bf90: 6f6e 2077 6974 6820 6120 6269 6720 616e  on with a big an
-0002bfa0: 696d 6174 696f 6e2e 0a20 2020 2020 2020  imation..       
-0002bfb0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-0002bfc0: 7320 746f 2046 616c 7365 2e0a 2020 2020  s to False..    
-0002bfd0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0002bfe0: 2020 2020 2061 6464 5f74 6f5f 7265 6365       add_to_rece
-0002bff0: 6e74 2028 6060 626f 6f6c 6060 2c20 2a6f  nt (``bool``, *o
-0002c000: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
-0002c010: 2020 2020 2020 2020 2020 2050 6173 7320             Pass 
-0002c020: 5472 7565 2069 6620 7468 6520 7265 6163  True if the reac
-0002c030: 7469 6f6e 2073 686f 756c 6420 6170 7065  tion should appe
-0002c040: 6172 2069 6e20 7468 6520 7265 6365 6e74  ar in the recent
-0002c050: 6c79 2075 7365 6420 7265 6163 7469 6f6e  ly used reaction
-0002c060: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-0002c070: 2020 2054 6869 7320 6f70 7469 6f6e 2069     This option i
-0002c080: 7320 6170 706c 6963 6162 6c65 206f 6e6c  s applicable onl
-0002c090: 7920 666f 7220 7573 6572 732e 0a20 2020  y for users..   
-0002c0a0: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-0002c0b0: 6175 6c74 7320 746f 2054 7275 652e 0a20  aults to True.. 
-0002c0c0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0002c0d0: 2020 2020 2020 2020 2020 2020 4f6e 2073              On s
-0002c0e0: 7563 6365 7373 2c20 3a6f 626a 3a60 7e70  uccess, :obj:`~p
-0002c0f0: 7972 6f67 7261 6d2e 7479 7065 732e 4d65  yrogram.types.Me
-0002c100: 7373 6167 6552 6561 6374 696f 6e73 603a  ssageReactions`:
-0002c110: 2069 7320 7265 7475 726e 6564 2e0a 0a20   is returned... 
-0002c120: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
-0002c130: 2020 2020 2020 2020 2020 2052 5043 4572             RPCEr
-0002c140: 726f 723a 2049 6e20 6361 7365 206f 6620  ror: In case of 
-0002c150: 6120 5465 6c65 6772 616d 2052 5043 2065  a Telegram RPC e
-0002c160: 7272 6f72 2e0a 2020 2020 2020 2020 2222  rror..        ""
-0002c170: 220a 2020 2020 2020 2020 7372 203d 204e  ".        sr = N
-0002c180: 6f6e 650a 0a20 2020 2020 2020 2069 6620  one..        if 
-0002c190: 6973 696e 7374 616e 6365 2872 6561 6374  isinstance(react
-0002c1a0: 696f 6e2c 204c 6973 7429 3a0a 2020 2020  ion, List):.    
-0002c1b0: 2020 2020 2020 2020 7372 203d 205b 5d0a          sr = [].
-0002c1c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0002c1d0: 6920 696e 2072 6561 6374 696f 6e3a 0a20  i in reaction:. 
-0002c1e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0002c1f0: 6620 6973 696e 7374 616e 6365 2869 2c20  f isinstance(i, 
-0002c200: 7479 7065 732e 5265 6163 7469 6f6e 5479  types.ReactionTy
-0002c210: 7065 293a 0a20 2020 2020 2020 2020 2020  pe):.           
-0002c220: 2020 2020 2020 2020 2073 722e 6170 7065           sr.appe
-0002c230: 6e64 2869 290a 2020 2020 2020 2020 2020  nd(i).          
-0002c240: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-0002c250: 7461 6e63 6528 692c 2069 6e74 293a 0a20  tance(i, int):. 
-0002c260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c270: 2020 2073 722e 6170 7065 6e64 2874 7970     sr.append(typ
-0002c280: 6573 2e52 6561 6374 696f 6e54 7970 6543  es.ReactionTypeC
-0002c290: 7573 746f 6d45 6d6f 6a69 280a 2020 2020  ustomEmoji(.    
-0002c2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c2b0: 2020 2020 6375 7374 6f6d 5f65 6d6f 6a69      custom_emoji
-0002c2c0: 5f69 643d 7374 7228 6929 0a20 2020 2020  _id=str(i).     
-0002c2d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0002c2e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002c2f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0002c300: 2020 2020 2020 2020 2020 2020 7372 2e61              sr.a
-0002c310: 7070 656e 6428 7479 7065 732e 5265 6163  ppend(types.Reac
-0002c320: 7469 6f6e 5479 7065 456d 6f6a 6928 0a20  tionTypeEmoji(. 
-0002c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c340: 2020 2020 2020 2065 6d6f 6a69 3d69 0a20         emoji=i. 
-0002c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c360: 2020 2029 290a 0a20 2020 2020 2020 2065     ))..        e
-0002c370: 6c69 6620 6973 696e 7374 616e 6365 2872  lif isinstance(r
-0002c380: 6561 6374 696f 6e2c 2069 6e74 293a 0a20  eaction, int):. 
-0002c390: 2020 2020 2020 2020 2020 2073 7220 3d20             sr = 
-0002c3a0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-0002c3b0: 2020 7479 7065 732e 5265 6163 7469 6f6e    types.Reaction
-0002c3c0: 5479 7065 4375 7374 6f6d 456d 6f6a 6928  TypeCustomEmoji(
-0002c3d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002c3e0: 2020 2020 2063 7573 746f 6d5f 656d 6f6a       custom_emoj
-0002c3f0: 695f 6964 3d73 7472 2872 6561 6374 696f  i_id=str(reactio
-0002c400: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-0002c410: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0002c420: 205d 0a0a 2020 2020 2020 2020 656c 6966   ]..        elif
-0002c430: 2069 7369 6e73 7461 6e63 6528 7265 6163   isinstance(reac
-0002c440: 7469 6f6e 2c20 7374 7229 3a0a 2020 2020  tion, str):.    
-0002c450: 2020 2020 2020 2020 7372 203d 205b 0a20          sr = [. 
-0002c460: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0002c470: 7970 6573 2e52 6561 6374 696f 6e54 7970  ypes.ReactionTyp
-0002c480: 6545 6d6f 6a69 280a 2020 2020 2020 2020  eEmoji(.        
-0002c490: 2020 2020 2020 2020 2020 2020 656d 6f6a              emoj
-0002c4a0: 693d 7265 6163 7469 6f6e 0a20 2020 2020  i=reaction.     
-0002c4b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0002c4c0: 2020 2020 2020 2020 205d 0a0a 2020 2020           ]..    
-0002c4d0: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-0002c4e0: 2073 656c 662e 5f63 6c69 656e 742e 7365   self._client.se
-0002c4f0: 745f 7265 6163 7469 6f6e 280a 2020 2020  t_reaction(.    
-0002c500: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
-0002c510: 7365 6c66 2e63 6861 742e 6964 2c0a 2020  self.chat.id,.  
-0002c520: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-0002c530: 655f 6964 3d73 656c 662e 6964 2c0a 2020  e_id=self.id,.  
-0002c540: 2020 2020 2020 2020 2020 7265 6163 7469            reacti
-0002c550: 6f6e 3d73 722c 0a20 2020 2020 2020 2020  on=sr,.         
-0002c560: 2020 2069 735f 6269 673d 6973 5f62 6967     is_big=is_big
-0002c570: 2c0a 2020 2020 2020 2020 2020 2020 6164  ,.            ad
-0002c580: 645f 746f 5f72 6563 656e 743d 6164 645f  d_to_recent=add_
-0002c590: 746f 5f72 6563 656e 740a 2020 2020 2020  to_recent.      
-0002c5a0: 2020 290a 0a20 2020 2061 7379 6e63 2064    )..    async d
-0002c5b0: 6566 2072 6574 7261 6374 5f76 6f74 6528  ef retract_vote(
-0002c5c0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0002c5d0: 2020 2029 202d 3e20 2274 7970 6573 2e50     ) -> "types.P
-0002c5e0: 6f6c 6c22 3a0a 2020 2020 2020 2020 2222  oll":.        ""
-0002c5f0: 2242 6f75 6e64 206d 6574 686f 6420 2a72  "Bound method *r
-0002c600: 6574 7261 6374 5f76 6f74 652a 206f 6620  etract_vote* of 
-0002c610: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
-0002c620: 7479 7065 732e 4d65 7373 6167 6560 2e0a  types.Message`..
-0002c630: 0a20 2020 2020 2020 2055 7365 2061 7320  .        Use as 
-0002c640: 6120 7368 6f72 7463 7574 2066 6f72 3a0a  a shortcut for:.
-0002c650: 0a20 2020 2020 2020 202e 2e20 636f 6465  .        .. code
-0002c660: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-0002c670: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-0002c680: 656e 742e 7265 7472 6163 745f 766f 7465  ent.retract_vote
-0002c690: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002c6a0: 2020 6368 6174 5f69 643d 6d65 7373 6167    chat_id=messag
-0002c6b0: 652e 6368 6174 2e69 642c 0a20 2020 2020  e.chat.id,.     
-0002c6c0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-0002c6d0: 6765 5f69 643d 6d65 7373 6167 655f 6964  ge_id=message_id
-0002c6e0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0002c6f0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-0002c700: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-0002c710: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-0002c720: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-0002c730: 2020 2020 2020 6d65 7373 6167 652e 7265        message.re
-0002c740: 7472 6163 745f 766f 7465 2829 0a0a 2020  tract_vote()..  
-0002c750: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-0002c760: 2020 2020 2020 2020 2020 203a 6f62 6a3a             :obj:
-0002c770: 607e 7079 726f 6772 616d 2e74 7970 6573  `~pyrogram.types
-0002c780: 2e50 6f6c 6c60 3a20 4f6e 2073 7563 6365  .Poll`: On succe
-0002c790: 7373 2c20 7468 6520 706f 6c6c 2077 6974  ss, the poll wit
-0002c7a0: 6820 7468 6520 7265 7472 6163 7465 6420  h the retracted 
-0002c7b0: 766f 7465 2069 7320 7265 7475 726e 6564  vote is returned
-0002c7c0: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-0002c7d0: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-0002c7e0: 5043 4572 726f 723a 2049 6e20 6361 7365  PCError: In case
-0002c7f0: 206f 6620 6120 5465 6c65 6772 616d 2052   of a Telegram R
-0002c800: 5043 2065 7272 6f72 2e0a 2020 2020 2020  PC error..      
-0002c810: 2020 2222 220a 0a20 2020 2020 2020 2072    """..        r
-0002c820: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-0002c830: 2e5f 636c 6965 6e74 2e72 6574 7261 6374  ._client.retract
-0002c840: 5f76 6f74 6528 0a20 2020 2020 2020 2020  _vote(.         
-0002c850: 2020 2063 6861 745f 6964 3d73 656c 662e     chat_id=self.
-0002c860: 6368 6174 2e69 642c 0a20 2020 2020 2020  chat.id,.       
-0002c870: 2020 2020 206d 6573 7361 6765 5f69 643d       message_id=
-0002c880: 7365 6c66 2e69 640a 2020 2020 2020 2020  self.id.        
-0002c890: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-0002c8a0: 2064 6f77 6e6c 6f61 6428 0a20 2020 2020   download(.     
-0002c8b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0002c8c0: 2066 696c 655f 6e61 6d65 3a20 7374 7220   file_name: str 
-0002c8d0: 3d20 2222 2c0a 2020 2020 2020 2020 696e  = "",.        in
-0002c8e0: 5f6d 656d 6f72 793a 2062 6f6f 6c20 3d20  _memory: bool = 
-0002c8f0: 4661 6c73 652c 0a20 2020 2020 2020 2062  False,.        b
-0002c900: 6c6f 636b 3a20 626f 6f6c 203d 2054 7275  lock: bool = Tru
-0002c910: 652c 0a20 2020 2020 2020 2070 726f 6772  e,.        progr
-0002c920: 6573 733a 2043 616c 6c61 626c 6520 3d20  ess: Callable = 
-0002c930: 4e6f 6e65 2c0a 2020 2020 2020 2020 7072  None,.        pr
-0002c940: 6f67 7265 7373 5f61 7267 733a 2074 7570  ogress_args: tup
-0002c950: 6c65 203d 2028 290a 2020 2020 2920 2d3e  le = ().    ) ->
-0002c960: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
-0002c970: 2242 6f75 6e64 206d 6574 686f 6420 2a64  "Bound method *d
-0002c980: 6f77 6e6c 6f61 642a 206f 6620 3a6f 626a  ownload* of :obj
-0002c990: 3a60 7e70 7972 6f67 7261 6d2e 7479 7065  :`~pyrogram.type
-0002c9a0: 732e 4d65 7373 6167 6560 2e0a 0a20 2020  s.Message`...   
-0002c9b0: 2020 2020 2055 7365 2061 7320 6120 7368       Use as a sh
-0002c9c0: 6f72 7463 7574 2066 6f72 3a0a 0a20 2020  ortcut for:..   
-0002c9d0: 2020 2020 202e 2e20 636f 6465 2d62 6c6f       .. code-blo
-0002c9e0: 636b 3a3a 2070 7974 686f 6e0a 0a20 2020  ck:: python..   
-0002c9f0: 2020 2020 2020 2020 2061 7761 6974 2063           await c
-0002ca00: 6c69 656e 742e 646f 776e 6c6f 6164 5f6d  lient.download_m
-0002ca10: 6564 6961 286d 6573 7361 6765 290a 0a20  edia(message).. 
-0002ca20: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
-0002ca30: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
-0002ca40: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-0002ca50: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-0002ca60: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
-0002ca70: 652e 646f 776e 6c6f 6164 2829 0a0a 2020  e.download()..  
-0002ca80: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0002ca90: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
-0002caa0: 6c65 5f6e 616d 6520 2860 6073 7472 6060  le_name (``str``
-0002cab0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
-0002cac0: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-0002cad0: 2063 7573 746f 6d20 2a66 696c 655f 6e61   custom *file_na
-0002cae0: 6d65 2a20 746f 2062 6520 7573 6564 2069  me* to be used i
-0002caf0: 6e73 7465 6164 206f 6620 7468 6520 6f6e  nstead of the on
-0002cb00: 6520 7072 6f76 6964 6564 2062 7920 5465  e provided by Te
-0002cb10: 6c65 6772 616d 2e0a 2020 2020 2020 2020  legram..        
-0002cb20: 2020 2020 2020 2020 4279 2064 6566 6175          By defau
-0002cb30: 6c74 2c20 616c 6c20 6669 6c65 7320 6172  lt, all files ar
-0002cb40: 6520 646f 776e 6c6f 6164 6564 2069 6e20  e downloaded in 
-0002cb50: 7468 6520 2a64 6f77 6e6c 6f61 6473 2a20  the *downloads* 
-0002cb60: 666f 6c64 6572 2069 6e20 796f 7572 2077  folder in your w
-0002cb70: 6f72 6b69 6e67 2064 6972 6563 746f 7279  orking directory
-0002cb80: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0002cb90: 2020 596f 7520 6361 6e20 616c 736f 2073    You can also s
-0002cba0: 7065 6369 6679 2061 2070 6174 6820 666f  pecify a path fo
-0002cbb0: 7220 646f 776e 6c6f 6164 696e 6720 6669  r downloading fi
-0002cbc0: 6c65 7320 696e 2061 2063 7573 746f 6d20  les in a custom 
-0002cbd0: 6c6f 6361 7469 6f6e 3a20 7061 7468 7320  location: paths 
-0002cbe0: 7468 6174 2065 6e64 2077 6974 6820 222f  that end with "/
-0002cbf0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0002cc00: 2020 6172 6520 636f 6e73 6964 6572 6564    are considered
-0002cc10: 2064 6972 6563 746f 7269 6573 2e20 416c   directories. Al
-0002cc20: 6c20 6e6f 6e2d 6578 6973 7465 6e74 2066  l non-existent f
-0002cc30: 6f6c 6465 7273 2077 696c 6c20 6265 2063  olders will be c
-0002cc40: 7265 6174 6564 2061 7574 6f6d 6174 6963  reated automatic
-0002cc50: 616c 6c79 2e0a 0a20 2020 2020 2020 2020  ally...         
-0002cc60: 2020 2069 6e5f 6d65 6d6f 7279 2028 6060     in_memory (``
-0002cc70: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
-0002cc80: 6c2a 293a 0a20 2020 2020 2020 2020 2020  l*):.           
-0002cc90: 2020 2020 2050 6173 7320 5472 7565 2074       Pass True t
-0002cca0: 6f20 646f 776e 6c6f 6164 2074 6865 206d  o download the m
-0002ccb0: 6564 6961 2069 6e2d 6d65 6d6f 7279 2e0a  edia in-memory..
-0002ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ccd0: 4120 6269 6e61 7279 2066 696c 652d 6c69  A binary file-li
-0002cce0: 6b65 206f 626a 6563 7420 7769 7468 2069  ke object with i
-0002ccf0: 7473 2061 7474 7269 6275 7465 2022 2e6e  ts attribute ".n
-0002cd00: 616d 6522 2073 6574 2077 696c 6c20 6265  ame" set will be
-0002cd10: 2072 6574 7572 6e65 642e 0a20 2020 2020   returned..     
-0002cd20: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-0002cd30: 6c74 7320 746f 2046 616c 7365 2e0a 0a20  lts to False... 
-0002cd40: 2020 2020 2020 2020 2020 2062 6c6f 636b             block
-0002cd50: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
-0002cd60: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
-0002cd70: 2020 2020 2020 2020 2042 6c6f 636b 7320           Blocks 
-0002cd80: 7468 6520 636f 6465 2065 7865 6375 7469  the code executi
-0002cd90: 6f6e 2075 6e74 696c 2074 6865 2066 696c  on until the fil
-0002cda0: 6520 6861 7320 6265 656e 2064 6f77 6e6c  e has been downl
-0002cdb0: 6f61 6465 642e 0a20 2020 2020 2020 2020  oaded..         
-0002cdc0: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-0002cdd0: 746f 2054 7275 652e 0a0a 2020 2020 2020  to True...      
-0002cde0: 2020 2020 2020 7072 6f67 7265 7373 2028        progress (
-0002cdf0: 6060 4361 6c6c 6162 6c65 6060 2c20 2a6f  ``Callable``, *o
-0002ce00: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
-0002ce10: 2020 2020 2020 2020 2020 2050 6173 7320             Pass 
-0002ce20: 6120 6361 6c6c 6261 636b 2066 756e 6374  a callback funct
-0002ce30: 696f 6e20 746f 2076 6965 7720 7468 6520  ion to view the 
-0002ce40: 6669 6c65 2074 7261 6e73 6d69 7373 696f  file transmissio
-0002ce50: 6e20 7072 6f67 7265 7373 2e0a 2020 2020  n progress..    
-0002ce60: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0002ce70: 6675 6e63 7469 6f6e 206d 7573 7420 7461  function must ta
-0002ce80: 6b65 202a 2863 7572 7265 6e74 2c20 746f  ke *(current, to
-0002ce90: 7461 6c29 2a20 6173 2070 6f73 6974 696f  tal)* as positio
-0002cea0: 6e61 6c20 6172 6775 6d65 6e74 7320 286c  nal arguments (l
-0002ceb0: 6f6f 6b20 6174 204f 7468 6572 2050 6172  ook at Other Par
-0002cec0: 616d 6574 6572 7320 6265 6c6f 7720 666f  ameters below fo
-0002ced0: 7220 610a 2020 2020 2020 2020 2020 2020  r a.            
-0002cee0: 2020 2020 6465 7461 696c 6564 2064 6573      detailed des
-0002cef0: 6372 6970 7469 6f6e 2920 616e 6420 7769  cription) and wi
-0002cf00: 6c6c 2062 6520 6361 6c6c 6564 2062 6163  ll be called bac
-0002cf10: 6b20 6561 6368 2074 696d 6520 6120 6e65  k each time a ne
-0002cf20: 7720 6669 6c65 2063 6875 6e6b 2068 6173  w file chunk has
-0002cf30: 2062 6565 6e20 7375 6363 6573 7366 756c   been successful
-0002cf40: 6c79 0a20 2020 2020 2020 2020 2020 2020  ly.             
-0002cf50: 2020 2074 7261 6e73 6d69 7474 6564 2e0a     transmitted..
-0002cf60: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-0002cf70: 6772 6573 735f 6172 6773 2028 6060 7475  gress_args (``tu
-0002cf80: 706c 6560 602c 202a 6f70 7469 6f6e 616c  ple``, *optional
-0002cf90: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
-0002cfa0: 2020 2020 4578 7472 6120 6375 7374 6f6d      Extra custom
-0002cfb0: 2061 7267 756d 656e 7473 2066 6f72 2074   arguments for t
-0002cfc0: 6865 2070 726f 6772 6573 7320 6361 6c6c  he progress call
-0002cfd0: 6261 636b 2066 756e 6374 696f 6e2e 0a20  back function.. 
-0002cfe0: 2020 2020 2020 2020 2020 2020 2020 2059                 Y
-0002cff0: 6f75 2063 616e 2070 6173 7320 616e 7974  ou can pass anyt
-0002d000: 6869 6e67 2079 6f75 206e 6565 6420 746f  hing you need to
-0002d010: 2062 6520 6176 6169 6c61 626c 6520 696e   be available in
-0002d020: 2074 6865 2070 726f 6772 6573 7320 6361   the progress ca
-0002d030: 6c6c 6261 636b 2073 636f 7065 3b20 666f  llback scope; fo
-0002d040: 7220 6578 616d 706c 652c 2061 204d 6573  r example, a Mes
-0002d050: 7361 6765 0a20 2020 2020 2020 2020 2020  sage.           
-0002d060: 2020 2020 206f 626a 6563 7420 6f72 2061       object or a
-0002d070: 2043 6c69 656e 7420 696e 7374 616e 6365   Client instance
-0002d080: 2069 6e20 6f72 6465 7220 746f 2065 6469   in order to edi
-0002d090: 7420 7468 6520 6d65 7373 6167 6520 7769  t the message wi
-0002d0a0: 7468 2074 6865 2075 7064 6174 6564 2070  th the updated p
-0002d0b0: 726f 6772 6573 7320 7374 6174 7573 2e0a  rogress status..
-0002d0c0: 0a20 2020 2020 2020 204f 7468 6572 2050  .        Other P
-0002d0d0: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
-0002d0e0: 2020 2020 2020 2063 7572 7265 6e74 2028         current (
-0002d0f0: 6060 696e 7460 6029 3a0a 2020 2020 2020  ``int``):.      
-0002d100: 2020 2020 2020 2020 2020 5468 6520 616d            The am
-0002d110: 6f75 6e74 206f 6620 6279 7465 7320 7472  ount of bytes tr
-0002d120: 616e 736d 6974 7465 6420 736f 2066 6172  ansmitted so far
-0002d130: 2e0a 0a20 2020 2020 2020 2020 2020 2074  ...            t
-0002d140: 6f74 616c 2028 6060 696e 7460 6029 3a0a  otal (``int``):.
-0002d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d160: 5468 6520 746f 7461 6c20 7369 7a65 206f  The total size o
-0002d170: 6620 7468 6520 6669 6c65 2e0a 0a20 2020  f the file...   
-0002d180: 2020 2020 2020 2020 202a 6172 6773 2028           *args (
-0002d190: 6060 7475 706c 6560 602c 202a 6f70 7469  ``tuple``, *opti
-0002d1a0: 6f6e 616c 2a29 3a0a 2020 2020 2020 2020  onal*):.        
-0002d1b0: 2020 2020 2020 2020 4578 7472 6120 6375          Extra cu
-0002d1c0: 7374 6f6d 2061 7267 756d 656e 7473 2061  stom arguments a
-0002d1d0: 7320 6465 6669 6e65 6420 696e 2074 6865  s defined in the
-0002d1e0: 2060 6070 726f 6772 6573 735f 6172 6773   ``progress_args
-0002d1f0: 6060 2070 6172 616d 6574 6572 2e0a 2020  `` parameter..  
-0002d200: 2020 2020 2020 2020 2020 2020 2020 596f                Yo
-0002d210: 7520 6361 6e20 6569 7468 6572 206b 6565  u can either kee
-0002d220: 7020 6060 2a61 7267 7360 6020 6f72 2061  p ``*args`` or a
-0002d230: 6464 2065 7665 7279 2073 696e 676c 6520  dd every single 
-0002d240: 6578 7472 6120 6172 6775 6d65 6e74 2069  extra argument i
-0002d250: 6e20 796f 7572 2066 756e 6374 696f 6e20  n your function 
-0002d260: 7369 676e 6174 7572 652e 0a0a 2020 2020  signature...    
-0002d270: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0002d280: 2020 2020 2020 2020 204f 6e20 7375 6363           On succ
-0002d290: 6573 732c 2074 6865 2061 6273 6f6c 7574  ess, the absolut
-0002d2a0: 6520 7061 7468 206f 6620 7468 6520 646f  e path of the do
-0002d2b0: 776e 6c6f 6164 6564 2066 696c 6520 6173  wnloaded file as
-0002d2c0: 2073 7472 696e 6720 6973 2072 6574 7572   string is retur
-0002d2d0: 6e65 642c 204e 6f6e 6520 6f74 6865 7277  ned, None otherw
-0002d2e0: 6973 652e 0a0a 2020 2020 2020 2020 5261  ise...        Ra
-0002d2f0: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
-0002d300: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
-0002d310: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
-0002d320: 6d20 5250 4320 6572 726f 722e 0a20 2020  m RPC error..   
-0002d330: 2020 2020 2020 2020 2060 6056 616c 7565           ``Value
-0002d340: 4572 726f 7260 603a 2049 6620 7468 6520  Error``: If the 
-0002d350: 6d65 7373 6167 6520 646f 6573 6e27 7420  message doesn't 
-0002d360: 636f 6e74 6169 6e20 616e 7920 646f 776e  contain any down
-0002d370: 6c6f 6164 6162 6c65 206d 6564 6961 0a20  loadable media. 
-0002d380: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0002d390: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-0002d3a0: 7365 6c66 2e5f 636c 6965 6e74 2e64 6f77  self._client.dow
-0002d3b0: 6e6c 6f61 645f 6d65 6469 6128 0a20 2020  nload_media(.   
-0002d3c0: 2020 2020 2020 2020 206d 6573 7361 6765           message
-0002d3d0: 3d73 656c 662c 0a20 2020 2020 2020 2020  =self,.         
-0002d3e0: 2020 2066 696c 655f 6e61 6d65 3d66 696c     file_name=fil
-0002d3f0: 655f 6e61 6d65 2c0a 2020 2020 2020 2020  e_name,.        
-0002d400: 2020 2020 696e 5f6d 656d 6f72 793d 696e      in_memory=in
-0002d410: 5f6d 656d 6f72 792c 0a20 2020 2020 2020  _memory,.       
-0002d420: 2020 2020 2062 6c6f 636b 3d62 6c6f 636b       block=block
-0002d430: 2c0a 2020 2020 2020 2020 2020 2020 7072  ,.            pr
-0002d440: 6f67 7265 7373 3d70 726f 6772 6573 732c  ogress=progress,
-0002d450: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-0002d460: 6772 6573 735f 6172 6773 3d70 726f 6772  gress_args=progr
-0002d470: 6573 735f 6172 6773 2c0a 2020 2020 2020  ess_args,.      
-0002d480: 2020 290a 0a20 2020 2061 7379 6e63 2064    )..    async d
-0002d490: 6566 2076 6f74 6528 0a20 2020 2020 2020  ef vote(.       
-0002d4a0: 2073 656c 662c 0a20 2020 2020 2020 206f   self,.        o
-0002d4b0: 7074 696f 6e3a 2069 6e74 2c0a 2020 2020  ption: int,.    
-0002d4c0: 2920 2d3e 2022 7479 7065 732e 506f 6c6c  ) -> "types.Poll
-0002d4d0: 223a 0a20 2020 2020 2020 2022 2222 426f  ":.        """Bo
-0002d4e0: 756e 6420 6d65 7468 6f64 202a 766f 7465  und method *vote
-0002d4f0: 2a20 6f66 203a 6f62 6a3a 607e 7079 726f  * of :obj:`~pyro
-0002d500: 6772 616d 2e74 7970 6573 2e4d 6573 7361  gram.types.Messa
-0002d510: 6765 602e 0a0a 2020 2020 2020 2020 5573  ge`...        Us
-0002d520: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
-0002d530: 666f 723a 0a0a 2020 2020 2020 2020 2e2e  for:..        ..
-0002d540: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-0002d550: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-0002d560: 2020 636c 6965 6e74 2e76 6f74 655f 706f    client.vote_po
-0002d570: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
-0002d580: 2020 2020 6368 6174 5f69 643d 6d65 7373      chat_id=mess
-0002d590: 6167 652e 6368 6174 2e69 642c 0a20 2020  age.chat.id,.   
-0002d5a0: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-0002d5b0: 7361 6765 5f69 643d 6d65 7373 6167 652e  sage_id=message.
-0002d5c0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-0002d5d0: 2020 2020 6f70 7469 6f6e 3d31 0a20 2020      option=1.   
-0002d5e0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0002d5f0: 2020 2020 4578 616d 706c 653a 0a20 2020      Example:.   
-0002d600: 2020 2020 2020 2020 202e 2e20 636f 6465           .. code
-0002d610: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-0002d620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002d630: 206d 6573 7361 6765 2e76 6f74 6528 3629   message.vote(6)
-0002d640: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0002d650: 7465 7273 3a0a 2020 2020 2020 2020 2020  ters:.          
-0002d660: 2020 6f70 7469 6f6e 2028 6060 696e 7460    option (``int`
-0002d670: 6029 3a0a 2020 2020 2020 2020 2020 2020  `):.            
-0002d680: 2020 2020 496e 6465 7820 6f66 2074 6865      Index of the
-0002d690: 2070 6f6c 6c20 6f70 7469 6f6e 2079 6f75   poll option you
-0002d6a0: 2077 616e 7420 746f 2076 6f74 6520 666f   want to vote fo
-0002d6b0: 7220 2830 2074 6f20 3929 2e0a 0a20 2020  r (0 to 9)...   
-0002d6c0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0002d6d0: 2020 2020 2020 2020 2020 3a6f 626a 3a60            :obj:`
-0002d6e0: 7e70 7972 6f67 7261 6d2e 7479 7065 732e  ~pyrogram.types.
-0002d6f0: 506f 6c6c 603a 204f 6e20 7375 6363 6573  Poll`: On succes
-0002d700: 732c 2074 6865 2070 6f6c 6c20 7769 7468  s, the poll with
-0002d710: 2074 6865 2063 686f 7365 6e20 6f70 7469   the chosen opti
-0002d720: 6f6e 2069 7320 7265 7475 726e 6564 2e0a  on is returned..
-0002d730: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
-0002d740: 0a20 2020 2020 2020 2020 2020 2052 5043  .            RPC
-0002d750: 4572 726f 723a 2049 6e20 6361 7365 206f  Error: In case o
-0002d760: 6620 6120 5465 6c65 6772 616d 2052 5043  f a Telegram RPC
-0002d770: 2065 7272 6f72 2e0a 2020 2020 2020 2020   error..        
-0002d780: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
-0002d790: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
-0002d7a0: 636c 6965 6e74 2e76 6f74 655f 706f 6c6c  client.vote_poll
-0002d7b0: 280a 2020 2020 2020 2020 2020 2020 6368  (.            ch
-0002d7c0: 6174 5f69 643d 7365 6c66 2e63 6861 742e  at_id=self.chat.
-0002d7d0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-0002d7e0: 6d65 7373 6167 655f 6964 3d73 656c 662e  message_id=self.
-0002d7f0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-0002d800: 6f70 7469 6f6e 733d 6f70 7469 6f6e 0a20  options=option. 
-0002d810: 2020 2020 2020 2029 0a0a 2020 2020 6173         )..    as
-0002d820: 796e 6320 6465 6620 7069 6e28 7365 6c66  ync def pin(self
-0002d830: 2c20 6469 7361 626c 655f 6e6f 7469 6669  , disable_notifi
-0002d840: 6361 7469 6f6e 3a20 626f 6f6c 203d 2046  cation: bool = F
-0002d850: 616c 7365 2c20 626f 7468 5f73 6964 6573  alse, both_sides
-0002d860: 3a20 626f 6f6c 203d 2046 616c 7365 2920  : bool = False) 
-0002d870: 2d3e 2022 7479 7065 732e 4d65 7373 6167  -> "types.Messag
-0002d880: 6522 3a0a 2020 2020 2020 2020 2222 2242  e":.        """B
-0002d890: 6f75 6e64 206d 6574 686f 6420 2a70 696e  ound method *pin
-0002d8a0: 2a20 6f66 203a 6f62 6a3a 607e 7079 726f  * of :obj:`~pyro
-0002d8b0: 6772 616d 2e74 7970 6573 2e4d 6573 7361  gram.types.Messa
-0002d8c0: 6765 602e 0a0a 2020 2020 2020 2020 5573  ge`...        Us
-0002d8d0: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
-0002d8e0: 666f 723a 0a0a 2020 2020 2020 2020 2e2e  for:..        ..
-0002d8f0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-0002d900: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-0002d910: 2020 6177 6169 7420 636c 6965 6e74 2e70    await client.p
-0002d920: 696e 5f63 6861 745f 6d65 7373 6167 6528  in_chat_message(
-0002d930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002d940: 2063 6861 745f 6964 3d6d 6573 7361 6765   chat_id=message
-0002d950: 2e63 6861 742e 6964 2c0a 2020 2020 2020  .chat.id,.      
-0002d960: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-0002d970: 655f 6964 3d6d 6573 7361 6765 5f69 640a  e_id=message_id.
-0002d980: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0002d990: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
-0002d9a0: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
-0002d9b0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-0002d9c0: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-0002d9d0: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
-0002d9e0: 652e 7069 6e28 290a 0a20 2020 2020 2020  e.pin()..       
-0002d9f0: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
-0002da00: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
-0002da10: 5f6e 6f74 6966 6963 6174 696f 6e20 2860  _notification (`
-0002da20: 6062 6f6f 6c60 6029 3a0a 2020 2020 2020  `bool``):.      
-0002da30: 2020 2020 2020 2020 2020 5061 7373 2054            Pass T
-0002da40: 7275 652c 2069 6620 6974 2069 7320 6e6f  rue, if it is no
-0002da50: 7420 6e65 6365 7373 6172 7920 746f 2073  t necessary to s
-0002da60: 656e 6420 6120 6e6f 7469 6669 6361 7469  end a notificati
-0002da70: 6f6e 2074 6f20 616c 6c20 6368 6174 206d  on to all chat m
-0002da80: 656d 6265 7273 2061 626f 7574 2074 6865  embers about the
-0002da90: 206e 6577 2070 696e 6e65 640a 2020 2020   new pinned.    
-0002daa0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-0002dab0: 6167 652e 204e 6f74 6966 6963 6174 696f  age. Notificatio
-0002dac0: 6e73 2061 7265 2061 6c77 6179 7320 6469  ns are always di
-0002dad0: 7361 626c 6564 2069 6e20 6368 616e 6e65  sabled in channe
-0002dae0: 6c73 2e0a 0a20 2020 2020 2020 2020 2020  ls...           
-0002daf0: 2062 6f74 685f 7369 6465 7320 2860 6062   both_sides (``b
-0002db00: 6f6f 6c60 602c 202a 6f70 7469 6f6e 616c  ool``, *optional
-0002db10: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
-0002db20: 2020 2020 5061 7373 2054 7275 6520 746f      Pass True to
-0002db30: 2070 696e 2074 6865 206d 6573 7361 6765   pin the message
-0002db40: 2066 6f72 2062 6f74 6820 7369 6465 7320   for both sides 
-0002db50: 2879 6f75 2061 6e64 2072 6563 6970 6965  (you and recipie
-0002db60: 6e74 292e 0a20 2020 2020 2020 2020 2020  nt)..           
-0002db70: 2020 2020 2041 7070 6c69 6361 626c 6520       Applicable 
-0002db80: 746f 2070 7269 7661 7465 2063 6861 7473  to private chats
-0002db90: 206f 6e6c 792e 2044 6566 6175 6c74 7320   only. Defaults 
-0002dba0: 746f 2046 616c 7365 2e0a 0a20 2020 2020  to False...     
-0002dbb0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0002dbc0: 2020 2020 2020 2020 3a6f 626a 3a60 7e70          :obj:`~p
-0002dbd0: 7972 6f67 7261 6d2e 7479 7065 732e 4d65  yrogram.types.Me
-0002dbe0: 7373 6167 6560 3a20 4f6e 2073 7563 6365  ssage`: On succe
-0002dbf0: 7373 2c20 7468 6520 7365 7276 6963 6520  ss, the service 
-0002dc00: 6d65 7373 6167 6520 6973 2072 6574 7572  message is retur
-0002dc10: 6e65 642e 0a0a 2020 2020 2020 2020 5261  ned...        Ra
-0002dc20: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
-0002dc30: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
-0002dc40: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
-0002dc50: 6d20 5250 4320 6572 726f 722e 0a20 2020  m RPC error..   
-0002dc60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0002dc70: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-0002dc80: 6c66 2e5f 636c 6965 6e74 2e70 696e 5f63  lf._client.pin_c
-0002dc90: 6861 745f 6d65 7373 6167 6528 0a20 2020  hat_message(.   
-0002dca0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-0002dcb0: 3d73 656c 662e 6368 6174 2e69 642c 0a20  =self.chat.id,. 
-0002dcc0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-0002dcd0: 6765 5f69 643d 7365 6c66 2e69 642c 0a20  ge_id=self.id,. 
-0002dce0: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-0002dcf0: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3d  le_notification=
-0002dd00: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-0002dd10: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-0002dd20: 2020 626f 7468 5f73 6964 6573 3d62 6f74    both_sides=bot
-0002dd30: 685f 7369 6465 730a 2020 2020 2020 2020  h_sides.        
-0002dd40: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-0002dd50: 2075 6e70 696e 2873 656c 6629 202d 3e20   unpin(self) -> 
-0002dd60: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-0002dd70: 2242 6f75 6e64 206d 6574 686f 6420 2a75  "Bound method *u
-0002dd80: 6e70 696e 2a20 6f66 203a 6f62 6a3a 607e  npin* of :obj:`~
-0002dd90: 7079 726f 6772 616d 2e74 7970 6573 2e4d  pyrogram.types.M
-0002dda0: 6573 7361 6765 602e 0a0a 2020 2020 2020  essage`...      
-0002ddb0: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
-0002ddc0: 6375 7420 666f 723a 0a0a 2020 2020 2020  cut for:..      
-0002ddd0: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-0002dde0: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
-0002ddf0: 2020 2020 2020 6177 6169 7420 636c 6965        await clie
-0002de00: 6e74 2e75 6e70 696e 5f63 6861 745f 6d65  nt.unpin_chat_me
-0002de10: 7373 6167 6528 0a20 2020 2020 2020 2020  ssage(.         
-0002de20: 2020 2020 2020 2063 6861 745f 6964 3d6d         chat_id=m
-0002de30: 6573 7361 6765 2e63 6861 742e 6964 2c0a  essage.chat.id,.
-0002de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002de50: 6d65 7373 6167 655f 6964 3d6d 6573 7361  message_id=messa
-0002de60: 6765 5f69 640a 2020 2020 2020 2020 2020  ge_id.          
-0002de70: 2020 290a 0a20 2020 2020 2020 2045 7861    )..        Exa
-0002de80: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
-0002de90: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-0002dea0: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
-0002deb0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-0002dec0: 6d65 7373 6167 652e 756e 7069 6e28 290a  message.unpin().
-0002ded0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0002dee0: 3a0a 2020 2020 2020 2020 2020 2020 5472  :.            Tr
-0002def0: 7565 206f 6e20 7375 6363 6573 732e 0a0a  ue on success...
-0002df00: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
-0002df10: 2020 2020 2020 2020 2020 2020 5250 4345              RPCE
-0002df20: 7272 6f72 3a20 496e 2063 6173 6520 6f66  rror: In case of
-0002df30: 2061 2054 656c 6567 7261 6d20 5250 4320   a Telegram RPC 
-0002df40: 6572 726f 722e 0a20 2020 2020 2020 2022  error..        "
-0002df50: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-0002df60: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
-0002df70: 6965 6e74 2e75 6e70 696e 5f63 6861 745f  ient.unpin_chat_
-0002df80: 6d65 7373 6167 6528 0a20 2020 2020 2020  message(.       
-0002df90: 2020 2020 2063 6861 745f 6964 3d73 656c       chat_id=sel
-0002dfa0: 662e 6368 6174 2e69 642c 0a20 2020 2020  f.chat.id,.     
-0002dfb0: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
-0002dfc0: 643d 7365 6c66 2e69 640a 2020 2020 2020  d=self.id.      
-0002dfd0: 2020 290a 0a20 2020 2023 2042 4547 494e    )..    # BEGIN
-0002dfe0: 3a20 7468 6520 6265 6c6f 7720 7072 6f70  : the below prop
-0002dff0: 6572 7469 6573 2077 6572 6520 7265 6d6f  erties were remo
-0002e000: 7665 6420 696e 2060 424f 5420 4150 4920  ved in `BOT API 
-0002e010: 372e 3020 3c68 7474 7073 3a2f 2f63 6f72  7.0 <https://cor
-0002e020: 652e 7465 6c65 6772 616d 2e6f 7267 2f62  e.telegram.org/b
-0002e030: 6f74 732f 6170 692d 6368 616e 6765 6c6f  ots/api-changelo
-0002e040: 6723 6465 6365 6d62 6572 2d32 392d 3230  g#december-29-20
-0002e050: 3233 3e60 5f0a 0a20 2020 2040 7072 6f70  23>`_..    @prop
-0002e060: 6572 7479 0a20 2020 2064 6566 2066 6f72  erty.    def for
-0002e070: 7761 7264 5f66 726f 6d28 7365 6c66 2920  ward_from(self) 
-0002e080: 2d3e 2022 7479 7065 732e 5573 6572 223a  -> "types.User":
-0002e090: 0a20 2020 2020 2020 206c 6f67 2e77 6172  .        log.war
-0002e0a0: 6e69 6e67 280a 2020 2020 2020 2020 2020  ning(.          
-0002e0b0: 2020 2254 6869 7320 7072 6f70 6572 7479    "This property
-0002e0c0: 2069 7320 6465 7072 6563 6174 6564 2e20   is deprecated. 
-0002e0d0: 220a 2020 2020 2020 2020 2020 2020 2250  ".            "P
-0002e0e0: 6c65 6173 6520 7573 6520 666f 7277 6172  lease use forwar
-0002e0f0: 645f 6f72 6967 696e 2069 6e73 7465 6164  d_origin instead
-0002e100: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
-0002e110: 2020 2020 7265 7475 726e 2067 6574 6174      return getat
-0002e120: 7472 2873 656c 662e 666f 7277 6172 645f  tr(self.forward_
-0002e130: 6f72 6967 696e 2c20 2273 656e 6465 725f  origin, "sender_
-0002e140: 7573 6572 222c 204e 6f6e 6529 0a20 2020  user", None).   
-0002e150: 200a 2020 2020 4070 726f 7065 7274 790a   .    @property.
-0002e160: 2020 2020 6465 6620 666f 7277 6172 645f      def forward_
-0002e170: 7365 6e64 6572 5f6e 616d 6528 7365 6c66  sender_name(self
-0002e180: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-0002e190: 2020 6c6f 672e 7761 726e 696e 6728 0a20    log.warning(. 
-0002e1a0: 2020 2020 2020 2020 2020 2022 5468 6973             "This
-0002e1b0: 2070 726f 7065 7274 7920 6973 2064 6570   property is dep
-0002e1c0: 7265 6361 7465 642e 2022 0a20 2020 2020  recated. ".     
-0002e1d0: 2020 2020 2020 2022 506c 6561 7365 2075         "Please u
-0002e1e0: 7365 2066 6f72 7761 7264 5f6f 7269 6769  se forward_origi
-0002e1f0: 6e20 696e 7374 6561 6422 0a20 2020 2020  n instead".     
-0002e200: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-0002e210: 7572 6e20 6765 7461 7474 7228 7365 6c66  urn getattr(self
-0002e220: 2e66 6f72 7761 7264 5f6f 7269 6769 6e2c  .forward_origin,
-0002e230: 2022 7365 6e64 6572 5f75 7365 725f 6e61   "sender_user_na
-0002e240: 6d65 222c 204e 6f6e 6529 0a0a 2020 2020  me", None)..    
-0002e250: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0002e260: 6620 666f 7277 6172 645f 6672 6f6d 5f63  f forward_from_c
-0002e270: 6861 7428 7365 6c66 2920 2d3e 2022 7479  hat(self) -> "ty
-0002e280: 7065 732e 4368 6174 223a 0a20 2020 2020  pes.Chat":.     
-0002e290: 2020 206c 6f67 2e77 6172 6e69 6e67 280a     log.warning(.
-0002e2a0: 2020 2020 2020 2020 2020 2020 2254 6869              "Thi
-0002e2b0: 7320 7072 6f70 6572 7479 2069 7320 6465  s property is de
-0002e2c0: 7072 6563 6174 6564 2e20 220a 2020 2020  precated. ".    
-0002e2d0: 2020 2020 2020 2020 2250 6c65 6173 6520          "Please 
-0002e2e0: 7573 6520 666f 7277 6172 645f 6f72 6967  use forward_orig
-0002e2f0: 696e 2069 6e73 7465 6164 220a 2020 2020  in instead".    
-0002e300: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-0002e310: 7475 726e 2067 6574 6174 7472 280a 2020  turn getattr(.  
-0002e320: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-0002e330: 6f72 7761 7264 5f6f 7269 6769 6e2c 0a20  orward_origin,. 
-0002e340: 2020 2020 2020 2020 2020 2022 6368 6174             "chat
-0002e350: 222c 0a20 2020 2020 2020 2020 2020 2067  ",.            g
-0002e360: 6574 6174 7472 280a 2020 2020 2020 2020  etattr(.        
-0002e370: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
-0002e380: 7761 7264 5f6f 7269 6769 6e2c 0a20 2020  ward_origin,.   
-0002e390: 2020 2020 2020 2020 2020 2020 2022 7365               "se
-0002e3a0: 6e64 6572 5f63 6861 7422 2c0a 2020 2020  nder_chat",.    
-0002e3b0: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
-0002e3c0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0002e3d0: 2020 2020 2020 2029 0a0a 2020 2020 4070         )..    @p
-0002e3e0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0002e3f0: 666f 7277 6172 645f 6672 6f6d 5f6d 6573  forward_from_mes
-0002e400: 7361 6765 5f69 6428 7365 6c66 2920 2d3e  sage_id(self) ->
-0002e410: 2069 6e74 3a0a 2020 2020 2020 2020 6c6f   int:.        lo
-0002e420: 672e 7761 726e 696e 6728 0a20 2020 2020  g.warning(.     
-0002e430: 2020 2020 2020 2022 5468 6973 2070 726f         "This pro
-0002e440: 7065 7274 7920 6973 2064 6570 7265 6361  perty is depreca
-0002e450: 7465 642e 2022 0a20 2020 2020 2020 2020  ted. ".         
-0002e460: 2020 2022 506c 6561 7365 2075 7365 2066     "Please use f
-0002e470: 6f72 7761 7264 5f6f 7269 6769 6e20 696e  orward_origin in
-0002e480: 7374 6561 6422 0a20 2020 2020 2020 2029  stead".        )
-0002e490: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002e4a0: 6765 7461 7474 7228 7365 6c66 2e66 6f72  getattr(self.for
-0002e4b0: 7761 7264 5f6f 7269 6769 6e2c 2022 6d65  ward_origin, "me
-0002e4c0: 7373 6167 655f 6964 222c 204e 6f6e 6529  ssage_id", None)
-0002e4d0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0002e4e0: 2020 2020 6465 6620 666f 7277 6172 645f      def forward_
-0002e4f0: 7369 676e 6174 7572 6528 7365 6c66 2920  signature(self) 
-0002e500: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-0002e510: 6c6f 672e 7761 726e 696e 6728 0a20 2020  log.warning(.   
-0002e520: 2020 2020 2020 2020 2022 5468 6973 2070           "This p
-0002e530: 726f 7065 7274 7920 6973 2064 6570 7265  roperty is depre
-0002e540: 6361 7465 642e 2022 0a20 2020 2020 2020  cated. ".       
-0002e550: 2020 2020 2022 506c 6561 7365 2075 7365       "Please use
-0002e560: 2066 6f72 7761 7264 5f6f 7269 6769 6e20   forward_origin 
-0002e570: 696e 7374 6561 6422 0a20 2020 2020 2020  instead".       
-0002e580: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-0002e590: 6e20 6765 7461 7474 7228 7365 6c66 2e66  n getattr(self.f
-0002e5a0: 6f72 7761 7264 5f6f 7269 6769 6e2c 2022  orward_origin, "
-0002e5b0: 6175 7468 6f72 5f73 6967 6e61 7475 7265  author_signature
-0002e5c0: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
-0002e5d0: 200a 2020 2020 4070 726f 7065 7274 790a   .    @property.
-0002e5e0: 2020 2020 6465 6620 666f 7277 6172 645f      def forward_
-0002e5f0: 6461 7465 2873 656c 6629 202d 3e20 6461  date(self) -> da
-0002e600: 7465 7469 6d65 3a0a 2020 2020 2020 2020  tetime:.        
-0002e610: 6c6f 672e 7761 726e 696e 6728 0a20 2020  log.warning(.   
-0002e620: 2020 2020 2020 2020 2022 5468 6973 2070           "This p
-0002e630: 726f 7065 7274 7920 6973 2064 6570 7265  roperty is depre
-0002e640: 6361 7465 642e 2022 0a20 2020 2020 2020  cated. ".       
-0002e650: 2020 2020 2022 506c 6561 7365 2075 7365       "Please use
-0002e660: 2066 6f72 7761 7264 5f6f 7269 6769 6e20   forward_origin 
-0002e670: 696e 7374 6561 6422 0a20 2020 2020 2020  instead".       
-0002e680: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-0002e690: 6e20 7365 6c66 2e66 6f72 7761 7264 5f6f  n self.forward_o
-0002e6a0: 7269 6769 6e2e 6461 7465 0a0a 2020 2020  rigin.date..    
-0002e6b0: 2320 454e 443a 2074 6865 2062 656c 6f77  # END: the below
-0002e6c0: 2070 726f 7065 7274 6965 7320 7765 7265   properties were
-0002e6d0: 2072 656d 6f76 6564 2069 6e20 6042 4f54   removed in `BOT
-0002e6e0: 2041 5049 2037 2e30 203c 6874 7470 733a   API 7.0 <https:
-0002e6f0: 2f2f 636f 7265 2e74 656c 6567 7261 6d2e  //core.telegram.
-0002e700: 6f72 672f 626f 7473 2f61 7069 2d63 6861  org/bots/api-cha
-0002e710: 6e67 656c 6f67 2364 6563 656d 6265 722d  ngelog#december-
-0002e720: 3239 2d32 3032 333e 605f 0a              29-2023>`_.
+00028c90: 2076 6361 7264 3d73 656c 662e 636f 6e74   vcard=self.cont
+00028ca0: 6163 742e 7663 6172 642c 0a20 2020 2020  act.vcard,.     
+00028cb0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00028cc0: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+00028cd0: 696f 6e3d 6469 7361 626c 655f 6e6f 7469  ion=disable_noti
+00028ce0: 6669 6361 7469 6f6e 2c0a 2020 2020 2020  fication,.      
+00028cf0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00028d00: 706c 795f 7061 7261 6d65 7465 7273 3d72  ply_parameters=r
+00028d10: 6570 6c79 5f70 6172 616d 6574 6572 732c  eply_parameters,
+00028d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028d30: 2020 2020 206d 6573 7361 6765 5f74 6872       message_thr
+00028d40: 6561 645f 6964 3d73 656c 662e 6d65 7373  ead_id=self.mess
+00028d50: 6167 655f 7468 7265 6164 5f69 642c 0a20  age_thread_id,. 
+00028d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028d70: 2020 2062 7573 696e 6573 735f 636f 6e6e     business_conn
+00028d80: 6563 7469 6f6e 5f69 643d 7365 6c66 2e62  ection_id=self.b
+00028d90: 7573 696e 6573 735f 636f 6e6e 6563 7469  usiness_connecti
+00028da0: 6f6e 5f69 642c 0a20 2020 2020 2020 2020  on_id,.         
+00028db0: 2020 2020 2020 2020 2020 2073 6368 6564             sched
+00028dc0: 756c 655f 6461 7465 3d73 6368 6564 756c  ule_date=schedul
+00028dd0: 655f 6461 7465 2c0a 2020 2020 2020 2020  e_date,.        
+00028de0: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
+00028df0: 6563 745f 636f 6e74 656e 743d 7365 6c66  ect_content=self
+00028e00: 2e68 6173 5f70 726f 7465 6374 6564 5f63  .has_protected_c
+00028e10: 6f6e 7465 6e74 2c0a 2020 2020 2020 2020  ontent,.        
+00028e20: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+00028e30: 795f 746f 5f6d 6573 7361 6765 5f69 643d  y_to_message_id=
+00028e40: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+00028e50: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+00028e60: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
+00028e70: 6172 6b75 703d 7265 706c 795f 6d61 726b  arkup=reply_mark
+00028e80: 7570 0a20 2020 2020 2020 2020 2020 2020  up.             
+00028e90: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00028ea0: 2065 6c69 6620 7365 6c66 2e6c 6f63 6174   elif self.locat
+00028eb0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+00028ec0: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+00028ed0: 7420 7365 6c66 2e5f 636c 6965 6e74 2e73  t self._client.s
+00028ee0: 656e 645f 6c6f 6361 7469 6f6e 280a 2020  end_location(.  
+00028ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028f00: 2020 6368 6174 5f69 642c 0a20 2020 2020    chat_id,.     
+00028f10: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00028f20: 6174 6974 7564 653d 7365 6c66 2e6c 6f63  atitude=self.loc
+00028f30: 6174 696f 6e2e 6c61 7469 7475 6465 2c0a  ation.latitude,.
+00028f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028f50: 2020 2020 6c6f 6e67 6974 7564 653d 7365      longitude=se
+00028f60: 6c66 2e6c 6f63 6174 696f 6e2e 6c6f 6e67  lf.location.long
+00028f70: 6974 7564 652c 0a20 2020 2020 2020 2020  itude,.         
+00028f80: 2020 2020 2020 2020 2020 2064 6973 6162             disab
+00028f90: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3d  le_notification=
+00028fa0: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+00028fb0: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+00028fc0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+00028fd0: 7061 7261 6d65 7465 7273 3d72 6570 6c79  parameters=reply
+00028fe0: 5f70 6172 616d 6574 6572 732c 0a20 2020  _parameters,.   
+00028ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029000: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
+00029010: 6964 3d73 656c 662e 6d65 7373 6167 655f  id=self.message_
+00029020: 7468 7265 6164 5f69 642c 0a20 2020 2020  thread_id,.     
+00029030: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00029040: 7573 696e 6573 735f 636f 6e6e 6563 7469  usiness_connecti
+00029050: 6f6e 5f69 643d 7365 6c66 2e62 7573 696e  on_id=self.busin
+00029060: 6573 735f 636f 6e6e 6563 7469 6f6e 5f69  ess_connection_i
+00029070: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00029080: 2020 2020 2020 2073 6368 6564 756c 655f         schedule_
+00029090: 6461 7465 3d73 6368 6564 756c 655f 6461  date=schedule_da
+000290a0: 7465 2c0a 2020 2020 2020 2020 2020 2020  te,.            
+000290b0: 2020 2020 2020 2020 7072 6f74 6563 745f          protect_
+000290c0: 636f 6e74 656e 743d 7365 6c66 2e68 6173  content=self.has
+000290d0: 5f70 726f 7465 6374 6564 5f63 6f6e 7465  _protected_conte
+000290e0: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+000290f0: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
+00029100: 5f6d 6573 7361 6765 5f69 643d 7265 706c  _message_id=repl
+00029110: 795f 746f 5f6d 6573 7361 6765 5f69 642c  y_to_message_id,
+00029120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029130: 2020 2020 2072 6570 6c79 5f6d 6172 6b75       reply_marku
+00029140: 703d 7265 706c 795f 6d61 726b 7570 0a20  p=reply_markup. 
+00029150: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00029160: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00029170: 6620 7365 6c66 2e76 656e 7565 3a0a 2020  f self.venue:.  
+00029180: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00029190: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+000291a0: 5f63 6c69 656e 742e 7365 6e64 5f76 656e  _client.send_ven
+000291b0: 7565 280a 2020 2020 2020 2020 2020 2020  ue(.            
+000291c0: 2020 2020 2020 2020 6368 6174 5f69 642c          chat_id,
+000291d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000291e0: 2020 2020 206c 6174 6974 7564 653d 7365       latitude=se
+000291f0: 6c66 2e76 656e 7565 2e6c 6f63 6174 696f  lf.venue.locatio
+00029200: 6e2e 6c61 7469 7475 6465 2c0a 2020 2020  n.latitude,.    
+00029210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029220: 6c6f 6e67 6974 7564 653d 7365 6c66 2e76  longitude=self.v
+00029230: 656e 7565 2e6c 6f63 6174 696f 6e2e 6c6f  enue.location.lo
+00029240: 6e67 6974 7564 652c 0a20 2020 2020 2020  ngitude,.       
+00029250: 2020 2020 2020 2020 2020 2020 2074 6974               tit
+00029260: 6c65 3d73 656c 662e 7665 6e75 652e 7469  le=self.venue.ti
+00029270: 746c 652c 0a20 2020 2020 2020 2020 2020  tle,.           
+00029280: 2020 2020 2020 2020 2061 6464 7265 7373           address
+00029290: 3d73 656c 662e 7665 6e75 652e 6164 6472  =self.venue.addr
+000292a0: 6573 732c 0a20 2020 2020 2020 2020 2020  ess,.           
+000292b0: 2020 2020 2020 2020 2066 6f75 7273 7175           foursqu
+000292c0: 6172 655f 6964 3d73 656c 662e 7665 6e75  are_id=self.venu
+000292d0: 652e 666f 7572 7371 7561 7265 5f69 642c  e.foursquare_id,
+000292e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000292f0: 2020 2020 2066 6f75 7273 7175 6172 655f       foursquare_
+00029300: 7479 7065 3d73 656c 662e 7665 6e75 652e  type=self.venue.
+00029310: 666f 7572 7371 7561 7265 5f74 7970 652c  foursquare_type,
+00029320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029330: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
+00029340: 6966 6963 6174 696f 6e3d 6469 7361 626c  ification=disabl
+00029350: 655f 6e6f 7469 6669 6361 7469 6f6e 2c0a  e_notification,.
+00029360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029370: 2020 2020 7265 706c 795f 7061 7261 6d65      reply_parame
+00029380: 7465 7273 3d72 6570 6c79 5f70 6172 616d  ters=reply_param
+00029390: 6574 6572 732c 0a20 2020 2020 2020 2020  eters,.         
+000293a0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+000293b0: 6765 5f74 6872 6561 645f 6964 3d73 656c  ge_thread_id=sel
+000293c0: 662e 6d65 7373 6167 655f 7468 7265 6164  f.message_thread
+000293d0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+000293e0: 2020 2020 2020 2020 2062 7573 696e 6573           busines
+000293f0: 735f 636f 6e6e 6563 7469 6f6e 5f69 643d  s_connection_id=
+00029400: 7365 6c66 2e62 7573 696e 6573 735f 636f  self.business_co
+00029410: 6e6e 6563 7469 6f6e 5f69 642c 0a20 2020  nnection_id,.   
+00029420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029430: 2073 6368 6564 756c 655f 6461 7465 3d73   schedule_date=s
+00029440: 6368 6564 756c 655f 6461 7465 2c0a 2020  chedule_date,.  
+00029450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029460: 2020 7072 6f74 6563 745f 636f 6e74 656e    protect_conten
+00029470: 743d 7365 6c66 2e68 6173 5f70 726f 7465  t=self.has_prote
+00029480: 6374 6564 5f63 6f6e 7465 6e74 2c0a 2020  cted_content,.  
+00029490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000294a0: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
+000294b0: 6765 5f69 643d 7265 706c 795f 746f 5f6d  ge_id=reply_to_m
+000294c0: 6573 7361 6765 5f69 642c 0a20 2020 2020  essage_id,.     
+000294d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000294e0: 6570 6c79 5f6d 6172 6b75 703d 7265 706c  eply_markup=repl
+000294f0: 795f 6d61 726b 7570 0a20 2020 2020 2020  y_markup.       
+00029500: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00029510: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+00029520: 2e70 6f6c 6c3a 0a20 2020 2020 2020 2020  .poll:.         
+00029530: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+00029540: 6169 7420 7365 6c66 2e5f 636c 6965 6e74  ait self._client
+00029550: 2e73 656e 645f 706f 6c6c 280a 2020 2020  .send_poll(.    
+00029560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029570: 6368 6174 5f69 642c 0a20 2020 2020 2020  chat_id,.       
+00029580: 2020 2020 2020 2020 2020 2020 2071 7565               que
+00029590: 7374 696f 6e3d 7365 6c66 2e70 6f6c 6c2e  stion=self.poll.
+000295a0: 7175 6573 7469 6f6e 2c0a 2020 2020 2020  question,.      
+000295b0: 2020 2020 2020 2020 2020 2020 2020 6f70                op
+000295c0: 7469 6f6e 733d 5b6f 7074 2e74 6578 7420  tions=[opt.text 
+000295d0: 666f 7220 6f70 7420 696e 2073 656c 662e  for opt in self.
+000295e0: 706f 6c6c 2e6f 7074 696f 6e73 5d2c 0a20  poll.options],. 
+000295f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029600: 2020 2069 735f 616e 6f6e 796d 6f75 733d     is_anonymous=
+00029610: 7365 6c66 2e70 6f6c 6c2e 6973 5f61 6e6f  self.poll.is_ano
+00029620: 6e79 6d6f 7573 2c0a 2020 2020 2020 2020  nymous,.        
+00029630: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00029640: 3d73 656c 662e 706f 6c6c 2e74 7970 652c  =self.poll.type,
+00029650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029660: 2020 2020 2061 6c6c 6f77 735f 6d75 6c74       allows_mult
+00029670: 6970 6c65 5f61 6e73 7765 7273 3d73 656c  iple_answers=sel
+00029680: 662e 706f 6c6c 2e61 6c6c 6f77 735f 6d75  f.poll.allows_mu
+00029690: 6c74 6970 6c65 5f61 6e73 7765 7273 2c0a  ltiple_answers,.
+000296a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000296b0: 2020 2020 636f 7272 6563 745f 6f70 7469      correct_opti
+000296c0: 6f6e 5f69 643d 7365 6c66 2e70 6f6c 6c2e  on_id=self.poll.
+000296d0: 636f 7272 6563 745f 6f70 7469 6f6e 5f69  correct_option_i
+000296e0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+000296f0: 2020 2020 2020 2065 7870 6c61 6e61 7469         explanati
+00029700: 6f6e 3d73 656c 662e 706f 6c6c 2e65 7870  on=self.poll.exp
+00029710: 6c61 6e61 7469 6f6e 2c0a 2020 2020 2020  lanation,.      
+00029720: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00029730: 706c 616e 6174 696f 6e5f 656e 7469 7469  planation_entiti
+00029740: 6573 3d73 656c 662e 706f 6c6c 2e65 7870  es=self.poll.exp
+00029750: 6c61 6e61 7469 6f6e 5f65 6e74 6974 6965  lanation_entitie
+00029760: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00029770: 2020 2020 2020 206f 7065 6e5f 7065 7269         open_peri
+00029780: 6f64 3d73 656c 662e 706f 6c6c 2e6f 7065  od=self.poll.ope
+00029790: 6e5f 7065 7269 6f64 2c0a 2020 2020 2020  n_period,.      
+000297a0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+000297b0: 6f73 655f 6461 7465 3d73 656c 662e 706f  ose_date=self.po
+000297c0: 6c6c 2e63 6c6f 7365 5f64 6174 652c 0a20  ll.close_date,. 
+000297d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000297e0: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
+000297f0: 6963 6174 696f 6e3d 6469 7361 626c 655f  ication=disable_
+00029800: 6e6f 7469 6669 6361 7469 6f6e 2c0a 2020  notification,.  
+00029810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029820: 2020 7072 6f74 6563 745f 636f 6e74 656e    protect_conten
+00029830: 743d 7365 6c66 2e68 6173 5f70 726f 7465  t=self.has_prote
+00029840: 6374 6564 5f63 6f6e 7465 6e74 2c0a 2020  cted_content,.  
+00029850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029860: 2020 7265 706c 795f 7061 7261 6d65 7465    reply_paramete
+00029870: 7273 3d72 6570 6c79 5f70 6172 616d 6574  rs=reply_paramet
+00029880: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
+00029890: 2020 2020 2020 2020 206d 6573 7361 6765           message
+000298a0: 5f74 6872 6561 645f 6964 3d73 656c 662e  _thread_id=self.
+000298b0: 6d65 7373 6167 655f 7468 7265 6164 5f69  message_thread_i
+000298c0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+000298d0: 2020 2020 2020 2062 7573 696e 6573 735f         business_
+000298e0: 636f 6e6e 6563 7469 6f6e 5f69 643d 7365  connection_id=se
+000298f0: 6c66 2e62 7573 696e 6573 735f 636f 6e6e  lf.business_conn
+00029900: 6563 7469 6f6e 5f69 642c 0a20 2020 2020  ection_id,.     
+00029910: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00029920: 6368 6564 756c 655f 6461 7465 3d73 6368  chedule_date=sch
+00029930: 6564 756c 655f 6461 7465 2c0a 2020 2020  edule_date,.    
+00029940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029950: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+00029960: 5f69 643d 7265 706c 795f 746f 5f6d 6573  _id=reply_to_mes
+00029970: 7361 6765 5f69 642c 0a20 2020 2020 2020  sage_id,.       
+00029980: 2020 2020 2020 2020 2020 2020 2072 6570               rep
+00029990: 6c79 5f6d 6172 6b75 703d 7265 706c 795f  ly_markup=reply_
+000299a0: 6d61 726b 7570 0a20 2020 2020 2020 2020  markup.         
+000299b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000299c0: 2020 2020 2065 6c69 6620 7365 6c66 2e67       elif self.g
+000299d0: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
+000299e0: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+000299f0: 7420 7365 6c66 2e5f 636c 6965 6e74 2e73  t self._client.s
+00029a00: 656e 645f 6761 6d65 280a 2020 2020 2020  end_game(.      
+00029a10: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+00029a20: 6174 5f69 642c 0a20 2020 2020 2020 2020  at_id,.         
+00029a30: 2020 2020 2020 2020 2020 2067 616d 655f             game_
+00029a40: 7368 6f72 745f 6e61 6d65 3d73 656c 662e  short_name=self.
+00029a50: 6761 6d65 2e73 686f 7274 5f6e 616d 652c  game.short_name,
+00029a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029a70: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
+00029a80: 6966 6963 6174 696f 6e3d 6469 7361 626c  ification=disabl
+00029a90: 655f 6e6f 7469 6669 6361 7469 6f6e 2c0a  e_notification,.
+00029aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029ab0: 2020 2020 7072 6f74 6563 745f 636f 6e74      protect_cont
+00029ac0: 656e 743d 7365 6c66 2e68 6173 5f70 726f  ent=self.has_pro
+00029ad0: 7465 6374 6564 5f63 6f6e 7465 6e74 2c0a  tected_content,.
+00029ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029af0: 2020 2020 6d65 7373 6167 655f 7468 7265      message_thre
+00029b00: 6164 5f69 643d 7365 6c66 2e6d 6573 7361  ad_id=self.messa
+00029b10: 6765 5f74 6872 6561 645f 6964 2c0a 2020  ge_thread_id,.  
+00029b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029b30: 2020 6275 7369 6e65 7373 5f63 6f6e 6e65    business_conne
+00029b40: 6374 696f 6e5f 6964 3d73 656c 662e 6275  ction_id=self.bu
+00029b50: 7369 6e65 7373 5f63 6f6e 6e65 6374 696f  siness_connectio
+00029b60: 6e5f 6964 2c0a 2020 2020 2020 2020 2020  n_id,.          
+00029b70: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+00029b80: 7061 7261 6d65 7465 7273 3d72 6570 6c79  parameters=reply
+00029b90: 5f70 6172 616d 6574 6572 732c 0a20 2020  _parameters,.   
+00029ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029bb0: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
+00029bc0: 655f 6964 3d72 6570 6c79 5f74 6f5f 6d65  e_id=reply_to_me
+00029bd0: 7373 6167 655f 6964 2c0a 2020 2020 2020  ssage_id,.      
+00029be0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00029bf0: 706c 795f 6d61 726b 7570 3d72 6570 6c79  ply_markup=reply
+00029c00: 5f6d 6172 6b75 700a 2020 2020 2020 2020  _markup.        
+00029c10: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00029c20: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00029c30: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00029c40: 6520 5661 6c75 6545 7272 6f72 2822 556e  e ValueError("Un
+00029c50: 6b6e 6f77 6e20 6d65 6469 6120 7479 7065  known media type
+00029c60: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
+00029c70: 6966 2063 6170 7469 6f6e 2069 7320 4e6f  if caption is No
+00029c80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00029c90: 2020 2020 6361 7074 696f 6e20 3d20 7365      caption = se
+00029ca0: 6c66 2e63 6170 7469 6f6e 206f 7220 2222  lf.caption or ""
+00029cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029cc0: 2063 6170 7469 6f6e 5f65 6e74 6974 6965   caption_entitie
+00029cd0: 7320 3d20 7365 6c66 2e63 6170 7469 6f6e  s = self.caption
+00029ce0: 5f65 6e74 6974 6965 730a 0a20 2020 2020  _entities..     
+00029cf0: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+00029d00: 6169 7420 7365 6e64 5f6d 6564 6961 280a  ait send_media(.
+00029d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029d20: 6669 6c65 5f69 643d 6669 6c65 5f69 642c  file_id=file_id,
+00029d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029d40: 2063 6170 7469 6f6e 3d63 6170 7469 6f6e   caption=caption
+00029d50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00029d60: 2020 7061 7273 655f 6d6f 6465 3d70 6172    parse_mode=par
+00029d70: 7365 5f6d 6f64 652c 0a20 2020 2020 2020  se_mode,.       
+00029d80: 2020 2020 2020 2020 2063 6170 7469 6f6e           caption
+00029d90: 5f65 6e74 6974 6965 733d 6361 7074 696f  _entities=captio
+00029da0: 6e5f 656e 7469 7469 6573 0a20 2020 2020  n_entities.     
+00029db0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00029dc0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00029dd0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00029de0: 726f 7228 2243 616e 2774 2063 6f70 7920  ror("Can't copy 
+00029df0: 7468 6973 206d 6573 7361 6765 2229 0a0a  this message")..
+00029e00: 2020 2020 6173 796e 6320 6465 6620 6465      async def de
+00029e10: 6c65 7465 2873 656c 662c 2072 6576 6f6b  lete(self, revok
+00029e20: 653a 2062 6f6f 6c20 3d20 5472 7565 293a  e: bool = True):
+00029e30: 0a20 2020 2020 2020 2022 2222 426f 756e  .        """Boun
+00029e40: 6420 6d65 7468 6f64 202a 6465 6c65 7465  d method *delete
+00029e50: 2a20 6f66 203a 6f62 6a3a 607e 7079 726f  * of :obj:`~pyro
+00029e60: 6772 616d 2e74 7970 6573 2e4d 6573 7361  gram.types.Messa
+00029e70: 6765 602e 0a0a 2020 2020 2020 2020 5573  ge`...        Us
+00029e80: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
+00029e90: 666f 723a 0a0a 2020 2020 2020 2020 2e2e  for:..        ..
+00029ea0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+00029eb0: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
+00029ec0: 2020 6177 6169 7420 636c 6965 6e74 2e64    await client.d
+00029ed0: 656c 6574 655f 6d65 7373 6167 6573 280a  elete_messages(.
+00029ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029ef0: 6368 6174 5f69 643d 6368 6174 5f69 642c  chat_id=chat_id,
+00029f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029f10: 206d 6573 7361 6765 5f69 6473 3d6d 6573   message_ids=mes
+00029f20: 7361 6765 2e69 640a 2020 2020 2020 2020  sage.id.        
+00029f30: 2020 2020 290a 0a20 2020 2020 2020 2045      )..        E
+00029f40: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
+00029f50: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+00029f60: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
+00029f70: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+00029f80: 7420 6d65 7373 6167 652e 6465 6c65 7465  t message.delete
+00029f90: 2829 0a0a 2020 2020 2020 2020 5061 7261  ()..        Para
+00029fa0: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
+00029fb0: 2020 2020 7265 766f 6b65 2028 6060 626f      revoke (``bo
+00029fc0: 6f6c 6060 2c20 2a6f 7074 696f 6e61 6c2a  ol``, *optional*
+00029fd0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00029fe0: 2020 2044 656c 6574 6573 206d 6573 7361     Deletes messa
+00029ff0: 6765 7320 6f6e 2062 6f74 6820 7061 7274  ges on both part
+0002a000: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+0002a010: 2020 2054 6869 7320 6973 206f 6e6c 7920     This is only 
+0002a020: 666f 7220 7072 6976 6174 6520 636c 6f75  for private clou
+0002a030: 6420 6368 6174 7320 616e 6420 6e6f 726d  d chats and norm
+0002a040: 616c 2067 726f 7570 732c 206d 6573 7361  al groups, messa
+0002a050: 6765 7320 6f6e 0a20 2020 2020 2020 2020  ges on.         
+0002a060: 2020 2020 2020 2063 6861 6e6e 656c 7320         channels 
+0002a070: 616e 6420 7375 7065 7267 726f 7570 7320  and supergroups 
+0002a080: 6172 6520 616c 7761 7973 2072 6576 6f6b  are always revok
+0002a090: 6564 2028 692e 652e 3a20 6465 6c65 7465  ed (i.e.: delete
+0002a0a0: 6420 666f 7220 6576 6572 796f 6e65 292e  d for everyone).
+0002a0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a0c0: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
+0002a0d0: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
+0002a0e0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0002a0f0: 2060 6069 6e74 6060 3a20 416d 6f75 6e74   ``int``: Amount
+0002a100: 206f 6620 6166 6665 6374 6564 206d 6573   of affected mes
+0002a110: 7361 6765 730a 0a20 2020 2020 2020 2052  sages..        R
+0002a120: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
+0002a130: 2020 2052 5043 4572 726f 723a 2049 6e20     RPCError: In 
+0002a140: 6361 7365 206f 6620 6120 5465 6c65 6772  case of a Telegr
+0002a150: 616d 2052 5043 2065 7272 6f72 2e0a 2020  am RPC error..  
+0002a160: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0002a170: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
+0002a180: 656c 662e 5f63 6c69 656e 742e 6465 6c65  elf._client.dele
+0002a190: 7465 5f6d 6573 7361 6765 7328 0a20 2020  te_messages(.   
+0002a1a0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
+0002a1b0: 3d73 656c 662e 6368 6174 2e69 642c 0a20  =self.chat.id,. 
+0002a1c0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+0002a1d0: 6765 5f69 6473 3d73 656c 662e 6964 2c0a  ge_ids=self.id,.
+0002a1e0: 2020 2020 2020 2020 2020 2020 7265 766f              revo
+0002a1f0: 6b65 3d72 6576 6f6b 652c 0a20 2020 2020  ke=revoke,.     
+0002a200: 2020 2020 2020 2069 735f 7363 6865 6475         is_schedu
+0002a210: 6c65 643d 7365 6c66 2e73 6368 6564 756c  led=self.schedul
+0002a220: 6564 0a20 2020 2020 2020 2029 0a0a 2020  ed.        )..  
+0002a230: 2020 6173 796e 6320 6465 6620 636c 6963    async def clic
+0002a240: 6b28 0a20 2020 2020 2020 2073 656c 662c  k(.        self,
+0002a250: 0a20 2020 2020 2020 2078 3a20 556e 696f  .        x: Unio
+0002a260: 6e5b 696e 742c 2073 7472 5d20 3d20 302c  n[int, str] = 0,
+0002a270: 0a20 2020 2020 2020 2079 3a20 696e 7420  .        y: int 
+0002a280: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0002a290: 7175 6f74 653a 2062 6f6f 6c20 3d20 4e6f  quote: bool = No
+0002a2a0: 6e65 2c0a 2020 2020 2020 2020 7469 6d65  ne,.        time
+0002a2b0: 6f75 743a 2069 6e74 203d 2031 302c 0a20  out: int = 10,. 
+0002a2c0: 2020 2020 2020 2072 6571 7565 7374 5f77         request_w
+0002a2d0: 7269 7465 5f61 6363 6573 733a 2062 6f6f  rite_access: boo
+0002a2e0: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
+0002a2f0: 2020 7061 7373 776f 7264 3a20 7374 7220    password: str 
+0002a300: 3d20 4e6f 6e65 0a20 2020 2029 3a0a 2020  = None.    ):.  
+0002a310: 2020 2020 2020 2222 2242 6f75 6e64 206d        """Bound m
+0002a320: 6574 686f 6420 2a63 6c69 636b 2a20 6f66  ethod *click* of
+0002a330: 203a 6f62 6a3a 607e 7079 726f 6772 616d   :obj:`~pyrogram
+0002a340: 2e74 7970 6573 2e4d 6573 7361 6765 602e  .types.Message`.
+0002a350: 0a0a 2020 2020 2020 2020 5573 6520 6173  ..        Use as
+0002a360: 2061 2073 686f 7274 6375 7420 666f 7220   a shortcut for 
+0002a370: 636c 6963 6b69 6e67 2061 2062 7574 746f  clicking a butto
+0002a380: 6e20 6174 7461 6368 6564 2074 6f20 7468  n attached to th
+0002a390: 6520 6d65 7373 6167 6520 696e 7374 6561  e message instea
+0002a3a0: 6420 6f66 3a0a 0a20 2020 2020 2020 202d  d of:..        -
+0002a3b0: 2043 6c69 636b 696e 6720 696e 6c69 6e65   Clicking inline
+0002a3c0: 2062 7574 746f 6e73 3a0a 0a20 2020 2020   buttons:..     
+0002a3d0: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+0002a3e0: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+0002a3f0: 2020 2020 2020 2061 7761 6974 2063 6c69         await cli
+0002a400: 656e 742e 7265 7175 6573 745f 6361 6c6c  ent.request_call
+0002a410: 6261 636b 5f61 6e73 7765 7228 0a20 2020  back_answer(.   
+0002a420: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+0002a430: 745f 6964 3d6d 6573 7361 6765 2e63 6861  t_id=message.cha
+0002a440: 742e 6964 2c0a 2020 2020 2020 2020 2020  t.id,.          
+0002a450: 2020 2020 2020 6d65 7373 6167 655f 6964        message_id
+0002a460: 3d6d 6573 7361 6765 2e69 642c 0a20 2020  =message.id,.   
+0002a470: 2020 2020 2020 2020 2020 2020 2063 616c               cal
+0002a480: 6c62 6163 6b5f 6461 7461 3d6d 6573 7361  lback_data=messa
+0002a490: 6765 2e72 6570 6c79 5f6d 6172 6b75 705b  ge.reply_markup[
+0002a4a0: 695d 5b6a 5d2e 6361 6c6c 6261 636b 5f64  i][j].callback_d
+0002a4b0: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
+0002a4c0: 290a 0a20 2020 2020 2020 202d 2043 6c69  )..        - Cli
+0002a4d0: 636b 696e 6720 6e6f 726d 616c 2062 7574  cking normal but
+0002a4e0: 746f 6e73 3a0a 0a20 2020 2020 2020 202e  tons:..        .
+0002a4f0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
+0002a500: 7974 686f 6e0a 0a20 2020 2020 2020 2020  ython..         
+0002a510: 2020 2061 7761 6974 2063 6c69 656e 742e     await client.
+0002a520: 7365 6e64 5f6d 6573 7361 6765 280a 2020  send_message(.  
+0002a530: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+0002a540: 6174 5f69 643d 6d65 7373 6167 652e 6368  at_id=message.ch
+0002a550: 6174 2e69 642c 0a20 2020 2020 2020 2020  at.id,.         
+0002a560: 2020 2020 2020 2074 6578 743d 6d65 7373         text=mess
+0002a570: 6167 652e 7265 706c 795f 6d61 726b 7570  age.reply_markup
+0002a580: 5b69 5d5b 6a5d 2e74 6578 740a 2020 2020  [i][j].text.    
+0002a590: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0002a5a0: 2020 2045 7861 6d70 6c65 3a0a 2020 2020     Example:.    
+0002a5b0: 2020 2020 2020 2020 5468 6973 206d 6574          This met
+0002a5c0: 686f 6420 6361 6e20 6265 2075 7365 6420  hod can be used 
+0002a5d0: 696e 2074 6872 6565 2064 6966 6665 7265  in three differe
+0002a5e0: 6e74 2077 6179 733a 0a0a 2020 2020 2020  nt ways:..      
+0002a5f0: 2020 2020 2020 312e 2020 5061 7373 206f        1.  Pass o
+0002a600: 6e65 2069 6e74 6567 6572 2061 7267 756d  ne integer argum
+0002a610: 656e 7420 6f6e 6c79 2028 652e 672e 3a20  ent only (e.g.: 
+0002a620: 6060 2e63 6c69 636b 2832 2960 602c 2074  ``.click(2)``, t
+0002a630: 6f20 636c 6963 6b20 6120 6275 7474 6f6e  o click a button
+0002a640: 2061 7420 696e 6465 7820 3229 2e0a 2020   at index 2)..  
+0002a650: 2020 2020 2020 2020 2020 2020 2020 4275                Bu
+0002a660: 7474 6f6e 7320 6172 6520 636f 756e 7465  ttons are counte
+0002a670: 6420 6c65 6674 2074 6f20 7269 6768 742c  d left to right,
+0002a680: 2073 7461 7274 696e 6720 6672 6f6d 2074   starting from t
+0002a690: 6865 2074 6f70 2e0a 0a20 2020 2020 2020  he top...       
+0002a6a0: 2020 2020 2032 2e20 2050 6173 7320 7477       2.  Pass tw
+0002a6b0: 6f20 696e 7465 6765 7220 6172 6775 6d65  o integer argume
+0002a6c0: 6e74 7320 2865 2e67 2e3a 2060 602e 636c  nts (e.g.: ``.cl
+0002a6d0: 6963 6b28 312c 2030 2960 602c 2074 6f20  ick(1, 0)``, to 
+0002a6e0: 636c 6963 6b20 6120 6275 7474 6f6e 2061  click a button a
+0002a6f0: 7420 706f 7369 7469 6f6e 2028 312c 2030  t position (1, 0
+0002a700: 2929 2e0a 2020 2020 2020 2020 2020 2020  ))..            
+0002a710: 2020 2020 5468 6520 6f72 6967 696e 2028      The origin (
+0002a720: 302c 2030 2920 6973 2074 6f70 2d6c 6566  0, 0) is top-lef
+0002a730: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
+0002a740: 332e 2020 5061 7373 206f 6e65 2073 7472  3.  Pass one str
+0002a750: 696e 6720 6172 6775 6d65 6e74 206f 6e6c  ing argument onl
+0002a760: 7920 2865 2e67 2e3a 2060 602e 636c 6963  y (e.g.: ``.clic
+0002a770: 6b28 2253 6574 7469 6e67 7322 2960 602c  k("Settings")``,
+0002a780: 2074 6f20 636c 6963 6b20 6120 6275 7474   to click a butt
+0002a790: 6f6e 2062 7920 7573 696e 6720 6974 7320  on by using its 
+0002a7a0: 6c61 6265 6c29 2e0a 2020 2020 2020 2020  label)..        
+0002a7b0: 2020 2020 2020 2020 4f6e 6c79 2074 6865          Only the
+0002a7c0: 2066 6972 7374 206d 6174 6368 696e 6720   first matching 
+0002a7d0: 6275 7474 6f6e 2077 696c 6c20 6265 2070  button will be p
+0002a7e0: 7265 7373 6564 2e0a 0a20 2020 2020 2020  ressed...       
+0002a7f0: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
+0002a800: 2020 2020 2020 2020 2078 2028 6060 696e           x (``in
+0002a810: 7460 6020 7c20 6060 7374 7260 6029 3a0a  t`` | ``str``):.
+0002a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a830: 5573 6564 2061 7320 696e 7465 6765 7220  Used as integer 
+0002a840: 696e 6465 782c 2069 6e74 6567 6572 2061  index, integer a
+0002a850: 6273 6369 7373 6120 2869 6e20 7061 6972  bscissa (in pair
+0002a860: 2077 6974 6820 7929 206f 7220 6173 2073   with y) or as s
+0002a870: 7472 696e 6720 6c61 6265 6c2e 0a20 2020  tring label..   
+0002a880: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+0002a890: 6175 6c74 7320 746f 2030 2028 6669 7273  aults to 0 (firs
+0002a8a0: 7420 6275 7474 6f6e 292e 0a0a 2020 2020  t button)...    
+0002a8b0: 2020 2020 2020 2020 7920 2860 6069 6e74          y (``int
+0002a8c0: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
+0002a8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a8e0: 2055 7365 6420 6173 206f 7264 696e 6174   Used as ordinat
+0002a8f0: 6520 6f6e 6c79 2028 696e 2070 6169 7220  e only (in pair 
+0002a900: 7769 7468 2078 292e 0a0a 2020 2020 2020  with x)...      
+0002a910: 2020 2020 2020 7175 6f74 6520 2860 6062        quote (``b
+0002a920: 6f6f 6c60 602c 202a 6f70 7469 6f6e 616c  ool``, *optional
+0002a930: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
+0002a940: 2020 2020 5573 6566 756c 2066 6f72 206e      Useful for n
+0002a950: 6f72 6d61 6c20 6275 7474 6f6e 7320 6f6e  ormal buttons on
+0002a960: 6c79 2c20 7768 6572 6520 7072 6573 7369  ly, where pressi
+0002a970: 6e67 2069 7420 7769 6c6c 2072 6573 756c  ng it will resul
+0002a980: 7420 696e 2061 206e 6577 206d 6573 7361  t in a new messa
+0002a990: 6765 2073 656e 742e 0a20 2020 2020 2020  ge sent..       
+0002a9a0: 2020 2020 2020 2020 2049 6620 6060 5472           If ``Tr
+0002a9b0: 7565 6060 2c20 7468 6520 6d65 7373 6167  ue``, the messag
+0002a9c0: 6520 7769 6c6c 2062 6520 7365 6e74 2061  e will be sent a
+0002a9d0: 7320 6120 7265 706c 7920 746f 2074 6869  s a reply to thi
+0002a9e0: 7320 6d65 7373 6167 652e 0a20 2020 2020  s message..     
+0002a9f0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+0002aa00: 6c74 7320 746f 2060 6054 7275 6560 6020  lts to ``True`` 
+0002aa10: 696e 2067 726f 7570 2063 6861 7473 2061  in group chats a
+0002aa20: 6e64 2060 6046 616c 7365 6060 2069 6e20  nd ``False`` in 
+0002aa30: 7072 6976 6174 6520 6368 6174 732e 0a0a  private chats...
+0002aa40: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0002aa50: 6f75 7420 2860 6069 6e74 6060 2c20 2a6f  out (``int``, *o
+0002aa60: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
+0002aa70: 2020 2020 2020 2020 2020 2054 696d 656f             Timeo
+0002aa80: 7574 2069 6e20 7365 636f 6e64 732e 0a0a  ut in seconds...
+0002aa90: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+0002aaa0: 6573 745f 7772 6974 655f 6163 6365 7373  est_write_access
+0002aab0: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
+0002aac0: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
+0002aad0: 2020 2020 2020 2020 204f 6e6c 7920 7573           Only us
+0002aae0: 6564 2069 6e20 6361 7365 206f 6620 3a6f  ed in case of :o
+0002aaf0: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
+0002ab00: 7065 732e 4c6f 6769 6e55 726c 6020 6275  pes.LoginUrl` bu
+0002ab10: 7474 6f6e 2e0a 2020 2020 2020 2020 2020  tton..          
+0002ab20: 2020 2020 2020 5472 7565 2c20 6966 2074        True, if t
+0002ab30: 6865 2062 6f74 2063 616e 2073 656e 6420  he bot can send 
+0002ab40: 6d65 7373 6167 6573 2074 6f20 7468 6520  messages to the 
+0002ab50: 7573 6572 2e0a 2020 2020 2020 2020 2020  user..          
+0002ab60: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+0002ab70: 6f20 6060 5472 7565 6060 2e0a 0a20 2020  o ``True``...   
+0002ab80: 2020 2020 2020 2020 2070 6173 7377 6f72           passwor
+0002ab90: 6420 2860 6073 7472 6060 2c20 2a6f 7074  d (``str``, *opt
+0002aba0: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
+0002abb0: 2020 2020 2020 2020 2057 6865 6e20 636c           When cl
+0002abc0: 6963 6b69 6e67 2063 6572 7461 696e 2062  icking certain b
+0002abd0: 7574 746f 6e73 2028 7375 6368 2061 7320  uttons (such as 
+0002abe0: 426f 7446 6174 6865 7227 7320 636f 6e66  BotFather's conf
+0002abf0: 6972 6d61 7469 6f6e 2062 7574 746f 6e20  irmation button 
+0002ac00: 746f 2074 7261 6e73 6665 7220 6f77 6e65  to transfer owne
+0002ac10: 7273 6869 7029 2c20 6966 2079 6f75 7220  rship), if your 
+0002ac20: 6163 636f 756e 7420 6861 7320 3246 4120  account has 2FA 
+0002ac30: 656e 6162 6c65 642c 2079 6f75 206e 6565  enabled, you nee
+0002ac40: 6420 746f 2070 726f 7669 6465 2079 6f75  d to provide you
+0002ac50: 7220 6163 636f 756e 7427 7320 7061 7373  r account's pass
+0002ac60: 776f 7264 2e20 0a20 2020 2020 2020 2020  word. .         
+0002ac70: 2020 2020 2020 2054 6865 2032 2d73 7465         The 2-ste
+0002ac80: 7020 7665 7269 6669 6361 7469 6f6e 2070  p verification p
+0002ac90: 6173 7377 6f72 6420 666f 7220 7468 6520  assword for the 
+0002aca0: 6375 7272 656e 7420 7573 6572 2e20 4f6e  current user. On
+0002acb0: 6c79 2061 7070 6c69 6361 626c 652c 2069  ly applicable, i
+0002acc0: 6620 7468 6520 3a6f 626a 3a60 7e70 7972  f the :obj:`~pyr
+0002acd0: 6f67 7261 6d2e 7479 7065 732e 496e 6c69  ogram.types.Inli
+0002ace0: 6e65 4b65 7962 6f61 7264 4275 7474 6f6e  neKeyboardButton
+0002acf0: 6020 636f 6e74 6169 6e73 2060 6063 616c  ` contains ``cal
+0002ad00: 6c62 6163 6b5f 6461 7461 5f77 6974 685f  lback_data_with_
+0002ad10: 7061 7373 776f 7264 6060 2e0a 0a20 2020  password``...   
+0002ad20: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+0002ad30: 2020 2020 2020 2020 2020 2d20 2020 5468            -   Th
+0002ad40: 6520 7265 7375 6c74 206f 6620 3a6d 6574  e result of :met
+0002ad50: 683a 607e 7079 726f 6772 616d 2e43 6c69  h:`~pyrogram.Cli
+0002ad60: 656e 742e 7265 7175 6573 745f 6361 6c6c  ent.request_call
+0002ad70: 6261 636b 5f61 6e73 7765 7260 2069 6e20  back_answer` in 
+0002ad80: 6361 7365 206f 6620 696e 6c69 6e65 2063  case of inline c
+0002ad90: 616c 6c62 6163 6b20 6275 7474 6f6e 2063  allback button c
+0002ada0: 6c69 636b 732e 0a20 2020 2020 2020 2020  licks..         
+0002adb0: 2020 202d 2020 2054 6865 2072 6573 756c     -   The resul
+0002adc0: 7420 6f66 203a 6d65 7468 3a60 7e4d 6573  t of :meth:`~Mes
+0002add0: 7361 6765 2e72 6570 6c79 2829 6020 696e  sage.reply()` in
+0002ade0: 2063 6173 6520 6f66 206e 6f72 6d61 6c20   case of normal 
+0002adf0: 6275 7474 6f6e 2063 6c69 636b 732e 0a20  button clicks.. 
+0002ae00: 2020 2020 2020 2020 2020 202d 2020 2041             -   A
+0002ae10: 2073 7472 696e 6720 696e 2063 6173 6520   string in case 
+0002ae20: 7468 6520 696e 6c69 6e65 2062 7574 746f  the inline butto
+0002ae30: 6e20 6973 2061 2055 524c 2c20 6120 2a73  n is a URL, a *s
+0002ae40: 7769 7463 685f 696e 6c69 6e65 5f71 7565  witch_inline_que
+0002ae50: 7279 2a20 6f72 2061 0a20 2020 2020 2020  ry* or a.       
+0002ae60: 2020 2020 2020 2020 202a 7377 6974 6368           *switch
+0002ae70: 5f69 6e6c 696e 655f 7175 6572 795f 6375  _inline_query_cu
+0002ae80: 7272 656e 745f 6368 6174 2a20 6275 7474  rrent_chat* butt
+0002ae90: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+0002aea0: 2d20 2020 4120 7374 7269 6e67 2055 524c  -   A string URL
+0002aeb0: 2077 6974 6820 7468 6520 7573 6572 2064   with the user d
+0002aec0: 6574 6169 6c73 2c20 696e 2063 6173 6520  etails, in case 
+0002aed0: 6f66 2061 204c 6f67 696e 5572 6c20 6275  of a LoginUrl bu
+0002aee0: 7474 6f6e 2e0a 2020 2020 2020 2020 2020  tton..          
+0002aef0: 2020 2d20 2020 4120 3a6f 626a 3a60 7e70    -   A :obj:`~p
+0002af00: 7972 6f67 7261 6d2e 7479 7065 732e 5377  yrogram.types.Sw
+0002af10: 6974 6368 496e 6c69 6e65 5175 6572 7943  itchInlineQueryC
+0002af20: 686f 7365 6e43 6861 7460 206f 626a 6563  hosenChat` objec
+0002af30: 7420 696e 2063 6173 6520 6f66 2061 2060  t in case of a `
+0002af40: 6073 7769 7463 685f 696e 6c69 6e65 5f71  `switch_inline_q
+0002af50: 7565 7279 5f63 686f 7365 6e5f 6368 6174  uery_chosen_chat
+0002af60: 6060 2e0a 2020 2020 2020 2020 2020 2020  ``..            
+0002af70: 2d20 2020 4120 3a6f 626a 3a60 7e70 7972  -   A :obj:`~pyr
+0002af80: 6f67 7261 6d2e 7479 7065 732e 5573 6572  ogram.types.User
+0002af90: 6020 6f62 6a65 6374 2069 6e20 6361 7365  ` object in case
+0002afa0: 206f 6620 6120 6060 4b65 7962 6f61 7264   of a ``Keyboard
+0002afb0: 4275 7474 6f6e 5573 6572 5072 6f66 696c  ButtonUserProfil
+0002afc0: 6560 6020 6275 7474 6f6e 2e0a 0a20 2020  e`` button...   
+0002afd0: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+0002afe0: 2020 2020 2020 2020 2052 5043 4572 726f           RPCErro
+0002aff0: 723a 2049 6e20 6361 7365 206f 6620 6120  r: In case of a 
+0002b000: 5465 6c65 6772 616d 2052 5043 2065 7272  Telegram RPC err
+0002b010: 6f72 2e0a 2020 2020 2020 2020 2020 2020  or..            
+0002b020: 5661 6c75 6545 7272 6f72 3a20 496e 2063  ValueError: In c
+0002b030: 6173 6520 7468 6520 7072 6f76 6964 6564  ase the provided
+0002b040: 2069 6e64 6578 206f 7220 706f 7369 7469   index or positi
+0002b050: 6f6e 2069 7320 6f75 7420 6f66 2072 616e  on is out of ran
+0002b060: 6765 206f 7220 7468 6520 6275 7474 6f6e  ge or the button
+0002b070: 206c 6162 656c 2077 6173 206e 6f74 2066   label was not f
+0002b080: 6f75 6e64 2e0a 2020 2020 2020 2020 2020  ound..          
+0002b090: 2020 5469 6d65 6f75 7445 7272 6f72 3a20    TimeoutError: 
+0002b0a0: 496e 2063 6173 652c 2061 6674 6572 2063  In case, after c
+0002b0b0: 6c69 636b 696e 6720 616e 2069 6e6c 696e  licking an inlin
+0002b0c0: 6520 6275 7474 6f6e 2c20 7468 6520 626f  e button, the bo
+0002b0d0: 7420 6661 696c 7320 746f 2061 6e73 7765  t fails to answe
+0002b0e0: 7220 7769 7468 696e 2074 6865 2074 696d  r within the tim
+0002b0f0: 656f 7574 2e0a 2020 2020 2020 2020 2222  eout..        ""
+0002b100: 220a 0a20 2020 2020 2020 2069 6620 6973  "..        if is
+0002b110: 696e 7374 616e 6365 2873 656c 662e 7265  instance(self.re
+0002b120: 706c 795f 6d61 726b 7570 2c20 7479 7065  ply_markup, type
+0002b130: 732e 5265 706c 794b 6579 626f 6172 644d  s.ReplyKeyboardM
+0002b140: 6172 6b75 7029 3a0a 2020 2020 2020 2020  arkup):.        
+0002b150: 2020 2020 6b65 7962 6f61 7264 203d 2073      keyboard = s
+0002b160: 656c 662e 7265 706c 795f 6d61 726b 7570  elf.reply_markup
+0002b170: 2e6b 6579 626f 6172 640a 2020 2020 2020  .keyboard.      
+0002b180: 2020 2020 2020 6973 5f69 6e6c 696e 6520        is_inline 
+0002b190: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+0002b1a0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+0002b1b0: 7365 6c66 2e72 6570 6c79 5f6d 6172 6b75  self.reply_marku
+0002b1c0: 702c 2074 7970 6573 2e49 6e6c 696e 654b  p, types.InlineK
+0002b1d0: 6579 626f 6172 644d 6172 6b75 7029 3a0a  eyboardMarkup):.
+0002b1e0: 2020 2020 2020 2020 2020 2020 6b65 7962              keyb
+0002b1f0: 6f61 7264 203d 2073 656c 662e 7265 706c  oard = self.repl
+0002b200: 795f 6d61 726b 7570 2e69 6e6c 696e 655f  y_markup.inline_
+0002b210: 6b65 7962 6f61 7264 0a20 2020 2020 2020  keyboard.       
+0002b220: 2020 2020 2069 735f 696e 6c69 6e65 203d       is_inline =
+0002b230: 2054 7275 650a 2020 2020 2020 2020 656c   True.        el
+0002b240: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0002b250: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0002b260: 2822 5468 6520 6d65 7373 6167 6520 646f  ("The message do
+0002b270: 6573 6e27 7420 636f 6e74 6169 6e20 616e  esn't contain an
+0002b280: 7920 6b65 7962 6f61 7264 2229 0a0a 2020  y keyboard")..  
+0002b290: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0002b2a0: 6e63 6528 782c 2069 6e74 2920 616e 6420  nce(x, int) and 
+0002b2b0: 7920 6973 204e 6f6e 653a 0a20 2020 2020  y is None:.     
+0002b2c0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0002b2d0: 2020 2020 2020 2020 2020 2020 6275 7474              butt
+0002b2e0: 6f6e 203d 205b 0a20 2020 2020 2020 2020  on = [.         
+0002b2f0: 2020 2020 2020 2020 2020 2062 7574 746f             butto
+0002b300: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+0002b310: 2020 2020 2020 666f 7220 726f 7720 696e        for row in
+0002b320: 206b 6579 626f 6172 640a 2020 2020 2020   keyboard.      
+0002b330: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0002b340: 7220 6275 7474 6f6e 2069 6e20 726f 770a  r button in row.
+0002b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b360: 5d5b 785d 0a20 2020 2020 2020 2020 2020  ][x].           
+0002b370: 2065 7863 6570 7420 496e 6465 7845 7272   except IndexErr
+0002b380: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+0002b390: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0002b3a0: 7272 6f72 2866 2254 6865 2062 7574 746f  rror(f"The butto
+0002b3b0: 6e20 6174 2069 6e64 6578 207b 787d 2064  n at index {x} d
+0002b3c0: 6f65 736e 2774 2065 7869 7374 2229 0a20  oesn't exist"). 
+0002b3d0: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+0002b3e0: 7374 616e 6365 2878 2c20 696e 7429 2061  stance(x, int) a
+0002b3f0: 6e64 2069 7369 6e73 7461 6e63 6528 792c  nd isinstance(y,
+0002b400: 2069 6e74 293a 0a20 2020 2020 2020 2020   int):.         
+0002b410: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0002b420: 2020 2020 2020 2020 6275 7474 6f6e 203d          button =
+0002b430: 206b 6579 626f 6172 645b 795d 5b78 5d0a   keyboard[y][x].
+0002b440: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+0002b450: 7074 2049 6e64 6578 4572 726f 723a 0a20  pt IndexError:. 
+0002b460: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0002b470: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0002b480: 6622 5468 6520 6275 7474 6f6e 2061 7420  f"The button at 
+0002b490: 706f 7369 7469 6f6e 2028 7b78 7d2c 207b  position ({x}, {
+0002b4a0: 797d 2920 646f 6573 6e27 7420 6578 6973  y}) doesn't exis
+0002b4b0: 7422 290a 2020 2020 2020 2020 656c 6966  t").        elif
+0002b4c0: 2069 7369 6e73 7461 6e63 6528 782c 2073   isinstance(x, s
+0002b4d0: 7472 2920 616e 6420 7920 6973 204e 6f6e  tr) and y is Non
+0002b4e0: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
+0002b4f0: 6162 656c 203d 2078 2e65 6e63 6f64 6528  abel = x.encode(
+0002b500: 2275 7466 2d31 3622 2c20 2273 7572 726f  "utf-16", "surro
+0002b510: 6761 7465 7061 7373 2229 2e64 6563 6f64  gatepass").decod
+0002b520: 6528 2275 7466 2d31 3622 290a 0a20 2020  e("utf-16")..   
+0002b530: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+0002b540: 2020 2020 2020 2020 2020 2020 2020 6275                bu
+0002b550: 7474 6f6e 203d 205b 0a20 2020 2020 2020  tton = [.       
+0002b560: 2020 2020 2020 2020 2020 2020 2062 7574               but
+0002b570: 746f 6e0a 2020 2020 2020 2020 2020 2020  ton.            
+0002b580: 2020 2020 2020 2020 666f 7220 726f 7720          for row 
+0002b590: 696e 206b 6579 626f 6172 640a 2020 2020  in keyboard.    
+0002b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b5b0: 666f 7220 6275 7474 6f6e 2069 6e20 726f  for button in ro
+0002b5c0: 770a 2020 2020 2020 2020 2020 2020 2020  w.              
+0002b5d0: 2020 2020 2020 6966 206c 6162 656c 203d        if label =
+0002b5e0: 3d20 6275 7474 6f6e 2e74 6578 740a 2020  = button.text.  
+0002b5f0: 2020 2020 2020 2020 2020 2020 2020 5d5b                ][
+0002b600: 305d 0a20 2020 2020 2020 2020 2020 2065  0].            e
+0002b610: 7863 6570 7420 496e 6465 7845 7272 6f72  xcept IndexError
+0002b620: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002b630: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0002b640: 6f72 2866 2254 6865 2062 7574 746f 6e20  or(f"The button 
+0002b650: 7769 7468 206c 6162 656c 2027 7b78 7d27  with label '{x}'
+0002b660: 2064 6f65 736e 2774 2065 7869 7374 7322   doesn't exists"
+0002b670: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0002b680: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0002b690: 6520 5661 6c75 6545 7272 6f72 2822 496e  e ValueError("In
+0002b6a0: 7661 6c69 6420 6172 6775 6d65 6e74 7322  valid arguments"
+0002b6b0: 290a 0a20 2020 2020 2020 2069 6620 6973  )..        if is
+0002b6c0: 5f69 6e6c 696e 653a 0a20 2020 2020 2020  _inline:.       
+0002b6d0: 2020 2020 2069 6620 6275 7474 6f6e 2e63       if button.c
+0002b6e0: 616c 6c62 6163 6b5f 6461 7461 3a0a 2020  allback_data:.  
+0002b6f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0002b700: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+0002b710: 5f63 6c69 656e 742e 7265 7175 6573 745f  _client.request_
+0002b720: 6361 6c6c 6261 636b 5f61 6e73 7765 7228  callback_answer(
+0002b730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b740: 2020 2020 2063 6861 745f 6964 3d73 656c       chat_id=sel
+0002b750: 662e 6368 6174 2e69 642c 0a20 2020 2020  f.chat.id,.     
+0002b760: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0002b770: 6573 7361 6765 5f69 643d 7365 6c66 2e69  essage_id=self.i
+0002b780: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+0002b790: 2020 2020 2020 2063 616c 6c62 6163 6b5f         callback_
+0002b7a0: 6461 7461 3d62 7574 746f 6e2e 6361 6c6c  data=button.call
+0002b7b0: 6261 636b 5f64 6174 612c 0a20 2020 2020  back_data,.     
+0002b7c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0002b7d0: 696d 656f 7574 3d74 696d 656f 7574 0a20  imeout=timeout. 
+0002b7e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0002b7f0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0002b800: 6620 6275 7474 6f6e 2e63 616c 6c62 6163  f button.callbac
+0002b810: 6b5f 6461 7461 5f77 6974 685f 7061 7373  k_data_with_pass
+0002b820: 776f 7264 3a0a 2020 2020 2020 2020 2020  word:.          
+0002b830: 2020 2020 2020 6966 2070 6173 7377 6f72        if passwor
+0002b840: 6420 6973 204e 6f6e 653a 0a20 2020 2020  d is None:.     
+0002b850: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0002b860: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0002b870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b880: 2020 2020 2020 2020 2022 496e 7661 6c69           "Invali
+0002b890: 6420 6172 6775 6d65 6e74 2070 6173 7365  d argument passe
+0002b8a0: 6422 0a20 2020 2020 2020 2020 2020 2020  d".             
+0002b8b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0002b8c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0002b8d0: 6177 6169 7420 7365 6c66 2e5f 636c 6965  await self._clie
+0002b8e0: 6e74 2e72 6571 7565 7374 5f63 616c 6c62  nt.request_callb
+0002b8f0: 6163 6b5f 616e 7377 6572 280a 2020 2020  ack_answer(.    
+0002b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b910: 6368 6174 5f69 643d 7365 6c66 2e63 6861  chat_id=self.cha
+0002b920: 742e 6964 2c0a 2020 2020 2020 2020 2020  t.id,.          
+0002b930: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+0002b940: 655f 6964 3d73 656c 662e 6964 2c0a 2020  e_id=self.id,.  
+0002b950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b960: 2020 6361 6c6c 6261 636b 5f64 6174 613d    callback_data=
+0002b970: 6275 7474 6f6e 2e63 616c 6c62 6163 6b5f  button.callback_
+0002b980: 6461 7461 5f77 6974 685f 7061 7373 776f  data_with_passwo
+0002b990: 7264 2c0a 2020 2020 2020 2020 2020 2020  rd,.            
+0002b9a0: 2020 2020 2020 2020 7061 7373 776f 7264          password
+0002b9b0: 3d70 6173 7377 6f72 642c 0a20 2020 2020  =password,.     
+0002b9c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0002b9d0: 696d 656f 7574 3d74 696d 656f 7574 0a20  imeout=timeout. 
+0002b9e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0002b9f0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0002ba00: 6620 6275 7474 6f6e 2e75 726c 3a0a 2020  f button.url:.  
+0002ba10: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0002ba20: 7475 726e 2062 7574 746f 6e2e 7572 6c0a  turn button.url.
+0002ba30: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0002ba40: 2062 7574 746f 6e2e 6c6f 6769 6e5f 7572   button.login_ur
+0002ba50: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+0002ba60: 2020 2074 6c75 203d 2062 7574 746f 6e2e     tlu = button.
+0002ba70: 6c6f 6769 6e5f 7572 6c0a 2020 2020 2020  login_url.      
+0002ba80: 2020 2020 2020 2020 2020 7269 6565 7020            rieep 
+0002ba90: 3d20 6177 6169 7420 7365 6c66 2e5f 636c  = await self._cl
+0002baa0: 6965 6e74 2e72 6573 6f6c 7665 5f70 6565  ient.resolve_pee
+0002bab0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+0002bac0: 2020 2020 2020 2073 656c 662e 6368 6174         self.chat
+0002bad0: 2e69 640a 2020 2020 2020 2020 2020 2020  .id.            
+0002bae0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0002baf0: 2020 2020 2020 6f6b 6475 6974 203d 2061        okduit = a
+0002bb00: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
+0002bb10: 742e 696e 766f 6b65 280a 2020 2020 2020  t.invoke(.      
+0002bb20: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0002bb30: 772e 6675 6e63 7469 6f6e 732e 6d65 7373  w.functions.mess
+0002bb40: 6167 6573 2e52 6571 7565 7374 5572 6c41  ages.RequestUrlA
+0002bb50: 7574 6828 0a20 2020 2020 2020 2020 2020  uth(.           
+0002bb60: 2020 2020 2020 2020 2020 2020 2070 6565               pee
+0002bb70: 723d 7269 6565 702c 0a20 2020 2020 2020  r=rieep,.       
+0002bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bb90: 206d 7367 5f69 643d 7365 6c66 2e69 642c   msg_id=self.id,
+0002bba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002bbb0: 2020 2020 2020 2020 2062 7574 746f 6e5f           button_
+0002bbc0: 6964 3d74 6c75 2e62 7574 746f 6e5f 6964  id=tlu.button_id
+0002bbd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002bbe0: 2020 2020 2020 2020 2020 7572 6c3d 746c            url=tl
+0002bbf0: 752e 7572 6c0a 2020 2020 2020 2020 2020  u.url.          
+0002bc00: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0002bc10: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0002bc20: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+0002bc30: 7564 6b6f 203d 2061 7761 6974 2073 656c  udko = await sel
+0002bc40: 662e 5f63 6c69 656e 742e 696e 766f 6b65  f._client.invoke
+0002bc50: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0002bc60: 2020 2020 2020 7261 772e 6675 6e63 7469        raw.functi
+0002bc70: 6f6e 732e 6d65 7373 6167 6573 2e41 6363  ons.messages.Acc
+0002bc80: 6570 7455 726c 4175 7468 280a 2020 2020  eptUrlAuth(.    
+0002bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bca0: 2020 2020 7772 6974 655f 616c 6c6f 7765      write_allowe
+0002bcb0: 643d 7265 7175 6573 745f 7772 6974 655f  d=request_write_
+0002bcc0: 6163 6365 7373 2c0a 2020 2020 2020 2020  access,.        
+0002bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bce0: 7065 6572 3d72 6965 6570 2c0a 2020 2020  peer=rieep,.    
+0002bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bd00: 2020 2020 6d73 675f 6964 3d73 656c 662e      msg_id=self.
+0002bd10: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0002bd20: 2020 2020 2020 2020 2020 2020 6275 7474              butt
+0002bd30: 6f6e 5f69 643d 746c 752e 6275 7474 6f6e  on_id=tlu.button
+0002bd40: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+0002bd50: 2020 2020 2020 2020 2020 2020 2075 726c               url
+0002bd60: 3d74 6c75 2e75 726c 0a20 2020 2020 2020  =tlu.url.       
+0002bd70: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0002bd80: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0002bd90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002bda0: 2072 6574 7572 6e20 7469 7564 6b6f 2e75   return tiudko.u
+0002bdb0: 726c 0a20 2020 2020 2020 2020 2020 2065  rl.            e
+0002bdc0: 6c69 6620 6275 7474 6f6e 2e77 6562 5f61  lif button.web_a
+0002bdd0: 7070 3a0a 2020 2020 2020 2020 2020 2020  pp:.            
+0002bde0: 2020 2020 746c 7520 3d20 6275 7474 6f6e      tlu = button
+0002bdf0: 2e77 6562 5f61 7070 0a20 2020 2020 2020  .web_app.       
+0002be00: 2020 2020 2020 2020 2077 6869 6368 626f           whichbo
+0002be10: 7463 6861 7420 3d20 280a 2020 2020 2020  tchat = (.      
+0002be20: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0002be30: 6c66 2e76 6961 5f62 6f74 2061 6e64 0a20  lf.via_bot and. 
+0002be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002be50: 2020 2073 656c 662e 7669 615f 626f 742e     self.via_bot.
+0002be60: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
+0002be70: 2020 2029 206f 7220 280a 2020 2020 2020     ) or (.      
+0002be80: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0002be90: 6c66 2e66 726f 6d5f 7573 6572 2061 6e64  lf.from_user and
+0002bea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002beb0: 2020 2020 2073 656c 662e 6672 6f6d 5f75       self.from_u
+0002bec0: 7365 722e 6973 5f62 6f74 2061 6e64 0a20  ser.is_bot and. 
+0002bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bee0: 2020 2073 656c 662e 6672 6f6d 5f75 7365     self.from_use
+0002bef0: 722e 6964 0a20 2020 2020 2020 2020 2020  r.id.           
+0002bf00: 2020 2020 2029 206f 7220 4e6f 6e65 0a20       ) or None. 
+0002bf10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0002bf20: 6620 6e6f 7420 7768 6963 6862 6f74 6368  f not whichbotch
+0002bf30: 6174 3a0a 2020 2020 2020 2020 2020 2020  at:.            
+0002bf40: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+0002bf50: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+0002bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bf70: 2020 2249 6e76 616c 6964 2043 6861 7442    "Invalid ChatB
+0002bf80: 6f74 5479 7065 220a 2020 2020 2020 2020  otType".        
+0002bf90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0002bfa0: 2020 2020 2020 2020 2020 2020 2020 7269                ri
+0002bfb0: 6565 7020 3d20 6177 6169 7420 7365 6c66  eep = await self
+0002bfc0: 2e5f 636c 6965 6e74 2e72 6573 6f6c 7665  ._client.resolve
+0002bfd0: 5f70 6565 7228 0a20 2020 2020 2020 2020  _peer(.         
+0002bfe0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002bff0: 6368 6174 2e69 640a 2020 2020 2020 2020  chat.id.        
+0002c000: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0002c010: 2020 2020 2020 2020 2020 6965 6570 7220            ieepr 
+0002c020: 3d20 6177 6169 7420 7365 6c66 2e5f 636c  = await self._cl
+0002c030: 6965 6e74 2e72 6573 6f6c 7665 5f70 6565  ient.resolve_pee
+0002c040: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+0002c050: 2020 2020 2020 2077 6869 6368 626f 7463         whichbotc
+0002c060: 6861 740a 2020 2020 2020 2020 2020 2020  hat.            
+0002c070: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0002c080: 2020 2020 2020 6f6b 6475 6974 203d 2061        okduit = a
+0002c090: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
+0002c0a0: 742e 696e 766f 6b65 280a 2020 2020 2020  t.invoke(.      
+0002c0b0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0002c0c0: 772e 6675 6e63 7469 6f6e 732e 6d65 7373  w.functions.mess
+0002c0d0: 6167 6573 2e52 6571 7565 7374 5765 6256  ages.RequestWebV
+0002c0e0: 6965 7728 0a20 2020 2020 2020 2020 2020  iew(.           
+0002c0f0: 2020 2020 2020 2020 2020 2020 2070 6565               pee
+0002c100: 723d 7269 6565 702c 0a20 2020 2020 2020  r=rieep,.       
+0002c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c120: 2062 6f74 3d69 6565 7072 2c0a 2020 2020   bot=ieepr,.    
+0002c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c140: 2020 2020 7572 6c3d 746c 752e 7572 6c2c      url=tlu.url,
+0002c150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c160: 2020 2020 2020 2020 2070 6c61 7466 6f72           platfor
+0002c170: 6d3d 7365 6c66 2e5f 636c 6965 6e74 2e63  m=self._client.c
+0002c180: 6c69 656e 745f 706c 6174 666f 726d 2e76  lient_platform.v
+0002c190: 616c 7565 2c0a 2020 2020 2020 2020 2020  alue,.          
+0002c1a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0002c1b0: 544f 444f 0a20 2020 2020 2020 2020 2020  TODO.           
+0002c1c0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0002c1d0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0002c1e0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0002c1f0: 7572 6e20 6f6b 6475 6974 2e75 726c 0a20  urn okduit.url. 
+0002c200: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0002c210: 6275 7474 6f6e 2e75 7365 725f 6964 3a0a  button.user_id:.
+0002c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c230: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+0002c240: 662e 5f63 6c69 656e 742e 6765 745f 6368  f._client.get_ch
+0002c250: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+0002c260: 2020 2020 2020 2020 6275 7474 6f6e 2e75          button.u
+0002c270: 7365 725f 6964 2c0a 2020 2020 2020 2020  ser_id,.        
+0002c280: 2020 2020 2020 2020 2020 2020 4661 6c73              Fals
+0002c290: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0002c2a0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0002c2b0: 656c 6966 2062 7574 746f 6e2e 7377 6974  elif button.swit
+0002c2c0: 6368 5f69 6e6c 696e 655f 7175 6572 793a  ch_inline_query:
+0002c2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c2e0: 2072 6574 7572 6e20 6275 7474 6f6e 2e73   return button.s
+0002c2f0: 7769 7463 685f 696e 6c69 6e65 5f71 7565  witch_inline_que
+0002c300: 7279 0a20 2020 2020 2020 2020 2020 2065  ry.            e
+0002c310: 6c69 6620 6275 7474 6f6e 2e73 7769 7463  lif button.switc
+0002c320: 685f 696e 6c69 6e65 5f71 7565 7279 5f63  h_inline_query_c
+0002c330: 7572 7265 6e74 5f63 6861 743a 0a20 2020  urrent_chat:.   
+0002c340: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0002c350: 7572 6e20 6275 7474 6f6e 2e73 7769 7463  urn button.switc
+0002c360: 685f 696e 6c69 6e65 5f71 7565 7279 5f63  h_inline_query_c
+0002c370: 7572 7265 6e74 5f63 6861 740a 2020 2020  urrent_chat.    
+0002c380: 2020 2020 2020 2020 656c 6966 2062 7574          elif but
+0002c390: 746f 6e2e 7377 6974 6368 5f69 6e6c 696e  ton.switch_inlin
+0002c3a0: 655f 7175 6572 795f 6368 6f73 656e 5f63  e_query_chosen_c
+0002c3b0: 6861 743a 0a20 2020 2020 2020 2020 2020  hat:.           
+0002c3c0: 2020 2020 2072 6574 7572 6e20 6275 7474       return butt
+0002c3d0: 6f6e 2e73 7769 7463 685f 696e 6c69 6e65  on.switch_inline
+0002c3e0: 5f71 7565 7279 5f63 686f 7365 6e5f 6368  _query_chosen_ch
+0002c3f0: 6174 0a20 2020 2020 2020 2020 2020 2065  at.            e
+0002c400: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0002c410: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0002c420: 4572 726f 7228 2254 6869 7320 6275 7474  Error("This butt
+0002c430: 6f6e 2069 7320 6e6f 7420 7375 7070 6f72  on is not suppor
+0002c440: 7465 6420 7965 7422 290a 2020 2020 2020  ted yet").      
+0002c450: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002c460: 2020 2020 6177 6169 7420 7365 6c66 2e72      await self.r
+0002c470: 6570 6c79 2874 6578 743d 6275 7474 6f6e  eply(text=button
+0002c480: 2c20 7175 6f74 653d 7175 6f74 6529 0a0a  , quote=quote)..
+0002c490: 2020 2020 6173 796e 6320 6465 6620 7265      async def re
+0002c4a0: 6163 7428 0a20 2020 2020 2020 2073 656c  act(.        sel
+0002c4b0: 662c 0a20 2020 2020 2020 2072 6561 6374  f,.        react
+0002c4c0: 696f 6e3a 2055 6e69 6f6e 5b0a 2020 2020  ion: Union[.    
+0002c4d0: 2020 2020 2020 2020 696e 742c 0a20 2020          int,.   
+0002c4e0: 2020 2020 2020 2020 2073 7472 2c0a 2020           str,.  
+0002c4f0: 2020 2020 2020 2020 2020 4c69 7374 5b55            List[U
+0002c500: 6e69 6f6e 5b69 6e74 2c20 7374 722c 2022  nion[int, str, "
+0002c510: 7479 7065 732e 5265 6163 7469 6f6e 5479  types.ReactionTy
+0002c520: 7065 225d 5d0a 2020 2020 2020 2020 5d20  pe"]].        ] 
+0002c530: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0002c540: 6973 5f62 6967 3a20 626f 6f6c 203d 2046  is_big: bool = F
+0002c550: 616c 7365 2c0a 2020 2020 2020 2020 6164  alse,.        ad
+0002c560: 645f 746f 5f72 6563 656e 743a 2062 6f6f  d_to_recent: boo
+0002c570: 6c20 3d20 5472 7565 0a20 2020 2029 202d  l = True.    ) -
+0002c580: 3e20 2274 7970 6573 2e4d 6573 7361 6765  > "types.Message
+0002c590: 5265 6163 7469 6f6e 7322 3a0a 2020 2020  Reactions":.    
+0002c5a0: 2020 2020 2222 2242 6f75 6e64 206d 6574      """Bound met
+0002c5b0: 686f 6420 2a72 6561 6374 2a20 6f66 203a  hod *react* of :
+0002c5c0: 6f62 6a3a 607e 7079 726f 6772 616d 2e74  obj:`~pyrogram.t
+0002c5d0: 7970 6573 2e4d 6573 7361 6765 602e 0a0a  ypes.Message`...
+0002c5e0: 2020 2020 2020 2020 5573 6520 6173 2061          Use as a
+0002c5f0: 2073 686f 7274 6375 7420 666f 723a 0a0a   shortcut for:..
+0002c600: 2020 2020 2020 2020 2e2e 2063 6f64 652d          .. code-
+0002c610: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
+0002c620: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+0002c630: 7420 636c 6965 6e74 2e73 6574 5f72 6561  t client.set_rea
+0002c640: 6374 696f 6e28 0a20 2020 2020 2020 2020  ction(.         
+0002c650: 2020 2020 2020 2063 6861 745f 6964 3d63         chat_id=c
+0002c660: 6861 745f 6964 2c0a 2020 2020 2020 2020  hat_id,.        
+0002c670: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
+0002c680: 6964 3d6d 6573 7361 6765 2e69 642c 0a20  id=message.id,. 
+0002c690: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0002c6a0: 6561 6374 696f 6e3d 5b52 6561 6374 696f  eaction=[Reactio
+0002c6b0: 6e54 7970 6545 6d6f 6a69 2865 6d6f 6a69  nTypeEmoji(emoji
+0002c6c0: 3d22 f09f 918d 2229 5d0a 2020 2020 2020  ="....")].      
+0002c6d0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0002c6e0: 2045 7861 6d70 6c65 3a0a 2020 2020 2020   Example:.      
+0002c6f0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
+0002c700: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
+0002c710: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0002c720: 5365 6e64 2061 2072 6561 6374 696f 6e0a  Send a reaction.
+0002c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c740: 6177 6169 7420 6d65 7373 6167 652e 7265  await message.re
+0002c750: 6163 7428 5b52 6561 6374 696f 6e54 7970  act([ReactionTyp
+0002c760: 6545 6d6f 6a69 2865 6d6f 6a69 3d22 f09f  eEmoji(emoji="..
+0002c770: 918d 2229 5d29 0a0a 2020 2020 2020 2020  ..")])..        
+0002c780: 2020 2020 2020 2020 2320 5265 7472 6163          # Retrac
+0002c790: 7420 6120 7265 6163 7469 6f6e 0a20 2020  t a reaction.   
+0002c7a0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
+0002c7b0: 6974 206d 6573 7361 6765 2e72 6561 6374  it message.react
+0002c7c0: 2829 0a0a 2020 2020 2020 2020 5061 7261  ()..        Para
+0002c7d0: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
+0002c7e0: 2020 2020 7265 6163 7469 6f6e 2028 6060      reaction (``
+0002c7f0: 696e 7460 6020 7c20 6060 7374 7260 6020  int`` | ``str`` 
+0002c800: 7c20 4c69 7374 206f 6620 6060 696e 7460  | List of ``int`
+0002c810: 6020 4f52 2060 6073 7472 6060 207c 204c  ` OR ``str`` | L
+0002c820: 6973 7420 6f66 203a 6f62 6a3a 607e 7079  ist of :obj:`~py
+0002c830: 726f 6772 616d 2e74 7970 6573 2e52 6561  rogram.types.Rea
+0002c840: 6374 696f 6e54 7970 6560 2c20 2a6f 7074  ctionType`, *opt
+0002c850: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
+0002c860: 2020 2020 2020 2020 204e 6577 206c 6973           New lis
+0002c870: 7420 6f66 2072 6561 6374 696f 6e20 7479  t of reaction ty
+0002c880: 7065 7320 746f 2073 6574 206f 6e20 7468  pes to set on th
+0002c890: 6520 6d65 7373 6167 652e 0a20 2020 2020  e message..     
+0002c8a0: 2020 2020 2020 2020 2020 2050 6173 7320             Pass 
+0002c8b0: 4e6f 6e65 2061 7320 656d 6f6a 6920 2864  None as emoji (d
+0002c8c0: 6566 6175 6c74 2920 746f 2072 6574 7261  efault) to retra
+0002c8d0: 6374 2074 6865 2072 6561 6374 696f 6e2e  ct the reaction.
+0002c8e0: 0a0a 2020 2020 2020 2020 2020 2020 6973  ..            is
+0002c8f0: 5f62 6967 2028 6060 626f 6f6c 6060 2c20  _big (``bool``, 
+0002c900: 2a6f 7074 696f 6e61 6c2a 293a 0a20 2020  *optional*):.   
+0002c910: 2020 2020 2020 2020 2020 2020 2050 6173               Pas
+0002c920: 7320 5472 7565 2074 6f20 7365 7420 7468  s True to set th
+0002c930: 6520 7265 6163 7469 6f6e 2077 6974 6820  e reaction with 
+0002c940: 6120 6269 6720 616e 696d 6174 696f 6e2e  a big animation.
+0002c950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c960: 2044 6566 6175 6c74 7320 746f 2046 616c   Defaults to Fal
+0002c970: 7365 2e0a 2020 2020 2020 2020 2020 2020  se..            
+0002c980: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
+0002c990: 5f74 6f5f 7265 6365 6e74 2028 6060 626f  _to_recent (``bo
+0002c9a0: 6f6c 6060 2c20 2a6f 7074 696f 6e61 6c2a  ol``, *optional*
+0002c9b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0002c9c0: 2020 2050 6173 7320 5472 7565 2069 6620     Pass True if 
+0002c9d0: 7468 6520 7265 6163 7469 6f6e 2073 686f  the reaction sho
+0002c9e0: 756c 6420 6170 7065 6172 2069 6e20 7468  uld appear in th
+0002c9f0: 6520 7265 6365 6e74 6c79 2075 7365 6420  e recently used 
+0002ca00: 7265 6163 7469 6f6e 732e 0a20 2020 2020  reactions..     
+0002ca10: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+0002ca20: 6f70 7469 6f6e 2069 7320 6170 706c 6963  option is applic
+0002ca30: 6162 6c65 206f 6e6c 7920 666f 7220 7573  able only for us
+0002ca40: 6572 732e 0a20 2020 2020 2020 2020 2020  ers..           
+0002ca50: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+0002ca60: 2054 7275 652e 0a20 2020 2020 2020 2052   True..        R
+0002ca70: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0002ca80: 2020 2020 4f6e 2073 7563 6365 7373 2c20      On success, 
+0002ca90: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
+0002caa0: 7479 7065 732e 4d65 7373 6167 6552 6561  types.MessageRea
+0002cab0: 6374 696f 6e73 603a 2069 7320 7265 7475  ctions`: is retu
+0002cac0: 726e 6564 2e0a 0a20 2020 2020 2020 2052  rned...        R
+0002cad0: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
+0002cae0: 2020 2052 5043 4572 726f 723a 2049 6e20     RPCError: In 
+0002caf0: 6361 7365 206f 6620 6120 5465 6c65 6772  case of a Telegr
+0002cb00: 616d 2052 5043 2065 7272 6f72 2e0a 2020  am RPC error..  
+0002cb10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0002cb20: 2020 7372 203d 204e 6f6e 650a 0a20 2020    sr = None..   
+0002cb30: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+0002cb40: 6365 2872 6561 6374 696f 6e2c 204c 6973  ce(reaction, Lis
+0002cb50: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+0002cb60: 7372 203d 205b 5d0a 2020 2020 2020 2020  sr = [].        
+0002cb70: 2020 2020 666f 7220 6920 696e 2072 6561      for i in rea
+0002cb80: 6374 696f 6e3a 0a20 2020 2020 2020 2020  ction:.         
+0002cb90: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0002cba0: 616e 6365 2869 2c20 7479 7065 732e 5265  ance(i, types.Re
+0002cbb0: 6163 7469 6f6e 5479 7065 293a 0a20 2020  actionType):.   
+0002cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cbd0: 2073 722e 6170 7065 6e64 2869 290a 2020   sr.append(i).  
+0002cbe0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0002cbf0: 6966 2069 7369 6e73 7461 6e63 6528 692c  if isinstance(i,
+0002cc00: 2069 6e74 293a 0a20 2020 2020 2020 2020   int):.         
+0002cc10: 2020 2020 2020 2020 2020 2073 722e 6170             sr.ap
+0002cc20: 7065 6e64 2874 7970 6573 2e52 6561 6374  pend(types.React
+0002cc30: 696f 6e54 7970 6543 7573 746f 6d45 6d6f  ionTypeCustomEmo
+0002cc40: 6a69 280a 2020 2020 2020 2020 2020 2020  ji(.            
+0002cc50: 2020 2020 2020 2020 2020 2020 6375 7374              cust
+0002cc60: 6f6d 5f65 6d6f 6a69 5f69 643d 7374 7228  om_emoji_id=str(
+0002cc70: 6929 0a20 2020 2020 2020 2020 2020 2020  i).             
+0002cc80: 2020 2020 2020 2029 290a 2020 2020 2020         )).      
+0002cc90: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0002cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ccb0: 2020 2020 7372 2e61 7070 656e 6428 7479      sr.append(ty
+0002ccc0: 7065 732e 5265 6163 7469 6f6e 5479 7065  pes.ReactionType
+0002ccd0: 456d 6f6a 6928 0a20 2020 2020 2020 2020  Emoji(.         
+0002cce0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0002ccf0: 6d6f 6a69 3d69 0a20 2020 2020 2020 2020  moji=i.         
+0002cd00: 2020 2020 2020 2020 2020 2029 290a 0a20             )).. 
+0002cd10: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+0002cd20: 7374 616e 6365 2872 6561 6374 696f 6e2c  stance(reaction,
+0002cd30: 2069 6e74 293a 0a20 2020 2020 2020 2020   int):.         
+0002cd40: 2020 2073 7220 3d20 5b0a 2020 2020 2020     sr = [.      
+0002cd50: 2020 2020 2020 2020 2020 7479 7065 732e            types.
+0002cd60: 5265 6163 7469 6f6e 5479 7065 4375 7374  ReactionTypeCust
+0002cd70: 6f6d 456d 6f6a 6928 0a20 2020 2020 2020  omEmoji(.       
+0002cd80: 2020 2020 2020 2020 2020 2020 2063 7573               cus
+0002cd90: 746f 6d5f 656d 6f6a 695f 6964 3d73 7472  tom_emoji_id=str
+0002cda0: 2872 6561 6374 696f 6e29 0a20 2020 2020  (reaction).     
+0002cdb0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0002cdc0: 2020 2020 2020 2020 205d 0a0a 2020 2020           ]..    
+0002cdd0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+0002cde0: 6e63 6528 7265 6163 7469 6f6e 2c20 7374  nce(reaction, st
+0002cdf0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0002ce00: 7372 203d 205b 0a20 2020 2020 2020 2020  sr = [.         
+0002ce10: 2020 2020 2020 2074 7970 6573 2e52 6561         types.Rea
+0002ce20: 6374 696f 6e54 7970 6545 6d6f 6a69 280a  ctionTypeEmoji(.
+0002ce30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ce40: 2020 2020 656d 6f6a 693d 7265 6163 7469      emoji=reacti
+0002ce50: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+0002ce60: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0002ce70: 205d 0a0a 2020 2020 2020 2020 7265 7475   ]..        retu
+0002ce80: 726e 2061 7761 6974 2073 656c 662e 5f63  rn await self._c
+0002ce90: 6c69 656e 742e 7365 745f 7265 6163 7469  lient.set_reacti
+0002cea0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+0002ceb0: 6368 6174 5f69 643d 7365 6c66 2e63 6861  chat_id=self.cha
+0002cec0: 742e 6964 2c0a 2020 2020 2020 2020 2020  t.id,.          
+0002ced0: 2020 6d65 7373 6167 655f 6964 3d73 656c    message_id=sel
+0002cee0: 662e 6964 2c0a 2020 2020 2020 2020 2020  f.id,.          
+0002cef0: 2020 7265 6163 7469 6f6e 3d73 722c 0a20    reaction=sr,. 
+0002cf00: 2020 2020 2020 2020 2020 2069 735f 6269             is_bi
+0002cf10: 673d 6973 5f62 6967 2c0a 2020 2020 2020  g=is_big,.      
+0002cf20: 2020 2020 2020 6164 645f 746f 5f72 6563        add_to_rec
+0002cf30: 656e 743d 6164 645f 746f 5f72 6563 656e  ent=add_to_recen
+0002cf40: 740a 2020 2020 2020 2020 290a 0a20 2020  t.        )..   
+0002cf50: 2061 7379 6e63 2064 6566 2072 6574 7261   async def retra
+0002cf60: 6374 5f76 6f74 6528 0a20 2020 2020 2020  ct_vote(.       
+0002cf70: 2073 656c 662c 0a20 2020 2029 202d 3e20   self,.    ) -> 
+0002cf80: 2274 7970 6573 2e50 6f6c 6c22 3a0a 2020  "types.Poll":.  
+0002cf90: 2020 2020 2020 2222 2242 6f75 6e64 206d        """Bound m
+0002cfa0: 6574 686f 6420 2a72 6574 7261 6374 5f76  ethod *retract_v
+0002cfb0: 6f74 652a 206f 6620 3a6f 626a 3a60 7e70  ote* of :obj:`~p
+0002cfc0: 7972 6f67 7261 6d2e 7479 7065 732e 4d65  yrogram.types.Me
+0002cfd0: 7373 6167 6560 2e0a 0a20 2020 2020 2020  ssage`...       
+0002cfe0: 2055 7365 2061 7320 6120 7368 6f72 7463   Use as a shortc
+0002cff0: 7574 2066 6f72 3a0a 0a20 2020 2020 2020  ut for:..       
+0002d000: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+0002d010: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+0002d020: 2020 2020 2063 6c69 656e 742e 7265 7472       client.retr
+0002d030: 6163 745f 766f 7465 280a 2020 2020 2020  act_vote(.      
+0002d040: 2020 2020 2020 2020 2020 6368 6174 5f69            chat_i
+0002d050: 643d 6d65 7373 6167 652e 6368 6174 2e69  d=message.chat.i
+0002d060: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+0002d070: 2020 206d 6573 7361 6765 5f69 643d 6d65     message_id=me
+0002d080: 7373 6167 655f 6964 2c0a 2020 2020 2020  ssage_id,.      
+0002d090: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0002d0a0: 2045 7861 6d70 6c65 3a0a 2020 2020 2020   Example:.      
+0002d0b0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
+0002d0c0: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
+0002d0d0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0002d0e0: 7373 6167 652e 7265 7472 6163 745f 766f  ssage.retract_vo
+0002d0f0: 7465 2829 0a0a 2020 2020 2020 2020 5265  te()..        Re
+0002d100: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0002d110: 2020 203a 6f62 6a3a 607e 7079 726f 6772     :obj:`~pyrogr
+0002d120: 616d 2e74 7970 6573 2e50 6f6c 6c60 3a20  am.types.Poll`: 
+0002d130: 4f6e 2073 7563 6365 7373 2c20 7468 6520  On success, the 
+0002d140: 706f 6c6c 2077 6974 6820 7468 6520 7265  poll with the re
+0002d150: 7472 6163 7465 6420 766f 7465 2069 7320  tracted vote is 
+0002d160: 7265 7475 726e 6564 2e0a 0a20 2020 2020  returned...     
+0002d170: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+0002d180: 2020 2020 2020 2052 5043 4572 726f 723a         RPCError:
+0002d190: 2049 6e20 6361 7365 206f 6620 6120 5465   In case of a Te
+0002d1a0: 6c65 6772 616d 2052 5043 2065 7272 6f72  legram RPC error
+0002d1b0: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+0002d1c0: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+0002d1d0: 6169 7420 7365 6c66 2e5f 636c 6965 6e74  ait self._client
+0002d1e0: 2e72 6574 7261 6374 5f76 6f74 6528 0a20  .retract_vote(. 
+0002d1f0: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
+0002d200: 6964 3d73 656c 662e 6368 6174 2e69 642c  id=self.chat.id,
+0002d210: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
+0002d220: 7361 6765 5f69 643d 7365 6c66 2e69 640a  sage_id=self.id.
+0002d230: 2020 2020 2020 2020 290a 0a20 2020 2061          )..    a
+0002d240: 7379 6e63 2064 6566 2064 6f77 6e6c 6f61  sync def downloa
+0002d250: 6428 0a20 2020 2020 2020 2073 656c 662c  d(.        self,
+0002d260: 0a20 2020 2020 2020 2066 696c 655f 6e61  .        file_na
+0002d270: 6d65 3a20 7374 7220 3d20 2222 2c0a 2020  me: str = "",.  
+0002d280: 2020 2020 2020 696e 5f6d 656d 6f72 793a        in_memory:
+0002d290: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+0002d2a0: 2020 2020 2020 2062 6c6f 636b 3a20 626f         block: bo
+0002d2b0: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
+0002d2c0: 2020 2070 726f 6772 6573 733a 2043 616c     progress: Cal
+0002d2d0: 6c61 626c 6520 3d20 4e6f 6e65 2c0a 2020  lable = None,.  
+0002d2e0: 2020 2020 2020 7072 6f67 7265 7373 5f61        progress_a
+0002d2f0: 7267 733a 2074 7570 6c65 203d 2028 290a  rgs: tuple = ().
+0002d300: 2020 2020 2920 2d3e 2073 7472 3a0a 2020      ) -> str:.  
+0002d310: 2020 2020 2020 2222 2242 6f75 6e64 206d        """Bound m
+0002d320: 6574 686f 6420 2a64 6f77 6e6c 6f61 642a  ethod *download*
+0002d330: 206f 6620 3a6f 626a 3a60 7e70 7972 6f67   of :obj:`~pyrog
+0002d340: 7261 6d2e 7479 7065 732e 4d65 7373 6167  ram.types.Messag
+0002d350: 6560 2e0a 0a20 2020 2020 2020 2055 7365  e`...        Use
+0002d360: 2061 7320 6120 7368 6f72 7463 7574 2066   as a shortcut f
+0002d370: 6f72 3a0a 0a20 2020 2020 2020 202e 2e20  or:..        .. 
+0002d380: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
+0002d390: 686f 6e0a 0a20 2020 2020 2020 2020 2020  hon..           
+0002d3a0: 2061 7761 6974 2063 6c69 656e 742e 646f   await client.do
+0002d3b0: 776e 6c6f 6164 5f6d 6564 6961 286d 6573  wnload_media(mes
+0002d3c0: 7361 6765 290a 0a20 2020 2020 2020 2045  sage)..        E
+0002d3d0: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
+0002d3e0: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+0002d3f0: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
+0002d400: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+0002d410: 7420 6d65 7373 6167 652e 646f 776e 6c6f  t message.downlo
+0002d420: 6164 2829 0a0a 2020 2020 2020 2020 5061  ad()..        Pa
+0002d430: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
+0002d440: 2020 2020 2020 6669 6c65 5f6e 616d 6520        file_name 
+0002d450: 2860 6073 7472 6060 2c20 2a6f 7074 696f  (``str``, *optio
+0002d460: 6e61 6c2a 293a 0a20 2020 2020 2020 2020  nal*):.         
+0002d470: 2020 2020 2020 2041 2063 7573 746f 6d20         A custom 
+0002d480: 2a66 696c 655f 6e61 6d65 2a20 746f 2062  *file_name* to b
+0002d490: 6520 7573 6564 2069 6e73 7465 6164 206f  e used instead o
+0002d4a0: 6620 7468 6520 6f6e 6520 7072 6f76 6964  f the one provid
+0002d4b0: 6564 2062 7920 5465 6c65 6772 616d 2e0a  ed by Telegram..
+0002d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d4d0: 4279 2064 6566 6175 6c74 2c20 616c 6c20  By default, all 
+0002d4e0: 6669 6c65 7320 6172 6520 646f 776e 6c6f  files are downlo
+0002d4f0: 6164 6564 2069 6e20 7468 6520 2a64 6f77  aded in the *dow
+0002d500: 6e6c 6f61 6473 2a20 666f 6c64 6572 2069  nloads* folder i
+0002d510: 6e20 796f 7572 2077 6f72 6b69 6e67 2064  n your working d
+0002d520: 6972 6563 746f 7279 2e0a 2020 2020 2020  irectory..      
+0002d530: 2020 2020 2020 2020 2020 596f 7520 6361            You ca
+0002d540: 6e20 616c 736f 2073 7065 6369 6679 2061  n also specify a
+0002d550: 2070 6174 6820 666f 7220 646f 776e 6c6f   path for downlo
+0002d560: 6164 696e 6720 6669 6c65 7320 696e 2061  ading files in a
+0002d570: 2063 7573 746f 6d20 6c6f 6361 7469 6f6e   custom location
+0002d580: 3a20 7061 7468 7320 7468 6174 2065 6e64  : paths that end
+0002d590: 2077 6974 6820 222f 220a 2020 2020 2020   with "/".      
+0002d5a0: 2020 2020 2020 2020 2020 6172 6520 636f            are co
+0002d5b0: 6e73 6964 6572 6564 2064 6972 6563 746f  nsidered directo
+0002d5c0: 7269 6573 2e20 416c 6c20 6e6f 6e2d 6578  ries. All non-ex
+0002d5d0: 6973 7465 6e74 2066 6f6c 6465 7273 2077  istent folders w
+0002d5e0: 696c 6c20 6265 2063 7265 6174 6564 2061  ill be created a
+0002d5f0: 7574 6f6d 6174 6963 616c 6c79 2e0a 0a20  utomatically... 
+0002d600: 2020 2020 2020 2020 2020 2069 6e5f 6d65             in_me
+0002d610: 6d6f 7279 2028 6060 626f 6f6c 6060 2c20  mory (``bool``, 
+0002d620: 2a6f 7074 696f 6e61 6c2a 293a 0a20 2020  *optional*):.   
+0002d630: 2020 2020 2020 2020 2020 2020 2050 6173               Pas
+0002d640: 7320 5472 7565 2074 6f20 646f 776e 6c6f  s True to downlo
+0002d650: 6164 2074 6865 206d 6564 6961 2069 6e2d  ad the media in-
+0002d660: 6d65 6d6f 7279 2e0a 2020 2020 2020 2020  memory..        
+0002d670: 2020 2020 2020 2020 4120 6269 6e61 7279          A binary
+0002d680: 2066 696c 652d 6c69 6b65 206f 626a 6563   file-like objec
+0002d690: 7420 7769 7468 2069 7473 2061 7474 7269  t with its attri
+0002d6a0: 6275 7465 2022 2e6e 616d 6522 2073 6574  bute ".name" set
+0002d6b0: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+0002d6c0: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
+0002d6d0: 2020 2044 6566 6175 6c74 7320 746f 2046     Defaults to F
+0002d6e0: 616c 7365 2e0a 0a20 2020 2020 2020 2020  alse...         
+0002d6f0: 2020 2062 6c6f 636b 2028 6060 626f 6f6c     block (``bool
+0002d700: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
+0002d710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002d720: 2042 6c6f 636b 7320 7468 6520 636f 6465   Blocks the code
+0002d730: 2065 7865 6375 7469 6f6e 2075 6e74 696c   execution until
+0002d740: 2074 6865 2066 696c 6520 6861 7320 6265   the file has be
+0002d750: 656e 2064 6f77 6e6c 6f61 6465 642e 0a20  en downloaded.. 
+0002d760: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+0002d770: 6566 6175 6c74 7320 746f 2054 7275 652e  efaults to True.
+0002d780: 0a0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+0002d790: 6f67 7265 7373 2028 6060 4361 6c6c 6162  ogress (``Callab
+0002d7a0: 6c65 6060 2c20 2a6f 7074 696f 6e61 6c2a  le``, *optional*
+0002d7b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0002d7c0: 2020 2050 6173 7320 6120 6361 6c6c 6261     Pass a callba
+0002d7d0: 636b 2066 756e 6374 696f 6e20 746f 2076  ck function to v
+0002d7e0: 6965 7720 7468 6520 6669 6c65 2074 7261  iew the file tra
+0002d7f0: 6e73 6d69 7373 696f 6e20 7072 6f67 7265  nsmission progre
+0002d800: 7373 2e0a 2020 2020 2020 2020 2020 2020  ss..            
+0002d810: 2020 2020 5468 6520 6675 6e63 7469 6f6e      The function
+0002d820: 206d 7573 7420 7461 6b65 202a 2863 7572   must take *(cur
+0002d830: 7265 6e74 2c20 746f 7461 6c29 2a20 6173  rent, total)* as
+0002d840: 2070 6f73 6974 696f 6e61 6c20 6172 6775   positional argu
+0002d850: 6d65 6e74 7320 286c 6f6f 6b20 6174 204f  ments (look at O
+0002d860: 7468 6572 2050 6172 616d 6574 6572 7320  ther Parameters 
+0002d870: 6265 6c6f 7720 666f 7220 610a 2020 2020  below for a.    
+0002d880: 2020 2020 2020 2020 2020 2020 6465 7461              deta
+0002d890: 696c 6564 2064 6573 6372 6970 7469 6f6e  iled description
+0002d8a0: 2920 616e 6420 7769 6c6c 2062 6520 6361  ) and will be ca
+0002d8b0: 6c6c 6564 2062 6163 6b20 6561 6368 2074  lled back each t
+0002d8c0: 696d 6520 6120 6e65 7720 6669 6c65 2063  ime a new file c
+0002d8d0: 6875 6e6b 2068 6173 2062 6565 6e20 7375  hunk has been su
+0002d8e0: 6363 6573 7366 756c 6c79 0a20 2020 2020  ccessfully.     
+0002d8f0: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
+0002d900: 6d69 7474 6564 2e0a 0a20 2020 2020 2020  mitted...       
+0002d910: 2020 2020 2070 726f 6772 6573 735f 6172       progress_ar
+0002d920: 6773 2028 6060 7475 706c 6560 602c 202a  gs (``tuple``, *
+0002d930: 6f70 7469 6f6e 616c 2a29 3a0a 2020 2020  optional*):.    
+0002d940: 2020 2020 2020 2020 2020 2020 4578 7472              Extr
+0002d950: 6120 6375 7374 6f6d 2061 7267 756d 656e  a custom argumen
+0002d960: 7473 2066 6f72 2074 6865 2070 726f 6772  ts for the progr
+0002d970: 6573 7320 6361 6c6c 6261 636b 2066 756e  ess callback fun
+0002d980: 6374 696f 6e2e 0a20 2020 2020 2020 2020  ction..         
+0002d990: 2020 2020 2020 2059 6f75 2063 616e 2070         You can p
+0002d9a0: 6173 7320 616e 7974 6869 6e67 2079 6f75  ass anything you
+0002d9b0: 206e 6565 6420 746f 2062 6520 6176 6169   need to be avai
+0002d9c0: 6c61 626c 6520 696e 2074 6865 2070 726f  lable in the pro
+0002d9d0: 6772 6573 7320 6361 6c6c 6261 636b 2073  gress callback s
+0002d9e0: 636f 7065 3b20 666f 7220 6578 616d 706c  cope; for exampl
+0002d9f0: 652c 2061 204d 6573 7361 6765 0a20 2020  e, a Message.   
+0002da00: 2020 2020 2020 2020 2020 2020 206f 626a               obj
+0002da10: 6563 7420 6f72 2061 2043 6c69 656e 7420  ect or a Client 
+0002da20: 696e 7374 616e 6365 2069 6e20 6f72 6465  instance in orde
+0002da30: 7220 746f 2065 6469 7420 7468 6520 6d65  r to edit the me
+0002da40: 7373 6167 6520 7769 7468 2074 6865 2075  ssage with the u
+0002da50: 7064 6174 6564 2070 726f 6772 6573 7320  pdated progress 
+0002da60: 7374 6174 7573 2e0a 0a20 2020 2020 2020  status...       
+0002da70: 204f 7468 6572 2050 6172 616d 6574 6572   Other Parameter
+0002da80: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+0002da90: 7572 7265 6e74 2028 6060 696e 7460 6029  urrent (``int``)
+0002daa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002dab0: 2020 5468 6520 616d 6f75 6e74 206f 6620    The amount of 
+0002dac0: 6279 7465 7320 7472 616e 736d 6974 7465  bytes transmitte
+0002dad0: 6420 736f 2066 6172 2e0a 0a20 2020 2020  d so far...     
+0002dae0: 2020 2020 2020 2074 6f74 616c 2028 6060         total (``
+0002daf0: 696e 7460 6029 3a0a 2020 2020 2020 2020  int``):.        
+0002db00: 2020 2020 2020 2020 5468 6520 746f 7461          The tota
+0002db10: 6c20 7369 7a65 206f 6620 7468 6520 6669  l size of the fi
+0002db20: 6c65 2e0a 0a20 2020 2020 2020 2020 2020  le...           
+0002db30: 202a 6172 6773 2028 6060 7475 706c 6560   *args (``tuple`
+0002db40: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
+0002db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002db60: 4578 7472 6120 6375 7374 6f6d 2061 7267  Extra custom arg
+0002db70: 756d 656e 7473 2061 7320 6465 6669 6e65  uments as define
+0002db80: 6420 696e 2074 6865 2060 6070 726f 6772  d in the ``progr
+0002db90: 6573 735f 6172 6773 6060 2070 6172 616d  ess_args`` param
+0002dba0: 6574 6572 2e0a 2020 2020 2020 2020 2020  eter..          
+0002dbb0: 2020 2020 2020 596f 7520 6361 6e20 6569        You can ei
+0002dbc0: 7468 6572 206b 6565 7020 6060 2a61 7267  ther keep ``*arg
+0002dbd0: 7360 6020 6f72 2061 6464 2065 7665 7279  s`` or add every
+0002dbe0: 2073 696e 676c 6520 6578 7472 6120 6172   single extra ar
+0002dbf0: 6775 6d65 6e74 2069 6e20 796f 7572 2066  gument in your f
+0002dc00: 756e 6374 696f 6e20 7369 676e 6174 7572  unction signatur
+0002dc10: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
+0002dc20: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0002dc30: 204f 6e20 7375 6363 6573 732c 2074 6865   On success, the
+0002dc40: 2061 6273 6f6c 7574 6520 7061 7468 206f   absolute path o
+0002dc50: 6620 7468 6520 646f 776e 6c6f 6164 6564  f the downloaded
+0002dc60: 2066 696c 6520 6173 2073 7472 696e 6720   file as string 
+0002dc70: 6973 2072 6574 7572 6e65 642c 204e 6f6e  is returned, Non
+0002dc80: 6520 6f74 6865 7277 6973 652e 0a0a 2020  e otherwise...  
+0002dc90: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
+0002dca0: 2020 2020 2020 2020 2020 5250 4345 7272            RPCErr
+0002dcb0: 6f72 3a20 496e 2063 6173 6520 6f66 2061  or: In case of a
+0002dcc0: 2054 656c 6567 7261 6d20 5250 4320 6572   Telegram RPC er
+0002dcd0: 726f 722e 0a20 2020 2020 2020 2020 2020  ror..           
+0002dce0: 2060 6056 616c 7565 4572 726f 7260 603a   ``ValueError``:
+0002dcf0: 2049 6620 7468 6520 6d65 7373 6167 6520   If the message 
+0002dd00: 646f 6573 6e27 7420 636f 6e74 6169 6e20  doesn't contain 
+0002dd10: 616e 7920 646f 776e 6c6f 6164 6162 6c65  any downloadable
+0002dd20: 206d 6564 6961 0a20 2020 2020 2020 2022   media.        "
+0002dd30: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0002dd40: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
+0002dd50: 6965 6e74 2e64 6f77 6e6c 6f61 645f 6d65  ient.download_me
+0002dd60: 6469 6128 0a20 2020 2020 2020 2020 2020  dia(.           
+0002dd70: 206d 6573 7361 6765 3d73 656c 662c 0a20   message=self,. 
+0002dd80: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+0002dd90: 6e61 6d65 3d66 696c 655f 6e61 6d65 2c0a  name=file_name,.
+0002dda0: 2020 2020 2020 2020 2020 2020 696e 5f6d              in_m
+0002ddb0: 656d 6f72 793d 696e 5f6d 656d 6f72 792c  emory=in_memory,
+0002ddc0: 0a20 2020 2020 2020 2020 2020 2062 6c6f  .            blo
+0002ddd0: 636b 3d62 6c6f 636b 2c0a 2020 2020 2020  ck=block,.      
+0002dde0: 2020 2020 2020 7072 6f67 7265 7373 3d70        progress=p
+0002ddf0: 726f 6772 6573 732c 0a20 2020 2020 2020  rogress,.       
+0002de00: 2020 2020 2070 726f 6772 6573 735f 6172       progress_ar
+0002de10: 6773 3d70 726f 6772 6573 735f 6172 6773  gs=progress_args
+0002de20: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+0002de30: 2061 7379 6e63 2064 6566 2076 6f74 6528   async def vote(
+0002de40: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0002de50: 2020 2020 2020 206f 7074 696f 6e3a 2069         option: i
+0002de60: 6e74 2c0a 2020 2020 2920 2d3e 2022 7479  nt,.    ) -> "ty
+0002de70: 7065 732e 506f 6c6c 223a 0a20 2020 2020  pes.Poll":.     
+0002de80: 2020 2022 2222 426f 756e 6420 6d65 7468     """Bound meth
+0002de90: 6f64 202a 766f 7465 2a20 6f66 203a 6f62  od *vote* of :ob
+0002dea0: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
+0002deb0: 6573 2e4d 6573 7361 6765 602e 0a0a 2020  es.Message`...  
+0002dec0: 2020 2020 2020 5573 6520 6173 2061 2073        Use as a s
+0002ded0: 686f 7274 6375 7420 666f 723a 0a0a 2020  hortcut for:..  
+0002dee0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
+0002def0: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
+0002df00: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+0002df10: 2e76 6f74 655f 706f 6c6c 280a 2020 2020  .vote_poll(.    
+0002df20: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+0002df30: 5f69 643d 6d65 7373 6167 652e 6368 6174  _id=message.chat
+0002df40: 2e69 642c 0a20 2020 2020 2020 2020 2020  .id,.           
+0002df50: 2020 2020 206d 6573 7361 6765 5f69 643d       message_id=
+0002df60: 6d65 7373 6167 652e 6964 2c0a 2020 2020  message.id,.    
+0002df70: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+0002df80: 6f6e 3d31 0a20 2020 2020 2020 2020 2020  on=1.           
+0002df90: 2029 0a0a 2020 2020 2020 2020 4578 616d   )..        Exam
+0002dfa0: 706c 653a 0a20 2020 2020 2020 2020 2020  ple:.           
+0002dfb0: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+0002dfc0: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+0002dfd0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+0002dfe0: 2e76 6f74 6528 3629 0a0a 2020 2020 2020  .vote(6)..      
+0002dff0: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
+0002e000: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
+0002e010: 2028 6060 696e 7460 6029 3a0a 2020 2020   (``int``):.    
+0002e020: 2020 2020 2020 2020 2020 2020 496e 6465              Inde
+0002e030: 7820 6f66 2074 6865 2070 6f6c 6c20 6f70  x of the poll op
+0002e040: 7469 6f6e 2079 6f75 2077 616e 7420 746f  tion you want to
+0002e050: 2076 6f74 6520 666f 7220 2830 2074 6f20   vote for (0 to 
+0002e060: 3929 2e0a 0a20 2020 2020 2020 2052 6574  9)...        Ret
+0002e070: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+0002e080: 2020 3a6f 626a 3a60 7e70 7972 6f67 7261    :obj:`~pyrogra
+0002e090: 6d2e 7479 7065 732e 506f 6c6c 603a 204f  m.types.Poll`: O
+0002e0a0: 6e20 7375 6363 6573 732c 2074 6865 2070  n success, the p
+0002e0b0: 6f6c 6c20 7769 7468 2074 6865 2063 686f  oll with the cho
+0002e0c0: 7365 6e20 6f70 7469 6f6e 2069 7320 7265  sen option is re
+0002e0d0: 7475 726e 6564 2e0a 0a20 2020 2020 2020  turned...       
+0002e0e0: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+0002e0f0: 2020 2020 2052 5043 4572 726f 723a 2049       RPCError: I
+0002e100: 6e20 6361 7365 206f 6620 6120 5465 6c65  n case of a Tele
+0002e110: 6772 616d 2052 5043 2065 7272 6f72 2e0a  gram RPC error..
+0002e120: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+0002e130: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+0002e140: 7420 7365 6c66 2e5f 636c 6965 6e74 2e76  t self._client.v
+0002e150: 6f74 655f 706f 6c6c 280a 2020 2020 2020  ote_poll(.      
+0002e160: 2020 2020 2020 6368 6174 5f69 643d 7365        chat_id=se
+0002e170: 6c66 2e63 6861 742e 6964 2c0a 2020 2020  lf.chat.id,.    
+0002e180: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
+0002e190: 6964 3d73 656c 662e 6964 2c0a 2020 2020  id=self.id,.    
+0002e1a0: 2020 2020 2020 2020 6f70 7469 6f6e 733d          options=
+0002e1b0: 6f70 7469 6f6e 0a20 2020 2020 2020 2029  option.        )
+0002e1c0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+0002e1d0: 7069 6e28 7365 6c66 2c20 6469 7361 626c  pin(self, disabl
+0002e1e0: 655f 6e6f 7469 6669 6361 7469 6f6e 3a20  e_notification: 
+0002e1f0: 626f 6f6c 203d 2046 616c 7365 2c20 626f  bool = False, bo
+0002e200: 7468 5f73 6964 6573 3a20 626f 6f6c 203d  th_sides: bool =
+0002e210: 2046 616c 7365 2920 2d3e 2022 7479 7065   False) -> "type
+0002e220: 732e 4d65 7373 6167 6522 3a0a 2020 2020  s.Message":.    
+0002e230: 2020 2020 2222 2242 6f75 6e64 206d 6574      """Bound met
+0002e240: 686f 6420 2a70 696e 2a20 6f66 203a 6f62  hod *pin* of :ob
+0002e250: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
+0002e260: 6573 2e4d 6573 7361 6765 602e 0a0a 2020  es.Message`...  
+0002e270: 2020 2020 2020 5573 6520 6173 2061 2073        Use as a s
+0002e280: 686f 7274 6375 7420 666f 723a 0a0a 2020  hortcut for:..  
+0002e290: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
+0002e2a0: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
+0002e2b0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+0002e2c0: 636c 6965 6e74 2e70 696e 5f63 6861 745f  client.pin_chat_
+0002e2d0: 6d65 7373 6167 6528 0a20 2020 2020 2020  message(.       
+0002e2e0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
+0002e2f0: 3d6d 6573 7361 6765 2e63 6861 742e 6964  =message.chat.id
+0002e300: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002e310: 2020 6d65 7373 6167 655f 6964 3d6d 6573    message_id=mes
+0002e320: 7361 6765 5f69 640a 2020 2020 2020 2020  sage_id.        
+0002e330: 2020 2020 290a 0a20 2020 2020 2020 2045      )..        E
+0002e340: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
+0002e350: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+0002e360: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
+0002e370: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+0002e380: 7420 6d65 7373 6167 652e 7069 6e28 290a  t message.pin().
+0002e390: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0002e3a0: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+0002e3b0: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
+0002e3c0: 6174 696f 6e20 2860 6062 6f6f 6c60 6029  ation (``bool``)
+0002e3d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002e3e0: 2020 5061 7373 2054 7275 652c 2069 6620    Pass True, if 
+0002e3f0: 6974 2069 7320 6e6f 7420 6e65 6365 7373  it is not necess
+0002e400: 6172 7920 746f 2073 656e 6420 6120 6e6f  ary to send a no
+0002e410: 7469 6669 6361 7469 6f6e 2074 6f20 616c  tification to al
+0002e420: 6c20 6368 6174 206d 656d 6265 7273 2061  l chat members a
+0002e430: 626f 7574 2074 6865 206e 6577 2070 696e  bout the new pin
+0002e440: 6e65 640a 2020 2020 2020 2020 2020 2020  ned.            
+0002e450: 2020 2020 6d65 7373 6167 652e 204e 6f74      message. Not
+0002e460: 6966 6963 6174 696f 6e73 2061 7265 2061  ifications are a
+0002e470: 6c77 6179 7320 6469 7361 626c 6564 2069  lways disabled i
+0002e480: 6e20 6368 616e 6e65 6c73 2e0a 0a20 2020  n channels...   
+0002e490: 2020 2020 2020 2020 2062 6f74 685f 7369           both_si
+0002e4a0: 6465 7320 2860 6062 6f6f 6c60 602c 202a  des (``bool``, *
+0002e4b0: 6f70 7469 6f6e 616c 2a29 3a0a 2020 2020  optional*):.    
+0002e4c0: 2020 2020 2020 2020 2020 2020 5061 7373              Pass
+0002e4d0: 2054 7275 6520 746f 2070 696e 2074 6865   True to pin the
+0002e4e0: 206d 6573 7361 6765 2066 6f72 2062 6f74   message for bot
+0002e4f0: 6820 7369 6465 7320 2879 6f75 2061 6e64  h sides (you and
+0002e500: 2072 6563 6970 6965 6e74 292e 0a20 2020   recipient)..   
+0002e510: 2020 2020 2020 2020 2020 2020 2041 7070               App
+0002e520: 6c69 6361 626c 6520 746f 2070 7269 7661  licable to priva
+0002e530: 7465 2063 6861 7473 206f 6e6c 792e 2044  te chats only. D
+0002e540: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
+0002e550: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0002e560: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0002e570: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
+0002e580: 7479 7065 732e 4d65 7373 6167 6560 3a20  types.Message`: 
+0002e590: 4f6e 2073 7563 6365 7373 2c20 7468 6520  On success, the 
+0002e5a0: 7365 7276 6963 6520 6d65 7373 6167 6520  service message 
+0002e5b0: 6973 2072 6574 7572 6e65 642e 0a0a 2020  is returned...  
+0002e5c0: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
+0002e5d0: 2020 2020 2020 2020 2020 5250 4345 7272            RPCErr
+0002e5e0: 6f72 3a20 496e 2063 6173 6520 6f66 2061  or: In case of a
+0002e5f0: 2054 656c 6567 7261 6d20 5250 4320 6572   Telegram RPC er
+0002e600: 726f 722e 0a20 2020 2020 2020 2022 2222  ror..        """
+0002e610: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002e620: 6177 6169 7420 7365 6c66 2e5f 636c 6965  await self._clie
+0002e630: 6e74 2e70 696e 5f63 6861 745f 6d65 7373  nt.pin_chat_mess
+0002e640: 6167 6528 0a20 2020 2020 2020 2020 2020  age(.           
+0002e650: 2063 6861 745f 6964 3d73 656c 662e 6368   chat_id=self.ch
+0002e660: 6174 2e69 642c 0a20 2020 2020 2020 2020  at.id,.         
+0002e670: 2020 206d 6573 7361 6765 5f69 643d 7365     message_id=se
+0002e680: 6c66 2e69 642c 0a20 2020 2020 2020 2020  lf.id,.         
+0002e690: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
+0002e6a0: 6963 6174 696f 6e3d 6469 7361 626c 655f  ication=disable_
+0002e6b0: 6e6f 7469 6669 6361 7469 6f6e 2c0a 2020  notification,.  
+0002e6c0: 2020 2020 2020 2020 2020 626f 7468 5f73            both_s
+0002e6d0: 6964 6573 3d62 6f74 685f 7369 6465 730a  ides=both_sides.
+0002e6e0: 2020 2020 2020 2020 290a 0a20 2020 2061          )..    a
+0002e6f0: 7379 6e63 2064 6566 2075 6e70 696e 2873  sync def unpin(s
+0002e700: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+0002e710: 2020 2020 2020 2222 2242 6f75 6e64 206d        """Bound m
+0002e720: 6574 686f 6420 2a75 6e70 696e 2a20 6f66  ethod *unpin* of
+0002e730: 203a 6f62 6a3a 607e 7079 726f 6772 616d   :obj:`~pyrogram
+0002e740: 2e74 7970 6573 2e4d 6573 7361 6765 602e  .types.Message`.
+0002e750: 0a0a 2020 2020 2020 2020 5573 6520 6173  ..        Use as
+0002e760: 2061 2073 686f 7274 6375 7420 666f 723a   a shortcut for:
+0002e770: 0a0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
+0002e780: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+0002e790: 0a0a 2020 2020 2020 2020 2020 2020 6177  ..            aw
+0002e7a0: 6169 7420 636c 6965 6e74 2e75 6e70 696e  ait client.unpin
+0002e7b0: 5f63 6861 745f 6d65 7373 6167 6528 0a20  _chat_message(. 
+0002e7c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0002e7d0: 6861 745f 6964 3d6d 6573 7361 6765 2e63  hat_id=message.c
+0002e7e0: 6861 742e 6964 2c0a 2020 2020 2020 2020  hat.id,.        
+0002e7f0: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
+0002e800: 6964 3d6d 6573 7361 6765 5f69 640a 2020  id=message_id.  
+0002e810: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0002e820: 2020 2020 2045 7861 6d70 6c65 3a0a 2020       Example:.  
+0002e830: 2020 2020 2020 2020 2020 2e2e 2063 6f64            .. cod
+0002e840: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+0002e850: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0002e860: 2020 6177 6169 7420 6d65 7373 6167 652e    await message.
+0002e870: 756e 7069 6e28 290a 0a20 2020 2020 2020  unpin()..       
+0002e880: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0002e890: 2020 2020 2020 5472 7565 206f 6e20 7375        True on su
+0002e8a0: 6363 6573 732e 0a0a 2020 2020 2020 2020  ccess...        
+0002e8b0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+0002e8c0: 2020 2020 5250 4345 7272 6f72 3a20 496e      RPCError: In
+0002e8d0: 2063 6173 6520 6f66 2061 2054 656c 6567   case of a Teleg
+0002e8e0: 7261 6d20 5250 4320 6572 726f 722e 0a20  ram RPC error.. 
+0002e8f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0002e900: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+0002e910: 7365 6c66 2e5f 636c 6965 6e74 2e75 6e70  self._client.unp
+0002e920: 696e 5f63 6861 745f 6d65 7373 6167 6528  in_chat_message(
+0002e930: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+0002e940: 745f 6964 3d73 656c 662e 6368 6174 2e69  t_id=self.chat.i
+0002e950: 642c 0a20 2020 2020 2020 2020 2020 206d  d,.            m
+0002e960: 6573 7361 6765 5f69 643d 7365 6c66 2e69  essage_id=self.i
+0002e970: 640a 2020 2020 2020 2020 290a 0a20 2020  d.        )..   
+0002e980: 2023 2042 4547 494e 3a20 7468 6520 6265   # BEGIN: the be
+0002e990: 6c6f 7720 7072 6f70 6572 7469 6573 2077  low properties w
+0002e9a0: 6572 6520 7265 6d6f 7665 6420 696e 2060  ere removed in `
+0002e9b0: 424f 5420 4150 4920 372e 3020 3c68 7474  BOT API 7.0 <htt
+0002e9c0: 7073 3a2f 2f63 6f72 652e 7465 6c65 6772  ps://core.telegr
+0002e9d0: 616d 2e6f 7267 2f62 6f74 732f 6170 692d  am.org/bots/api-
+0002e9e0: 6368 616e 6765 6c6f 6723 6465 6365 6d62  changelog#decemb
+0002e9f0: 6572 2d32 392d 3230 3233 3e60 5f0a 0a20  er-29-2023>`_.. 
+0002ea00: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0002ea10: 2064 6566 2066 6f72 7761 7264 5f66 726f   def forward_fro
+0002ea20: 6d28 7365 6c66 2920 2d3e 2022 7479 7065  m(self) -> "type
+0002ea30: 732e 5573 6572 223a 0a20 2020 2020 2020  s.User":.       
+0002ea40: 206c 6f67 2e77 6172 6e69 6e67 280a 2020   log.warning(.  
+0002ea50: 2020 2020 2020 2020 2020 2254 6869 7320            "This 
+0002ea60: 7072 6f70 6572 7479 2069 7320 6465 7072  property is depr
+0002ea70: 6563 6174 6564 2e20 220a 2020 2020 2020  ecated. ".      
+0002ea80: 2020 2020 2020 2250 6c65 6173 6520 7573        "Please us
+0002ea90: 6520 666f 7277 6172 645f 6f72 6967 696e  e forward_origin
+0002eaa0: 2069 6e73 7465 6164 220a 2020 2020 2020   instead".      
+0002eab0: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+0002eac0: 726e 2067 6574 6174 7472 2873 656c 662e  rn getattr(self.
+0002ead0: 666f 7277 6172 645f 6f72 6967 696e 2c20  forward_origin, 
+0002eae0: 2273 656e 6465 725f 7573 6572 222c 204e  "sender_user", N
+0002eaf0: 6f6e 6529 0a20 2020 200a 2020 2020 4070  one).    .    @p
+0002eb00: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0002eb10: 666f 7277 6172 645f 7365 6e64 6572 5f6e  forward_sender_n
+0002eb20: 616d 6528 7365 6c66 2920 2d3e 2073 7472  ame(self) -> str
+0002eb30: 3a0a 2020 2020 2020 2020 6c6f 672e 7761  :.        log.wa
+0002eb40: 726e 696e 6728 0a20 2020 2020 2020 2020  rning(.         
+0002eb50: 2020 2022 5468 6973 2070 726f 7065 7274     "This propert
+0002eb60: 7920 6973 2064 6570 7265 6361 7465 642e  y is deprecated.
+0002eb70: 2022 0a20 2020 2020 2020 2020 2020 2022   ".            "
+0002eb80: 506c 6561 7365 2075 7365 2066 6f72 7761  Please use forwa
+0002eb90: 7264 5f6f 7269 6769 6e20 696e 7374 6561  rd_origin instea
+0002eba0: 6422 0a20 2020 2020 2020 2029 0a20 2020  d".        ).   
+0002ebb0: 2020 2020 2072 6574 7572 6e20 6765 7461       return geta
+0002ebc0: 7474 7228 7365 6c66 2e66 6f72 7761 7264  ttr(self.forward
+0002ebd0: 5f6f 7269 6769 6e2c 2022 7365 6e64 6572  _origin, "sender
+0002ebe0: 5f75 7365 725f 6e61 6d65 222c 204e 6f6e  _user_name", Non
+0002ebf0: 6529 0a0a 2020 2020 4070 726f 7065 7274  e)..    @propert
+0002ec00: 790a 2020 2020 6465 6620 666f 7277 6172  y.    def forwar
+0002ec10: 645f 6672 6f6d 5f63 6861 7428 7365 6c66  d_from_chat(self
+0002ec20: 2920 2d3e 2022 7479 7065 732e 4368 6174  ) -> "types.Chat
+0002ec30: 223a 0a20 2020 2020 2020 206c 6f67 2e77  ":.        log.w
+0002ec40: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
+0002ec50: 2020 2020 2254 6869 7320 7072 6f70 6572      "This proper
+0002ec60: 7479 2069 7320 6465 7072 6563 6174 6564  ty is deprecated
+0002ec70: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
+0002ec80: 2250 6c65 6173 6520 7573 6520 666f 7277  "Please use forw
+0002ec90: 6172 645f 6f72 6967 696e 2069 6e73 7465  ard_origin inste
+0002eca0: 6164 220a 2020 2020 2020 2020 290a 2020  ad".        ).  
+0002ecb0: 2020 2020 2020 7265 7475 726e 2067 6574        return get
+0002ecc0: 6174 7472 280a 2020 2020 2020 2020 2020  attr(.          
+0002ecd0: 2020 7365 6c66 2e66 6f72 7761 7264 5f6f    self.forward_o
+0002ece0: 7269 6769 6e2c 0a20 2020 2020 2020 2020  rigin,.         
+0002ecf0: 2020 2022 6368 6174 222c 0a20 2020 2020     "chat",.     
+0002ed00: 2020 2020 2020 2067 6574 6174 7472 280a         getattr(.
+0002ed10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ed20: 7365 6c66 2e66 6f72 7761 7264 5f6f 7269  self.forward_ori
+0002ed30: 6769 6e2c 0a20 2020 2020 2020 2020 2020  gin,.           
+0002ed40: 2020 2020 2022 7365 6e64 6572 5f63 6861       "sender_cha
+0002ed50: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+0002ed60: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
+0002ed70: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
+0002ed80: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0002ed90: 2020 2020 6465 6620 666f 7277 6172 645f      def forward_
+0002eda0: 6672 6f6d 5f6d 6573 7361 6765 5f69 6428  from_message_id(
+0002edb0: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
+0002edc0: 2020 2020 2020 6c6f 672e 7761 726e 696e        log.warnin
+0002edd0: 6728 0a20 2020 2020 2020 2020 2020 2022  g(.            "
+0002ede0: 5468 6973 2070 726f 7065 7274 7920 6973  This property is
+0002edf0: 2064 6570 7265 6361 7465 642e 2022 0a20   deprecated. ". 
+0002ee00: 2020 2020 2020 2020 2020 2022 506c 6561             "Plea
+0002ee10: 7365 2075 7365 2066 6f72 7761 7264 5f6f  se use forward_o
+0002ee20: 7269 6769 6e20 696e 7374 6561 6422 0a20  rigin instead". 
+0002ee30: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0002ee40: 2072 6574 7572 6e20 6765 7461 7474 7228   return getattr(
+0002ee50: 7365 6c66 2e66 6f72 7761 7264 5f6f 7269  self.forward_ori
+0002ee60: 6769 6e2c 2022 6d65 7373 6167 655f 6964  gin, "message_id
+0002ee70: 222c 204e 6f6e 6529 0a0a 2020 2020 4070  ", None)..    @p
+0002ee80: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0002ee90: 666f 7277 6172 645f 7369 676e 6174 7572  forward_signatur
+0002eea0: 6528 7365 6c66 2920 2d3e 2073 7472 3a0a  e(self) -> str:.
+0002eeb0: 2020 2020 2020 2020 6c6f 672e 7761 726e          log.warn
+0002eec0: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+0002eed0: 2022 5468 6973 2070 726f 7065 7274 7920   "This property 
+0002eee0: 6973 2064 6570 7265 6361 7465 642e 2022  is deprecated. "
+0002eef0: 0a20 2020 2020 2020 2020 2020 2022 506c  .            "Pl
+0002ef00: 6561 7365 2075 7365 2066 6f72 7761 7264  ease use forward
+0002ef10: 5f6f 7269 6769 6e20 696e 7374 6561 6422  _origin instead"
+0002ef20: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0002ef30: 2020 2072 6574 7572 6e20 6765 7461 7474     return getatt
+0002ef40: 7228 7365 6c66 2e66 6f72 7761 7264 5f6f  r(self.forward_o
+0002ef50: 7269 6769 6e2c 2022 6175 7468 6f72 5f73  rigin, "author_s
+0002ef60: 6967 6e61 7475 7265 222c 204e 6f6e 6529  ignature", None)
+0002ef70: 0a20 2020 2020 2020 200a 2020 2020 4070  .        .    @p
+0002ef80: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0002ef90: 666f 7277 6172 645f 6461 7465 2873 656c  forward_date(sel
+0002efa0: 6629 202d 3e20 6461 7465 7469 6d65 3a0a  f) -> datetime:.
+0002efb0: 2020 2020 2020 2020 6c6f 672e 7761 726e          log.warn
+0002efc0: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+0002efd0: 2022 5468 6973 2070 726f 7065 7274 7920   "This property 
+0002efe0: 6973 2064 6570 7265 6361 7465 642e 2022  is deprecated. "
+0002eff0: 0a20 2020 2020 2020 2020 2020 2022 506c  .            "Pl
+0002f000: 6561 7365 2075 7365 2066 6f72 7761 7264  ease use forward
+0002f010: 5f6f 7269 6769 6e20 696e 7374 6561 6422  _origin instead"
+0002f020: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0002f030: 2020 2072 6574 7572 6e20 7365 6c66 2e66     return self.f
+0002f040: 6f72 7761 7264 5f6f 7269 6769 6e2e 6461  orward_origin.da
+0002f050: 7465 0a0a 2020 2020 2320 454e 443a 2074  te..    # END: t
+0002f060: 6865 2062 656c 6f77 2070 726f 7065 7274  he below propert
+0002f070: 6965 7320 7765 7265 2072 656d 6f76 6564  ies were removed
+0002f080: 2069 6e20 6042 4f54 2041 5049 2037 2e30   in `BOT API 7.0
+0002f090: 203c 6874 7470 733a 2f2f 636f 7265 2e74   <https://core.t
+0002f0a0: 656c 6567 7261 6d2e 6f72 672f 626f 7473  elegram.org/bots
+0002f0b0: 2f61 7069 2d63 6861 6e67 656c 6f67 2364  /api-changelog#d
+0002f0c0: 6563 656d 6265 722d 3239 2d32 3032 333e  ecember-29-2023>
+0002f0d0: 605f 0a                                  `_.
```

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/message_entity.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/message_reaction_count_updated.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/message_reaction_updated.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/message_reactions.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/photo.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/poll.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/poll.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from typing import List, Union, Optional
 
 import pyrogram
 from pyrogram import raw, enums, utils
 from pyrogram import types
 from ..object import Object
 from ..update import Update
+from .message import Str
 
 
 class Poll(Object, Update):
     """A Poll.
 
     Parameters:
         id (``str``):
@@ -133,24 +134,24 @@
                     chosen_option_id = i
 
                 if result.correct:
                     correct_option_id = i
 
             options.append(
                 types.PollOption(
-                    text=answer.text,
+                    text=Str(answer.text.text).init(answer.text.entities),
                     voter_count=voter_count,
                     data=answer.option,
                     client=client
                 )
             )
 
         return Poll(
             id=str(poll.id),
-            question=poll.question,
+            question=Str(poll.question.text).init(poll.question.entities),
             options=options,
             total_voter_count=media_poll.results.total_voters,
             is_closed=poll.closed,
             is_anonymous=not poll.public_voters,
             type=enums.PollType.QUIZ if poll.quiz else enums.PollType.REGULAR,
             allows_multiple_answers=poll.multiple_choice,
             chosen_option_id=chosen_option_id,
```

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/poll_option.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/reaction.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/sticker.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/story.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/story.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/thumbnail.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/venue.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/video.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/video_note.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/voice.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/web_app_data.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/messages_and_media/web_page.py` & `pyrotgfork-2.1.26/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/__init__.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/birthdate.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/birthdate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
         return Chat(
             id=peer_id,
             type=enums.ChatType.GROUP,
             title=chat.title,
             is_creator=getattr(chat, "creator", None),
             photo=types.ChatPhoto._parse(client, getattr(chat, "photo", None), peer_id, 0),
             permissions=types.ChatPermissions._parse(getattr(chat, "default_banned_rights", None)),
-            members_count=getattr(chat, "participants_count", None),
+            members_count=getattr(chat, "participants_count", 0),
             dc_id=getattr(getattr(chat, "photo", None), "dc_id", None),
             has_protected_content=getattr(chat, "noforwards", None),
             client=client,
             _raw=chat
         )
 
     @staticmethod
@@ -432,15 +432,15 @@
             restrictions=types.List(
                 [
                     types.Restriction._parse(r)
                     for r in getattr(channel, "restriction_reason", None)
                 ]
             ) or None,
             permissions=types.ChatPermissions._parse(getattr(channel, "default_banned_rights", None)),
-            members_count=getattr(channel, "participants_count", None),
+            members_count=getattr(channel, "participants_count", 0),
             dc_id=getattr(getattr(channel, "photo", None), "dc_id", None),
             has_protected_content=getattr(channel, "noforwards", None),
             is_forum=getattr(channel, "forum", None),
             client=client,
             active_usernames=active_usernames,
             accent_color=types.ChatColor._parse(getattr(channel, "color", None)),
             profile_color=types.ChatColor._parse_profile_color(getattr(channel, "profile_color", None)),
@@ -566,15 +566,15 @@
                     if isinstance(default_send_as, raw.types.PeerUser):
                         send_as_raw = users[default_send_as.user_id]
                     else:
                         send_as_raw = chats[default_send_as.channel_id]
 
                     parsed_chat.send_as_chat = Chat._parse_chat(client, send_as_raw)
 
-                parsed_chat.members_count = getattr(full_chat, "participants_count")                
+                parsed_chat.members_count = getattr(full_chat, "participants_count", 0)                
                 parsed_chat.has_visible_history = not getattr(full_chat, "hidden_prehistory", False)
                 parsed_chat.has_hidden_members = not getattr(full_chat, "participants_hidden", True)
                 parsed_chat.has_aggressive_anti_spam_enabled = getattr(full_chat, "antispam", False)
 
                 parsed_chat.slow_mode_delay = getattr(full_chat, "slowmode_seconds")
                 parsed_chat.slowmode_next_send_date = utils.timestamp_to_datetime(
                     getattr(full_chat, "slowmode_next_send_date")
```

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_color.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_event.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_event_filter.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_invite_link.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_join_request.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_joiner.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_member.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_member_updated.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_permissions.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_photo.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_privileges.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_reactions.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/chat_shared.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/chat_shared.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/dialog.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/emoji_status.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/invite_link_importer.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/restriction.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/user.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/username.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/users_shared.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/users_shared.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/video_chat_ended.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/video_chat_participants_invited.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/video_chat_participants_invited.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyrogram/types/user_and_chats/video_chat_started.py` & `pyrotgfork-2.1.26/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/.gitignore` & `pyrotgfork-2.1.26/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/COPYING` & `pyrotgfork-2.1.26/COPYING`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/COPYING.lesser` & `pyrotgfork-2.1.26/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/NOTICE` & `pyrotgfork-2.1.26/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/README.md` & `pyrotgfork-2.1.26/README.md`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/hatch_build.py` & `pyrotgfork-2.1.26/hatch_build.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.25/pyproject.toml` & `pyrotgfork-2.1.26/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,18 @@
 allow-direct-references = true
 
 [tool.hatch.build]
 include = ["pyrogram/py.typed"]
 exclude = ["tests", "docs", "requirements.lock", "requirements-dev.lock", ".github", ".gitignore"]
 
 [tool.hatch.build.targets.sdist]
-include = ["pyrogram"]
+include = [
+    "compiler",
+    "pyrogram",
+]
 exclude = [
     ".github/",
     "docs/",
     "tests/",
     ".editorconfig",
     ".gitignore",
     ".pre-commit-config.yaml",
```

### Comparing `pyrotgfork-2.1.25/PKG-INFO` & `pyrotgfork-2.1.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyrotgfork
-Version: 2.1.25
+Version: 2.1.26
 Summary: Fork of Pyrogram. Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Project-URL: Homepage, https://telegramplayground.github.io/pyrogram/releases/
 Project-URL: Tracker, https://github.com/TelegramPlayGround/Pyrogram/issues
 Project-URL: Community, https://t.me/PyroTGFork
 Project-URL: Source, https://github.com/TelegramPlayGround/Pyrogram
 Project-URL: Documentation, https://telegramplayground.github.io/pyrogram/
 Author-email: SpEcHIDe <pyrogram@iamidiotareyoutoo.com>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: pyrotgfork Version: 2.1.25 Summary: Fork of
+Metadata-Version: 2.3 Name: pyrotgfork Version: 2.1.26 Summary: Fork of
 Pyrogram. Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Project-URL: Homepage, https://
 telegramplayground.github.io/pyrogram/releases/ Project-URL: Tracker, https://
 github.com/TelegramPlayGround/Pyrogram/issues Project-URL: Community, https://
 t.me/PyroTGFork Project-URL: Source, https://github.com/TelegramPlayGround/
 Pyrogram Project-URL: Documentation, https://telegramplayground.github.io/
 pyrogram/ Author-email: SpEcHIDe
```

