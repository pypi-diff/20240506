# Comparing `tmp/g4f-0.3.0.8.tar.gz` & `tmp/g4f-0.3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.0.8.tar", last modified: Thu May  2 21:54:17 2024, max compression
+gzip compressed data, was "g4f-0.3.0.9.tar", last modified: Sun May  5 21:52:53 2024, max compression
```

## Comparing `g4f-0.3.0.8.tar` & `g4f-0.3.0.9.tar`

### file list

```diff
@@ -1,247 +1,248 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.091830 g4f-0.3.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-02 21:54:13.000000 g4f-0.3.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 21:54:13.000000 g4f-0.3.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55611 2024-05-02 21:54:17.091830 g4f-0.3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    52415 2024-05-02 21:54:13.000000 g4f-0.3.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.059831 g4f-0.3.0.8/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.067830 g4f-0.3.0.8/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/MetaAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/MetaAIAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Reka.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.067830 g4f-0.3.0.8/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.071830 g4f-0.3.0.8/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.071830 g4f-0.3.0.8/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.075830 g4f-0.3.0.8/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    33742 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.075830 g4f-0.3.0.8/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.075830 g4f-0.3.0.8/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.075830 g4f-0.3.0.8/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.075830 g4f-0.3.0.8/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.075830 g4f-0.3.0.8/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/openai/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/openai/proofofwork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.055830 g4f-0.3.0.8/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.079830 g4f-0.3.0.8/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22896 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.083830 g4f-0.3.0.8/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.083830 g4f-0.3.0.8/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    47420 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.083830 g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.087830 g4f-0.3.0.8/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.087830 g4f-0.3.0.8/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.087830 g4f-0.3.0.8/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.087830 g4f-0.3.0.8/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.087830 g4f-0.3.0.8/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-02 21:54:13.000000 g4f-0.3.0.8/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:54:17.087830 g4f-0.3.0.8/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55611 2024-05-02 21:54:17.000000 g4f-0.3.0.8/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-02 21:54:17.000000 g4f-0.3.0.8/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:54:17.000000 g4f-0.3.0.8/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 21:54:17.000000 g4f-0.3.0.8/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-02 21:54:17.000000 g4f-0.3.0.8/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 21:54:17.000000 g4f-0.3.0.8/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 21:54:17.091830 g4f-0.3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-02 21:54:13.000000 g4f-0.3.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.812929 g4f-0.3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-05 21:52:50.000000 g4f-0.3.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-05 21:52:50.000000 g4f-0.3.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55611 2024-05-05 21:52:53.812929 g4f-0.3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    52415 2024-05-05 21:52:50.000000 g4f-0.3.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.768930 g4f-0.3.0.9/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.780930 g4f-0.3.0.9/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/MetaAIAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Reka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.780930 g4f-0.3.0.9/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.788930 g4f-0.3.0.9/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.788930 g4f-0.3.0.9/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.788930 g4f-0.3.0.9/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33742 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.792930 g4f-0.3.0.9/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.792930 g4f-0.3.0.9/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.792930 g4f-0.3.0.9/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.792930 g4f-0.3.0.9/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.792930 g4f-0.3.0.9/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/openai/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/openai/proofofwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.796929 g4f-0.3.0.9/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.796929 g4f-0.3.0.9/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.796929 g4f-0.3.0.9/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.796929 g4f-0.3.0.9/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.800929 g4f-0.3.0.9/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.800929 g4f-0.3.0.9/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.800929 g4f-0.3.0.9/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.768930 g4f-0.3.0.9/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.800929 g4f-0.3.0.9/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22896 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.800929 g4f-0.3.0.9/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.800929 g4f-0.3.0.9/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    47420 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.804929 g4f-0.3.0.9/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.804929 g4f-0.3.0.9/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.804929 g4f-0.3.0.9/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.804929 g4f-0.3.0.9/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.808930 g4f-0.3.0.9/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.808930 g4f-0.3.0.9/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-05 21:52:50.000000 g4f-0.3.0.9/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:52:53.808930 g4f-0.3.0.9/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55611 2024-05-05 21:52:53.000000 g4f-0.3.0.9/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-05-05 21:52:53.000000 g4f-0.3.0.9/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:52:53.000000 g4f-0.3.0.9/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-05 21:52:53.000000 g4f-0.3.0.9/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-05 21:52:53.000000 g4f-0.3.0.9/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-05 21:52:53.000000 g4f-0.3.0.9/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:52:53.812929 g4f-0.3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-05 21:52:50.000000 g4f-0.3.0.9/setup.py
```

### Comparing `g4f-0.3.0.8/LICENSE` & `g4f-0.3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/PKG-INFO` & `g4f-0.3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.0.8
+Version: 0.3.0.9
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.0.8 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.9 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.3.0.8/README.md` & `g4f-0.3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Aichatos.py` & `g4f-0.3.0.9/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Aura.py` & `g4f-0.3.0.9/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Bing.py` & `g4f-0.3.0.9/g4f/Provider/Bing.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,18 +453,21 @@
                     image_request, web_search, gpt4_turbo,
                     new_conversation
                 ))
                 response_txt = ''
                 returned_text = ''
                 message_id = None
                 while do_read:
-                    msg = await wss.receive_str()
+                    try:
+                        msg = await wss.receive_str()
+                    except TypeError:
+                        continue
                     objects = msg.split(Defaults.delimiter)
                     for obj in objects:
-                        if obj is None or not obj:
+                        if not obj:
                             continue
                         try:
                             response = json.loads(obj)
                         except json.JSONDecodeError:
                             continue
                         if response and response.get('type') == 1 and response['arguments'][0].get('messages'):
                             message = response['arguments'][0]['messages'][0]
```

### Comparing `g4f-0.3.0.8/g4f/Provider/BingCreateImages.py` & `g4f-0.3.0.9/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Blackbox.py` & `g4f-0.3.0.9/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/ChatForAi.py` & `g4f-0.3.0.9/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.0.9/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/ChatgptAi.py` & `g4f-0.3.0.9/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/ChatgptFree.py` & `g4f-0.3.0.9/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/ChatgptNext.py` & `g4f-0.3.0.9/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/ChatgptX.py` & `g4f-0.3.0.9/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Cnote.py` & `g4f-0.3.0.9/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Cohere.py` & `g4f-0.3.0.9/g4f/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/DeepInfra.py` & `g4f-0.3.0.9/g4f/Provider/DeepInfra.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import requests
-from ..typing import AsyncResult, Messages, ImageType
-from ..image import to_data_uri
+from ..typing import AsyncResult, Messages
 from .needs_auth.Openai import Openai
 
 class DeepInfra(Openai):
     label = "DeepInfra"
     url = "https://deepinfra.com"
     working = True
     needs_auth = False
@@ -29,15 +28,14 @@
 
     @classmethod
     def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         stream: bool,
-        image: ImageType = None,
         api_base: str = "https://api.deepinfra.com/v1/openai",
         temperature: float = 0.7,
         max_tokens: int = 1028,
         **kwargs
     ) -> AsyncResult:
         headers = {
             'Accept-Encoding': 'gzip, deflate, br',
@@ -50,27 +48,14 @@
             'Sec-Fetch-Site': 'same-site',
             'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Safari/537.36',
             'X-Deepinfra-Source': 'web-embed',
             'sec-ch-ua': '"Google Chrome";v="119", "Chromium";v="119", "Not?A_Brand";v="24"',
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"macOS"',
         }
-        if image is not None:
-            if not model:
-                model = cls.default_vision_model
-            messages[-1]["content"] = [
-                {
-                    "type": "image_url",
-                    "image_url": {"url": to_data_uri(image)}
-                },
-                {
-                    "type": "text",
-                    "text": messages[-1]["content"]
-                }
-            ]
         return super().create_async_generator(
             model, messages,
             stream=stream,
             api_base=api_base,
             temperature=temperature,
             max_tokens=max_tokens,
             headers=headers,
```

### Comparing `g4f-0.3.0.8/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.0.9/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.0.9/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Ecosia.py` & `g4f-0.3.0.9/g4f/Provider/Ecosia.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Feedough.py` & `g4f-0.3.0.9/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/FlowGpt.py` & `g4f-0.3.0.9/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.0.9/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/FreeGpt.py` & `g4f-0.3.0.9/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/GeminiPro.py` & `g4f-0.3.0.9/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/GeminiProChat.py` & `g4f-0.3.0.9/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/GigaChat.py` & `g4f-0.3.0.9/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/GptTalkRu.py` & `g4f-0.3.0.9/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/HuggingChat.py` & `g4f-0.3.0.9/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/HuggingFace.py` & `g4f-0.3.0.9/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Koala.py` & `g4f-0.3.0.9/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Liaobots.py` & `g4f-0.3.0.9/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Llama.py` & `g4f-0.3.0.9/g4f/Provider/Llama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Local.py` & `g4f-0.3.0.9/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/MetaAI.py` & `g4f-0.3.0.9/g4f/Provider/MetaAI.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/MetaAIAccount.py` & `g4f-0.3.0.9/g4f/Provider/MetaAIAccount.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.0.9/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Pi.py` & `g4f-0.3.0.9/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Reka.py` & `g4f-0.3.0.9/g4f/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Replicate.py` & `g4f-0.3.0.9/g4f/Provider/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/ReplicateImage.py` & `g4f-0.3.0.9/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/Vercel.py` & `g4f-0.3.0.9/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.0.9/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/You.py` & `g4f-0.3.0.9/g4f/Provider/You.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,21 @@
         default_model,
         "gpt-4",
         "gpt-4-turbo",
         "claude-instant",
         "claude-2",
         "claude-3-opus",
         "claude-3-sonnet",
+        "claude-3-haiku",
         "gemini-pro",
+        "gemini-1-5-pro",
+        "databricks-dbrx-instruct",
+        "command-r",
+        "command-r-plus",
+        "llama3",
         "zephyr",
         default_vision_model,
         *image_models
     ]
     model_aliases = {
         "claude-v2": "claude-2"
     }
```

### Comparing `g4f-0.3.0.8/g4f/Provider/__init__.py` & `g4f-0.3.0.9/g4f/Provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from .HuggingFace      import HuggingFace
 from .Koala            import Koala
 from .Liaobots         import Liaobots
 from .Llama            import Llama
 from .Local            import Local
 from .MetaAI           import MetaAI
 from .MetaAIAccount    import MetaAIAccount
+from .Ollama           import Ollama
 from .PerplexityLabs   import PerplexityLabs
 from .Pi               import Pi
 from .Replicate        import Replicate
 from .ReplicateImage   import ReplicateImage
 from .Vercel           import Vercel
 from .WhiteRabbitNeo   import WhiteRabbitNeo
 from .You              import You
```

### Comparing `g4f-0.3.0.8/g4f/Provider/bing/conversation.py` & `g4f-0.3.0.9/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/bing/create_images.py` & `g4f-0.3.0.9/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/bing/upload_image.py` & `g4f-0.3.0.9/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/V50.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.0.9/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.0.9/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.0.9/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.0.9/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.0.9/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.0.9/g4f/Provider/needs_auth/Openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import json
 
 from ..helper import filter_none
 from ..base_provider import AsyncGeneratorProvider, ProviderModelMixin, FinishReason
-from ...typing import Union, Optional, AsyncResult, Messages
+from ...typing import Union, Optional, AsyncResult, Messages, ImageType
 from ...requests import StreamSession, raise_for_status
 from ...errors import MissingAuthError, ResponseError
+from ...image import to_data_uri
 
 class Openai(AsyncGeneratorProvider, ProviderModelMixin):
     label = "OpenAI API"
     url = "https://openai.com"
     working = True
     needs_auth = True
     supports_message_history = True
@@ -19,27 +20,41 @@
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
         timeout: int = 120,
+        image: ImageType = None,
         api_key: str = None,
         api_base: str = "https://api.openai.com/v1",
         temperature: float = None,
         max_tokens: int = None,
         top_p: float = None,
         stop: Union[str, list[str]] = None,
         stream: bool = False,
         headers: dict = None,
         extra_data: dict = {},
         **kwargs
     ) -> AsyncResult:
         if cls.needs_auth and api_key is None:
             raise MissingAuthError('Add a "api_key"')
+        if image is not None:
+            if not model and hasattr(cls, "default_vision_model"):
+                model = cls.default_vision_model
+            messages[-1]["content"] = [
+                {
+                    "type": "image_url",
+                    "image_url": {"url": to_data_uri(image)}
+                },
+                {
+                    "type": "text",
+                    "text": messages[-1]["content"]
+                }
+            ]
         async with StreamSession(
             proxies={"all": proxy},
             headers=cls.get_headers(stream, api_key, headers),
             timeout=timeout
         ) as session:
             data = filter_none(
                 messages=messages,
@@ -47,15 +62,14 @@
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
                 stop=stop,
                 stream=stream,
                 **extra_data
             )
-            
             async with session.post(f"{api_base.rstrip('/')}/chat/completions", json=data) as response:
                 await raise_for_status(response)
                 if not stream:
                     data = await response.json()
                     cls.raise_error(data)
                     choice = data["choices"][0]
                     if "content" in choice["message"]:
@@ -99,12 +113,11 @@
     @classmethod
     def get_headers(cls, stream: bool, api_key: str = None, headers: dict = None) -> dict:
         return {
             "Accept": "text/event-stream" if stream else "application/json",
             "Content-Type": "application/json",
             **(
                 {"Authorization": f"Bearer {api_key}"}
-                if cls.needs_auth and api_key is not None
-                else {}
+                if api_key is not None else {}
             ),
             **({} if headers is None else headers)
         }
```

### Comparing `g4f-0.3.0.8/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.0.9/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.0.9/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.0.9/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.0.9/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.0.9/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.0.9/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.0.9/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.0.9/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.0.9/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.0.9/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.0.9/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.0.9/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.0.9/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.0.9/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.0.9/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.0.9/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.0.9/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.0.9/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.0.9/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.0.9/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/npm/package-lock.json` & `g4f-0.3.0.9/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/openai/crypt.py` & `g4f-0.3.0.9/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/openai/har_file.py` & `g4f-0.3.0.9/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/openai/proofofwork.py` & `g4f-0.3.0.9/g4f/Provider/openai/proofofwork.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.0.9/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/selenium/Bard.py` & `g4f-0.3.0.9/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.0.9/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.0.9/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/selenium/Phind.py` & `g4f-0.3.0.9/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.0.9/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.0.9/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.0.9/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.0.9/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.0.9/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/Provider/you/har_file.py` & `g4f-0.3.0.9/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/__init__.py` & `g4f-0.3.0.9/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/api/__init__.py` & `g4f-0.3.0.9/g4f/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,14 +197,14 @@
 ) -> None:
     print(f'Starting server... [g4f v-{g4f.version.utils.current_version}]' + (" (debug)" if debug else ""))
     if use_colors is None:
         use_colors = debug
     if bind is not None:
         host, port = bind.split(":")
     uvicorn.run(
-        f"g4f.api:{'create_app_debug' if debug else 'create_app'}",
+        f"g4f.api:create_app{'_debug' if debug else ''}",
         host=host, port=int(port),
         workers=workers,
         use_colors=use_colors,
         factory=True,
         reload=debug
     )
```

### Comparing `g4f-0.3.0.8/g4f/api/_logging.py` & `g4f-0.3.0.9/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/cli.py` & `g4f-0.3.0.9/g4f/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 def main():
     parser = argparse.ArgumentParser(description="Run gpt4free")
     subparsers = parser.add_subparsers(dest="mode", help="Mode to run the g4f in.")
     api_parser = subparsers.add_parser("api")
     api_parser.add_argument("--bind", default="0.0.0.0:1337", help="The bind string.")
     api_parser.add_argument("--debug", action="store_true", help="Enable verbose logging.")
+    api_parser.add_argument("--model", default=None, help="Default model for chat completion. (incompatible with --debug and --workers)")
+    api_parser.add_argument("--provider", choices=[provider.__name__ for provider in Provider.__providers__ if provider.working],
+                            default=None, help="Default provider for chat completion. (incompatible with --debug and --workers)")
+    api_parser.add_argument("--proxy", default=None, help="Default used proxy.")
     api_parser.add_argument("--workers", type=int, default=None, help="Number of workers.")
     api_parser.add_argument("--disable-colors", action="store_true", help="Don't use colors.")
     api_parser.add_argument("--ignore-cookie-files", action="store_true", help="Don't read .har and cookie files.")
     api_parser.add_argument("--g4f-api-key", type=str, default=None, help="Sets an authentication key for your API. (incompatible with --debug and --workers)")
     api_parser.add_argument("--ignored-providers", nargs="+", choices=[provider.__name__ for provider in Provider.__providers__ if provider.working],
                             default=[], help="List of providers to ignore when processing request. (incompatible with --debug and --workers)")
     subparsers.add_parser("gui", parents=[gui_parser()], add_help=False)
@@ -27,22 +31,23 @@
     else:
         parser.print_help()
         exit(1)
 
 def run_api_args(args):
     from g4f.api import AppConfig, run_api
 
-    AppConfig.set_ignore_cookie_files(
-        args.ignore_cookie_files
-    )
-    AppConfig.set_list_ignored_providers(
-        args.ignored_providers
-    )
-    AppConfig.set_g4f_api_key(
-        args.g4f_api_key
+    AppConfig.set_config(
+        ignore_cookie_files=args.ignore_cookie_files,
+        ignored_providers=args.ignored_providers,
+        g4f_api_key=args.g4f_api_key,
+        defaults={
+            "model": args.model,
+            "provider": args.provider,
+            "proxy": args.proxy
+        }
     )
     run_api(
         bind=args.bind,
         debug=args.debug,
         workers=args.workers,
         use_colors=not args.disable_colors
     )
```

### Comparing `g4f-0.3.0.8/g4f/client/async_client.py` & `g4f-0.3.0.9/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/client/client.py` & `g4f-0.3.0.9/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/client/helper.py` & `g4f-0.3.0.9/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/client/image_models.py` & `g4f-0.3.0.9/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/client/service.py` & `g4f-0.3.0.9/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/client/stubs.py` & `g4f-0.3.0.9/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/client/types.py` & `g4f-0.3.0.9/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/cookies.py` & `g4f-0.3.0.9/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/errors.py` & `g4f-0.3.0.9/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/__init__.py` & `g4f-0.3.0.9/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/index.html` & `g4f-0.3.0.9/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/css/style.css` & `g4f-0.3.0.9/g4f/gui/client/static/css/style.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.0.9/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.0.9/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.0.9/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.0.9/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.0.9/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/img/user.png` & `g4f-0.3.0.9/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.0.9/g4f/gui/client/static/js/chat.v1.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.0.9/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.0.9/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/js/icons.js` & `g4f-0.3.0.9/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.0.9/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.0.9/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.0.9/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/server/android_gallery.py` & `g4f-0.3.0.9/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/server/api.py` & `g4f-0.3.0.9/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/server/backend.py` & `g4f-0.3.0.9/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/server/config.py` & `g4f-0.3.0.9/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/server/internet.py` & `g4f-0.3.0.9/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/server/js_api.py` & `g4f-0.3.0.9/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/server/website.py` & `g4f-0.3.0.9/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/gui/webview.py` & `g4f-0.3.0.9/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/image.py` & `g4f-0.3.0.9/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/local/__init__.py` & `g4f-0.3.0.9/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/locals/models.py` & `g4f-0.3.0.9/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/locals/provider.py` & `g4f-0.3.0.9/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/models.py` & `g4f-0.3.0.9/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/providers/base_provider.py` & `g4f-0.3.0.9/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/providers/create_images.py` & `g4f-0.3.0.9/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/providers/helper.py` & `g4f-0.3.0.9/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/providers/retry_provider.py` & `g4f-0.3.0.9/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/providers/types.py` & `g4f-0.3.0.9/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/requests/__init__.py` & `g4f-0.3.0.9/g4f/requests/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     headers = {
         **WEBVIEW_HAEDERS,
         "User-Agent": window.evaluate_js("this.navigator.userAgent"),
         "Accept-Language": window.evaluate_js("this.navigator.language"),
         "Referer": window.real_url
     }
     cookies = [list(*cookie.items()) for cookie in window.get_cookies()]
-    cookies = dict([(name, cookie.value) for name, cookie in cookies])
+    cookies = {name: cookie.value for name, cookie in cookies}
     window.destroy()
     return {"headers": headers, "cookies": cookies}
 
 def get_args_from_browser(
     url: str,
     webdriver: WebDriver = None,
     proxy: str = None,
```

### Comparing `g4f-0.3.0.8/g4f/requests/aiohttp.py` & `g4f-0.3.0.9/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/requests/curl_cffi.py` & `g4f-0.3.0.9/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/requests/defaults.py` & `g4f-0.3.0.9/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/requests/raise_for_status.py` & `g4f-0.3.0.9/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/stubs.py` & `g4f-0.3.0.9/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/typing.py` & `g4f-0.3.0.9/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/version.py` & `g4f-0.3.0.9/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f/webdriver.py` & `g4f-0.3.0.9/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/g4f.egg-info/PKG-INFO` & `g4f-0.3.0.9/g4f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.0.8
+Version: 0.3.0.9
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.0.8 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.9 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.3.0.8/g4f.egg-info/SOURCES.txt` & `g4f-0.3.0.9/g4f.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 g4f/Provider/HuggingFace.py
 g4f/Provider/Koala.py
 g4f/Provider/Liaobots.py
 g4f/Provider/Llama.py
 g4f/Provider/Local.py
 g4f/Provider/MetaAI.py
 g4f/Provider/MetaAIAccount.py
+g4f/Provider/Ollama.py
 g4f/Provider/PerplexityLabs.py
 g4f/Provider/Pi.py
 g4f/Provider/Reka.py
 g4f/Provider/Replicate.py
 g4f/Provider/ReplicateImage.py
 g4f/Provider/Vercel.py
 g4f/Provider/WhiteRabbitNeo.py
```

### Comparing `g4f-0.3.0.8/g4f.egg-info/requires.txt` & `g4f-0.3.0.9/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.8/setup.py` & `g4f-0.3.0.9/setup.py`

 * *Files identical despite different names*

