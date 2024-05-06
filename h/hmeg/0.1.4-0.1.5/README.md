# Comparing `tmp/hmeg-0.1.4.tar.gz` & `tmp/hmeg-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmeg-0.1.4.tar", max compression
+gzip compressed data, was "hmeg-0.1.5.tar", max compression
```

## Comparing `hmeg-0.1.4.tar` & `hmeg-0.1.5.tar`

### file list

```diff
@@ -1,77 +1,97 @@
--rw-r--r--   0        0        0     1066 2024-03-01 07:41:02.775209 hmeg-0.1.4/LICENSE
--rw-r--r--   0        0        0     4437 2024-04-06 02:58:35.143708 hmeg-0.1.4/README.md
--rw-r--r--   0        0        0      137 2024-03-31 04:16:50.659172 hmeg-0.1.4/hmeg/__init__.py
--rw-r--r--   0        0        0     2782 2024-04-17 14:37:13.372136 hmeg-0.1.4/hmeg/entities.py
--rw-r--r--   0        0        0     1652 2024-04-17 14:37:13.372136 hmeg-0.1.4/hmeg/exercise_generator.py
--rw-r--r--   0        0        0     1500 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/ab.toml
--rw-r--r--   0        0        0     1782 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/cd.toml
--rw-r--r--   0        0        0     1897 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/efg.toml
--rw-r--r--   0        0        0     1384 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/h.toml
--rw-r--r--   0        0        0     1631 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/ikl.toml
--rw-r--r--   0        0        0     1809 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/mn.toml
--rw-r--r--   0        0        0     1216 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/opr.toml
--rw-r--r--   0        0        0     3075 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/stu.toml
--rw-r--r--   0        0        0     2146 2024-04-06 02:58:35.143708 hmeg-0.1.4/hmeg/miniphrase/wy.toml
--rw-r--r--   0        0        0     2327 2024-04-17 14:37:13.372136 hmeg-0.1.4/hmeg/registry.py
--rw-r--r--   0        0        0      423 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_basic_present_tense.toml
--rw-r--r--   0        0        0      793 2024-04-24 14:03:25.414198 hmeg-0.1.4/hmeg/topics/1_from_a_to_b_from_c_until_d.toml
--rw-r--r--   0        0        0      370 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_have_dont_have_there_is_there_isnt.toml
--rw-r--r--   0        0        0      419 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_i_want_to.toml
--rw-r--r--   0        0        0      550 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_negative_sentenses.toml
--rw-r--r--   0        0        0      366 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_past_tense.toml
--rw-r--r--   0        0        0      323 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_please_give_me.toml
--rw-r--r--   0        0        0      356 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_this_is.toml
--rw-r--r--   0        0        0      388 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_topic_subject_particle.toml
--rw-r--r--   0        0        0      456 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_what_do_you_want_to_do.toml
--rw-r--r--   0        0        0      392 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/2_and_and_then_therefore_so.toml
--rw-r--r--   0        0        0      566 2024-04-24 14:08:53.431398 hmeg-0.1.4/hmeg/topics/2_and_with.toml
--rw-r--r--   0        0        0      600 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/2_but_however.toml
--rw-r--r--   0        0        0      412 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/2_can_cannot.toml
--rw-r--r--   0        0        0      364 2024-04-24 14:15:05.256760 hmeg-0.1.4/hmeg/topics/2_dont_do_it.toml
--rw-r--r--   0        0        0      375 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/2_future_tense.toml
--rw-r--r--   0        0        0      443 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/2_have_to_should_must.toml
--rw-r--r--   0        0        0      347 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_if_in_case.toml
--rw-r--r--   0        0        0      300 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_imperative.toml
--rw-r--r--   0        0        0      310 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_particles_for_method_way.toml
--rw-r--r--   0        0        0      389 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_please_do_it_for_me.toml
--rw-r--r--   0        0        0      380 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_present_progressive.toml
--rw-r--r--   0        0        0      419 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_to_be_good_poor_at.toml
--rw-r--r--   0        0        0      420 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_to_like.toml
--rw-r--r--   0        0        0      396 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_after_ing.toml
--rw-r--r--   0        0        0      612 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_approximately_about.toml
--rw-r--r--   0        0        0      442 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_before_ing.toml
--rw-r--r--   0        0        0      330 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_but_still_nevertheless.toml
--rw-r--r--   0        0        0      400 2024-04-27 08:55:56.656265 hmeg-0.1.4/hmeg/topics/3_even_if_even_though.toml
--rw-r--r--   0        0        0      417 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_in_front_of_behind.toml
--rw-r--r--   0        0        0      529 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_in_order_to_for_the_sake_of.toml
--rw-r--r--   0        0        0      332 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_linking_verbs_고.toml
--rw-r--r--   0        0        0      294 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_linking_verbs_여서.toml
--rw-r--r--   0        0        0      411 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_linking_words_는데.toml
--rw-r--r--   0        0        0      556 2024-04-24 14:11:33.291983 hmeg-0.1.4/hmeg/topics/3_maybe_i_might.toml
--rw-r--r--   0        0        0      438 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_nothing_but_only.toml
--rw-r--r--   0        0        0      468 2024-04-27 08:55:56.656265 hmeg-0.1.4/hmeg/topics/3_shall_we_i_wonder.toml
--rw-r--r--   0        0        0      360 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_to_look_like_seem_like.toml
--rw-r--r--   0        0        0      293 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_too_much_very.toml
--rw-r--r--   0        0        0      314 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_verb_ending_네요.toml
--rw-r--r--   0        0        0      670 2024-04-24 14:18:15.221455 hmeg-0.1.4/hmeg/topics/3_well_then_in_that_case.toml
--rw-r--r--   0        0        0      446 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_among_between.toml
--rw-r--r--   0        0        0      330 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_do_you_want_to.toml
--rw-r--r--   0        0        0      673 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_i_think_past_future.toml
--rw-r--r--   0        0        0      418 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_it_cant_be.toml
--rw-r--r--   0        0        0      668 2024-04-27 08:55:56.656265 hmeg-0.1.4/hmeg/topics/4_it_is_ok_to.toml
--rw-r--r--   0        0        0      413 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_less_not_completely.toml
--rw-r--r--   0        0        0      445 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_most_best.toml
--rw-r--r--   0        0        0      352 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_much_more_much_less.toml
--rw-r--r--   0        0        0      468 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_the_more_the_more.toml
--rw-r--r--   0        0        0      351 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_to_become_adj.toml
--rw-r--r--   0        0        0      527 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_to_gradually_get_to_do.toml
--rw-r--r--   0        0        0      608 2024-04-24 14:07:24.823074 hmeg-0.1.4/hmeg/topics/4_to_try_doing_something.toml
--rw-r--r--   0        0        0      403 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_verb_ending_지_죠.toml
--rw-r--r--   0        0        0      568 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_you_should_not.toml
--rw-r--r--   0        0        0      510 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/9_while.toml
--rw-r--r--   0        0        0     5902 2024-04-27 08:55:56.656265 hmeg-0.1.4/hmeg/usecases.py
--rw-r--r--   0        0        0     2654 2024-04-24 13:53:05.935930 hmeg-0.1.4/hmeg/vocabs/minilex.toml
--rw-r--r--   0        0        0      989 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/vocabs/nanolex.toml
--rw-r--r--   0        0        0     5598 2024-04-17 14:37:13.372136 hmeg-0.1.4/hmeg/vocabulary.py
--rw-r--r--   0        0        0      500 2024-04-27 08:56:20.804362 hmeg-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 hmeg-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-01 07:41:02.775209 hmeg-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4437 2024-04-06 02:58:35.143708 hmeg-0.1.5/README.md
+-rw-r--r--   0        0        0      137 2024-03-31 04:16:50.659172 hmeg-0.1.5/hmeg/__init__.py
+-rw-r--r--   0        0        0     3010 2024-05-05 01:42:15.076152 hmeg-0.1.5/hmeg/entities.py
+-rw-r--r--   0        0        0     1652 2024-04-17 14:37:13.372136 hmeg-0.1.5/hmeg/exercise_generator.py
+-rw-r--r--   0        0        0     1566 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/miniphrase/ab.toml
+-rw-r--r--   0        0        0     1848 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/miniphrase/cd.toml
+-rw-r--r--   0        0        0     1963 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/miniphrase/efg.toml
+-rw-r--r--   0        0        0     1450 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/miniphrase/h.toml
+-rw-r--r--   0        0        0     1697 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/miniphrase/ikl.toml
+-rw-r--r--   0        0        0     1875 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/miniphrase/mn.toml
+-rw-r--r--   0        0        0     1282 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/miniphrase/opr.toml
+-rw-r--r--   0        0        0     3141 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/miniphrase/stu.toml
+-rw-r--r--   0        0        0     2212 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/miniphrase/wy.toml
+-rw-r--r--   0        0        0     2369 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/registry.py
+-rw-r--r--   0        0        0      431 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/1_basic_present_tense.toml
+-rw-r--r--   0        0        0      801 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/1_from_a_to_b_from_c_until_d.toml
+-rw-r--r--   0        0        0      378 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/1_have_dont_have_there_is_there_isnt.toml
+-rw-r--r--   0        0        0      427 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/1_i_want_to.toml
+-rw-r--r--   0        0        0      558 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/1_negative_sentenses.toml
+-rw-r--r--   0        0        0      374 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/1_past_tense.toml
+-rw-r--r--   0        0        0      331 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/1_please_give_me.toml
+-rw-r--r--   0        0        0      364 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/1_this_is.toml
+-rw-r--r--   0        0        0      396 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/1_topic_subject_particle.toml
+-rw-r--r--   0        0        0      464 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/1_what_do_you_want_to_do.toml
+-rw-r--r--   0        0        0      400 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_and_and_then_therefore_so.toml
+-rw-r--r--   0        0        0      574 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_and_with.toml
+-rw-r--r--   0        0        0      608 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_but_however.toml
+-rw-r--r--   0        0        0      420 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_can_cannot.toml
+-rw-r--r--   0        0        0      372 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_dont_do_it.toml
+-rw-r--r--   0        0        0      383 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_future_tense.toml
+-rw-r--r--   0        0        0      451 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_have_to_should_must.toml
+-rw-r--r--   0        0        0      355 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_if_in_case.toml
+-rw-r--r--   0        0        0      308 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_imperative.toml
+-rw-r--r--   0        0        0      318 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_particles_for_method_way.toml
+-rw-r--r--   0        0        0      397 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_please_do_it_for_me.toml
+-rw-r--r--   0        0        0      388 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_present_progressive.toml
+-rw-r--r--   0        0        0      427 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_to_be_good_poor_at.toml
+-rw-r--r--   0        0        0      428 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/2_to_like.toml
+-rw-r--r--   0        0        0      404 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_after_ing.toml
+-rw-r--r--   0        0        0      620 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_approximately_about.toml
+-rw-r--r--   0        0        0      450 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_before_ing.toml
+-rw-r--r--   0        0        0      338 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_but_still_nevertheless.toml
+-rw-r--r--   0        0        0      424 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_even_if_even_though.toml
+-rw-r--r--   0        0        0      425 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_in_front_of_behind.toml
+-rw-r--r--   0        0        0      537 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_in_order_to_for_the_sake_of.toml
+-rw-r--r--   0        0        0      340 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_linking_verbs_고.toml
+-rw-r--r--   0        0        0      302 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_linking_verbs_여서.toml
+-rw-r--r--   0        0        0      419 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_linking_words_는데.toml
+-rw-r--r--   0        0        0      564 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_maybe_i_might.toml
+-rw-r--r--   0        0        0      446 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_nothing_but_only.toml
+-rw-r--r--   0        0        0      492 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_shall_we_i_wonder.toml
+-rw-r--r--   0        0        0      368 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_to_look_like_seem_like.toml
+-rw-r--r--   0        0        0      301 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_too_much_very.toml
+-rw-r--r--   0        0        0      322 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_verb_ending_네요.toml
+-rw-r--r--   0        0        0      678 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/3_well_then_in_that_case.toml
+-rw-r--r--   0        0        0      454 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/4_among_between.toml
+-rw-r--r--   0        0        0      338 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/4_do_you_want_to.toml
+-rw-r--r--   0        0        0      681 2024-05-04 01:57:47.052373 hmeg-0.1.5/hmeg/topics/4_i_think_past_future.toml
+-rw-r--r--   0        0        0      426 2024-05-04 01:57:47.056373 hmeg-0.1.5/hmeg/topics/4_it_cant_be.toml
+-rw-r--r--   0        0        0      692 2024-05-04 01:57:47.056373 hmeg-0.1.5/hmeg/topics/4_it_is_ok_to.toml
+-rw-r--r--   0        0        0      421 2024-05-04 01:57:47.056373 hmeg-0.1.5/hmeg/topics/4_less_not_completely.toml
+-rw-r--r--   0        0        0      453 2024-05-04 01:57:47.056373 hmeg-0.1.5/hmeg/topics/4_most_best.toml
+-rw-r--r--   0        0        0      360 2024-05-04 01:57:47.056373 hmeg-0.1.5/hmeg/topics/4_much_more_much_less.toml
+-rw-r--r--   0        0        0      476 2024-05-04 01:57:47.056373 hmeg-0.1.5/hmeg/topics/4_the_more_the_more.toml
+-rw-r--r--   0        0        0      359 2024-05-04 01:57:47.056373 hmeg-0.1.5/hmeg/topics/4_to_become_adj.toml
+-rw-r--r--   0        0        0      535 2024-05-04 01:57:47.056373 hmeg-0.1.5/hmeg/topics/4_to_gradually_get_to_do.toml
+-rw-r--r--   0        0        0      616 2024-05-04 01:57:47.056373 hmeg-0.1.5/hmeg/topics/4_to_try_doing_something.toml
+-rw-r--r--   0        0        0      411 2024-05-04 01:57:47.056373 hmeg-0.1.5/hmeg/topics/4_verb_ending_지_죠.toml
+-rw-r--r--   0        0        0      576 2024-05-04 01:57:47.056373 hmeg-0.1.5/hmeg/topics/4_you_should_not.toml
+-rw-r--r--   0        0        0      389 2024-05-05 01:22:20.439045 hmeg-0.1.5/hmeg/topics/5_almost_did.toml
+-rw-r--r--   0        0        0      498 2024-05-05 01:22:20.439045 hmeg-0.1.5/hmeg/topics/5_as_soon_as.toml
+-rw-r--r--   0        0        0      423 2024-05-05 01:22:20.439045 hmeg-0.1.5/hmeg/topics/5_at_least_instead_it_might_be_not_the_best_but.toml
+-rw-r--r--   0        0        0      548 2024-05-05 01:22:20.439045 hmeg-0.1.5/hmeg/topics/5_compare_to_relatively.toml
+-rw-r--r--   0        0        0      561 2024-05-05 01:22:20.439045 hmeg-0.1.5/hmeg/topics/5_honorifit_suffix.toml
+-rw-r--r--   0        0        0      682 2024-05-05 01:22:20.439045 hmeg-0.1.5/hmeg/topics/5_i_guess_i_assume.toml
+-rw-r--r--   0        0        0      469 2024-05-05 01:22:20.439045 hmeg-0.1.5/hmeg/topics/5_instead_of.toml
+-rw-r--r--   0        0        0      552 2024-05-05 01:22:20.439045 hmeg-0.1.5/hmeg/topics/5_it_is_about_to_i_am_planning_to.toml
+-rw-r--r--   0        0        0      448 2024-05-05 01:22:20.439045 hmeg-0.1.5/hmeg/topics/5_it_seems_like_i_assume.toml
+-rw-r--r--   0        0        0      525 2024-05-05 01:22:20.439045 hmeg-0.1.5/hmeg/topics/5_not_a_but_b_dont_do_this_but_do_that.toml
+-rw-r--r--   0        0        0      414 2024-05-05 01:22:20.443045 hmeg-0.1.5/hmeg/topics/5_noun_that_is_called.toml
+-rw-r--r--   0        0        0      587 2024-05-05 01:22:20.443045 hmeg-0.1.5/hmeg/topics/5_since_because_as.toml
+-rw-r--r--   0        0        0      477 2024-05-05 01:22:20.443045 hmeg-0.1.5/hmeg/topics/5_they_said_that_they_had_done_would.toml
+-rw-r--r--   0        0        0      417 2024-05-05 01:22:20.443045 hmeg-0.1.5/hmeg/topics/5_to_have_no_other_choice_but.toml
+-rw-r--r--   0        0        0      429 2024-05-05 01:22:20.443045 hmeg-0.1.5/hmeg/topics/5_to_say_that_something_is_noun.toml
+-rw-r--r--   0        0        0      882 2024-05-05 01:22:20.443045 hmeg-0.1.5/hmeg/topics/5_to_say_that_something_verb.toml
+-rw-r--r--   0        0        0      365 2024-05-05 01:22:20.443045 hmeg-0.1.5/hmeg/topics/5_to_tell_someone_to_do_something.toml
+-rw-r--r--   0        0        0      654 2024-05-05 01:22:20.443045 hmeg-0.1.5/hmeg/topics/5_whether_or_not.toml
+-rw-r--r--   0        0        0      489 2024-05-05 01:22:20.443045 hmeg-0.1.5/hmeg/topics/5_while_i_was_doing.toml
+-rw-r--r--   0        0        0      446 2024-05-05 01:22:20.443045 hmeg-0.1.5/hmeg/topics/5_you_know_isng_it_you_see_come_on.toml
+-rw-r--r--   0        0        0      534 2024-05-04 01:57:47.056373 hmeg-0.1.5/hmeg/topics/9_while.toml
+-rw-r--r--   0        0        0     6704 2024-05-05 01:42:15.080152 hmeg-0.1.5/hmeg/usecases.py
+-rw-r--r--   0        0        0     2661 2024-05-05 01:22:20.443045 hmeg-0.1.5/hmeg/vocabs/minilex.toml
+-rw-r--r--   0        0        0      989 2024-04-27 08:58:06.884788 hmeg-0.1.5/hmeg/vocabs/nanolex.toml
+-rw-r--r--   0        0        0     6131 2024-05-05 01:43:13.596381 hmeg-0.1.5/hmeg/vocabulary.py
+-rw-r--r--   0        0        0      500 2024-05-06 03:04:37.015533 hmeg-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 hmeg-0.1.5/PKG-INFO
```

### Comparing `hmeg-0.1.4/LICENSE` & `hmeg-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.4/README.md` & `hmeg-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.4/hmeg/entities.py` & `hmeg-0.1.5/hmeg/entities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 from __future__ import annotations
 import dataclasses
 
 
 VOWELS = "aeiou"
 
 
+@dataclasses.dataclass
+class VocabularyInfo:
+    name: str
+    num_words: int
+    num_nouns: int
+    num_verbs: int
+    num_adjectives: int
+    num_adverbs: int
+
+
 class VocabularyPlaceholders:
     Adjective = "{adj}"  # adjective
     Adverb = "{adverb}"  # adverb
     ANoun = "{a:noun}"  # noun, singular, with a preceding a/an article
     ANounNonPerson = "{a:noun:nonperson}"  # noun, singular, with a preceding a/an article, excluding people
     City = "{city}"  # name of the country
     Country = "{country}"  # name of the country
@@ -16,14 +26,15 @@
     Nationality = "{nationality}"  # nationality
     Noun = "{noun}"  # noun, singular
     NounNonPerson = "{noun:nonperson}"  # noun, singular, except of people related
     NounPlural = "{noun:plural}"  # noun, plural
     Number100 = "{number:100}"  # number below 100
     Number1000 = "{number:1000}"  # number below 1000
     Number100k = "{number:100000}"  # number below 100000
+    Person = "{person}"  # place or location
     Place = "{place}"  # place or location
     # Pronoun = "{pronoun}"  # personal pronoun: I, we, they, you
     # PronounSingular3rd = "{pronoun:3s}"  # personal pronoun for 3rd person, singular: he, she, it
     Season = "{season}"  # season
     Verb = "{verb}"  # verb, present simple
     VerbSingular3rd = "{verb:3s}"  # verb in the present simple for 3rd person, singular
     VerbPast = "{verb:past}"  # verb, past
@@ -52,15 +63,15 @@
             VocabularyPlaceholders.VerbProgressive,
         ]
 
 
 @dataclasses.dataclass
 class TopicLevelInfo:
     resource_name: str
-    level: int
+    level: int | str | None = None
 
 
 @dataclasses.dataclass
 class GrammarDescription:
     name: str
     links: list[str]
     exercises: list[str]
```

### Comparing `hmeg-0.1.4/hmeg/exercise_generator.py` & `hmeg-0.1.5/hmeg/exercise_generator.py`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.4/hmeg/miniphrase/ab.toml` & `hmeg-0.1.5/hmeg/miniphrase/ab.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 name="Miniphrase: A, B"
-levels=[]
+levels=[
+    {resource_name="The Art and Science of Learning Languages"},
+]
 links=[]
 exercises=[
     """
     S -> '[afraid] I am afraid I can`t help' P
     P -> 'me' | 'them' | 'you' | 'us' | 'him' | 'her' | 'it' |
     """,
     """
```

### Comparing `hmeg-0.1.4/hmeg/miniphrase/cd.toml` & `hmeg-0.1.5/hmeg/miniphrase/cd.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 name="Miniphrase: C, D"
-levels=[]
+levels=[
+    {resource_name="The Art and Science of Learning Languages"},
+]
 links=[]
 exercises=[
     """
     S -> 'Could/Can I have another' C
     C -> 'cup of tea' | 'cup of coffee' | 'glass of water' | 'glass of juice' | 'beer'
     """,
     """
```

### Comparing `hmeg-0.1.4/hmeg/miniphrase/efg.toml` & `hmeg-0.1.5/hmeg/miniphrase/efg.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 name="Miniphrase: E, F, G"
-levels=[]
+levels=[
+    {resource_name="The Art and Science of Learning Languages"},
+]
 links=[]
 exercises=[
     """
     S -> 'That`s enough' | 'Exactly.' | 'Excuse me (How do I ...)' | 'That`s fine' | 'I am fine, thank you!'
     """,
     """
     S -> 'I`ve forgotten (it).'
```

### Comparing `hmeg-0.1.4/hmeg/miniphrase/h.toml` & `hmeg-0.1.5/hmeg/miniphrase/h.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 name="Miniphrase: H"
-levels=[]
+levels=[
+    {resource_name="The Art and Science of Learning Languages"},
+]
 links=[]
 exercises=[
     """
     S -> 'We had better go now.'
     """,
     """
     S -> 'Half a kilo.' | 'Half the town.'
```

### Comparing `hmeg-0.1.4/hmeg/miniphrase/ikl.toml` & `hmeg-0.1.5/hmeg/miniphrase/ikl.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 name="Miniphrase: I, K, L"
-levels=[]
+levels=[
+    {resource_name="The Art and Science of Learning Languages"},
+]
 links=[]
 exercises=[
     """
     S -> 'That`s a good idea.' | 'That`s very kind of you.'
     """,
     """
     S -> 'I don`t know what to do.' | 'Do you know how to do it?' | 'Do you know Hong Gil Dong?' | 'Do you know a good restaurant?'
```

### Comparing `hmeg-0.1.4/hmeg/miniphrase/mn.toml` & `hmeg-0.1.5/hmeg/miniphrase/mn.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 name="Miniphrase: M, N"
-levels=[]
+levels=[
+    {resource_name="The Art and Science of Learning Languages"},
+]
 links=[]
 exercises=[
     """
     S -> P 'married?'
     P -> 'Is she' | 'Is he' | 'Are they' | 'Are you'
     """,
     """
```

### Comparing `hmeg-0.1.4/hmeg/miniphrase/opr.toml` & `hmeg-0.1.5/hmeg/miniphrase/opr.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 name="Miniphrase: O, P, R"
-levels=[]
+levels=[
+    {resource_name="The Art and Science of Learning Languages"},
+]
 links=[]
 exercises=[
     """
     S -> 'The meeting is off'
     """,
     """
     S -> 'OK.' | 'Is that OK? (=Is that agreed?)' | 'That`s OK. (=Don`t worry about it.)'
```

### Comparing `hmeg-0.1.4/hmeg/miniphrase/stu.toml` & `hmeg-0.1.5/hmeg/miniphrase/stu.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 name="Miniphrase: S, T, U"
-levels=[]
+levels=[
+    {resource_name="The Art and Science of Learning Languages"},
+]
 links=[]
 exercises=[
     """
     S -> '(Thank you) Same to you.'
     """,
     """
     S -> 'Could you please say that again?'
```

### Comparing `hmeg-0.1.4/hmeg/miniphrase/wy.toml` & `hmeg-0.1.5/hmeg/miniphrase/wy.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 name="Miniphrase: W, Y"
-levels=[]
+levels=[
+    {resource_name="The Art and Science of Learning Languages"},
+]
 links=[]
 exercises=[
     """
     S -> 'What do you want?'
     """,
     """
     S -> P 'wants him to do it.'
```

### Comparing `hmeg-0.1.4/hmeg/registry.py` & `hmeg-0.1.5/hmeg/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         The levels are grouped by the resource and sorted in the ascending order.
         """
         res = dict()
         for topic in GrammarRegistry.topics.values():
             for level_descr in topic.levels:
                 if level_descr.resource_name not in res:
                     res[level_descr.resource_name] = list()
-                res[level_descr.resource_name].append(level_descr.level)
+                if level_descr.level:
+                    res[level_descr.resource_name].append(level_descr.level)
 
         for key in res:
             res[key] = sorted(set(res[key]))
         return res
 
     @staticmethod
     def find_topics(topic_name: str) -> list[str]:
```

### Comparing `hmeg-0.1.4/hmeg/topics/1_from_a_to_b_from_c_until_d.toml` & `hmeg-0.1.5/hmeg/topics/1_from_a_to_b_from_c_until_d.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name="From A To B, From C Until D / -에서/부터 -까지"
 levels=[
-    {resource_name="TTMIK", level=1},
+    {resource_name="TTMIK", level="Level 1"},
     {resource_name="HTSK", level="Unit 1"},
 ]
 links=[
     "https://www.howtostudykorean.com/unit1/unit-1-lessons-9-16/lesson-12/#kp4"
 ]
 exercises=[
     """
```

### Comparing `hmeg-0.1.4/hmeg/topics/2_and_with.toml` & `hmeg-0.1.5/hmeg/topics/2_and_with.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name="And, with / -하고, -(이)랑"
 levels=[
-    {resource_name="TTMIK", level=2},
+    {resource_name="TTMIK", level="Level 2"},
     {resource_name="HTSK", level="Unit 1"},
 ]
 links=[
     "https://www.howtostudykorean.com/unit1/unit-1-lessons-9-16/lesson-13/#kp1"
 ]
 exercises=[
     """
```

### Comparing `hmeg-0.1.4/hmeg/topics/2_but_however.toml` & `hmeg-0.1.5/hmeg/topics/2_but_however.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name="But, However / 그렇지만, 그런데"
 levels=[
-    {resource_name="TTMIK", level=2},
+    {resource_name="TTMIK", level="Level 2"},
     {resource_name="HTSK", level="Unit 2"},
     {resource_name="HTSK", level="Unit 4"},
 ]
 links=[
     "https://www.howtostudykorean.com/unit-2-lower-intermediate-korean-grammar/unit-2-lessons-42-50/lesson-47/",
     "https://www.howtostudykorean.com/upper-intermediate-korean-grammar/unit-4-lessons-76-83/lesson-77/#771"
 ]
```

### Comparing `hmeg-0.1.4/hmeg/topics/3_approximately_about.toml` & `hmeg-0.1.5/hmeg/topics/3_approximately_about.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name="Approximately, About / 쯤, 약, 정도"
 levels=[
-    {resource_name="TTMIK", level=3},
+    {resource_name="TTMIK", level="Level 3"},
     {resource_name="HTSK", level="Unit 3"},
     {resource_name="HTSK", level="Unit 5"},
 ]
 links=[
     "https://www.howtostudykorean.com/unit-3-intermediate-korean-grammar/lessons-67-75/lesson-72/#new",
     "https://learnkorean24.com/course/lesson-56/",
     "https://www.topikguide.com/korean-grammar-noun-%EC%AF%A4-almost-around/",
```

### Comparing `hmeg-0.1.4/hmeg/topics/3_in_order_to_for_the_sake_of.toml` & `hmeg-0.1.5/hmeg/topics/3_in_order_to_for_the_sake_of.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name="In order to, For the sake of / 위하다, 위해, 위해서"
 levels=[
-    {resource_name="TTMIK", level=3},
+    {resource_name="TTMIK", level="Level 3"},
     {resource_name="HTSK", level="Unit 1"},
 ]
 links=[
     "https://www.howtostudykorean.com/unit1/unit-1-lessons-9-16/lesson-13/#kp5",
     "https://www.topikguide.com/noun-%EC%9D%84-%EB%A5%BC-%EC%9C%84%ED%95%B4%EC%84%9C-%EC%9C%84%ED%95%B4-and-verb-%EA%B8%B0-%EC%9C%84%ED%95%B4%EC%84%9C-%EC%9C%84%ED%95%B4-korean-grammar/"
 ]
 exercises=[
```

### Comparing `hmeg-0.1.4/hmeg/topics/3_maybe_i_might.toml` & `hmeg-0.1.5/hmeg/topics/3_maybe_i_might.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name="Maybe I might… / -(으)ㄹ 수도 있어요"
 levels=[
-    {resource_name="TTMIK", level=3},
+    {resource_name="TTMIK", level="Level 3"},
     {resource_name="HTSK", level="Unit 5"},
 ]
 links=[
     "https://www.howtostudykorean.com/unit-5/lessons-101-108/lesson-107/#1073c",
     "https://123learnkorean.wordpress.com/2009/08/25/%E3%84%B9%EC%9D%84-%EC%88%98%EB%8F%84-%EC%9E%88%EB%8B%A4-might-verb/"
 ]
 exercises=[
```

### Comparing `hmeg-0.1.4/hmeg/topics/3_well_then_in_that_case.toml` & `hmeg-0.1.5/hmeg/topics/3_well_then_in_that_case.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name="Well then, In that case, If so / 그러면, 그럼"
 levels=[
-    {resource_name="TTMIK", level=3},
+    {resource_name="TTMIK", level="Level 3"},
     {resource_name="HTSK", level="Unit 2"},
 ]
 links=[
     "https://www.howtostudykorean.com/unit-2-lower-intermediate-korean-grammar/unit-2-lessons-42-50/lesson-43/#431"
 ]
 exercises=[
     """
```

### Comparing `hmeg-0.1.4/hmeg/topics/4_i_think_past_future.toml` & `hmeg-0.1.5/hmeg/topics/4_i_think_past_future.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name="I think … (+ future tense) / -(으)ㄴ/(으)ㄹ/ㄴ 것 같다, 한 것 같다, 할 것 같다"
 levels=[
-    {resource_name="TTMIK", level=4},
+    {resource_name="TTMIK", level="Level 4"},
     {resource_name="HTSK", level="Unit 2"},
 ]
 links=[
     "https://www.howtostudykorean.com/unit-2-lower-intermediate-korean-grammar/unit-2-lessons-34-41/lesson-35/#351"
 ]
 exercises=[
     """
```

### Comparing `hmeg-0.1.4/hmeg/topics/4_it_is_ok_to.toml` & `hmeg-0.1.5/hmeg/topics/4_it_is_ok_to.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name="It is okay to…, You don’t have to… / -아/어/여도 돼요, 해도 돼요"
 levels=[
-    {resource_name="TTMIK", level=4},
+    {resource_name="TTMIK", level="Level 4"},
     {resource_name="HTSK", level="Unit 2"},
-    {resource_name="King Sejong Institute Practical Korean", level=3},
+    {resource_name="King Sejong Institute Practical Korean", level="3. Intermediate"},
 ]
 links=[
     "https://www.howtostudykorean.com/unit-2-lower-intermediate-korean-grammar/unit-2-lessons-42-50/lesson-49/"
 ]
 exercises=[
     """
     S -> 'It is ok to {verb}.'
```

### Comparing `hmeg-0.1.4/hmeg/topics/4_to_gradually_get_to_do.toml` & `hmeg-0.1.5/hmeg/topics/4_to_gradually_get_to_do.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name="To gradually/eventually get to do something / -게 되다, 하게 되다"
 levels=[
-    {resource_name="TTMIK", level=4},
+    {resource_name="TTMIK", level="Level 4"},
     {resource_name="HTSK", level="Unit 4"},
 ]
 links=[
     "https://www.howtostudykorean.com/upper-intermediate-korean-grammar/unit-4-lessons-92-100/lesson-94/#941"
 ]
 exercises=[
     """
```

### Comparing `hmeg-0.1.4/hmeg/topics/4_to_try_doing_something.toml` & `hmeg-0.1.5/hmeg/topics/4_to_try_doing_something.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name="To try doing something / -아/어/여 보다, 해 보다"
 levels=[
-    {resource_name="TTMIK", level=4},
+    {resource_name="TTMIK", level="Level 4"},
     {resource_name="HTSK", level="Unit 2"},
 ]
 links=[
     "https://www.howtostudykorean.com/unit-2-lower-intermediate-korean-grammar/unit-2-lessons-26-33/lesson-32/#323"
 ]
 exercises=[
     """
```

### Comparing `hmeg-0.1.4/hmeg/topics/4_you_should_not.toml` & `hmeg-0.1.5/hmeg/topics/4_you_should_not.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name="You shouldn’t…, You’re not supposed to… / -(으)면 안 돼요, 하면 안 돼요"
 levels=[
-    {resource_name="TTMIK", level=4},
+    {resource_name="TTMIK", level="Level 4"},
     {resource_name="HTSK", level="Unit 4"},
 ]
 links=[
     "https://www.howtostudykorean.com/upper-intermediate-korean-grammar/unit-4-lessons-76-83/lesson-80/#802"
 ]
 exercises=[
     """
```

### Comparing `hmeg-0.1.4/hmeg/usecases.py` & `hmeg-0.1.5/hmeg/usecases.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import partial
 import os
 import pandas as pd
 import re
 import toml
 
-from .entities import GrammarDescription, VocabularyPlaceholders
+from .entities import GrammarDescription, VocabularyPlaceholders, VocabularyInfo
 from .registry import GrammarRegistry
 from .vocabulary import Vocabulary
 
 
 def register_miniphrase():
     cur_dir = os.path.split(__file__)[0]
     miniphrase_dir = os.path.join(cur_dir, "miniphrase")
@@ -43,14 +43,35 @@
     for file in os.listdir(vocabs_dir):
         with open(os.path.join(vocabs_dir, file), "r") as f:
             vocab_info = toml.loads(f.read())
         res.append(vocab_info["name"])
     return res
 
 
+def get_vocabularies_info() -> list[VocabularyInfo]:
+    """
+    Returns list with names of the built-in vocabularies.
+    """
+    vocabs_dir = os.path.join(os.path.dirname(__file__), "vocabs")
+    res = []
+    for file in os.listdir(vocabs_dir):
+        vocab = Vocabulary(os.path.join(vocabs_dir, file))
+        res.append(
+            VocabularyInfo(
+                name=vocab.name,
+                num_words=len(vocab.nouns) + len(vocab.verbs) + len(vocab.adjectives) + len(vocab.adverbs),
+                num_nouns=len(vocab.nouns),
+                num_verbs=len(vocab.verbs),
+                num_adjectives=len(vocab.adjectives),
+                num_adverbs=len(vocab.adverbs),
+            )
+        )
+    return res
+
+
 def apply_vocabulary(s: str, vocab: Vocabulary) -> str:
     """
     Takes input string and replaces placeholders with respective minilex entities.
     """
 
     vocab_function = {
         VocabularyPlaceholders.Verb: vocab.random_verb,
@@ -58,14 +79,15 @@
         VocabularyPlaceholders.VerbPast: vocab.random_verb_past,
         VocabularyPlaceholders.VerbProgressive: vocab.random_verb_progressive,
         VocabularyPlaceholders.Noun: vocab.random_noun,
         VocabularyPlaceholders.ANoun: vocab.random_anoun,
         VocabularyPlaceholders.NounPlural: vocab.random_noun_plural,
         VocabularyPlaceholders.NounNonPerson: vocab.random_noun_non_person,
         VocabularyPlaceholders.ANounNonPerson: vocab.random_anoun_non_person,
+        VocabularyPlaceholders.Person: vocab.random_person,
         VocabularyPlaceholders.Number100: partial(vocab.random_number, max=100),
         VocabularyPlaceholders.Number1000: partial(vocab.random_number, max=1000),
         VocabularyPlaceholders.Number100k: partial(vocab.random_number, max=100_000),
         VocabularyPlaceholders.Weekday: partial(vocab.random_weekday),
         VocabularyPlaceholders.Season: partial(vocab.random_season),
         VocabularyPlaceholders.Month: partial(vocab.random_month),
         VocabularyPlaceholders.Adjective: partial(vocab.random_adjective),
```

### Comparing `hmeg-0.1.4/hmeg/vocabs/minilex.toml` & `hmeg-0.1.5/hmeg/vocabs/minilex.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 import = "nanolex.toml"
 name = "Minilex"
 nouns = [ "accident", "anybody", "anything", "apartment", "bag", "beginning", "bottom", "boy", "bread", "brother", "child", "clothes", "cold", "colour", "cry", "damage", "daughter", "earth", "evening", "everybody", "everything", "eye", "fall", "father", "flat", "foot", "front", "fun", "girl", "ground", "half", "hand", "head", "hope", "hour", "husband", "joke", "journey", "lady", "laugh", "lie", "light", "mistake", "moment", "month", "morning", "mother", "mouth", "newspaper", "night", "nobody", "nothing", "pain", "pen", "pencil", "picture", "reason", "relative", "sister", "sleep", "somebody", "son", "sound", "stand", "stop", "suitcase", "sun", "surprise", "talk", "teacher", "thing", "ticket", "tomorrow", "town", "true", "voice", "walk", "weather", "wife", "woman", "word", "worry", "yesterday",]
-adverbs = [ "angrily", "badly", "beautifully", "boringly", "calmly", "certainly", "cheaply", "cheerfully", "cleanly", "clearly", "coldly", "commonly", "dangerously", "deadly", "dearly", "differently", "difficultly", "dirtily", "dryly", "easily", "expensively", "famously", "fast", "firstly", "freely", "fully", "funnily", "gladly", "greatly", "happily", "heavily", "highly", "hotly", "importantly", "impossibly", "interestingly", "kindly", "lastly", "lately", "lightly", "nearly", "necessarily", "newly", "nicely", "openly", "possibly", "prettily", "quietly", "relatively", "rightly", "safely", "shortly", "slowly", "sorrily", "strangely", "strongly", "stupidly", "surprisingly", "terribly", "tiredly", "urgently", "usually", "warmly", "wonderfully", "wrongly",]
+adverbs = [ "angrily", "badly", "beautifully", "boringly", "calmly", "certainly", "cheaply", "cheerfully", "cleanly", "clearly", "coldly", "commonly", "dangerously", "deadly", "dearly", "differently", "difficultly", "dirtily", "dryly", "easily", "expensively", "famously", "fast", "firstly", "freely", "fully", "funnily", "gladly", "greatly", "happily", "heavily", "highly", "hotly", "importantly", "impossibly", "interestingly", "kindly", "lastly", "lately", "lightly", "nearly", "necessarily", "newly", "nicely", "now", "openly", "possibly", "prettily", "quietly", "relatively", "rightly", "safely", "shortly", "slowly", "sorrily", "strangely", "strongly", "stupidly", "surprisingly", "terribly", "tiredly", "urgently", "usually", "warmly", "wonderfully", "wrongly",]
 adjectives = [ "angry", "bad", "beautiful", "boring", "calm", "certain", "cheap", "cheerful", "clean", "clear", "cold", "common", "dangerous", "dead", "dear", "difficult", "dirty", "dry", "easy", "expensive", "famous", "fast", "finished", "fun", "funny", "glad", "happy", "heavy", "ill", "impossible", "interesting", "kind", "late", "light", "mean", "near", "necessary", "nice", "possible", "pretty", "quiet", "relative", "safe", "several", "short", "shut", "slow", "sorry", "strange", "strong", "stupid", "surprised", "tall", "terrible", "tired", "urgent", "usual", "warm", "whole", "wonderful", "worst", "wrong",]
 verbs = [ "arrive", "ask", "become", "begin", "believe", "borrow", "bring", "clean", "continue", "cry", "damage", "drop", "eat", "fall", "feel", "finish", "forget", "hold", "hope", "hurt", "joke", "keep", "laugh", "leave", "lend", "lie", "listen", "look for", "mean", "meet", "pay", "put", "remember", "shut", "sing", "speak", "stand", "stay", "stop", "suggest", "talk", "teach", "understand", "wait", "walk", "worry", "write",]
```

### Comparing `hmeg-0.1.4/hmeg/vocabs/nanolex.toml` & `hmeg-0.1.5/hmeg/vocabs/nanolex.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.4/hmeg/vocabulary.py` & `hmeg-0.1.5/hmeg/vocabulary.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,21 @@
 # dictionary with fixes for conjugation of the mlconjug3
 verbs_singular_3rd = {
     'borrow': 'borrows',
     'hurt': 'hurts',
     'look for': 'looks for',
     'name': 'names',
 }
+verbs_progressive = {
+    'look for': 'looking for',
+}
+verbs_past = {
+    'borrow': 'borrowed',
+    'look for': 'looked for',
+}
 
 
 class Vocabulary:
     vocab_file: str | None  # file with the current vocabulary
     name: str | None
     adjectives: list[str]
     adverbs: list[str]
@@ -56,15 +63,15 @@
     person_nouns = [
         "anybody", "boy", "brother", "child", "daughter", "everybody",
         "family", "father", "friend", "girl", "husband", "lady", "man", "mother",
         "nobody", "people", "person", "relative", "sister", "somebody", "son",
         "teacher", "wife", "woman"
     ]
     places = [
-        "airport", "apartment", "country", "flat", "home", "house", "road", "room",
+        "airport", "apartment", "country", "flat", "home", "hospital", "house", "road", "room",
         "school", "shop", "side", "street", "town", "work", "bathroom"
     ]
 
     def __init__(self, vocab_file: str | None = None):
         self.vocab_file = vocab_file
         self.name = None
         self.adjectives = []
@@ -105,20 +112,26 @@
             cur_verb.name,
             cur_verb["indicative"]["indicative present"]["he/she/it"]
         )
         return conj_verb
 
     def random_verb_past(self) -> str:
         cur_verb = conj.conjugate(self.random_verb())
-        conj_verb = cur_verb["indicative"]["indicative past tense"]["I"]
+        conj_verb = verbs_past.get(
+            cur_verb.name,
+            cur_verb["indicative"]["indicative past tense"]["I"]
+        )
         return conj_verb
 
     def random_verb_progressive(self) -> str:
         cur_verb = conj.conjugate(self.random_verb())
-        conj_verb = cur_verb["indicative"]["indicative present continuous"]["I"]
+        conj_verb = verbs_progressive.get(
+            cur_verb.name,
+            cur_verb["indicative"]["indicative present continuous"]["I"]
+        )
         return conj_verb
 
     def random_noun(self) -> str:
         return random.choice(self.nouns)
 
     def random_anoun(self) -> str:
         noun = self.random_noun()
@@ -136,14 +149,18 @@
         return res
 
     def random_anoun_non_person(self) -> str:
         noun = self.random_noun_non_person()
         article = "an" if noun[0] in VOWELS else "a"
         return f"{article} {noun}"
 
+    def random_person(self) -> str:
+        res = random.choice(self.person_nouns)
+        return res
+
     def random_adjective(self) -> str:
         return random.choice(self.adjectives)
 
     def random_adverb(self) -> str:
         return random.choice(self.adverbs)
 
     def random_weekday(self) -> str:
@@ -170,7 +187,12 @@
     def random_nationality(self) -> str:
         return random.choice(self.nationalities)
 
 
 def load_minilex() -> Vocabulary:
     cur_dir = os.path.split(__file__)[0]
     return Vocabulary.load(os.path.join(cur_dir, "vocabs", "minilex.toml"))
+
+
+def load_nanolex() -> Vocabulary:
+    cur_dir = os.path.split(__file__)[0]
+    return Vocabulary.load(os.path.join(cur_dir, "vocabs", "nanolex.toml"))
```

### Comparing `hmeg-0.1.4/PKG-INFO` & `hmeg-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmeg
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generator of exercises for practicing speaking for language learning.
 Home-page: https://github.com/yurytsoy/hmeg
 License: MIT
 Author: Yury Choi
 Author-email: yurytsoy@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

