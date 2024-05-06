# Comparing `tmp/pyrotgfork-2.1.29.tar.gz` & `tmp/pyrotgfork-2.1.30.tar.gz`

## Comparing `pyrotgfork-2.1.29.tar` & `pyrotgfork-2.1.30.tar`

### file list

```diff
@@ -1,506 +1,507 @@
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/__init__.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/api/__init__.py
--rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/api/compiler.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/api/source/auth_key.tl
--rw-r--r--   0        0        0   208081 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/api/source/main_api.tl
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/api/source/sys_msgs.tl
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/api/template/combinator.txt
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/api/template/type.txt
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/__init__.py
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/compiler.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/sort.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0        0        0    34482 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/template/class.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/compiler/errors/template/sub_class.txt
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/__init__.py
--rw-r--r--   0        0        0    46382 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/client.py
--rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/dispatcher.py
--rw-r--r--   0        0        0   208021 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/emoji.py
--rw-r--r--   0        0        0    16314 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/file_id.py
--rw-r--r--   0        0        0    28542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/filters.py
--rw-r--r--   0        0        0    61915 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/mime_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/py.typed
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/sync.py
--rw-r--r--   0        0        0    17454 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/utils.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/connection/__init__.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/connection/connection.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/connection/transport/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/crypto/__init__.py
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/crypto/aes.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/crypto/mtproto.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/crypto/prime.py
--rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/crypto/rsa.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/accent_color.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/auto_name.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/chat_action.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/chat_event_action.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/chat_member_status.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/chat_type.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/client_platform.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/message_entity_type.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/message_media_type.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/message_service_type.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/messages_filter.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/next_code_type.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/parse_mode.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/poll_type.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/profile_color.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/sent_code_type.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/enums/user_status.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/errors/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/errors/rpc_error.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/__init__.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/handler.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/message_handler.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/message_reaction_count_updated_handler.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/message_reaction_updated_handler.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/poll_handler.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/handlers/user_status_handler.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/__init__.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/advanced/save_file.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/check_password.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/connect.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/initialize.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/log_out.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/send_code.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/auth/terminate.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/__init__.py
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/get_bot_info_description.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/get_bot_info_short_description.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/get_bot_name.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/send_game.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/set_bot_info_description.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/set_bot_info_short_description.py
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/set_bot_name.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/bots/set_game_score.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/business/__init__.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/business/get_business_connection.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/business/get_collectible_item_info.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chat_topics/__init__.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chat_topics/close_forum_topic.py
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chat_topics/create_forum_topic.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chat_topics/delete_forum_topic.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chat_topics/edit_forum_topic.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chat_topics/get_forum_topic.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chat_topics/get_forum_topics.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chat_topics/hide_forum_topic.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chat_topics/reopen_forum_topic.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chat_topics/unhide_forum_topic.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/__init__.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/create_group.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/get_created_chats.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/search_chats.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_ttl.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/chats/unpin_chat_message.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/contacts/import_contacts.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_message_reaction_count_updated.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_message_reaction_updated.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/decorators/on_user_status.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/invite_links/revoke_chat_invite_link.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/__init__.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/download_media.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/edit_cached_media.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/search_global.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_document.py
--rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_location.py
--rw-r--r--   0        0        0    22833 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_message.py
--rw-r--r--   0        0        0    12533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0        0        0    15141 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_video.py
--rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/set_reaction.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/messages/vote_poll.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/password/__init__.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/password/remove_cloud_password.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/stickers/get_stickers.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/__init__.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/block_user.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/get_me.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/get_users.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/set_birthdate.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/set_personal_chat.py
--rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/set_username.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/users/update_profile.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/utilities/compose.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/utilities/idle.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/utilities/restart.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/utilities/run.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/utilities/start.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/utilities/stop.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/parser/__init__.py
--rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/parser/html.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/parser/markdown.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/parser/parser.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/parser/utils.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/__init__.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/__init__.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/future_salt.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/future_salts.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/list.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/message.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/msg_container.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/tl_object.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/session/__init__.py
--rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/session/auth.py
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/session/session.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/session/internals/__init__.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/session/internals/data_center.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/session/internals/msg_id.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/session/internals/seq_no.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/storage/__init__.py
--rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/storage/aio_sqlite_storage.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/storage/file_storage.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/storage/memory_storage.py
--rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/storage/storage.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/list.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/object.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/update.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/authorization/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/authorization/terms_of_service.py
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0        0        0    14613 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/web_app_info.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/business/__init__.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/business/business_connection.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/business/business_intro.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/business/business_location.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/business/business_opening_hours.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/business/business_opening_hours_interval.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/business/collectible_item_info.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/chat_topics/__init__.py
--rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/chat_topics/forum_topic.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/chat_topics/forum_topic_closed.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/chat_topics/forum_topic_created.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/chat_topics/forum_topic_edited.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/chat_topics/forum_topic_reopened.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/chat_topics/general_forum_topic_hidden.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/chat_topics/general_forum_topic_unhidden.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_voice.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_media/__init__.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_media/input_media.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_media/input_phone_contact.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_media/link_preview_options.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0        0        0    13513 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_message_content/external_reply_info.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_message_content/reply_parameters.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/input_message_content/text_quote.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/message_origin/__init__.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/message_origin/message_import_info.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/message_origin/message_origin.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/message_origin/message_origin_channel.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/message_origin/message_origin_chat.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/message_origin/message_origin_hidden_user.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/message_origin/message_origin_user.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/chat_boost_added.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/gift_code.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/gifted_premium.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/giveaway.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/giveaway_completed.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/giveaway_winners.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0        0        0   194811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/message_reaction_count_updated.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/message_reaction_updated.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/story.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/birthdate.py
--rw-r--r--   0        0        0    47270 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_color.py
--rw-r--r--   0        0        0    19921 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_shared.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0        0        0    18749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/users_shared.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/video_chat_participants_invited.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/COPYING
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/COPYING.lesser
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/NOTICE
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/README.md
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/hatch_build.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/pyproject.toml
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 pyrotgfork-2.1.29/PKG-INFO
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/__init__.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/__init__.py
+-rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/compiler.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/source/auth_key.tl
+-rw-r--r--   0        0        0   208169 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/source/main_api.tl
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/source/sys_msgs.tl
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/template/combinator.txt
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/template/type.txt
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/__init__.py
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/compiler.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/sort.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0        0        0    34482 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/template/class.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/template/sub_class.txt
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/__init__.py
+-rw-r--r--   0        0        0    46382 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/client.py
+-rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/dispatcher.py
+-rw-r--r--   0        0        0   208021 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/emoji.py
+-rw-r--r--   0        0        0    16314 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/file_id.py
+-rw-r--r--   0        0        0    28542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/filters.py
+-rw-r--r--   0        0        0    61915 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/mime_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/py.typed
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/sync.py
+-rw-r--r--   0        0        0    17454 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/utils.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/__init__.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/connection.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/crypto/__init__.py
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/crypto/aes.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/crypto/mtproto.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/crypto/prime.py
+-rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/crypto/rsa.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/accent_color.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/auto_name.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/chat_action.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/chat_type.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/client_platform.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/message_media_type.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/message_service_type.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/messages_filter.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/next_code_type.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/parse_mode.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/poll_type.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/profile_color.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/user_status.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/errors/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/errors/rpc_error.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/__init__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/handler.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/message_handler.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/message_reaction_count_updated_handler.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/message_reaction_updated_handler.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/user_status_handler.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/__init__.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/advanced/save_file.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/connect.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/terminate.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_info_description.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_info_short_description.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_name.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_info_description.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_info_short_description.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_name.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_game_score.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/business/__init__.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/business/get_business_connection.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/business/get_collectible_item_info.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/__init__.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/close_forum_topic.py
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/create_forum_topic.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/delete_forum_topic.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/edit_forum_topic.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/get_forum_topic.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/get_forum_topics.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/hide_forum_topic.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/reopen_forum_topic.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/unhide_forum_topic.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_created_chats.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/search_chats.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_ttl.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/unpin_chat_message.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/contacts/import_contacts.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_message_reaction_count_updated.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_message_reaction_updated.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_user_status.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_cached_media.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0        0        0    22833 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0        0        0    12533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0        0        0    15141 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/set_reaction.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/vote_poll.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/password/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/password/remove_cloud_password.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/stickers/get_stickers.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/__init__.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/block_user.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/get_me.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/get_users.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/set_birthdate.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/set_personal_chat.py
+-rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/set_username.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/update_profile.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/run.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/start.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/parser/__init__.py
+-rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/parser/html.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/parser/markdown.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/parser/parser.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/parser/utils.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/__init__.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/__init__.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/list.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/message.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/msg_container.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/tl_object.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/__init__.py
+-rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/auth.py
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/session.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/internals/__init__.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/internals/data_center.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/storage/__init__.py
+-rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/storage/aio_sqlite_storage.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/storage/file_storage.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/storage/memory_storage.py
+-rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/storage/storage.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/list.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/object.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/update.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/authorization/terms_of_service.py
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0        0        0    14613 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/web_app_info.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/__init__.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/business_connection.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/business_intro.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/business_location.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/business_opening_hours.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/business_opening_hours_interval.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/collectible_item_info.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/__init__.py
+-rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_closed.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_created.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_edited.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_reopened.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/general_forum_topic_hidden.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/general_forum_topic_unhidden.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_voice.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_phone_contact.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/link_preview_options.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0        0        0    13513 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/external_reply_info.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/input_poll_option.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/reply_parameters.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/text_quote.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/message_import_info.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_channel.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_chat.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_hidden_user.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_user.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/chat_boost_added.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/gift_code.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/gifted_premium.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/giveaway.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/giveaway_completed.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/giveaway_winners.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0        0        0   194829 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_reaction_count_updated.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_reaction_updated.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/story.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/birthdate.py
+-rw-r--r--   0        0        0    47521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_color.py
+-rw-r--r--   0        0        0    19921 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_shared.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0        0        0    18749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/users_shared.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_participants_invited.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/COPYING
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/COPYING.lesser
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/NOTICE
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/README.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/hatch_build.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyproject.toml
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/PKG-INFO
```

### Comparing `pyrotgfork-2.1.29/compiler/__init__.py` & `pyrotgfork-2.1.30/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/api/__init__.py` & `pyrotgfork-2.1.30/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/api/compiler.py` & `pyrotgfork-2.1.30/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/api/source/auth_key.tl` & `pyrotgfork-2.1.30/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/api/source/main_api.tl` & `pyrotgfork-2.1.30/compiler/api/source/main_api.tl`

 * *Files 1% similar despite different names*

```diff
@@ -432,14 +432,15 @@
 updateQuickReplyMessage#3e050d0f message:Message = Update;
 updateDeleteQuickReplyMessages#566fe7cd shortcut_id:int messages:Vector<int> = Update;
 updateBotBusinessConnect#8ae5c97a connection:BotBusinessConnection qts:int = Update;
 updateBotNewBusinessMessage#9ddb347c flags:# connection_id:string message:Message reply_to_message:flags.0?Message qts:int = Update;
 updateBotEditBusinessMessage#7df587c flags:# connection_id:string message:Message reply_to_message:flags.0?Message qts:int = Update;
 updateBotDeleteBusinessMessage#a02a982e connection_id:string peer:Peer messages:Vector<int> qts:int = Update;
 updateNewStoryReaction#1824e40b story_id:int peer:Peer reaction:Reaction = Update;
+updateBroadcastRevenueTransactions#5c65d358 balances:BroadcastRevenueBalances = Update;
 
 updates.state#a56c2a3e pts:int qts:int date:int seq:int unread_count:int = updates.State;
 
 updates.differenceEmpty#5d75a138 date:int seq:int = updates.Difference;
 updates.difference#f49ca0 new_messages:Vector<Message> new_encrypted_messages:Vector<EncryptedMessage> other_updates:Vector<Update> chats:Vector<Chat> users:Vector<User> state:updates.State = updates.Difference;
 updates.differenceSlice#a8fb1981 new_messages:Vector<Message> new_encrypted_messages:Vector<EncryptedMessage> other_updates:Vector<Update> chats:Vector<Chat> users:Vector<User> intermediate_state:updates.State = updates.Difference;
 updates.differenceTooLong#4afe8f6d pts:int = updates.Difference;
```

### Comparing `pyrotgfork-2.1.29/compiler/api/source/sys_msgs.tl` & `pyrotgfork-2.1.30/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/api/template/combinator.txt` & `pyrotgfork-2.1.30/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/api/template/type.txt` & `pyrotgfork-2.1.30/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/errors/__init__.py` & `pyrotgfork-2.1.30/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/errors/compiler.py` & `pyrotgfork-2.1.30/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/errors/sort.py` & `pyrotgfork-2.1.30/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/errors/source/400_BAD_REQUEST.tsv` & `pyrotgfork-2.1.30/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/errors/source/401_UNAUTHORIZED.tsv` & `pyrotgfork-2.1.30/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/errors/source/403_FORBIDDEN.tsv` & `pyrotgfork-2.1.30/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `pyrotgfork-2.1.30/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/errors/source/420_FLOOD.tsv` & `pyrotgfork-2.1.30/compiler/errors/source/420_FLOOD.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `pyrotgfork-2.1.30/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/__init__.py` & `pyrotgfork-2.1.30/pyrogram/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "pyrotgfork"
-__version__ = "2.1.29"
+__version__ = "2.1.30"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `pyrotgfork-2.1.29/pyrogram/client.py` & `pyrotgfork-2.1.30/pyrogram/client.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/dispatcher.py` & `pyrotgfork-2.1.30/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/emoji.py` & `pyrotgfork-2.1.30/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/file_id.py` & `pyrotgfork-2.1.30/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/filters.py` & `pyrotgfork-2.1.30/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/mime_types.py` & `pyrotgfork-2.1.30/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/sync.py` & `pyrotgfork-2.1.30/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/utils.py` & `pyrotgfork-2.1.30/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/connection/__init__.py` & `pyrotgfork-2.1.30/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/connection/connection.py` & `pyrotgfork-2.1.30/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/connection/transport/__init__.py` & `pyrotgfork-2.1.30/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/__init__.py` & `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/tcp.py` & `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/tcp_abridged.py` & `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/tcp_full.py` & `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/crypto/__init__.py` & `pyrotgfork-2.1.30/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/crypto/aes.py` & `pyrotgfork-2.1.30/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/crypto/mtproto.py` & `pyrotgfork-2.1.30/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/crypto/prime.py` & `pyrotgfork-2.1.30/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/crypto/rsa.py` & `pyrotgfork-2.1.30/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/__init__.py` & `pyrotgfork-2.1.30/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/accent_color.py` & `pyrotgfork-2.1.30/pyrogram/enums/accent_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/auto_name.py` & `pyrotgfork-2.1.30/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/chat_action.py` & `pyrotgfork-2.1.30/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/chat_event_action.py` & `pyrotgfork-2.1.30/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/chat_member_status.py` & `pyrotgfork-2.1.30/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/chat_members_filter.py` & `pyrotgfork-2.1.30/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/chat_type.py` & `pyrotgfork-2.1.30/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/client_platform.py` & `pyrotgfork-2.1.30/pyrogram/enums/client_platform.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/message_entity_type.py` & `pyrotgfork-2.1.30/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/message_media_type.py` & `pyrotgfork-2.1.30/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/message_service_type.py` & `pyrotgfork-2.1.30/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/messages_filter.py` & `pyrotgfork-2.1.30/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/next_code_type.py` & `pyrotgfork-2.1.30/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/parse_mode.py` & `pyrotgfork-2.1.30/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/poll_type.py` & `pyrotgfork-2.1.30/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/profile_color.py` & `pyrotgfork-2.1.30/pyrogram/enums/profile_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/sent_code_type.py` & `pyrotgfork-2.1.30/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/enums/user_status.py` & `pyrotgfork-2.1.30/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/errors/__init__.py` & `pyrotgfork-2.1.30/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/errors/rpc_error.py` & `pyrotgfork-2.1.30/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/__init__.py` & `pyrotgfork-2.1.30/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/callback_query_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/chat_join_request_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/chat_member_updated_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/chosen_inline_result_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/deleted_messages_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/disconnect_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/edited_message_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/inline_query_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/message_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/message_reaction_count_updated_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/message_reaction_count_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/message_reaction_updated_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/message_reaction_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/poll_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/raw_update_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/handlers/user_status_handler.py` & `pyrotgfork-2.1.30/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/advanced/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/advanced/invoke.py` & `pyrotgfork-2.1.30/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/advanced/resolve_peer.py` & `pyrotgfork-2.1.30/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/advanced/save_file.py` & `pyrotgfork-2.1.30/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/accept_terms_of_service.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/check_password.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/connect.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/disconnect.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/get_password_hint.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/initialize.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/log_out.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/recover_password.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/resend_code.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/send_code.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/send_recovery_code.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/sign_in.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/sign_in_bot.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/sign_up.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/auth/terminate.py` & `pyrotgfork-2.1.30/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/answer_callback_query.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/answer_inline_query.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/answer_web_app_query.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/delete_bot_commands.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/get_bot_commands.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/get_bot_default_privileges.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/get_bot_info_description.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_info_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/get_bot_info_short_description.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_info_short_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/get_bot_name.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_name.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/get_chat_menu_button.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/get_game_high_scores.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/get_inline_bot_results.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/request_callback_answer.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/send_game.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/send_inline_bot_result.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/set_bot_commands.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/set_bot_default_privileges.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/set_bot_info_description.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_info_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/set_bot_info_short_description.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_info_short_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/set_bot_name.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_name.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/set_chat_menu_button.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/bots/set_game_score.py` & `pyrotgfork-2.1.30/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/business/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/business/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/business/get_business_connection.py` & `pyrotgfork-2.1.30/pyrogram/methods/business/get_business_connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/business/get_collectible_item_info.py` & `pyrotgfork-2.1.30/pyrogram/methods/business/get_collectible_item_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chat_topics/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chat_topics/close_forum_topic.py` & `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chat_topics/create_forum_topic.py` & `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chat_topics/delete_forum_topic.py` & `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chat_topics/edit_forum_topic.py` & `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chat_topics/get_forum_topic.py` & `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/get_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py` & `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chat_topics/get_forum_topics.py` & `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chat_topics/hide_forum_topic.py` & `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/hide_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chat_topics/reopen_forum_topic.py` & `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chat_topics/unhide_forum_topic.py` & `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/unhide_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/add_chat_members.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/archive_chats.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/ban_chat_member.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/create_channel.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/create_group.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/create_supergroup.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/delete_channel.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/delete_chat_photo.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/delete_supergroup.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/delete_user_history.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/get_chat.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/get_chat_event_log.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/get_chat_member.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/get_chat_members.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/get_chat_members_count.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/get_chat_online_count.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/get_created_chats.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/get_created_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/get_dialogs.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/get_dialogs_count.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/get_nearby_chats.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/get_send_as_chats.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/join_chat.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/leave_chat.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/mark_chat_unread.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/pin_chat_message.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/promote_chat_member.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/restrict_chat_member.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/search_chats.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/search_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/set_administrator_title.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_description.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_permissions.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_photo.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_protected_content.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_title.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_ttl.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_ttl.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/set_chat_username.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/set_send_as_chat.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/set_slow_mode.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/unarchive_chats.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/unban_chat_member.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/unpin_all_chat_messages.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/chats/unpin_chat_message.py` & `pyrotgfork-2.1.30/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/contacts/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/contacts/add_contact.py` & `pyrotgfork-2.1.30/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/contacts/delete_contacts.py` & `pyrotgfork-2.1.30/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/contacts/get_contacts.py` & `pyrotgfork-2.1.30/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/contacts/get_contacts_count.py` & `pyrotgfork-2.1.30/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/contacts/import_contacts.py` & `pyrotgfork-2.1.30/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_callback_query.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_chat_join_request.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_chat_member_updated.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_chosen_inline_result.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_deleted_messages.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_disconnect.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_edited_message.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_inline_query.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_message.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_message_reaction_count_updated.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_message_reaction_updated.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_poll.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_raw_update.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/decorators/on_user_status.py` & `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/approve_chat_join_request.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/create_chat_invite_link.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/decline_chat_join_request.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/export_chat_invite_link.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_invite_link.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/get_chat_join_requests.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `pyrotgfork-2.1.30/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/copy_media_group.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/copy_message.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/delete_messages.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/download_media.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/edit_cached_media.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/edit_inline_caption.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/edit_inline_media.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/edit_inline_reply_markup.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/edit_inline_text.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/edit_message_caption.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/edit_message_media.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/edit_message_reply_markup.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/edit_message_text.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/forward_messages.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/get_chat_history.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/get_chat_history_count.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/get_discussion_message.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/get_discussion_replies.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/get_discussion_replies_count.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/get_media_group.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/get_messages.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/inline_session.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/read_chat_history.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/retract_vote.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/search_global.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/search_global_count.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/search_messages.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/search_messages_count.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_animation.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_audio.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_cached_media.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_chat_action.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_contact.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_dice.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_document.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_location.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_media_group.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_message.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_photo.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_poll.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_poll.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 
 
 class SendPoll:
     async def send_poll(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
         question: str,
-        options: List[str],
+        options: List["types.InputPollOption"],
+        question_parse_mode: "enums.ParseMode" = None,
+        question_entities: List["types.MessageEntity"] = None,
         is_anonymous: bool = True,
         type: "enums.PollType" = enums.PollType.REGULAR,
         allows_multiple_answers: bool = None,
         correct_option_id: int = None,
         explanation: str = None,
         explanation_parse_mode: "enums.ParseMode" = None,
         explanation_entities: List["types.MessageEntity"] = None,
@@ -65,16 +67,23 @@
                 Unique identifier (int) or username (str) of the target chat.
                 For your personal cloud (Saved Messages) you can simply use "me" or "self".
                 For a contact that exists in your Telegram address book you can use his phone number (str).
 
             question (``str``):
                 Poll question, 1-255 characters.
 
-            options (List of ``str``):
-                List of answer options, 2-10 strings 1-100 characters each.
+            options (List of :obj:`~pyrogram.types.InputPollOption`):
+                List of answer options, 2-10 answer options.
+
+            question_parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+                By default, texts are parsed using both Markdown and HTML styles.
+                You can combine both syntaxes together.
+
+            question_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+                List of special entities that appear in the poll question, which can be specified instead of *question_parse_mode*.
 
             is_anonymous (``bool``, *optional*):
                 True, if the poll needs to be anonymous.
                 Defaults to True.
 
             type (:obj`~pyrogram.enums.PollType`, *optional*):
                 Poll type, :obj:`~pyrogram.enums.PollType.QUIZ` or :obj:`~pyrogram.enums.PollType.REGULAR`.
@@ -93,15 +102,15 @@
 
             explanation_parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             explanation_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the poll explanation, which can be specified instead of
-                *parse_mode*.
+                *explanation_parse_mode*.
 
             open_period (``int``, *optional*):
                 Amount of time in seconds the poll will be active after creation, 5-600.
                 Can't be used together with *close_date*.
 
             close_date (:py:obj:`~datetime.datetime`, *optional*):
                 Point in time when the poll will be automatically closed.
@@ -163,22 +172,21 @@
 
         reply_to = await utils._get_reply_message_parameters(
             self,
             message_thread_id,
             reply_parameters
         )
 
-        # TODO: wait for BOT API update?
-        question, question_entities = (await utils.parse_text_entities(self, question, None, None)).values()
+        question, question_entities = (await utils.parse_text_entities(self, question, question_parse_mode, question_entities)).values()
         if not question_entities:
             question_entities = []
 
         answers = []
         for i, answer_ in enumerate(options):
-            answer, answer_entities = (await utils.parse_text_entities(self, answer_, None, None)).values()
+            answer, answer_entities = (await utils.parse_text_entities(self, answer_.text, answer_.text_parse_mode, answer_.text_entities)).values()
             if not answer_entities:
                 answer_entities = []
             answers.append(
                 raw.types.PollAnswer(
                     text=raw.types.TextWithEntities(
                         text=answer,
                         entities=answer_entities
```

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_sticker.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_venue.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_video.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_video_note.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/send_voice.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/set_reaction.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/set_reaction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/stop_poll.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/stop_poll.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             raw.functions.messages.EditMessage(
                 peer=await self.resolve_peer(chat_id),
                 id=message_id,
                 media=raw.types.InputMediaPoll(
                     poll=raw.types.Poll(
                         id=int(poll.id),
                         closed=True,
-                        question="",
+                        question=raw.types.TextWithEntities(text="", entities=[]),
                         answers=[]
                     )
                 ),
                 reply_markup=await reply_markup.write(self) if reply_markup else None
             )
         )
```

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/stream_media.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/messages/vote_poll.py` & `pyrotgfork-2.1.30/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/password/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/password/change_cloud_password.py` & `pyrotgfork-2.1.30/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/password/enable_cloud_password.py` & `pyrotgfork-2.1.30/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/password/remove_cloud_password.py` & `pyrotgfork-2.1.30/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/stickers/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/stickers/get_stickers.py` & `pyrotgfork-2.1.30/pyrogram/methods/stickers/get_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/block_user.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/delete_profile_photos.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/get_chat_photos.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/get_chat_photos_count.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/get_common_chats.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/get_default_emoji_statuses.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/get_me.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/get_users.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/set_birthdate.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/set_birthdate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/set_emoji_status.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/set_personal_chat.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/set_personal_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/set_profile_photo.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/set_username.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/unblock_user.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/users/update_profile.py` & `pyrotgfork-2.1.30/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/utilities/__init__.py` & `pyrotgfork-2.1.30/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/utilities/add_handler.py` & `pyrotgfork-2.1.30/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/utilities/compose.py` & `pyrotgfork-2.1.30/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/utilities/export_session_string.py` & `pyrotgfork-2.1.30/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/utilities/idle.py` & `pyrotgfork-2.1.30/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/utilities/remove_handler.py` & `pyrotgfork-2.1.30/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/utilities/restart.py` & `pyrotgfork-2.1.30/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/utilities/run.py` & `pyrotgfork-2.1.30/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/utilities/start.py` & `pyrotgfork-2.1.30/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/utilities/stop.py` & `pyrotgfork-2.1.30/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/methods/utilities/stop_transmission.py` & `pyrotgfork-2.1.30/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/parser/__init__.py` & `pyrotgfork-2.1.30/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/parser/html.py` & `pyrotgfork-2.1.30/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/parser/markdown.py` & `pyrotgfork-2.1.30/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/parser/parser.py` & `pyrotgfork-2.1.30/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/parser/utils.py` & `pyrotgfork-2.1.30/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/__init__.py` & `pyrotgfork-2.1.30/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/__init__.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/future_salt.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/future_salts.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/gzip_packed.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/list.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/message.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/msg_container.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/tl_object.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/primitives/__init__.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/primitives/bool.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/primitives/bytes.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/primitives/double.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/primitives/int.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/primitives/string.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/raw/core/primitives/vector.py` & `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/session/__init__.py` & `pyrotgfork-2.1.30/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/session/auth.py` & `pyrotgfork-2.1.30/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/session/session.py` & `pyrotgfork-2.1.30/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/session/internals/__init__.py` & `pyrotgfork-2.1.30/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/session/internals/data_center.py` & `pyrotgfork-2.1.30/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/session/internals/msg_factory.py` & `pyrotgfork-2.1.30/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/session/internals/msg_id.py` & `pyrotgfork-2.1.30/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/session/internals/seq_no.py` & `pyrotgfork-2.1.30/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/storage/__init__.py` & `pyrotgfork-2.1.30/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/storage/aio_sqlite_storage.py` & `pyrotgfork-2.1.30/pyrogram/storage/aio_sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/storage/file_storage.py` & `pyrotgfork-2.1.30/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/storage/memory_storage.py` & `pyrotgfork-2.1.30/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/storage/sqlite_storage.py` & `pyrotgfork-2.1.30/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/storage/storage.py` & `pyrotgfork-2.1.30/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/__init__.py` & `pyrotgfork-2.1.30/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/list.py` & `pyrotgfork-2.1.30/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/object.py` & `pyrotgfork-2.1.30/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/update.py` & `pyrotgfork-2.1.30/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/authorization/__init__.py` & `pyrotgfork-2.1.30/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/authorization/sent_code.py` & `pyrotgfork-2.1.30/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/authorization/terms_of_service.py` & `pyrotgfork-2.1.30/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/__init__.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/callback_game.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/callback_query.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/force_reply.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/game_high_score.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/login_url.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/menu_button.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/bots_and_keyboards/web_app_info.py` & `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/business/__init__.py` & `pyrotgfork-2.1.30/pyrogram/types/business/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/business/business_connection.py` & `pyrotgfork-2.1.30/pyrogram/types/business/business_connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/business/business_intro.py` & `pyrotgfork-2.1.30/pyrogram/types/business/business_intro.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/business/business_location.py` & `pyrotgfork-2.1.30/pyrogram/types/business/business_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/business/business_opening_hours.py` & `pyrotgfork-2.1.30/pyrogram/types/business/business_opening_hours.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/business/business_opening_hours_interval.py` & `pyrotgfork-2.1.30/pyrogram/types/business/business_opening_hours_interval.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/business/collectible_item_info.py` & `pyrotgfork-2.1.30/pyrogram/types/business/collectible_item_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/chat_topics/__init__.py` & `pyrotgfork-2.1.30/pyrogram/types/chat_topics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/chat_topics/forum_topic.py` & `pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/chat_topics/forum_topic_closed.py` & `pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/chat_topics/forum_topic_created.py` & `pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/chat_topics/forum_topic_edited.py` & `pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/chat_topics/forum_topic_reopened.py` & `pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/chat_topics/general_forum_topic_hidden.py` & `pyrotgfork-2.1.30/pyrogram/types/chat_topics/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/chat_topics/general_forum_topic_unhidden.py` & `pyrotgfork-2.1.30/pyrogram/types/chat_topics/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/__init__.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/chosen_inline_result.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_animation.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_article.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_audio.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_contact.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_document.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_location.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_photo.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_venue.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_video.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/inline_mode/inline_query_result_voice.py` & `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_media/__init__.py` & `pyrotgfork-2.1.30/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_media/input_media.py` & `pyrotgfork-2.1.30/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_media/input_media_animation.py` & `pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_media/input_media_audio.py` & `pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_media/input_media_document.py` & `pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_media/input_media_photo.py` & `pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_media/input_media_video.py` & `pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_media/input_phone_contact.py` & `pyrotgfork-2.1.30/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_media/link_preview_options.py` & `pyrotgfork-2.1.30/pyrogram/types/input_media/link_preview_options.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_message_content/__init__.py` & `pyrotgfork-2.1.30/pyrogram/types/input_message_content/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from .input_message_content import InputMessageContent
 from .input_text_message_content import InputTextMessageContent
 from .reply_parameters import ReplyParameters
 from .external_reply_info import ExternalReplyInfo
 from .text_quote import TextQuote
+from .input_poll_option import InputPollOption
 
 __all__ = [
     "ExternalReplyInfo",
     "InputMessageContent",
+    "InputPollOption",
     "InputTextMessageContent",
     "ReplyParameters",
     "TextQuote",
 ]
```

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_message_content/external_reply_info.py` & `pyrotgfork-2.1.30/pyrogram/types/input_message_content/external_reply_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_message_content/input_message_content.py` & `pyrotgfork-2.1.30/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_message_content/input_text_message_content.py` & `pyrotgfork-2.1.30/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_message_content/reply_parameters.py` & `pyrotgfork-2.1.30/pyrogram/types/input_message_content/reply_parameters.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/input_message_content/text_quote.py` & `pyrotgfork-2.1.30/pyrogram/types/input_message_content/text_quote.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/message_origin/__init__.py` & `pyrotgfork-2.1.30/pyrogram/types/message_origin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/message_origin/message_import_info.py` & `pyrotgfork-2.1.30/pyrogram/types/message_origin/message_import_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/message_origin/message_origin.py` & `pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/message_origin/message_origin_channel.py` & `pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/message_origin/message_origin_chat.py` & `pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/message_origin/message_origin_hidden_user.py` & `pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_hidden_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/message_origin/message_origin_user.py` & `pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/__init__.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/animation.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/audio.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/chat_boost_added.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/chat_boost_added.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/contact.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/dice.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/document.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/game.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/gift_code.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/gift_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/gifted_premium.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/gifted_premium.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/giveaway.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/giveaway.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/giveaway_completed.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/giveaway_completed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/giveaway_winners.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/giveaway_winners.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/location.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/message.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -12160,17 +12160,18 @@
 0002f7f0: 2020 2020 2020 2020 2022 5468 6973 2070           "This p
 0002f800: 726f 7065 7274 7920 6973 2064 6570 7265  roperty is depre
 0002f810: 6361 7465 642e 2022 0a20 2020 2020 2020  cated. ".       
 0002f820: 2020 2020 2022 506c 6561 7365 2075 7365       "Please use
 0002f830: 2066 6f72 7761 7264 5f6f 7269 6769 6e20   forward_origin 
 0002f840: 696e 7374 6561 6422 0a20 2020 2020 2020  instead".       
 0002f850: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-0002f860: 6e20 7365 6c66 2e66 6f72 7761 7264 5f6f  n self.forward_o
-0002f870: 7269 6769 6e2e 6461 7465 0a0a 2020 2020  rigin.date..    
-0002f880: 2320 454e 443a 2074 6865 2062 656c 6f77  # END: the below
-0002f890: 2070 726f 7065 7274 6965 7320 7765 7265   properties were
-0002f8a0: 2072 656d 6f76 6564 2069 6e20 6042 4f54   removed in `BOT
-0002f8b0: 2041 5049 2037 2e30 203c 6874 7470 733a   API 7.0 <https:
-0002f8c0: 2f2f 636f 7265 2e74 656c 6567 7261 6d2e  //core.telegram.
-0002f8d0: 6f72 672f 626f 7473 2f61 7069 2d63 6861  org/bots/api-cha
-0002f8e0: 6e67 656c 6f67 2364 6563 656d 6265 722d  ngelog#december-
-0002f8f0: 3239 2d32 3032 333e 605f 0a              29-2023>`_.
+0002f860: 6e20 6765 7461 7474 7228 7365 6c66 2e66  n getattr(self.f
+0002f870: 6f72 7761 7264 5f6f 7269 6769 6e2c 2022  orward_origin, "
+0002f880: 6461 7465 222c 204e 6f6e 6529 0a0a 2020  date", None)..  
+0002f890: 2020 2320 454e 443a 2074 6865 2062 656c    # END: the bel
+0002f8a0: 6f77 2070 726f 7065 7274 6965 7320 7765  ow properties we
+0002f8b0: 7265 2072 656d 6f76 6564 2069 6e20 6042  re removed in `B
+0002f8c0: 4f54 2041 5049 2037 2e30 203c 6874 7470  OT API 7.0 <http
+0002f8d0: 733a 2f2f 636f 7265 2e74 656c 6567 7261  s://core.telegra
+0002f8e0: 6d2e 6f72 672f 626f 7473 2f61 7069 2d63  m.org/bots/api-c
+0002f8f0: 6861 6e67 656c 6f67 2364 6563 656d 6265  hangelog#decembe
+0002f900: 722d 3239 2d32 3032 333e 605f 0a         r-29-2023>`_.
```

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/message_entity.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/message_reaction_count_updated.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/message_reaction_updated.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/message_reactions.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/photo.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/poll.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/poll.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     Parameters:
         id (``str``):
             Unique poll identifier.
 
         question (``str``):
             Poll question, 1-255 characters.
 
+        question_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            Special entities that appear in the question. Currently, only custom emoji entities are allowed in poll questions.
+
         options (List of :obj:`~pyrogram.types.PollOption`):
             List of poll options.
 
         total_voter_count (``int``):
             Total number of users that voted in the poll.
 
         is_closed (``bool``):
@@ -80,14 +83,15 @@
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
         id: str,
         question: str,
         options: List["types.PollOption"],
+        question_entities: List["types.MessageEntity"] = None,
         total_voter_count: int,
         is_closed: bool,
         is_anonymous: bool = None,
         type: "enums.PollType" = None,
         allows_multiple_answers: bool = None,
         chosen_option_id: Optional[int] = None,
         correct_option_id: Optional[int] = None,
@@ -97,14 +101,15 @@
         close_date: Optional[datetime] = None
     ):
         super().__init__(client)
 
         self.id = id
         self.question = question
         self.options = options
+        self.question_entities = question_entities
         self.total_voter_count = total_voter_count
         self.is_closed = is_closed
         self.is_anonymous = is_anonymous
         self.type = type
         self.allows_multiple_answers = allows_multiple_answers
         self.chosen_option_id = chosen_option_id
         self.correct_option_id = correct_option_id
@@ -145,14 +150,15 @@
                 for entity in (answer.text.entities or [])
             ]
             entities = types.List(filter(lambda x: x is not None, entities))
 
             options.append(
                 types.PollOption(
                     text=Str(answer.text.text).init(entities),
+                    text_entities=entities,
                     voter_count=voter_count,
                     data=answer.option,
                     client=client
                 )
             )
 
         entities = [
@@ -165,14 +171,15 @@
         ]
         entities = types.List(filter(lambda x: x is not None, entities))
 
         return Poll(
             id=str(poll.id),
             question=Str(poll.question.text).init(entities),
             options=options,
+            question_entities=entities,
             total_voter_count=media_poll.results.total_voters,
             is_closed=poll.closed,
             is_anonymous=not poll.public_voters,
             type=enums.PollType.QUIZ if poll.quiz else enums.PollType.REGULAR,
             allows_multiple_answers=poll.multiple_choice,
             chosen_option_id=chosen_option_id,
             correct_option_id=correct_option_id,
@@ -202,14 +209,15 @@
 
             if result.correct:
                 correct_option_id = i
 
             options.append(
                 types.PollOption(
                     text="",
+                    text_entities=[],
                     voter_count=result.voters,
                     data=result.option,
                     client=client
                 )
             )
 
         return Poll(
```

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/poll_option.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/poll_option.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,39 +12,48 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import List
+
 import pyrogram
+from pyrogram import types
+
 from ..object import Object
 
 
 class PollOption(Object):
     """Contains information about one answer option in a poll.
 
     Parameters:
         text (``str``):
             Option text, 1-100 characters.
+        
+        text_entities (List of :obj:`~pyrogram.types.MessageEntity`, *optional*):
+            Special entities that appear in the option text. Currently, only custom emoji entities are allowed in poll option texts.
 
         voter_count (``int``):
             Number of users that voted for this option.
             Equals to 0 until you vote.
 
         data (``bytes``):
             The data this poll option is holding.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
         text: str,
+        text_entities: List["types.MessageEntity"],
         voter_count: int,
         data: bytes
     ):
         super().__init__(client)
 
         self.text = text
+        self.text_entities = text_entities
         self.voter_count = voter_count
         self.data = data
```

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/reaction.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/sticker.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/story.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/story.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/thumbnail.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/venue.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/video.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/video_note.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/voice.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/web_app_data.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/messages_and_media/web_page.py` & `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/__init__.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/birthdate.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/birthdate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 
         last_name (``str``, *optional*):
             Last name of the other party in a private chat, for private chats.
 
         is_forum (``bool``, *optional*):
             True, if the supergroup chat is a forum
 
+        max_reaction_count (``int``):
+            The maximum number of reactions that can be set on a message in the chat
+
         photo (:obj:`~pyrogram.types.ChatPhoto`, *optional*):
             Chat photo. Suitable for downloads only.
 
         active_usernames (List of :obj:`~pyrogram.types.Username`, *optional*):
             If non-empty, the list of all `active chat usernames <https://telegram.org/blog/topics-in-groups-collectible-usernames#collectible-usernames>`_; for private chats, supergroups and channels.
 
         birthdate (:obj:`~pyrogram.types.Birthdate`, *optional*):
@@ -256,14 +259,15 @@
         has_aggressive_anti_spam_enabled: bool = None,
         message_auto_delete_time: int = None,
         slow_mode_delay: int = None,
         slowmode_next_send_date: datetime = None,
         unrestrict_boost_count: int = None,
         is_forum: bool = None,
         is_peak_preview: bool = None,
+        max_reaction_count: int = None,
         _raw: Union[
             "raw.types.ChatInvite",
             "raw.types.Channel",
             "raw.types.Chat",
             "raw.types.User",
             "raw.types.messages.ChatFull",
             "raw.types.users.UserFull"
@@ -606,14 +610,15 @@
                 parsed_chat.invite_link = full_chat.exported_invite.link
 
             parsed_chat.available_reactions = types.ChatReactions._parse(
                 client,
                 full_chat.available_reactions,
                 reactions_limit=getattr(full_chat, "reactions_limit", None)
             )
+            parsed_chat.max_reaction_count = getattr(full_chat, "reactions_limit", 11)
 
         parsed_chat.personal_chat = personal_chat
         parsed_chat.personal_chat_message = personal_chat_message
         parsed_chat._raw = chat_full
 
         return parsed_chat
```

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_color.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_event.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_event_filter.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_invite_link.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_join_request.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_joiner.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_member.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_member_updated.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,38 +43,43 @@
 
         new_chat_member (:obj:`~pyrogram.types.ChatMember`, *optional*):
             New information about the chat member.
 
         invite_link (:obj:`~pyrogram.types.ChatInviteLink`, *optional*):
             Chat invite link, which was used by the user to join the chat; for joining by invite link events only.
         
+        via_join_request (``bool``, *optional*):
+            True, if the user joined the chat after sending a direct join request and being approved by an administrator
+
         via_chat_folder_invite_link (``bool``, *optional*):
             True, if the user joined the chat via a chat folder invite link
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
         chat: "types.Chat",
         from_user: "types.User",
         date: datetime,
         old_chat_member: "types.ChatMember",
         new_chat_member: "types.ChatMember",
         invite_link: "types.ChatInviteLink" = None,
+        via_join_request: bool = None,
         via_chat_folder_invite_link: bool = None
     ):
         super().__init__(client)
 
         self.chat = chat
         self.from_user = from_user
         self.date = date
         self.old_chat_member = old_chat_member
         self.new_chat_member = new_chat_member
         self.invite_link = invite_link
+        self.via_join_request = via_join_request
         self.via_chat_folder_invite_link = via_chat_folder_invite_link
 
     @staticmethod
     def _parse(
         client: "pyrogram.Client",
         update: Union["raw.types.UpdateChatParticipant", "raw.types.UpdateChannelParticipant", "raw.types.UpdateBotStopped"],
         users: Dict[int, "raw.types.User"],
@@ -111,27 +116,31 @@
             )
 
         chat_id = getattr(update, "chat_id", None) or getattr(update, "channel_id")
 
         old_chat_member = None
         new_chat_member = None
         invite_link = None
+        via_join_request = None
 
         if update.prev_participant:
             old_chat_member = types.ChatMember._parse(client, update.prev_participant, users, chats)
 
         if update.new_participant:
             new_chat_member = types.ChatMember._parse(client, update.new_participant, users, chats)
 
         if update.invite:
             invite_link = types.ChatInviteLink._parse(client, update.invite, users)
+            if isinstance(update.invite, raw.types.ChatInvitePublicJoinRequests):
+                via_join_request = True
 
         return ChatMemberUpdated(
             chat=types.Chat._parse_chat(client, chats[chat_id]),
             from_user=types.User._parse(client, users[update.actor_id]),
             date=utils.timestamp_to_datetime(update.date),
             old_chat_member=old_chat_member,
             new_chat_member=new_chat_member,
             invite_link=invite_link,
             client=client,
+            via_join_request=via_join_request,
             via_chat_folder_invite_link=getattr(update, "via_chatlist", False)
         )
```

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_permissions.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_photo.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_privileges.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_reactions.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/chat_shared.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_shared.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/dialog.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/emoji_status.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/invite_link_importer.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/restriction.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/user.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/username.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/users_shared.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/users_shared.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/video_chat_ended.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/video_chat_participants_invited.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_participants_invited.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyrogram/types/user_and_chats/video_chat_started.py` & `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/.gitignore` & `pyrotgfork-2.1.30/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/COPYING` & `pyrotgfork-2.1.30/COPYING`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/COPYING.lesser` & `pyrotgfork-2.1.30/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/NOTICE` & `pyrotgfork-2.1.30/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/README.md` & `pyrotgfork-2.1.30/README.md`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/hatch_build.py` & `pyrotgfork-2.1.30/hatch_build.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/pyproject.toml` & `pyrotgfork-2.1.30/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.29/PKG-INFO` & `pyrotgfork-2.1.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyrotgfork
-Version: 2.1.29
+Version: 2.1.30
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
-Metadata-Version: 2.3 Name: pyrotgfork Version: 2.1.29 Summary: Fork of
+Metadata-Version: 2.3 Name: pyrotgfork Version: 2.1.30 Summary: Fork of
 Pyrogram. Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Project-URL: Homepage, https://
 telegramplayground.github.io/pyrogram/releases/ Project-URL: Tracker, https://
 github.com/TelegramPlayGround/Pyrogram/issues Project-URL: Community, https://
 t.me/PyroTGFork Project-URL: Source, https://github.com/TelegramPlayGround/
 Pyrogram Project-URL: Documentation, https://telegramplayground.github.io/
 pyrogram/ Author-email: SpEcHIDe
```

