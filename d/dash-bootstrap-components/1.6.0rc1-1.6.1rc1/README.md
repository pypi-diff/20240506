# Comparing `tmp/dash_bootstrap_components-1.6.0rc1.tar.gz` & `tmp/dash_bootstrap_components-1.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_bootstrap_components-1.6.0rc1.tar", last modified: Sun Apr 14 18:11:43 2024, max compression
+gzip compressed data, was "dash_bootstrap_components-1.6.1rc1.tar", last modified: Mon May  6 17:15:01 2024, max compression
```

## Comparing `dash_bootstrap_components-1.6.0rc1.tar` & `dash_bootstrap_components-1.6.1rc1.tar`

### file list

```diff
@@ -1,101 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:11:43.277799 dash_bootstrap_components-1.6.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-04-14 18:11:43.277799 dash_bootstrap_components-1.6.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:11:43.261799 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:11:43.277799 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Accordion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/AccordionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Badge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Breadcrumb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Button.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ButtonGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardBody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardFooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardImg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardImgOverlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardLink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Carousel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Checklist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Col.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Container.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/DropdownMenu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/DropdownMenuItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Fade.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/FormFeedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/FormFloating.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/FormText.py
--rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/InputGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/InputGroupText.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Label.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ListGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ListGroupItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Modal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalBody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalFooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalTitle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Nav.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavLink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Navbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavbarBrand.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavbarSimple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavbarToggler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Offcanvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Popover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/PopoverBody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/PopoverHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/RadioButton.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/RadioItems.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Row.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Textarea.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   235048 2024-04-14 18:11:28.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/dash_bootstrap_components.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   362389 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/themes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:11:43.277799 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-04-14 18:11:43.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-14 18:11:43.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:11:43.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 18:11:43.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 18:11:43.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/landing-page.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-14 18:11:43.281799 dash_bootstrap_components-1.6.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:11:43.277799 dash_bootstrap_components-1.6.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_components_as_props.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_navlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_popover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_positional_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_xss_links.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:15:01.316337 dash_bootstrap_components-1.6.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-06 17:15:01.316337 dash_bootstrap_components-1.6.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:15:01.300337 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:15:01.316337 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Accordion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/AccordionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Breadcrumb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ButtonGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardFooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardImg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardImgOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardLink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Carousel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Checklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Col.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/DropdownMenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/DropdownMenuItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Fade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/FormFeedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/FormFloating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/FormText.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/InputGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/InputGroupText.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ListGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ListGroupItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalFooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalTitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Nav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavLink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Navbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavbarBrand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavbarSimple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavbarToggler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Offcanvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Popover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/PopoverBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/PopoverHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/RadioButton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/RadioItems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Textarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   233998 2024-05-06 17:14:46.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/dash_bootstrap_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   363181 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/themes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:15:01.316337 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-06 17:15:01.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-06 17:15:01.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:15:01.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 17:15:01.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 17:15:01.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/landing-page.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-06 17:15:01.316337 dash_bootstrap_components-1.6.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:15:01.316337 dash_bootstrap_components-1.6.1rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_components_as_props.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_navlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_popover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_positional_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_version.py
```

### Comparing `dash_bootstrap_components-1.6.0rc1/LICENSE` & `dash_bootstrap_components-1.6.1rc1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
   replaced with your own identifying information. (Don't include
   the brackets!)  The text should be enclosed in the appropriate
   comment syntax for the file format. We also recommend that a
   file or class name and description of purpose be included on the
   same "printed page" as the copyright notice for easier
   identification within third-party archives.
 
-Copyright 2018-2022 Faculty Science Limited
+Copyright 2018-2024 Faculty Science Limited
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `dash_bootstrap_components-1.6.0rc1/PKG-INFO` & `dash_bootstrap_components-1.6.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-bootstrap-components
-Version: 1.6.0rc1
+Version: 1.6.1rc1
 Summary: Bootstrap themed components for use in Plotly Dash
 Home-page: https://dash-bootstrap-components.opensource.faculty.ai/
 Author: Faculty
 Author-email: opensource@faculty.ai
 License: Apache Software License
 Project-URL: Bug Reports, https://github.com/facultyai/dash-bootstrap-components/issues
 Project-URL: Source, https://github.com/facultyai/dash-bootstrap-components/
@@ -110,15 +110,15 @@
 for new features please feel free to make a [feature request][feature-request].
 If you would like to submit a pull request, please read our
 [contributing guide][contribution-guide].
 
 ## Copyright and license
 
 Code and documentation is copyright [Faculty Science Ltd.][faculty]
-2018-2022, and released under the [Apache 2.0 license](./LICENSE.txt)
+2018-2024, and released under the [Apache 2.0 license](./LICENSE.txt)
 
 [dash-homepage]: https://dash.plot.ly/
 [dash-docs-external]: https:/dash.plot.ly/external-resources
 [bootstrap-homepage]: https://getbootstrap.com/
 [dbc-repo]: https://github.com/facultyai/dash-bootstrap-components
 [reactstrap-homepage]: https://reactstrap.github.io/
 [docs-homepage]: https://dash-bootstrap-components.opensource.faculty.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.6.0rc1
+Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.6.1rc1
 Summary: Bootstrap themed components for use in Plotly Dash Home-page: https://
 dash-bootstrap-components.opensource.faculty.ai/ Author: Faculty Author-email:
 opensource@faculty.ai License: Apache Software License Project-URL: Bug
 Reports, https://github.com/facultyai/dash-bootstrap-components/issues Project-
 URL: Source, https://github.com/facultyai/dash-bootstrap-components/
 Classifier: Framework :: Dash Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -40,15 +40,15 @@
 Bootstrap components. See our [_documentation_][docs-components] for a full
 list of available components. ## Contributing We welcome contributions to
 _dash-bootstrap-components_. If you find a bug or something is unclear please
 [submit a bug report][bug-report], if you have ideas for new features please
 feel free to make a [feature request][feature-request]. If you would like to
 submit a pull request, please read our [contributing guide][contribution-
 guide]. ## Copyright and license Code and documentation is copyright [Faculty
-Science Ltd.][faculty] 2018-2022, and released under the [Apache 2.0 license]
+Science Ltd.][faculty] 2018-2024, and released under the [Apache 2.0 license]
 (./LICENSE.txt) [dash-homepage]: https://dash.plot.ly/ [dash-docs-external]:
 https:/dash.plot.ly/external-resources [bootstrap-homepage]: https://
 getbootstrap.com/ [dbc-repo]: https://github.com/facultyai/dash-bootstrap-
 components [reactstrap-homepage]: https://reactstrap.github.io/ [docs-
 homepage]: https://dash-bootstrap-components.opensource.faculty.ai [docs-
 components]: https://dash-bootstrap-components.opensource.faculty.ai/l/
 components [bootstrapcdn]: https://www.bootstrapcdn.com/ [faculty]: https://
```

### Comparing `dash_bootstrap_components-1.6.0rc1/README.md` & `dash_bootstrap_components-1.6.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/__init__.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Accordion.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Accordion.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/AccordionItem.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/AccordionItem.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Alert.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Alert.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Badge.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Badge.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Breadcrumb.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Breadcrumb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
 class Breadcrumb(Component):
     """A Breadcrumb component.
-
+Use breadcrumbs to create a navigation breadcrumb in your app.
 
 Keyword arguments:
 
 - id (string; optional):
     The ID of this component, used to identify dash components in
     callbacks. The ID needs to be unique across all of the components
     in an app.
```

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Button.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Button.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ButtonGroup.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ButtonGroup.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Card.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Card.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardBody.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardBody.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardFooter.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardFooter.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardGroup.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardGroup.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardHeader.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardHeader.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardImg.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardImg.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardImgOverlay.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardImgOverlay.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardLink.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardLink.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Carousel.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Carousel.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Checkbox.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Checkbox.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Checklist.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Checklist.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Col.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Col.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Collapse.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Collapse.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Container.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Container.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/DropdownMenu.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/DropdownMenu.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/DropdownMenuItem.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/DropdownMenuItem.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Fade.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Fade.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Form.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Form.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/FormFeedback.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/FormFeedback.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/FormFloating.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/FormFloating.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/FormText.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/FormText.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Input.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Input.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/InputGroup.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/InputGroup.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/InputGroupText.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/InputGroupText.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Label.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Label.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ListGroup.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ListGroup.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ListGroupItem.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ListGroupItem.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Modal.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Modal.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,17 +46,29 @@
 - class_name (string; optional):
     Often used with CSS to style elements with common properties.
 
 - contentClassName (string; optional):
     **DEPRECATED** Use `content_class_name` instead  CSS class to
     apply to the modal content.
 
+- contentStyle (dict; optional):
+    Inline CSS styles to apply to the content.
+
 - content_class_name (string; optional):
     CSS class to apply to the modal content.
 
+- content_style (dict; optional):
+    Inline CSS styles to apply to the content.
+
+- dialogStyle (dict; optional):
+    Inline CSS styles to apply to the dialog.
+
+- dialog_style (dict; optional):
+    Inline CSS styles to apply to the dialog.
+
 - enforceFocus (boolean; optional):
     When True The modal will prevent focus from leaving the Modal
     while open.
 
 - fade (boolean; optional):
     Set to False for a modal that simply appears rather than fades
     into view.
@@ -109,18 +121,18 @@
 - zindex (number | string; optional):
     Set the z-index of the modal. Default 1050."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'dash_bootstrap_components'
     _type = 'Modal'
     @_explicitize_args
-    def __init__(self, children=None, id=Component.UNDEFINED, style=Component.UNDEFINED, class_name=Component.UNDEFINED, className=Component.UNDEFINED, tag=Component.UNDEFINED, is_open=Component.UNDEFINED, centered=Component.UNDEFINED, scrollable=Component.UNDEFINED, autofocus=Component.UNDEFINED, autoFocus=Component.UNDEFINED, enforceFocus=Component.UNDEFINED, size=Component.UNDEFINED, role=Component.UNDEFINED, labelledby=Component.UNDEFINED, labelledBy=Component.UNDEFINED, keyboard=Component.UNDEFINED, backdrop=Component.UNDEFINED, modal_class_name=Component.UNDEFINED, modalClassName=Component.UNDEFINED, backdrop_class_name=Component.UNDEFINED, backdropClassName=Component.UNDEFINED, content_class_name=Component.UNDEFINED, contentClassName=Component.UNDEFINED, fade=Component.UNDEFINED, fullscreen=Component.UNDEFINED, zindex=Component.UNDEFINED, zIndex=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['children', 'id', 'autoFocus', 'autofocus', 'backdrop', 'backdropClassName', 'backdrop_class_name', 'centered', 'className', 'class_name', 'contentClassName', 'content_class_name', 'enforceFocus', 'fade', 'fullscreen', 'is_open', 'keyboard', 'labelledBy', 'labelledby', 'modalClassName', 'modal_class_name', 'role', 'scrollable', 'size', 'style', 'tag', 'zIndex', 'zindex']
+    def __init__(self, children=None, id=Component.UNDEFINED, style=Component.UNDEFINED, dialog_style=Component.UNDEFINED, dialogStyle=Component.UNDEFINED, content_style=Component.UNDEFINED, contentStyle=Component.UNDEFINED, class_name=Component.UNDEFINED, className=Component.UNDEFINED, tag=Component.UNDEFINED, is_open=Component.UNDEFINED, centered=Component.UNDEFINED, scrollable=Component.UNDEFINED, autofocus=Component.UNDEFINED, autoFocus=Component.UNDEFINED, enforceFocus=Component.UNDEFINED, size=Component.UNDEFINED, role=Component.UNDEFINED, labelledby=Component.UNDEFINED, labelledBy=Component.UNDEFINED, keyboard=Component.UNDEFINED, backdrop=Component.UNDEFINED, modal_class_name=Component.UNDEFINED, modalClassName=Component.UNDEFINED, backdrop_class_name=Component.UNDEFINED, backdropClassName=Component.UNDEFINED, content_class_name=Component.UNDEFINED, contentClassName=Component.UNDEFINED, fade=Component.UNDEFINED, fullscreen=Component.UNDEFINED, zindex=Component.UNDEFINED, zIndex=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['children', 'id', 'autoFocus', 'autofocus', 'backdrop', 'backdropClassName', 'backdrop_class_name', 'centered', 'className', 'class_name', 'contentClassName', 'contentStyle', 'content_class_name', 'content_style', 'dialogStyle', 'dialog_style', 'enforceFocus', 'fade', 'fullscreen', 'is_open', 'keyboard', 'labelledBy', 'labelledby', 'modalClassName', 'modal_class_name', 'role', 'scrollable', 'size', 'style', 'tag', 'zIndex', 'zindex']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['children', 'id', 'autoFocus', 'autofocus', 'backdrop', 'backdropClassName', 'backdrop_class_name', 'centered', 'className', 'class_name', 'contentClassName', 'content_class_name', 'enforceFocus', 'fade', 'fullscreen', 'is_open', 'keyboard', 'labelledBy', 'labelledby', 'modalClassName', 'modal_class_name', 'role', 'scrollable', 'size', 'style', 'tag', 'zIndex', 'zindex']
+        self.available_properties = ['children', 'id', 'autoFocus', 'autofocus', 'backdrop', 'backdropClassName', 'backdrop_class_name', 'centered', 'className', 'class_name', 'contentClassName', 'contentStyle', 'content_class_name', 'content_style', 'dialogStyle', 'dialog_style', 'enforceFocus', 'fade', 'fullscreen', 'is_open', 'keyboard', 'labelledBy', 'labelledby', 'modalClassName', 'modal_class_name', 'role', 'scrollable', 'size', 'style', 'tag', 'zIndex', 'zindex']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args if k != 'children'}
 
         super(Modal, self).__init__(children=children, **args)
```

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalBody.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalBody.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalFooter.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalFooter.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalHeader.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalHeader.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalTitle.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalTitle.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Nav.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Nav.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavItem.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavItem.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavLink.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavLink.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Navbar.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Navbar.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavbarBrand.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavbarBrand.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavbarSimple.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavbarSimple.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavbarToggler.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavbarToggler.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Offcanvas.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Offcanvas.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Pagination.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Pagination.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Placeholder.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Placeholder.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Popover.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Popover.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/PopoverBody.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/PopoverBody.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/PopoverHeader.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/PopoverHeader.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Progress.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Progress.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/RadioButton.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/RadioButton.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/RadioItems.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/RadioItems.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Row.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Row.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Select.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Select.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Spinner.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Spinner.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Stack.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Stack.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Switch.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Switch.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Tab.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Tab.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Table.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Table.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Tabs.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Tabs.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Textarea.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Textarea.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Toast.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Toast.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Tooltip.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Tooltip.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/__init__.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/dash_bootstrap_components.min.js` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/dash_bootstrap_components.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -698,41 +698,14 @@
                     key: c,
                     ref: u,
                     props: s,
                     _owner: o.current
                 }
             }
             t.jsx = c, t.jsxs = c
-        }, (e, t, n) => {
-            "use strict";
-            t.J = void 0;
-            var r = n(20);
-            t.J = function(e) {
-                if (!e) return r.BLANK_URL;
-                var t, n, a = e;
-                do {
-                    t = (a = (n = a, n.replace(r.ctrlCharactersRegex, "").replace(r.htmlEntitiesRegex, (function(e, t) {
-                        return String.fromCharCode(t)
-                    }))).replace(r.htmlCtrlEntityRegex, "").replace(r.ctrlCharactersRegex, "").trim()).match(r.ctrlCharactersRegex) || a.match(r.htmlEntitiesRegex) || a.match(r.htmlCtrlEntityRegex)
-                } while (t && t.length > 0);
-                var s = a;
-                if (!s) return r.BLANK_URL;
-                if (function(e) {
-                        return r.relativeFirstCharacters.indexOf(e[0]) > -1
-                    }(s)) return s;
-                var o = s.match(r.urlSchemeRegex);
-                if (!o) return s;
-                var i = o[0];
-                return r.invalidProtocolRegex.test(i) ? r.BLANK_URL : s
-            }
-        }, (e, t) => {
-            "use strict";
-            Object.defineProperty(t, "__esModule", {
-                value: !0
-            }), t.BLANK_URL = t.relativeFirstCharacters = t.urlSchemeRegex = t.ctrlCharactersRegex = t.htmlCtrlEntityRegex = t.htmlEntitiesRegex = t.invalidProtocolRegex = void 0, t.invalidProtocolRegex = /^([^\w]*)(javascript|data|vbscript)/im, t.htmlEntitiesRegex = /&#(\w+)(^\w|;)?/g, t.htmlCtrlEntityRegex = /&(newline|tab);/gi, t.ctrlCharactersRegex = /[\u0000-\u001F\u007F-\u009F\u2000-\u200D\uFEFF]/gim, t.urlSchemeRegex = /^.+(:|&colon;)/gim, t.relativeFirstCharacters = [".", "/"], t.BLANK_URL = "about:blank"
         }],
         t = {};
 
     function n(r) {
         var a = t[r];
         if (void 0 !== a) return a.exports;
         var s = t[r] = {
@@ -806,80 +779,80 @@
             if (Object.getOwnPropertySymbols) {
                 var o = Object.getOwnPropertySymbols(e);
                 for (r = 0; r < o.length; r++) n = o[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (a[n] = e[n])
             }
             return a
         }
         n.r(r), n.d(r, {
-            Accordion: () => Ke,
-            AccordionItem: () => We,
-            Alert: () => Pt,
-            Badge: () => Wt,
-            Breadcrumb: () => en,
-            Button: () => sn,
-            ButtonGroup: () => dn,
-            Card: () => Bn,
-            CardBody: () => Hn,
-            CardFooter: () => qn,
-            CardGroup: () => Jn,
-            CardHeader: () => er,
-            CardImg: () => rr,
-            CardImgOverlay: () => or,
-            CardLink: () => cr,
-            Carousel: () => wr,
-            Checkbox: () => Er,
-            Checklist: () => ua,
-            Col: () => va,
-            Collapse: () => Oa,
-            Container: () => ka,
-            DropdownMenu: () => $i,
-            DropdownMenuItem: () => Fi,
-            Fade: () => Hi,
-            Form: () => wl,
-            FormFeedback: () => jl,
-            FormFloating: () => Cl,
-            FormText: () => Ll,
-            Input: () => Ul,
-            InputGroup: () => Jl,
-            InputGroupText: () => ec,
-            Label: () => cc,
-            ListGroup: () => bc,
-            ListGroupItem: () => xc,
-            Modal: () => cu,
-            ModalBody: () => mu,
-            ModalFooter: () => vu,
-            ModalHeader: () => ju,
-            ModalTitle: () => Ru,
-            Nav: () => Au,
-            NavItem: () => Rd,
-            NavLink: () => Id,
-            Navbar: () => hd,
-            NavbarBrand: () => xd,
-            NavbarSimple: () => Cd,
-            NavbarToggler: () => Nd,
-            Offcanvas: () => Md,
-            Pagination: () => Qd,
-            Placeholder: () => ip,
-            Popover: () => Mp,
-            PopoverBody: () => Kp,
-            PopoverHeader: () => Wp,
-            Progress: () => af,
-            RadioButton: () => df,
-            RadioItems: () => cf,
-            Row: () => hf,
-            Select: () => xf,
-            Spinner: () => Pf,
-            Stack: () => Lf,
-            Switch: () => If,
-            Tab: () => Ff,
-            Table: () => pm,
-            Tabs: () => im,
-            Textarea: () => gm,
-            Toast: () => Pm,
-            Tooltip: () => Sm
+            Accordion: () => Be,
+            AccordionItem: () => He,
+            Alert: () => jt,
+            Badge: () => Ht,
+            Breadcrumb: () => Xt,
+            Button: () => tn,
+            ButtonGroup: () => on,
+            Card: () => $n,
+            CardBody: () => Fn,
+            CardFooter: () => Kn,
+            CardGroup: () => Vn,
+            CardHeader: () => Xn,
+            CardImg: () => Zn,
+            CardImgOverlay: () => nr,
+            CardLink: () => sr,
+            Carousel: () => vr,
+            Checkbox: () => xr,
+            Checklist: () => oa,
+            Col: () => ga,
+            Collapse: () => ha,
+            Container: () => wa,
+            DropdownMenu: () => Si,
+            DropdownMenuItem: () => Li,
+            Fade: () => Fi,
+            Form: () => vl,
+            FormFeedback: () => Ol,
+            FormFloating: () => El,
+            FormText: () => Tl,
+            Input: () => Bl,
+            InputGroup: () => Vl,
+            InputGroupText: () => Xl,
+            Label: () => sc,
+            ListGroup: () => pc,
+            ListGroupItem: () => yc,
+            Modal: () => ou,
+            ModalBody: () => du,
+            ModalFooter: () => bu,
+            ModalHeader: () => wu,
+            ModalTitle: () => Cu,
+            Nav: () => Lu,
+            NavItem: () => Cd,
+            NavLink: () => Dd,
+            Navbar: () => gd,
+            NavbarBrand: () => hd,
+            NavbarSimple: () => jd,
+            NavbarToggler: () => xd,
+            Offcanvas: () => $d,
+            Pagination: () => Yd,
+            Placeholder: () => ap,
+            Popover: () => $p,
+            PopoverBody: () => Fp,
+            PopoverHeader: () => Kp,
+            Progress: () => tf,
+            RadioButton: () => lf,
+            RadioItems: () => sf,
+            Row: () => gf,
+            Select: () => hf,
+            Spinner: () => Ef,
+            Stack: () => Sf,
+            Switch: () => Df,
+            Tab: () => If,
+            Table: () => cm,
+            Tabs: () => am,
+            Textarea: () => pm,
+            Toast: () => Em,
+            Tooltip: () => Pm
         });
         var i = n(0),
             l = n.n(i),
             c = n(15),
             u = n.n(c);
 
         function d(e) {
@@ -1026,40 +999,40 @@
                 var s = t[a];
                 s || 0 === s ? function(e) {
                     return !(!e || !D.test(e))
                 }(a) ? r += a + "(" + s + ") " : n += R(a) + ": " + s + ";" : e.style.removeProperty(R(a))
             })), r && (n += "transform: " + r + ";"), e.style.cssText += ";" + n
         };
 
-        function $(e, t) {
-            return $ = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function I(e, t) {
+            return I = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, $(e, t)
+            }, I(e, t)
         }
-        const I = window.ReactDOM;
-        var A = n.n(I);
-        const F = l().createContext(null);
-        var M = "unmounted",
+        const $ = window.ReactDOM;
+        var A = n.n($);
+        const M = l().createContext(null);
+        var F = "unmounted",
             B = "exited",
             z = "entering",
             K = "entered",
             H = "exiting",
-            U = function(e) {
+            W = function(e) {
                 var t, n;
 
                 function r(t, n) {
                     var r;
                     r = e.call(this, t, n) || this;
                     var a, s = n && !n.isMounting ? t.enter : t.appear;
-                    return r.appearStatus = null, t.in ? s ? (a = B, r.appearStatus = z) : a = K : a = t.unmountOnExit || t.mountOnEnter ? M : B, r.state = {
+                    return r.appearStatus = null, t.in ? s ? (a = B, r.appearStatus = z) : a = K : a = t.unmountOnExit || t.mountOnEnter ? F : B, r.state = {
                         status: a
                     }, r.nextCallback = null, r
                 }
-                n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, $(t, n), r.getDerivedStateFromProps = function(e, t) {
-                    return e.in && t.status === M ? {
+                n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, I(t, n), r.getDerivedStateFromProps = function(e, t) {
+                    return e.in && t.status === F ? {
                         status: B
                     } : null
                 };
                 var a = r.prototype;
                 return a.componentDidMount = function() {
                     this.updateStatus(!0, this.appearStatus)
                 }, a.componentDidUpdate = function(e) {
@@ -1086,15 +1059,15 @@
                                 n && function(e) {
                                     e.scrollTop
                                 }(n)
                             }
                             this.performEnter(e)
                         } else this.performExit();
                     else this.props.unmountOnExit && this.state.status === B && this.setState({
-                        status: M
+                        status: F
                     })
                 }, a.performEnter = function(e) {
                     var t = this,
                         n = this.props.enter,
                         r = this.context ? this.context.isMounting : e,
                         a = this.props.nodeRef ? [r] : [A().findDOMNode(this), r],
                         s = a[0],
@@ -1159,40 +1132,40 @@
                                 o = a[1];
                             this.props.addEndListener(s, o)
                         }
                         null != e && setTimeout(this.nextCallback, e)
                     } else setTimeout(this.nextCallback, 0)
                 }, a.render = function() {
                     var e = this.state.status;
-                    if (e === M) return null;
+                    if (e === F) return null;
                     var t = this.props,
                         n = t.children,
                         r = (t.in, t.mountOnEnter, t.unmountOnExit, t.appear, t.enter, t.exit, t.timeout, t.addEndListener, t.onEnter, t.onEntering, t.onEntered, t.onExit, t.onExiting, t.onExited, t.nodeRef, s(t, ["children", "in", "mountOnEnter", "unmountOnExit", "appear", "enter", "exit", "timeout", "addEndListener", "onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited", "nodeRef"]));
-                    return l().createElement(F.Provider, {
+                    return l().createElement(M.Provider, {
                         value: null
                     }, "function" == typeof n ? n(e, r) : l().cloneElement(l().Children.only(n), r))
                 }, r
             }(l().Component);
 
-        function W() {}
-        U.contextType = F, U.propTypes = {}, U.defaultProps = {
+        function U() {}
+        W.contextType = M, W.propTypes = {}, W.defaultProps = {
             in: !1,
             mountOnEnter: !1,
             unmountOnExit: !1,
             appear: !1,
             enter: !0,
             exit: !0,
-            onEnter: W,
-            onEntering: W,
-            onEntered: W,
-            onExit: W,
-            onExiting: W,
-            onExited: W
-        }, U.UNMOUNTED = M, U.EXITED = B, U.ENTERING = z, U.ENTERED = K, U.EXITING = H;
-        const q = U,
+            onEnter: U,
+            onEntering: U,
+            onEntered: U,
+            onExit: U,
+            onExiting: U,
+            onExited: U
+        }, W.UNMOUNTED = F, W.EXITED = B, W.ENTERING = z, W.ENTERED = K, W.EXITING = H;
+        const q = W,
             V = !("undefined" == typeof window || !window.document || !window.document.createElement);
         var G = !1,
             Y = !1;
         try {
             var X = {
                 get passive() {
                     return G = !0
@@ -1626,19 +1599,18 @@
             }(e, t) || a(e, t) || function() {
                 throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
             }()
         }
         const Re = p((function(e) {
             return null === e ? "Null" : void 0 === e ? "Undefined" : Object.prototype.toString.call(e).slice(8, -1)
         }));
-        var De = n(19),
-            Le = function(e) {
+        var De = function(e) {
                 return e && !Array.isArray(e) ? [e] : e
             },
-            $e = function(e) {
+            Le = function(e) {
                 return e.props._dashprivate_layout && e.props._dashprivate_layout.props ? e.props._dashprivate_layout.props : e.props
             },
             Ie = function(e) {
                 return "Object" === Re(e) ? Object.entries(e).map((function(e) {
                     var t = Se(e, 2),
                         n = t[0],
                         r = t[1];
@@ -1649,46 +1621,36 @@
                 })) : "Array" === Re(e) && e.length > 0 && ["String", "Number"].includes(Re(e[0])) ? e.map((function(e) {
                     return {
                         label: String(e),
                         value: e
                     }
                 })) : e
             },
-            Ae = function(e) {
+            $e = function(e) {
                 return "object" !== Te(e) ? e : "{" + Object.keys(e).sort().map((function(t) {
                     return JSON.stringify(t) + ":" + ((n = e[t]) && n.wild || JSON.stringify(n));
                     var n
                 })).join(",") + "}"
             },
-            Fe = function(e, t) {
-                var n = (0, i.useMemo)((function() {
-                    return e ? (0, De.J)(e) : void 0
-                }), [e]);
-                return (0, i.useEffect)((function() {
-                    n && n !== e && t({
-                        _dash_error: new Error("Dangerous link detected:: ".concat(e))
-                    })
-                }), [e, n]), n
-            },
-            Me = l().createContext({}),
-            Be = ["children", "active_item", "always_open", "start_collapsed", "loading_state", "key", "setProps", "class_name", "className"],
-            ze = function(n) {
+            Ae = l().createContext({}),
+            Me = ["children", "active_item", "always_open", "start_collapsed", "loading_state", "key", "setProps", "class_name", "className"],
+            Fe = function(n) {
                 var r = n.children,
                     s = n.active_item,
                     c = n.always_open,
                     u = n.start_collapsed,
                     d = n.loading_state,
                     p = n.key,
                     f = n.setProps,
                     g = n.class_name,
                     b = n.className,
-                    y = o(n, Be);
-                r = Le(r), (0, i.useEffect)((function() {
+                    y = o(n, Me);
+                r = De(r), (0, i.useEffect)((function() {
                     if (f && void 0 === s && !u) {
-                        var e = r && ($e(r[0]).item_id || "item-0");
+                        var e = r && (Le(r[0]).item_id || "item-0");
                         f({
                             active_item: c ? [e] : e
                         })
                     }
                 }), []);
                 var h = function(e) {
                         var n, r;
@@ -1701,16 +1663,16 @@
                         }(r) || a(r) || function() {
                             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                         }()) : [e] : s !== e ? e : null, f({
                             active_item: n
                         }))
                     },
                     v = r && r.map((function(e, t) {
-                        var n = $e(e).item_id || "item-".concat(t);
-                        return l().createElement(Me.Provider, {
+                        var n = Le(e).item_id || "item-".concat(t);
+                        return l().createElement(Ae.Provider, {
                             key: n,
                             value: {
                                 toggle: h,
                                 idx: t
                             }
                         }, e)
                     }));
@@ -1719,20 +1681,20 @@
                     "data-dash-is-loading": d && d.is_loading || void 0,
                     activeKey: s,
                     defaultActiveKey: u ? null : s,
                     alwaysOpen: c,
                     className: g || b
                 }, m(["setProps", "persistence", "persistence_type", "persisted_props"], y)), v)
             };
-        ze.defaultProps = {
+        Fe.defaultProps = {
             persisted_props: ["active_item"],
             persistence_type: "local",
             start_collapsed: !1,
             always_open: !1
-        }, ze.propTypes = {
+        }, Fe.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             flush: u().bool,
@@ -1744,137 +1706,137 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["active_item"])),
             persistence_type: u().oneOf(["local", "session", "memory"])
         };
-        const Ke = ze;
-        var He = ["title", "item_id", "loading_state", "class_name", "className", "id", "children"],
-            Ue = function(t) {
+        const Be = Fe;
+        var ze = ["title", "item_id", "loading_state", "class_name", "className", "id", "children"],
+            Ke = function(t) {
                 var n = t.title,
                     r = t.item_id,
                     a = t.loading_state,
                     s = t.class_name,
                     c = t.className,
                     u = t.id,
                     d = t.children,
-                    p = o(t, He),
-                    f = (0, i.useContext)(Me),
+                    p = o(t, ze),
+                    f = (0, i.useContext)(Ae),
                     g = f.toggle,
                     b = f.idx,
                     y = r || "item-".concat(b);
                 return l().createElement(Ce.Item, e({
-                    id: Ae(u),
+                    id: $e(u),
                     key: y,
                     eventKey: y,
                     className: s || c
                 }, m(["setProps", "persistence", "persistence_type", "persisted_props"], p), {
                     "data-dash-is-loading": a && a.is_loading || void 0
                 }), l().createElement(Ce.Header, {
                     onClick: function() {
                         g(y)
                     }
                 }, n), l().createElement(Ce.Body, null, d))
             };
-        Ue.propTypes = {
+        Ke.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             title: u().node,
             item_id: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const We = Ue;
+        const He = Ke;
 
-        function qe(e) {
+        function We(e) {
             var t = function(e, t) {
                 if ("object" != Te(e) || !e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, "string");
                     if ("object" != Te(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return String(e)
             }(e);
             return "symbol" == Te(t) ? t : t + ""
         }
 
-        function Ve(e, t, n) {
-            return (t = qe(t)) in e ? Object.defineProperty(e, t, {
+        function Ue(e, t, n) {
+            return (t = We(t)) in e ? Object.defineProperty(e, t, {
                 value: n,
                 enumerable: !0,
                 configurable: !0,
                 writable: !0
             }) : e[t] = n, e
         }
-        const Ge = function(e) {
+        const qe = function(e) {
             const t = (0, i.useRef)(e);
             return (0, i.useEffect)((() => {
                 t.current = e
             }), [e]), t
         };
 
-        function Ye(e) {
-            const t = Ge(e);
+        function Ve(e) {
+            const t = qe(e);
             return (0, i.useCallback)((function(...e) {
                 return t.current && t.current(...e)
             }), [t])
         }
-        const Xe = e => i.forwardRef(((t, n) => (0, _.jsx)("div", {
+        const Ge = e => i.forwardRef(((t, n) => (0, _.jsx)("div", {
                 ...t,
                 ref: n,
                 className: b()(t.className, e)
             }))),
-            Je = Xe("h4");
-        Je.displayName = "DivStyledAsH4";
-        const Qe = i.forwardRef((({
+            Ye = Ge("h4");
+        Ye.displayName = "DivStyledAsH4";
+        const Xe = i.forwardRef((({
             className: e,
             bsPrefix: t,
-            as: n = Je,
+            as: n = Ye,
             ...r
         }, a) => (t = E(t, "alert-heading"), (0, _.jsx)(n, {
             ref: a,
             className: b()(e, t),
             ...r
         }))));
-        Qe.displayName = "AlertHeading";
-        const Ze = Qe;
+        Xe.displayName = "AlertHeading";
+        const Je = Xe;
 
-        function et() {
+        function Qe() {
             return (0, i.useState)(null)
         }
 
-        function tt() {
+        function Ze() {
             const e = (0, i.useRef)(!0),
                 t = (0, i.useRef)((() => e.current));
             return (0, i.useEffect)((() => (e.current = !0, () => {
                 e.current = !1
             })), []), t.current
         }
 
-        function nt(e) {
+        function et(e) {
             const t = (0, i.useRef)(null);
             return (0, i.useEffect)((() => {
                 t.current = e
             })), t.current
         }
-        const rt = void 0 !== n.g && n.g.navigator && "ReactNative" === n.g.navigator.product,
-            at = "undefined" != typeof document || rt ? i.useLayoutEffect : i.useEffect;
+        const tt = void 0 !== n.g && n.g.navigator && "ReactNative" === n.g.navigator.product,
+            nt = "undefined" != typeof document || tt ? i.useLayoutEffect : i.useEffect;
         new WeakMap;
-        const st = ["as", "disabled"];
+        const rt = ["as", "disabled"];
 
-        function ot({
+        function at({
             tagName: e,
             disabled: t,
             href: n,
             target: r,
             rel: a,
             role: s,
             onClick: o,
@@ -1904,83 +1866,83 @@
                 rel: "a" === e ? a : void 0,
                 onClick: u,
                 onKeyDown: e => {
                     " " === e.key && (e.preventDefault(), u(e))
                 }
             }, c]
         }
-        const it = i.forwardRef(((e, t) => {
+        const st = i.forwardRef(((e, t) => {
             let {
                 as: n,
                 disabled: r
             } = e, a = function(e, t) {
                 if (null == e) return {};
                 var n, r, a = {},
                     s = Object.keys(e);
                 for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                 return a
-            }(e, st);
+            }(e, rt);
             const [s, {
                 tagName: o
-            }] = ot(Object.assign({
+            }] = at(Object.assign({
                 tagName: n,
                 disabled: r
             }, a));
             return (0, _.jsx)(o, Object.assign({}, a, s, {
                 ref: t
             }))
         }));
-        it.displayName = "Button";
-        const lt = it,
-            ct = ["onKeyDown"],
-            ut = i.forwardRef(((e, t) => {
+        st.displayName = "Button";
+        const ot = st,
+            it = ["onKeyDown"],
+            lt = i.forwardRef(((e, t) => {
                 let {
                     onKeyDown: n
                 } = e, r = function(e, t) {
                     if (null == e) return {};
                     var n, r, a = {},
                         s = Object.keys(e);
                     for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                     return a
-                }(e, ct);
-                const [a] = ot(Object.assign({
+                }(e, it);
+                const [a] = at(Object.assign({
                     tagName: "a"
-                }, r)), s = Ye((e => {
+                }, r)), s = Ve((e => {
                     a.onKeyDown(e), null == n || n(e)
                 }));
                 return (o = r.href) && "#" !== o.trim() && "button" !== r.role ? (0, _.jsx)("a", Object.assign({
                     ref: t
                 }, r, {
                     onKeyDown: n
                 })) : (0, _.jsx)("a", Object.assign({
                     ref: t
                 }, r, a, {
                     onKeyDown: s
                 }));
                 var o
             }));
-        ut.displayName = "Anchor";
-        const dt = ut,
-            pt = i.forwardRef((({
+        lt.displayName = "Anchor";
+        const ct = lt,
+            ut = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
-                as: n = dt,
+                as: n = ct,
                 ...r
             }, a) => (t = E(t, "alert-link"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        pt.displayName = "AlertLink";
-        const ft = pt,
-            mt = {
+        ut.displayName = "AlertLink";
+        const dt = ut,
+            pt = {
                 [z]: "show",
                 [K]: "show"
             },
-            gt = i.forwardRef((({
+            ft = i.forwardRef((({
                 className: e,
                 children: t,
                 transitionClasses: n = {},
                 onEnter: r,
                 ...a
             }, s) => {
                 const o = {
@@ -1998,153 +1960,153 @@
                     ref: s,
                     addEndListener: ne,
                     ...o,
                     onEnter: l,
                     childRef: t.ref,
                     children: (r, a) => i.cloneElement(t, {
                         ...a,
-                        className: b()("fade", e, t.props.className, mt[r], n[r])
+                        className: b()("fade", e, t.props.className, pt[r], n[r])
                     })
                 })
             }));
-        gt.displayName = "Fade";
-        const bt = gt,
-            yt = {
+        ft.displayName = "Fade";
+        const mt = ft,
+            gt = {
                 "aria-label": u().string,
                 onClick: u().func,
                 variant: u().oneOf(["white"])
             },
-            ht = i.forwardRef((({
+            bt = i.forwardRef((({
                 className: e,
                 variant: t,
                 "aria-label": n = "Close",
                 ...r
             }, a) => (0, _.jsx)("button", {
                 ref: a,
                 type: "button",
                 className: b()("btn-close", t && `btn-close-${t}`, e),
                 "aria-label": n,
                 ...r
             })));
-        ht.displayName = "CloseButton", ht.propTypes = yt;
-        const vt = ht,
-            _t = i.forwardRef(((e, t) => {
+        bt.displayName = "CloseButton", bt.propTypes = gt;
+        const yt = bt,
+            ht = i.forwardRef(((e, t) => {
                 const {
                     bsPrefix: n,
                     show: r = !0,
                     closeLabel: a = "Close alert",
                     closeVariant: s,
                     className: o,
                     children: i,
                     variant: l = "primary",
                     onClose: c,
                     dismissible: u,
-                    transition: d = bt,
+                    transition: d = mt,
                     ...p
                 } = v(e, {
                     show: "onClose"
-                }), f = E(n, "alert"), m = Ye((e => {
+                }), f = E(n, "alert"), m = Ve((e => {
                     c && c(!1, e)
-                })), g = !0 === d ? bt : d, y = (0, _.jsxs)("div", {
+                })), g = !0 === d ? mt : d, y = (0, _.jsxs)("div", {
                     role: "alert",
                     ...g ? void 0 : p,
                     ref: t,
                     className: b()(o, f, l && `${f}-${l}`, u && `${f}-dismissible`),
-                    children: [u && (0, _.jsx)(vt, {
+                    children: [u && (0, _.jsx)(yt, {
                         onClick: m,
                         "aria-label": a,
                         variant: s
                     }), i]
                 });
                 return g ? (0, _.jsx)(g, {
                     unmountOnExit: !0,
                     ...p,
                     ref: void 0,
                     in: r,
                     children: y
                 }) : r ? y : null
             }));
-        _t.displayName = "Alert";
-        const xt = Object.assign(_t, {
-            Link: ft,
-            Heading: Ze
+        ht.displayName = "Alert";
+        const vt = Object.assign(ht, {
+            Link: dt,
+            Heading: Je
         });
-        var Ot = new Set(["primary", "secondary", "success", "danger", "warning", "info", "light", "dark", "white", "transparent"]),
-            wt = new Set(["primary", "secondary", "success", "danger", "warning", "info", "light", "dark", "muted", "white", "black-50", "white-50"]),
-            Nt = ["children", "dismissable", "duration", "is_open", "loading_state", "setProps", "color", "style", "class_name", "className", "fade"];
+        var _t = new Set(["primary", "secondary", "success", "danger", "warning", "info", "light", "dark", "white", "transparent"]),
+            xt = new Set(["primary", "secondary", "success", "danger", "warning", "info", "light", "dark", "muted", "white", "black-50", "white-50"]),
+            Ot = ["children", "dismissable", "duration", "is_open", "loading_state", "setProps", "color", "style", "class_name", "className", "fade"];
 
-        function Et(e, t) {
+        function wt(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function jt(e) {
+        function Nt(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Et(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Et(Object(n)).forEach((function(t) {
+                t % 2 ? wt(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : wt(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var kt = function(t) {
+        var Et = function(t) {
             var n = t.children,
                 r = t.dismissable,
                 a = t.duration,
                 s = t.is_open,
                 c = t.loading_state,
                 u = t.setProps,
                 d = t.color,
                 p = t.style,
                 f = t.class_name,
                 g = t.className,
                 b = t.fade,
-                y = o(t, Nt),
+                y = o(t, Ot),
                 h = (0, i.useRef)(null);
             (0, i.useEffect)((function() {
                 return a && (s ? h.current = setTimeout(v, a) : h.current && (clearTimeout(h.current), h.current = null)),
                     function() {
                         return clearTimeout(h.current)
                     }
             }), [s]);
             var v = function() {
                     u && u({
                         is_open: !1
                     })
                 },
-                _ = Ot.has(d);
-            return l().createElement(xt, e({
+                _ = _t.has(d);
+            return l().createElement(vt, e({
                 show: s,
                 dismissible: r,
                 onClose: r ? v : null,
                 variant: _ ? d : null,
                 className: f || g,
                 transition: b,
-                style: _ ? p : jt({
+                style: _ ? p : Nt({
                     backgroundColor: d
                 }, p)
             }, m(["persistence", "persisted_props", "persistence_type", "setProps"], y), {
                 "data-dash-is-loading": c && c.is_loading || void 0
             }), n)
         };
-        kt.defaultProps = {
+        Et.defaultProps = {
             color: "success",
             is_open: !0,
             duration: null,
             persisted_props: ["is_open"],
             persistence_type: "local"
-        }, kt.propTypes = {
+        }, Et.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             color: u().string,
@@ -2157,16 +2119,16 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["is_open"])),
             persistence_type: u().oneOf(["local", "session", "memory"])
         };
-        const Pt = kt,
-            Ct = i.forwardRef((({
+        const jt = Et,
+            kt = i.forwardRef((({
                 bsPrefix: e,
                 bg: t = "primary",
                 pill: n = !1,
                 text: r,
                 className: a,
                 as: s = "span",
                 ...o
@@ -2174,207 +2136,206 @@
                 const l = E(e, "badge");
                 return (0, _.jsx)(s, {
                     ref: i,
                     ...o,
                     className: b()(a, l, n && "rounded-pill", r && `text-${r}`, t && `bg-${t}`)
                 })
             }));
-        Ct.displayName = "Badge";
-        const Tt = Ct;
+        kt.displayName = "Badge";
+        const Pt = kt;
 
-        function St(e, t) {
+        function Ct(e, t) {
             for (var n = 0; n < t.length; n++) {
                 var r = t[n];
-                r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, qe(r.key), r)
+                r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, We(r.key), r)
             }
         }
 
-        function Rt(e) {
-            return Rt = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
+        function Tt(e) {
+            return Tt = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
                 return e.__proto__ || Object.getPrototypeOf(e)
-            }, Rt(e)
+            }, Tt(e)
         }
-        var Dt = n(10),
-            Lt = n.n(Dt),
-            $t = ["children", "external_link", "preOnClick", "target", "linkTarget", "href", "download"];
+        var St = n(10),
+            Rt = n.n(St),
+            Dt = ["children", "external_link", "preOnClick", "target", "linkTarget", "href", "download"];
 
-        function It(e, t, n) {
-            return t = Rt(t),
+        function Lt(e, t, n) {
+            return t = Tt(t),
                 function(e, t) {
                     if (t && ("object" === Te(t) || "function" == typeof t)) return t;
                     if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
                     return function(e) {
                         if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                         return e
                     }(e)
-                }(e, At() ? Reflect.construct(t, n || [], Rt(e).constructor) : t.apply(e, n))
+                }(e, It() ? Reflect.construct(t, n || [], Tt(e).constructor) : t.apply(e, n))
         }
 
-        function At() {
+        function It() {
             try {
                 var e = !Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {})))
             } catch (e) {}
-            return (At = function() {
+            return (It = function() {
                 return !!e
             })()
         }
 
-        function Ft(e, t) {
+        function $t(e, t) {
             t = t || {
                 bubbles: !1,
                 cancelable: !1,
                 detail: void 0
             };
             var n = document.createEvent("CustomEvent");
             return n.initCustomEvent(e, t.bubbles, t.cancelable, t.detail), n
         }
 
-        function Mt(e, t) {
-            return null == e ? Lt()(t) : e
+        function At(e, t) {
+            return null == e ? Rt()(t) : e
         }
-        Ft.prototype = window.Event.prototype;
-        var Bt = function(t) {
+        $t.prototype = window.Event.prototype;
+        var Mt = function(t) {
             function n(e) {
                 var t;
                 return function(e, t) {
                     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                }(this, n), (t = It(this, n, [e])).updateLocation = t.updateLocation.bind(t), t
+                }(this, n), (t = Lt(this, n, [e])).updateLocation = t.updateLocation.bind(t), t
             }
             return function(e, t) {
                 if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                 e.prototype = Object.create(t && t.prototype, {
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }), Object.defineProperty(e, "prototype", {
                     writable: !1
-                }), t && $(e, t)
+                }), t && I(e, t)
             }(n, t), r = n, (a = [{
                 key: "updateLocation",
                 value: function(e) {
                     if (!(e.metaKey || e.shiftKey || e.altKey || e.ctrlKey))
                         if (this.props.disabled) e.preventDefault();
                         else {
                             this.props.preOnClick && this.props.preOnClick();
                             var t = this.props,
                                 n = t.external_link,
                                 r = t.href;
-                            if (r && !Mt(n, r)) {
+                            if (r && !At(n, r)) {
                                 e.preventDefault();
                                 var a = this.props.href;
-                                window.history.pushState({}, "", a), window.dispatchEvent(new Ft("_dashprivate_pushstate")), window.scrollTo(0, 0)
+                                window.history.pushState({}, "", a), window.dispatchEvent(new $t("_dashprivate_pushstate")), window.scrollTo(0, 0)
                             }
                         }
                 }
             }, {
                 key: "render",
                 value: function() {
                     var t = this,
                         n = this.props,
                         r = n.children,
                         a = n.external_link,
                         s = (n.preOnClick, n.target),
                         i = n.linkTarget,
                         c = n.href,
                         u = n.download,
-                        d = o(n, $t),
-                        p = c && Mt(a, c);
+                        d = o(n, Dt),
+                        p = c && At(a, c);
                     return l().createElement("a", e({
                         href: c,
                         target: p ? s || i : void 0,
                         download: u && p ? u : void 0
                     }, d, {
                         onClick: function(e) {
                             return t.updateLocation(e)
                         }
                     }), r)
                 }
-            }]) && St(r.prototype, a), Object.defineProperty(r, "prototype", {
+            }]) && Ct(r.prototype, a), Object.defineProperty(r, "prototype", {
                 writable: !1
             }), r;
             var r, a
         }(i.Component);
-        Bt.propTypes = {
+        Mt.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             href: u().string,
             disabled: u().bool,
             external_link: u().bool,
             preOnClick: u().func,
             target: u().string,
             download: u().string
-        }, Bt.defaultProps = {
+        }, Mt.defaultProps = {
             disabled: !1,
             external_link: null
         };
-        var zt = ["children", "href", "loading_state", "setProps", "color", "style", "className", "class_name", "text_color"];
+        var Ft = ["children", "href", "loading_state", "setProps", "color", "style", "className", "class_name", "text_color"];
 
-        function Kt(e, t) {
+        function Bt(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Ht(e) {
+        function zt(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Kt(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Kt(Object(n)).forEach((function(t) {
+                t % 2 ? Bt(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Bt(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Ut = function(t) {
+        var Kt = function(t) {
             var n = t.children,
                 r = t.href,
                 a = t.loading_state,
                 s = t.setProps,
                 i = t.color,
                 c = t.style,
                 u = t.className,
                 d = t.class_name,
                 p = t.text_color,
-                f = o(t, zt),
-                g = Fe(r, s),
-                b = Ot.has(i);
+                f = o(t, Ft),
+                g = _t.has(i);
             return f[r ? "preOnClick" : "onClick"] = function() {
                 s && s({
                     n_clicks: t.n_clicks + 1,
                     n_clicks_timestamp: Date.now()
                 })
-            }, l().createElement(Tt, e({
-                as: g && Bt,
-                href: g,
-                bg: b ? i : null,
+            }, l().createElement(Pt, e({
+                as: r && Mt,
+                href: r,
+                bg: g ? i : null,
                 text: p,
                 className: d || u,
-                style: b ? c : Ht({
+                style: g ? c : zt({
                     backgroundColor: i
                 }, c)
             }, m(["setProps", "n_clicks", "n_clicks_timestamp"], f), {
                 "data-dash-is-loading": a && a.is_loading || void 0
             }), n)
         };
-        Ut.defaultProps = {
+        Kt.defaultProps = {
             color: "secondary",
             n_clicks: 0,
             n_clicks_timestamp: -1
-        }, Ut.propTypes = {
+        }, Kt.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             color: u().string,
@@ -2389,22 +2350,22 @@
             }),
             external_link: u().bool,
             n_clicks: u().number,
             n_clicks_timestamp: u().number,
             target: u().string,
             title: u().string
         };
-        const Wt = Ut,
-            qt = i.forwardRef((({
+        const Ht = Kt,
+            Wt = i.forwardRef((({
                 bsPrefix: e,
                 active: t = !1,
                 children: n,
                 className: r,
                 as: a = "li",
-                linkAs: s = dt,
+                linkAs: s = ct,
                 linkProps: o = {},
                 href: i,
                 title: l,
                 target: c,
                 ...u
             }, d) => {
                 const p = E(e, "breadcrumb-item");
@@ -2420,17 +2381,17 @@
                         href: i,
                         title: l,
                         target: c,
                         children: n
                     })
                 })
             }));
-        qt.displayName = "BreadcrumbItem";
-        const Vt = qt,
-            Gt = i.forwardRef((({
+        Wt.displayName = "BreadcrumbItem";
+        const Ut = Wt,
+            qt = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 listProps: n = {},
                 children: r,
                 label: a = "breadcrumb",
                 as: s = "nav",
                 ...o
@@ -2444,58 +2405,46 @@
                     children: (0, _.jsx)("ol", {
                         ...n,
                         className: b()(l, null == n ? void 0 : n.className),
                         children: r
                     })
                 })
             }));
-        Gt.displayName = "Breadcrumb";
-        const Yt = Object.assign(Gt, {
-            Item: Vt
+        qt.displayName = "Breadcrumb";
+        const Vt = Object.assign(qt, {
+            Item: Ut
         });
-        var Xt = ["href", "setProps", "external_link", "label"],
-            Jt = ["items", "tag", "loading_state", "class_name", "className", "item_class_name", "itemClassName", "item_style", "setProps"],
-            Qt = function(t) {
-                var n = t.href,
-                    r = t.setProps,
-                    a = t.external_link,
-                    s = t.label,
-                    i = o(t, Xt),
-                    c = Fe(n, r);
-                return l().createElement(Yt.Item, e({
-                    linkAs: c && Bt,
-                    href: c,
-                    linkProps: c && {
-                        external_link: a
-                    }
-                }, i), s)
-            },
-            Zt = function(t) {
+        var Gt = ["items", "tag", "loading_state", "class_name", "className", "item_class_name", "itemClassName", "item_style"],
+            Yt = function(t) {
                 var n = t.items,
                     r = t.tag,
                     a = t.loading_state,
                     s = t.class_name,
                     i = t.className,
                     c = t.item_class_name,
                     u = t.itemClassName,
-                    d = (t.item_style, t.setProps),
-                    p = o(t, Jt);
-                return l().createElement(Yt, e({
+                    d = (t.item_style, o(t, Gt));
+                return l().createElement(Vt, e({
                     as: r,
                     "data-dash-is-loading": a && a.is_loading || void 0,
                     className: s || i
-                }, p), (n || []).map((function(t, n) {
-                    return l().createElement(Qt, e({
-                        key: "".concat(t.value).concat(n),
+                }, d), (n || []).map((function(e, t) {
+                    return l().createElement(Vt.Item, {
+                        key: "".concat(e.value).concat(t),
+                        active: e.active,
+                        linkAs: e.href && Mt,
                         className: c || u,
-                        setProps: d
-                    }, t))
+                        href: e.href,
+                        linkProps: e.href && {
+                            external_link: e.external_link
+                        }
+                    }, e.label)
                 })))
             };
-        Zt.propTypes = {
+        Yt.propTypes = {
             id: u().string,
             items: u().arrayOf(u().shape({
                 label: u().string,
                 href: u().string,
                 active: u().bool,
                 external_link: u().bool,
                 target: u().string,
@@ -2511,46 +2460,46 @@
             tag: u().object,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const en = Zt,
-            tn = i.forwardRef((({
+        const Xt = Yt,
+            Jt = i.forwardRef((({
                 as: e,
                 bsPrefix: t,
                 variant: n = "primary",
                 size: r,
                 active: a = !1,
                 disabled: s = !1,
                 className: o,
                 ...i
             }, l) => {
                 const c = E(t, "btn"),
                     [u, {
                         tagName: d
-                    }] = ot({
+                    }] = at({
                         tagName: e,
                         disabled: s,
                         ...i
                     }),
                     p = d;
                 return (0, _.jsx)(p, {
                     ...u,
                     ...i,
                     ref: l,
                     disabled: s,
                     className: b()(o, c, a && "active", n && `${c}-${n}`, r && `${c}-${r}`, i.href && s && "disabled")
                 })
             }));
-        tn.displayName = "Button";
-        const nn = tn;
-        var rn = ["children", "disabled", "href", "loading_state", "setProps", "n_clicks", "target", "type", "download", "name", "value", "className", "class_name", "color", "outline", "onClick", "rel"],
-            an = function(t) {
+        Jt.displayName = "Button";
+        const Qt = Jt;
+        var Zt = ["children", "disabled", "href", "loading_state", "setProps", "n_clicks", "target", "type", "download", "name", "value", "className", "class_name", "color", "outline", "onClick", "rel"],
+            en = function(t) {
                 var n = t.children,
                     r = t.disabled,
                     a = t.href,
                     s = t.loading_state,
                     i = t.setProps,
                     c = t.n_clicks,
                     u = t.target,
@@ -2560,41 +2509,40 @@
                     g = t.value,
                     b = t.className,
                     y = t.class_name,
                     h = t.color,
                     v = t.outline,
                     _ = t.onClick,
                     x = t.rel,
-                    O = o(t, rn),
-                    w = Fe(a, i),
-                    N = w && !r;
-                return O[N ? "preOnClick" : "onClick"] = _ || function() {
+                    O = o(t, Zt),
+                    w = a && !r;
+                return O[w ? "preOnClick" : "onClick"] = _ || function() {
                     !r && i && i({
                         n_clicks: c + 1,
                         n_clicks_timestamp: Date.now()
                     })
-                }, N && (O.linkTarget = u), l().createElement(nn, e({
-                    as: N ? Bt : "button",
+                }, w && (O.linkTarget = u), l().createElement(Qt, e({
+                    as: w ? Mt : "button",
                     variant: v ? "outline-".concat(h) : h,
-                    type: N ? void 0 : d,
-                    href: r ? void 0 : w,
+                    type: w ? void 0 : d,
+                    href: r ? void 0 : a,
                     disabled: r,
-                    download: N ? p : void 0,
-                    name: N ? void 0 : f,
-                    value: N ? void 0 : g,
+                    download: w ? p : void 0,
+                    name: w ? void 0 : f,
+                    value: w ? void 0 : g,
                     className: y || b,
-                    rel: N ? x : void 0
+                    rel: w ? x : void 0
                 }, m(["n_clicks_timestamp"], O), {
                     "data-dash-is-loading": s && s.is_loading || void 0
                 }), n)
             };
-        an.defaultProps = {
+        en.defaultProps = {
             n_clicks: 0,
             n_clicks_timestamp: -1
-        }, an.propTypes = {
+        }, en.propTypes = {
             id: u().string,
             children: u().node,
             class_name: u().string,
             className: u().string,
             style: u().object,
             key: u().string,
             href: u().string,
@@ -2615,16 +2563,16 @@
             target: u().string,
             type: u().oneOf(["button", "reset", "submit"]),
             download: u().string,
             name: u().string,
             value: u().string,
             rel: u().string
         };
-        const sn = an,
-            on = i.forwardRef((({
+        const tn = en,
+            nn = i.forwardRef((({
                 bsPrefix: e,
                 size: t,
                 vertical: n = !1,
                 className: r,
                 role: a = "group",
                 as: s = "div",
                 ...o
@@ -2634,172 +2582,172 @@
                 return n && (c = `${l}-vertical`), (0, _.jsx)(s, {
                     ...o,
                     ref: i,
                     role: a,
                     className: b()(r, c, t && `${l}-${t}`)
                 })
             }));
-        on.displayName = "ButtonGroup";
-        const ln = on;
-        var cn = ["children", "loading_state", "class_name", "className"],
-            un = function(t) {
+        nn.displayName = "ButtonGroup";
+        const rn = nn;
+        var an = ["children", "loading_state", "class_name", "className"],
+            sn = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.class_name,
                     s = t.className,
-                    i = o(t, cn);
-                return l().createElement(ln, e({
+                    i = o(t, an);
+                return l().createElement(rn, e({
                     className: a || s
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        un.propTypes = {
+        sn.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             vertical: u().bool,
             size: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const dn = un,
-            pn = i.forwardRef((({
+        const on = sn,
+            ln = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "card-body"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        pn.displayName = "CardBody";
-        const fn = pn,
-            mn = i.forwardRef((({
+        ln.displayName = "CardBody";
+        const cn = ln,
+            un = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "card-footer"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        mn.displayName = "CardFooter";
-        const gn = mn,
-            bn = i.createContext(null);
-        bn.displayName = "CardHeaderContext";
-        const yn = bn,
-            hn = i.forwardRef((({
+        un.displayName = "CardFooter";
+        const dn = un,
+            pn = i.createContext(null);
+        pn.displayName = "CardHeaderContext";
+        const fn = pn,
+            mn = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 as: n = "div",
                 ...r
             }, a) => {
                 const s = E(e, "card-header"),
                     o = (0, i.useMemo)((() => ({
                         cardHeaderBsPrefix: s
                     })), [s]);
-                return (0, _.jsx)(yn.Provider, {
+                return (0, _.jsx)(fn.Provider, {
                     value: o,
                     children: (0, _.jsx)(n, {
                         ref: a,
                         ...r,
                         className: b()(t, s)
                     })
                 })
             }));
-        hn.displayName = "CardHeader";
-        const vn = hn,
-            _n = i.forwardRef((({
+        mn.displayName = "CardHeader";
+        const gn = mn,
+            bn = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 variant: n,
                 as: r = "img",
                 ...a
             }, s) => {
                 const o = E(e, "card-img");
                 return (0, _.jsx)(r, {
                     ref: s,
                     className: b()(n ? `${o}-${n}` : o, t),
                     ...a
                 })
             }));
-        _n.displayName = "CardImg";
-        const xn = _n,
-            On = i.forwardRef((({
+        bn.displayName = "CardImg";
+        const yn = bn,
+            hn = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "card-img-overlay"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        On.displayName = "CardImgOverlay";
-        const wn = On,
-            Nn = i.forwardRef((({
+        hn.displayName = "CardImgOverlay";
+        const vn = hn,
+            _n = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "a",
                 ...r
             }, a) => (t = E(t, "card-link"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        Nn.displayName = "CardLink";
-        const En = Nn,
-            jn = Xe("h6"),
-            kn = i.forwardRef((({
+        _n.displayName = "CardLink";
+        const xn = _n,
+            On = Ge("h6"),
+            wn = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
-                as: n = jn,
+                as: n = On,
                 ...r
             }, a) => (t = E(t, "card-subtitle"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        kn.displayName = "CardSubtitle";
-        const Pn = kn,
-            Cn = i.forwardRef((({
+        wn.displayName = "CardSubtitle";
+        const Nn = wn,
+            En = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "p",
                 ...r
             }, a) => (t = E(t, "card-text"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        Cn.displayName = "CardText";
-        const Tn = Cn,
-            Sn = Xe("h5"),
-            Rn = i.forwardRef((({
+        En.displayName = "CardText";
+        const jn = En,
+            kn = Ge("h5"),
+            Pn = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
-                as: n = Sn,
+                as: n = kn,
                 ...r
             }, a) => (t = E(t, "card-title"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        Rn.displayName = "CardTitle";
-        const Dn = Rn,
-            Ln = i.forwardRef((({
+        Pn.displayName = "CardTitle";
+        const Cn = Pn,
+            Tn = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 bg: n,
                 text: r,
                 border: a,
                 body: s = !1,
                 children: o,
@@ -2807,78 +2755,78 @@
                 ...l
             }, c) => {
                 const u = E(e, "card");
                 return (0, _.jsx)(i, {
                     ref: c,
                     ...l,
                     className: b()(t, u, n && `bg-${n}`, r && `text-${r}`, a && `border-${a}`),
-                    children: s ? (0, _.jsx)(fn, {
+                    children: s ? (0, _.jsx)(cn, {
                         children: o
                     }) : o
                 })
             }));
-        Ln.displayName = "Card";
-        const $n = Object.assign(Ln, {
-            Img: xn,
-            Title: Dn,
-            Subtitle: Pn,
-            Body: fn,
-            Link: En,
-            Text: Tn,
-            Header: vn,
-            Footer: gn,
-            ImgOverlay: wn
+        Tn.displayName = "Card";
+        const Sn = Object.assign(Tn, {
+            Img: yn,
+            Title: Cn,
+            Subtitle: Nn,
+            Body: cn,
+            Link: xn,
+            Text: jn,
+            Header: gn,
+            Footer: dn,
+            ImgOverlay: vn
         });
-        var In = ["children", "color", "inverse", "outline", "style", "loading_state", "className", "class_name"];
+        var Rn = ["children", "color", "inverse", "outline", "style", "loading_state", "className", "class_name"];
 
-        function An(e, t) {
+        function Dn(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Fn(e) {
+        function Ln(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? An(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : An(Object(n)).forEach((function(t) {
+                t % 2 ? Dn(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Dn(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Mn = function(t) {
+        var In = function(t) {
             var n = t.children,
                 r = t.color,
                 a = t.inverse,
                 s = t.outline,
                 i = t.style,
                 c = t.loading_state,
                 u = t.className,
                 d = t.class_name,
-                p = o(t, In),
-                f = Ot.has(r);
-            return l().createElement($n, e({
+                p = o(t, Rn),
+                f = _t.has(r);
+            return l().createElement(Sn, e({
                 "data-dash-is-loading": c && c.is_loading || void 0,
                 text: a ? "white" : null,
                 bg: f && !s ? r : null,
                 border: f && s ? r : null,
-                style: f ? i : Fn({
+                style: f ? i : Ln({
                     backgroundColor: r
                 }, i),
                 className: d || u
             }, m(["setProps"], p)), n)
         };
-        Mn.propTypes = {
+        In.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             color: u().string,
@@ -2887,151 +2835,151 @@
             inverse: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Bn = Mn;
-        var zn = ["children", "loading_state", "className", "class_name"],
-            Kn = function(t) {
+        const $n = In;
+        var An = ["children", "loading_state", "className", "class_name"],
+            Mn = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, zn);
-                return l().createElement($n.Body, e({
+                    i = o(t, An);
+                return l().createElement(Sn.Body, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
                     className: s || a
                 }, m(["setProps"], i)), n)
             };
-        Kn.propTypes = {
+        Mn.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Hn = Kn;
-        var Un = ["children", "loading_state", "className", "class_name"],
-            Wn = function(t) {
+        const Fn = Mn;
+        var Bn = ["children", "loading_state", "className", "class_name"],
+            zn = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Un);
-                return l().createElement($n.Footer, e({
+                    i = o(t, Bn);
+                return l().createElement(Sn.Footer, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
                     className: s || a
                 }, m(["setProps"], i)), n)
             };
-        Wn.propTypes = {
+        zn.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const qn = Wn,
-            Vn = i.forwardRef((({
+        const Kn = zn,
+            Hn = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "card-group"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        Vn.displayName = "CardGroup";
-        const Gn = Vn;
-        var Yn = ["children", "loading_state", "className", "class_name"],
-            Xn = function(t) {
+        Hn.displayName = "CardGroup";
+        const Wn = Hn;
+        var Un = ["children", "loading_state", "className", "class_name"],
+            qn = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Yn);
-                return l().createElement(Gn, e({
+                    i = o(t, Un);
+                return l().createElement(Wn, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
                     className: s || a
                 }, m(["setProps"], i)), n)
             };
-        Xn.propTypes = {
+        qn.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Jn = Xn;
-        var Qn = ["children", "loading_state", "className", "class_name"],
-            Zn = function(t) {
+        const Vn = qn;
+        var Gn = ["children", "loading_state", "className", "class_name"],
+            Yn = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Qn);
-                return l().createElement(vn, e({
+                    i = o(t, Gn);
+                return l().createElement(gn, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
                     className: s || a
                 }, m(["setProps"], i)), n)
             };
-        Zn.propTypes = {
+        Yn.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const er = Zn;
-        var tr = ["children", "loading_state", "className", "class_name", "top", "bottom"],
-            nr = function(t) {
+        const Xn = Yn;
+        var Jn = ["children", "loading_state", "className", "class_name", "top", "bottom"],
+            Qn = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.top,
                     c = t.bottom,
-                    u = o(t, tr);
-                return l().createElement(xn, e({
+                    u = o(t, Jn);
+                return l().createElement(yn, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
                     className: s || a,
                     variant: i ? "top" : c ? "bottom" : null
                 }, m(["setProps"], u)), n)
             };
-        nr.propTypes = {
+        Qn.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
@@ -3042,71 +2990,67 @@
             title: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const rr = nr;
-        var ar = ["children", "loading_state", "className", "class_name"],
-            sr = function(t) {
+        const Zn = Qn;
+        var er = ["children", "loading_state", "className", "class_name"],
+            tr = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, ar);
-                return l().createElement($n.ImgOverlay, e({
+                    i = o(t, er);
+                return l().createElement(Sn.ImgOverlay, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
                     className: s || a
                 }, m(["setProps"], i)), n)
             };
-        sr.propTypes = {
+        tr.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const or = sr;
-        var ir = ["children", "loading_state", "disabled", "className", "class_name", "href", "setProps"],
-            lr = function(t) {
+        const nr = tr;
+        var rr = ["children", "loading_state", "disabled", "className", "class_name"],
+            ar = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.disabled,
                     s = t.className,
                     i = t.class_name,
-                    c = t.href,
-                    u = t.setProps,
-                    d = o(t, ir),
-                    p = Fe(c, u);
-                return l().createElement($n.Link, e({
+                    c = o(t, rr);
+                return l().createElement(Sn.Link, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
-                    as: Bt,
+                    as: Mt,
                     preOnClick: function() {
-                        !a && u && u({
+                        !a && t.setProps && t.setProps({
                             n_clicks: t.n_clicks + 1,
                             n_clicks_timestamp: Date.now()
                         })
                     },
                     disabled: a,
-                    href: p,
                     className: i || s
-                }, m(["n_clicks", "n_clicks_timestamp"], d)), n)
+                }, m(["setProps", "n_clicks", "n_clicks_timestamp"], c)), n)
             };
-        lr.defaultProps = {
+        ar.defaultProps = {
             n_clicks: 0,
             n_clicks_timestamp: -1
-        }, lr.propTypes = {
+        }, ar.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             href: u().string,
@@ -3116,77 +3060,77 @@
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             target: u().string
         };
-        const cr = lr;
+        const sr = ar;
 
-        function ur(e) {
+        function or(e) {
             const t = function(e) {
                 const t = (0, i.useRef)(e);
                 return t.current = e, t
             }(e);
             (0, i.useEffect)((() => () => t.current()), [])
         }
-        const dr = 2 ** 31 - 1;
+        const ir = 2 ** 31 - 1;
 
-        function pr(e, t, n) {
+        function lr(e, t, n) {
             const r = n - Date.now();
-            e.current = r <= dr ? setTimeout(t, r) : setTimeout((() => pr(e, t, n)), dr)
+            e.current = r <= ir ? setTimeout(t, r) : setTimeout((() => lr(e, t, n)), ir)
         }
 
-        function fr() {
-            const e = tt(),
+        function cr() {
+            const e = Ze(),
                 t = (0, i.useRef)();
-            return ur((() => clearTimeout(t.current))), (0, i.useMemo)((() => {
+            return or((() => clearTimeout(t.current))), (0, i.useMemo)((() => {
                 const n = () => clearTimeout(t.current);
                 return {
                     set: function(r, a = 0) {
-                        e() && (n(), a <= dr ? t.current = setTimeout(r, a) : pr(t, r, Date.now() + a))
+                        e() && (n(), a <= ir ? t.current = setTimeout(r, a) : lr(t, r, Date.now() + a))
                     },
                     clear: n,
                     handleRef: t
                 }
             }), [])
         }
-        const mr = i.forwardRef((({
+        const ur = i.forwardRef((({
             className: e,
             bsPrefix: t,
             as: n = "div",
             ...r
         }, a) => (t = E(t, "carousel-caption"), (0, _.jsx)(n, {
             ref: a,
             className: b()(e, t),
             ...r
         }))));
-        mr.displayName = "CarouselCaption";
-        const gr = mr,
-            br = i.forwardRef((({
+        ur.displayName = "CarouselCaption";
+        const dr = ur,
+            pr = i.forwardRef((({
                 as: e = "div",
                 bsPrefix: t,
                 className: n,
                 ...r
             }, a) => {
                 const s = b()(n, E(t, "carousel-item"));
                 return (0, _.jsx)(e, {
                     ref: a,
                     ...r,
                     className: s
                 })
             }));
-        br.displayName = "CarouselItem";
-        const yr = br;
+        pr.displayName = "CarouselItem";
+        const fr = pr;
 
-        function hr(e, t) {
+        function mr(e, t) {
             let n = 0;
             return i.Children.map(e, (e => i.isValidElement(e) ? t(e, n++) : e))
         }
-        const vr = i.forwardRef((({
+        const gr = i.forwardRef((({
             defaultActiveIndex: e = 0,
             ...t
         }, n) => {
             const {
                 as: r = "div",
                 bsPrefix: a,
                 slide: s = !0,
@@ -3215,64 +3159,64 @@
                 }),
                 prevLabel: R = "Previous",
                 nextIcon: D = (0, _.jsx)("span", {
                     "aria-hidden": "true",
                     className: "carousel-control-next-icon"
                 }),
                 nextLabel: L = "Next",
-                variant: $,
-                className: I,
+                variant: I,
+                className: $,
                 children: A,
-                ...F
+                ...M
             } = v({
                 defaultActiveIndex: e,
                 ...t
             }, {
                 activeIndex: "onSelect"
-            }), M = E(a, "carousel"), B = P(), z = (0, i.useRef)(null), [K, H] = (0, i.useState)("next"), [U, W] = (0, i.useState)(!1), [q, V] = (0, i.useState)(!1), [G, Y] = (0, i.useState)(d || 0);
+            }), F = E(a, "carousel"), B = P(), z = (0, i.useRef)(null), [K, H] = (0, i.useState)("next"), [W, U] = (0, i.useState)(!1), [q, V] = (0, i.useState)(!1), [G, Y] = (0, i.useState)(d || 0);
             (0, i.useEffect)((() => {
                 q || d === G || (z.current ? H(z.current) : H((d || 0) > G ? "next" : "prev"), s && V(!0), Y(d || 0))
             }), [d, q, G, s]), (0, i.useEffect)((() => {
                 z.current && (z.current = null)
             }));
             let X, J = 0;
             ! function(e, t) {
                 let n = 0;
                 i.Children.forEach(e, (e => {
                     i.isValidElement(e) && ((e, t) => {
                         ++J, t === d && (X = e.props.interval)
                     })(e, n++)
                 }))
             }(A);
-            const Q = Ge(X),
+            const Q = qe(X),
                 Z = (0, i.useCallback)((e => {
                     if (q) return;
                     let t = G - 1;
                     if (t < 0) {
                         if (!N) return;
                         t = J - 1
                     }
                     z.current = "prev", null == p || p(t, e)
                 }), [q, G, p, N, J]),
-                ee = Ye((e => {
+                ee = Ve((e => {
                     if (q) return;
                     let t = G + 1;
                     if (t >= J) {
                         if (!N) return;
                         t = 0
                     }
                     z.current = "next", null == p || p(t, e)
                 })),
                 te = (0, i.useRef)();
             (0, i.useImperativeHandle)(n, (() => ({
                 element: te.current,
                 prev: Z,
                 next: ee
             })));
-            const re = Ye((() => {
+            const re = Ve((() => {
                     !document.hidden && function(e) {
                         if (!(e && e.style && e.parentNode && e.parentNode.style)) return !1;
                         const t = getComputedStyle(e);
                         return "none" !== t.display && "hidden" !== t.visibility && "none" !== getComputedStyle(e.parentNode).display
                     }(te.current) && (B ? Z() : ee())
                 })),
                 se = "next" === K ? "start" : "end";
@@ -3281,16 +3225,16 @@
                 (0, i.useEffect)((() => {
                     if (!n.current) return e();
                     n.current = !1
                 }), t)
             }((() => {
                 s || (null == f || f(G, se), null == m || m(G, se))
             }), [G]);
-            const oe = `${M}-item-${K}`,
-                ie = `${M}-item-${se}`,
+            const oe = `${F}-item-${K}`,
+                ie = `${F}-item-${se}`,
                 ce = (0, i.useCallback)((e => {
                     ae(e), null == f || f(G, se)
                 }), [f, G, se]),
                 ue = (0, i.useCallback)((() => {
                     V(!1), null == m || m(G, se)
                 }), [m, G, se]),
                 de = (0, i.useCallback)((e => {
@@ -3299,38 +3243,38 @@
                             return e.preventDefault(), void(B ? ee(e) : Z(e));
                         case "ArrowRight":
                             return e.preventDefault(), void(B ? Z(e) : ee(e))
                     }
                     null == h || h(e)
                 }), [y, h, Z, ee, B]),
                 pe = (0, i.useCallback)((e => {
-                    "hover" === x && W(!0), null == O || O(e)
+                    "hover" === x && U(!0), null == O || O(e)
                 }), [x, O]),
                 fe = (0, i.useCallback)((e => {
-                    W(!1), null == w || w(e)
+                    U(!1), null == w || w(e)
                 }), [w]),
                 me = (0, i.useRef)(0),
                 ge = (0, i.useRef)(0),
-                be = fr(),
+                be = cr(),
                 ye = (0, i.useCallback)((e => {
-                    me.current = e.touches[0].clientX, ge.current = 0, "hover" === x && W(!0), null == k || k(e)
+                    me.current = e.touches[0].clientX, ge.current = 0, "hover" === x && U(!0), null == k || k(e)
                 }), [x, k]),
                 he = (0, i.useCallback)((e => {
                     e.touches && e.touches.length > 1 ? ge.current = 0 : ge.current = e.touches[0].clientX - me.current, null == C || C(e)
                 }), [C]),
                 ve = (0, i.useCallback)((e => {
                     if (j) {
                         const t = ge.current;
                         Math.abs(t) > 40 && (t > 0 ? Z(e) : ee(e))
                     }
                     "hover" === x && be.set((() => {
-                        W(!1)
+                        U(!1)
                     }), g || void 0), null == T || T(e)
                 }), [j, x, Z, ee, be, g, T]),
-                _e = null != g && !U && !q,
+                _e = null != g && !W && !q,
                 xe = (0, i.useRef)();
             (0, i.useEffect)((() => {
                 var e, t;
                 if (!_e) return;
                 const n = B ? Z : ee;
                 return xe.current = window.setInterval(document.visibilityState ? re : n, null != (e = null != (t = Q.current) ? t : g) ? e : void 0), () => {
                     null !== xe.current && clearInterval(xe.current)
@@ -3339,35 +3283,35 @@
             const Oe = (0, i.useMemo)((() => c && Array.from({
                 length: J
             }, ((e, t) => e => {
                 null == p || p(t, e)
             }))), [c, J, p]);
             return (0, _.jsxs)(r, {
                 ref: te,
-                ...F,
+                ...M,
                 onKeyDown: de,
                 onMouseOver: pe,
                 onMouseOut: fe,
                 onTouchStart: ye,
                 onTouchMove: he,
                 onTouchEnd: ve,
-                className: b()(I, M, s && "slide", o && `${M}-fade`, $ && `${M}-${$}`),
+                className: b()($, F, s && "slide", o && `${F}-fade`, I && `${F}-${I}`),
                 children: [c && (0, _.jsx)("div", {
-                    className: `${M}-indicators`,
-                    children: hr(A, ((e, t) => (0, _.jsx)("button", {
+                    className: `${F}-indicators`,
+                    children: mr(A, ((e, t) => (0, _.jsx)("button", {
                         type: "button",
                         "data-bs-target": "",
                         "aria-label": null != u && u.length ? u[t] : `Slide ${t+1}`,
                         className: t === G ? "active" : void 0,
                         onClick: Oe ? Oe[t] : void 0,
                         "aria-current": t === G
                     }, t)))
                 }), (0, _.jsx)("div", {
-                    className: `${M}-inner`,
-                    children: hr(A, ((e, t) => {
+                    className: `${F}-inner`,
+                    children: mr(A, ((e, t) => {
                         const n = t === G;
                         return s ? (0, _.jsx)(le, {
                             in: n,
                             onEnter: n ? ce : void 0,
                             onEntered: n ? ue : void 0,
                             addEndListener: ne,
                             children: (t, r) => i.cloneElement(e, {
@@ -3375,88 +3319,88 @@
                                 className: b()(e.props.className, n && "entered" !== t && oe, ("entered" === t || "exiting" === t) && "active", ("entering" === t || "exiting" === t) && ie)
                             })
                         }) : i.cloneElement(e, {
                             className: b()(e.props.className, n && "active")
                         })
                     }))
                 }), l && (0, _.jsxs)(_.Fragment, {
-                    children: [(N || 0 !== d) && (0, _.jsxs)(dt, {
-                        className: `${M}-control-prev`,
+                    children: [(N || 0 !== d) && (0, _.jsxs)(ct, {
+                        className: `${F}-control-prev`,
                         onClick: Z,
                         children: [S, R && (0, _.jsx)("span", {
                             className: "visually-hidden",
                             children: R
                         })]
-                    }), (N || d !== J - 1) && (0, _.jsxs)(dt, {
-                        className: `${M}-control-next`,
+                    }), (N || d !== J - 1) && (0, _.jsxs)(ct, {
+                        className: `${F}-control-next`,
                         onClick: ee,
                         children: [D, L && (0, _.jsx)("span", {
                             className: "visually-hidden",
                             children: L
                         })]
                     })]
                 })]
             })
         }));
-        vr.displayName = "Carousel";
-        const _r = Object.assign(vr, {
-            Caption: gr,
-            Item: yr
+        gr.displayName = "Carousel";
+        const br = Object.assign(gr, {
+            Caption: dr,
+            Item: fr
         });
-        var xr = ["items", "active_index", "style", "class_name", "className", "loading_state", "setProps", "interval"],
-            Or = function(t) {
+        var yr = ["items", "active_index", "style", "class_name", "className", "loading_state", "setProps", "interval"],
+            hr = function(t) {
                 var n = t.items,
                     r = t.active_index,
                     a = t.style,
                     s = t.class_name,
                     i = t.className,
                     c = t.loading_state,
                     u = t.setProps,
                     d = t.interval,
-                    p = o(t, xr),
+                    p = o(t, yr),
                     f = n.map((function(t) {
                         t.imgClassName = void 0 !== t.imgClassName ? t.imgClassName : "d-block w-100";
                         var n = t.href ? {
                             href: t.href,
                             external_link: t.external_link,
                             target: t.target || "_self"
                         } : {};
-                        return l().createElement(_r.Item, e({
+                        return l().createElement(br.Item, e({
                             key: t.key,
-                            as: t.href ? Bt : "div"
+                            as: t.href ? Mt : "div"
                         }, n), l().createElement("img", {
                             src: t.src,
                             className: t.img_class_name || t.imgClassName,
                             style: t.img_style,
                             alt: t.alt
-                        }), l().createElement(_r.Caption, {
+                        }), l().createElement(br.Caption, {
                             className: t.caption_class_name || t.captionClassName
                         }, t.header && l().createElement("h5", null, t.header), t.caption && l().createElement("p", null, t.caption)))
                     }));
                 return l().createElement("div", {
                     style: a,
                     className: s || i
-                }, l().createElement(_r, e({
+                }, l().createElement(br, e({
                     "data-dash-is-loading": c && c.is_loading || void 0,
                     activeIndex: r,
                     onSelect: function(e) {
                         return u({
                             active_index: e
                         })
                     },
                     interval: d || null
                 }, m(["persistence", "persisted_props", "persistence_type", "setProps"], p)), f))
             };
-        Or.defaultProps = {
+        hr.defaultProps = {
             active_index: 0,
             controls: !0,
             indicators: !0,
             persisted_props: ["active_index"],
             persistence_type: "local"
-        }, Or.propTypes = {
+        }, hr.propTypes = {
             id: u().string,
             style: u().object,
             class_name: u().string,
             className: u().string,
             items: u().arrayOf(u().exact({
                 key: u().string,
                 src: u().string,
@@ -3485,16 +3429,16 @@
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["active_index"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             setProps: u().func
         };
-        const wr = Or;
-        var Nr = function(e) {
+        const vr = hr;
+        var _r = function(e) {
             var t = e.value,
                 n = e.disabled,
                 r = e.className,
                 a = e.class_name,
                 s = e.style,
                 o = e.id,
                 i = e.input_class_name,
@@ -3528,15 +3472,15 @@
             }), l().createElement("label", {
                 id: p,
                 style: f,
                 className: b()(m || g, "form-check-label", "form-label"),
                 htmlFor: o
             }, d))
         };
-        Nr.propTypes = {
+        _r.propTypes = {
             id: u().string,
             class_name: u().string,
             className: u().string,
             style: u().object,
             input_style: u().object,
             inputStyle: u().object,
             input_class_name: u().string,
@@ -3555,129 +3499,129 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             setProps: u().func
-        }, Nr.defaultProps = {
+        }, _r.defaultProps = {
             inputStyle: {},
             input_style: null,
             inputClassName: "",
             input_class_name: "",
             labelStyle: {},
             label_style: null,
             labelClassName: "",
             label_class_name: "",
             persisted_props: ["value"],
             persistence_type: "local",
             value: !1,
             disabled: !1
         };
-        const Er = Nr;
+        const xr = _r;
 
-        function jr(e) {
+        function Or(e) {
             for (var t, n = []; !(t = e.next()).done;) n.push(t.value);
             return n
         }
 
-        function kr(e, t, n) {
+        function wr(e, t, n) {
             for (var r = 0, a = n.length; r < a;) {
                 if (e(t, n[r])) return !0;
                 r += 1
             }
             return !1
         }
 
-        function Pr(e, t) {
+        function Nr(e, t) {
             return Object.prototype.hasOwnProperty.call(t, e)
         }
-        const Cr = "function" == typeof Object.is ? Object.is : function(e, t) {
+        const Er = "function" == typeof Object.is ? Object.is : function(e, t) {
             return e === t ? 0 !== e || 1 / e == 1 / t : e != e && t != t
         };
-        var Tr = Object.prototype.toString;
-        const Sr = function() {
-            return "[object Arguments]" === Tr.call(arguments) ? function(e) {
-                return "[object Arguments]" === Tr.call(e)
+        var jr = Object.prototype.toString;
+        const kr = function() {
+            return "[object Arguments]" === jr.call(arguments) ? function(e) {
+                return "[object Arguments]" === jr.call(e)
             } : function(e) {
-                return Pr("callee", e)
+                return Nr("callee", e)
             }
         }();
-        var Rr = !{
+        var Pr = !{
                 toString: null
             }.propertyIsEnumerable("toString"),
-            Dr = ["constructor", "valueOf", "isPrototypeOf", "toString", "propertyIsEnumerable", "hasOwnProperty", "toLocaleString"],
-            Lr = function() {
+            Cr = ["constructor", "valueOf", "isPrototypeOf", "toString", "propertyIsEnumerable", "hasOwnProperty", "toLocaleString"],
+            Tr = function() {
                 return arguments.propertyIsEnumerable("length")
             }(),
-            $r = function(e, t) {
+            Sr = function(e, t) {
                 for (var n = 0; n < e.length;) {
                     if (e[n] === t) return !0;
                     n += 1
                 }
                 return !1
             };
-        const Ir = "function" != typeof Object.keys || Lr ? p((function(e) {
+        const Rr = "function" != typeof Object.keys || Tr ? p((function(e) {
             if (Object(e) !== e) return [];
             var t, n, r = [],
-                a = Lr && Sr(e);
-            for (t in e) !Pr(t, e) || a && "length" === t || (r[r.length] = t);
-            if (Rr)
-                for (n = Dr.length - 1; n >= 0;) Pr(t = Dr[n], e) && !$r(r, t) && (r[r.length] = t), n -= 1;
+                a = Tr && kr(e);
+            for (t in e) !Nr(t, e) || a && "length" === t || (r[r.length] = t);
+            if (Pr)
+                for (n = Cr.length - 1; n >= 0;) Nr(t = Cr[n], e) && !Sr(r, t) && (r[r.length] = t), n -= 1;
             return r
         })) : p((function(e) {
             return Object(e) !== e ? [] : Object.keys(e)
         }));
 
-        function Ar(e, t, n, r) {
-            var a = jr(e);
+        function Dr(e, t, n, r) {
+            var a = Or(e);
 
             function s(e, t) {
-                return Fr(e, t, n.slice(), r.slice())
+                return Lr(e, t, n.slice(), r.slice())
             }
-            return !kr((function(e, t) {
-                return !kr(s, t, e)
-            }), jr(t), a)
+            return !wr((function(e, t) {
+                return !wr(s, t, e)
+            }), Or(t), a)
         }
 
-        function Fr(e, t, n, r) {
-            if (Cr(e, t)) return !0;
+        function Lr(e, t, n, r) {
+            if (Er(e, t)) return !0;
             var a, s, o = Re(e);
             if (o !== Re(t)) return !1;
             if (null == e || null == t) return !1;
             if ("function" == typeof e["fantasy-land/equals"] || "function" == typeof t["fantasy-land/equals"]) return "function" == typeof e["fantasy-land/equals"] && e["fantasy-land/equals"](t) && "function" == typeof t["fantasy-land/equals"] && t["fantasy-land/equals"](e);
             if ("function" == typeof e.equals || "function" == typeof t.equals) return "function" == typeof e.equals && e.equals(t) && "function" == typeof t.equals && t.equals(e);
             switch (o) {
                 case "Arguments":
                 case "Array":
                 case "Object":
                     if ("function" == typeof e.constructor && "Promise" === (a = e.constructor, null == (s = String(a).match(/^function (\w*)/)) ? "" : s[1])) return e === t;
                     break;
                 case "Boolean":
                 case "Number":
                 case "String":
-                    if (typeof e != typeof t || !Cr(e.valueOf(), t.valueOf())) return !1;
+                    if (typeof e != typeof t || !Er(e.valueOf(), t.valueOf())) return !1;
                     break;
                 case "Date":
-                    if (!Cr(e.valueOf(), t.valueOf())) return !1;
+                    if (!Er(e.valueOf(), t.valueOf())) return !1;
                     break;
                 case "Error":
                     return e.name === t.name && e.message === t.message;
                 case "RegExp":
                     if (e.source !== t.source || e.global !== t.global || e.ignoreCase !== t.ignoreCase || e.multiline !== t.multiline || e.sticky !== t.sticky || e.unicode !== t.unicode) return !1
             }
             for (var i = n.length - 1; i >= 0;) {
                 if (n[i] === e) return r[i] === t;
                 i -= 1
             }
             switch (o) {
                 case "Map":
-                    return e.size === t.size && Ar(e.entries(), t.entries(), n.concat([e]), r.concat([t]));
+                    return e.size === t.size && Dr(e.entries(), t.entries(), n.concat([e]), r.concat([t]));
                 case "Set":
-                    return e.size === t.size && Ar(e.values(), t.values(), n.concat([e]), r.concat([t]));
+                    return e.size === t.size && Dr(e.values(), t.values(), n.concat([e]), r.concat([t]));
                 case "Arguments":
                 case "Array":
                 case "Object":
                 case "Boolean":
                 case "Number":
                 case "String":
                 case "Date":
@@ -3693,30 +3637,30 @@
                 case "Float32Array":
                 case "Float64Array":
                 case "ArrayBuffer":
                     break;
                 default:
                     return !1
             }
-            var l = Ir(e);
-            if (l.length !== Ir(t).length) return !1;
+            var l = Rr(e);
+            if (l.length !== Rr(t).length) return !1;
             var c = n.concat([e]),
                 u = r.concat([t]);
             for (i = l.length - 1; i >= 0;) {
                 var d = l[i];
-                if (!Pr(d, t) || !Fr(t[d], e[d], c, u)) return !1;
+                if (!Nr(d, t) || !Lr(t[d], e[d], c, u)) return !1;
                 i -= 1
             }
             return !0
         }
-        const Mr = f((function(e, t) {
-            return Fr(e, t, [], [])
+        const Ir = f((function(e, t) {
+            return Lr(e, t, [], [])
         }));
 
-        function Br(e, t) {
+        function $r(e, t) {
             return function(e, t, n) {
                 var r, a;
                 if ("function" == typeof e.indexOf) switch (typeof t) {
                     case "number":
                         if (0 === t) {
                             for (r = 1 / t; n < e.length;) {
                                 if (0 === (a = e[n]) && 1 / a === r) return n;
@@ -3737,23 +3681,23 @@
                     case "function":
                     case "undefined":
                         return e.indexOf(t, n);
                     case "object":
                         if (null === t) return e.indexOf(t, n)
                 }
                 for (; n < e.length;) {
-                    if (Mr(e[n], t)) return n;
+                    if (Ir(e[n], t)) return n;
                     n += 1
                 }
                 return -1
             }(t, e, 0) >= 0
         }
-        const zr = f(Br);
+        const Ar = f($r);
 
-        function Kr(e, t) {
+        function Mr(e, t) {
             switch (e) {
                 case 0:
                     return function() {
                         return t.apply(this, arguments)
                     };
                 case 1:
                     return function(e) {
@@ -3796,179 +3740,179 @@
                         return t.apply(this, arguments)
                     };
                 default:
                     throw new Error("First argument to _arity must be a non-negative integer no greater than ten")
             }
         }
 
-        function Hr(e, t, n) {
+        function Fr(e, t, n) {
             return function() {
                 for (var r = [], a = 0, s = e, o = 0; o < t.length || a < arguments.length;) {
                     var i;
                     o < t.length && (!d(t[o]) || a >= arguments.length) ? i = t[o] : (i = arguments[a], a += 1), r[o] = i, d(i) || (s -= 1), o += 1
                 }
-                return s <= 0 ? n.apply(this, r) : Kr(s, Hr(e, r, n))
+                return s <= 0 ? n.apply(this, r) : Mr(s, Fr(e, r, n))
             }
         }
-        const Ur = f((function(e, t) {
-                return 1 === e ? p(t) : Kr(e, Hr(e, [], t))
+        const Br = f((function(e, t) {
+                return 1 === e ? p(t) : Mr(e, Fr(e, [], t))
             })),
-            Wr = p((function(e) {
-                return Ur(e.length, (function(t, n) {
+            zr = p((function(e) {
+                return Br(e.length, (function(t, n) {
                     var r = Array.prototype.slice.call(arguments, 0);
                     return r[0] = n, r[1] = t, e.apply(this, r)
                 }))
             })),
-            qr = Array.isArray || function(e) {
+            Kr = Array.isArray || function(e) {
                 return null != e && e.length >= 0 && "[object Array]" === Object.prototype.toString.call(e)
             };
 
-        function Vr(e, t, n) {
+        function Hr(e, t, n) {
             return function() {
                 if (0 === arguments.length) return n();
                 var r = Array.prototype.slice.call(arguments, 0),
                     a = r.pop();
-                if (!qr(a)) {
+                if (!Kr(a)) {
                     for (var s = 0; s < e.length;) {
                         if ("function" == typeof a[e[s]]) return a[e[s]].apply(a, r);
                         s += 1
                     }
                     if (function(e) {
                             return null != e && "function" == typeof e["@@transducer/step"]
                         }(a)) return t.apply(null, r)(a)
                 }
                 return n.apply(this, arguments)
             }
         }
-        const Gr = p((function(e) {
-            return !!qr(e) || !!e && "object" == typeof e && ! function(e) {
+        const Wr = p((function(e) {
+            return !!Kr(e) || !!e && "object" == typeof e && ! function(e) {
                 return "[object String]" === Object.prototype.toString.call(e)
             }(e) && (1 === e.nodeType ? !!e.length : 0 === e.length || e.length > 0 && e.hasOwnProperty(0) && e.hasOwnProperty(e.length - 1))
         }));
-        var Yr = function() {
+        var Ur = function() {
             function e(e) {
                 this.f = e
             }
             return e.prototype["@@transducer/init"] = function() {
                 throw new Error("init not implemented on XWrap")
             }, e.prototype["@@transducer/result"] = function(e) {
                 return e
             }, e.prototype["@@transducer/step"] = function(e, t) {
                 return this.f(e, t)
             }, e
         }();
-        const Xr = f((function(e, t) {
-            return Kr(e.length, (function() {
+        const qr = f((function(e, t) {
+            return Mr(e.length, (function() {
                 return e.apply(t, arguments)
             }))
         }));
 
-        function Jr(e, t, n) {
+        function Vr(e, t, n) {
             for (var r = n.next(); !r.done;) {
                 if ((t = e["@@transducer/step"](t, r.value)) && t["@@transducer/reduced"]) {
                     t = t["@@transducer/value"];
                     break
                 }
                 r = n.next()
             }
             return e["@@transducer/result"](t)
         }
 
-        function Qr(e, t, n, r) {
-            return e["@@transducer/result"](n[r](Xr(e["@@transducer/step"], e), t))
+        function Gr(e, t, n, r) {
+            return e["@@transducer/result"](n[r](qr(e["@@transducer/step"], e), t))
         }
-        var Zr = "undefined" != typeof Symbol ? Symbol.iterator : "@@iterator";
-        const ea = function() {
+        var Yr = "undefined" != typeof Symbol ? Symbol.iterator : "@@iterator";
+        const Xr = function() {
                 return this.xf["@@transducer/init"]()
             },
-            ta = function(e) {
+            Jr = function(e) {
                 return this.xf["@@transducer/result"](e)
             };
-        var na = function() {
+        var Qr = function() {
             function e(e, t) {
                 this.xf = t, this.f = e
             }
-            return e.prototype["@@transducer/init"] = ea, e.prototype["@@transducer/result"] = ta, e.prototype["@@transducer/step"] = function(e, t) {
+            return e.prototype["@@transducer/init"] = Xr, e.prototype["@@transducer/result"] = Jr, e.prototype["@@transducer/step"] = function(e, t) {
                 return this.f(t) ? this.xf["@@transducer/step"](e, t) : e
             }, e
         }();
-        const ra = f(Vr(["filter"], f((function(e, t) {
-                return new na(e, t)
+        const Zr = f(Hr(["filter"], f((function(e, t) {
+                return new Qr(e, t)
             })), (function(e, t) {
                 return n = t, "[object Object]" === Object.prototype.toString.call(n) ? function(e, t, n) {
                     if ("function" == typeof e && (e = function(e) {
-                            return new Yr(e)
-                        }(e)), Gr(n)) return function(e, t, n) {
+                            return new Ur(e)
+                        }(e)), Wr(n)) return function(e, t, n) {
                         for (var r = 0, a = n.length; r < a;) {
                             if ((t = e["@@transducer/step"](t, n[r])) && t["@@transducer/reduced"]) {
                                 t = t["@@transducer/value"];
                                 break
                             }
                             r += 1
                         }
                         return e["@@transducer/result"](t)
                     }(e, t, n);
-                    if ("function" == typeof n["fantasy-land/reduce"]) return Qr(e, t, n, "fantasy-land/reduce");
-                    if (null != n[Zr]) return Jr(e, t, n[Zr]());
-                    if ("function" == typeof n.next) return Jr(e, t, n);
-                    if ("function" == typeof n.reduce) return Qr(e, t, n, "reduce");
+                    if ("function" == typeof n["fantasy-land/reduce"]) return Gr(e, t, n, "fantasy-land/reduce");
+                    if (null != n[Yr]) return Vr(e, t, n[Yr]());
+                    if ("function" == typeof n.next) return Vr(e, t, n);
+                    if ("function" == typeof n.reduce) return Gr(e, t, n, "reduce");
                     throw new TypeError("reduce: list must be array or iterable")
                 }((function(n, r) {
                     return e(t[r]) && (n[r] = t[r]), n
-                }), {}, Ir(t)) : function(e, t) {
+                }), {}, Rr(t)) : function(e, t) {
                     for (var n = 0, r = t.length, a = []; n < r;) e(t[n]) && (a[a.length] = t[n]), n += 1;
                     return a
                 }(e, t);
                 var n
             }))),
-            aa = f((function(e, t) {
-                return ra((n = e, function() {
+            ea = f((function(e, t) {
+                return Zr((n = e, function() {
                     return !n.apply(this, arguments)
                 }), t);
                 var n
             })),
-            sa = f((function(e, t) {
-                return aa(Wr(Br)(e), t)
+            ta = f((function(e, t) {
+                return ea(zr($r)(e), t)
             })),
-            oa = f((function(e, t) {
+            na = f((function(e, t) {
                 return function(e, t) {
                     var n;
                     t = t || [];
                     var r = (e = e || []).length,
                         a = t.length,
                         s = [];
                     for (n = 0; n < r;) s[s.length] = e[n], n += 1;
                     for (n = 0; n < a;) s[s.length] = t[n], n += 1;
                     return s
                 }(t, [e])
             }));
 
-        function ia(e, t) {
+        function ra(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function la(e) {
+        function aa(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? ia(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ia(Object(n)).forEach((function(t) {
+                t % 2 ? ra(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ra(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var ca = function(e) {
+        var sa = function(e) {
             var t = e.className,
                 n = e.class_name,
                 r = e.id,
                 a = e.options,
                 s = e.style,
                 o = e.key,
                 i = e.loading_state,
@@ -3992,17 +3936,17 @@
                             v = e.label_style,
                             _ = e.labelCheckedStyle,
                             x = e.label_checked_style,
                             O = e.setProps,
                             w = e.inline,
                             N = e.value,
                             E = e.switch,
-                            j = zr(t.value, N),
-                            k = j ? la(la({}, u || i), p || d) : u || i,
-                            P = j ? la(la({}, v || h), x || _) : v || h,
+                            j = Ar(t.value, N),
+                            k = j ? aa(aa({}, u || i), p || d) : u || i,
+                            P = j ? aa(aa({}, v || h), x || _) : v || h,
                             C = t.input_id || "_dbcprivate_checklist_".concat(n, "_input_").concat(t.value);
                         return l().createElement("div", {
                             className: b()("form-check", w && "form-check-inline", E && "form-switch"),
                             key: t.value
                         }, l().createElement("input", {
                             id: C,
                             name: c,
@@ -4010,15 +3954,15 @@
                             checked: j,
                             className: b()("form-check-input", a || r, j && (o || s)),
                             disabled: Boolean(t.disabled),
                             style: k,
                             type: "checkbox",
                             onChange: function() {
                                 var e;
-                                e = zr(t.value, N) ? sa([t.value], N) : oa(t.value, N), O({
+                                e = Ar(t.value, N) ? ta([t.value], N) : na(t.value, N), O({
                                     value: e
                                 })
                             }
                         }), l().createElement("label", {
                             id: t.label_id,
                             style: P,
                             className: b()("form-check-label", m || f, j && (y || g)),
@@ -4031,15 +3975,15 @@
                 id: r,
                 style: s,
                 className: n || t,
                 key: o,
                 "data-dash-is-loading": i && i.is_loading || void 0
             }, u)
         };
-        ca.propTypes = {
+        sa.propTypes = {
             options: u().oneOfType([u().arrayOf(u().oneOfType([u().string, u().number])), u().object, u().arrayOf(u().exact({
                 label: u().node.isRequired,
                 value: u().oneOfType([u().string, u().number]).isRequired,
                 disabled: u().bool,
                 input_id: u().string,
                 label_id: u().string
             }))]),
@@ -4073,31 +4017,31 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             name: u().string
-        }, ca.defaultProps = {
+        }, sa.defaultProps = {
             inputStyle: {},
             input_style: null,
             inputClassName: "",
             input_class_name: "",
             labelStyle: {},
             label_style: null,
             labelClassName: "",
             label_class_name: "",
             options: [],
             value: [],
             persisted_props: ["value"],
             persistence_type: "local"
         };
-        const ua = ca;
+        const oa = sa;
 
-        function da({
+        function ia({
             as: e,
             bsPrefix: t,
             className: n,
             ...r
         }) {
             t = E(t, "col");
             const a = j(),
@@ -4119,122 +4063,122 @@
                 className: b()(n, ...o, ...i)
             }, {
                 as: e,
                 bsPrefix: t,
                 spans: o
             }]
         }
-        const pa = i.forwardRef(((e, t) => {
+        const la = i.forwardRef(((e, t) => {
             const [{
                 className: n,
                 ...r
             }, {
                 as: a = "div",
                 bsPrefix: s,
                 spans: o
-            }] = da(e);
+            }] = ia(e);
             return (0, _.jsx)(a, {
                 ...r,
                 ref: t,
                 className: b()(n, !o.length && s)
             })
         }));
-        pa.displayName = "Col";
-        const fa = pa;
-        var ma = ["children", "width", "xs", "sm", "md", "lg", "xl", "xxl", "align", "className", "class_name", "loading_state"],
-            ga = {
+        la.displayName = "Col";
+        const ca = la;
+        var ua = ["children", "width", "xs", "sm", "md", "lg", "xl", "xxl", "align", "className", "class_name", "loading_state"],
+            da = {
                 start: "align-self-start",
                 center: "align-self-center",
                 end: "align-self-end",
                 stretch: "align-self-stretch",
                 baseline: "align-self-baseline"
             },
-            ba = function(t) {
+            pa = function(t) {
                 var n = t.children,
                     r = t.width,
                     a = t.xs,
                     s = t.sm,
                     i = t.md,
                     c = t.lg,
                     u = t.xl,
                     d = t.xxl,
                     p = t.align,
                     f = t.className,
                     g = t.class_name,
                     y = t.loading_state,
-                    h = o(t, ma);
+                    h = o(t, ua);
                 [r, a, s, i, c, u, d].forEach((function(e) {
                     "object" === Te(e) && null !== e && (e.span = e.size)
                 }));
-                var v = p && ga[p],
+                var v = p && da[p],
                     _ = b()(g || f, v);
-                return l().createElement(fa, e({
+                return l().createElement(ca, e({
                     xs: a || r,
                     sm: s,
                     md: i,
                     lg: c,
                     xl: u,
                     xxl: d,
                     className: _
                 }, m(["setProps"], h), {
                     "data-dash-is-loading": y && y.is_loading || void 0
                 }), n)
             },
-            ya = u().oneOfType([u().number, u().string]),
-            ha = u().oneOfType([u().string, u().number, u().bool, u().shape({
+            fa = u().oneOfType([u().number, u().string]),
+            ma = u().oneOfType([u().string, u().number, u().bool, u().shape({
                 size: u().oneOfType([u().bool, u().number, u().string]),
-                order: ya,
-                offset: ya
+                order: fa,
+                offset: fa
             })]);
-        ba.propTypes = {
+        pa.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
-            width: ha,
-            xs: ha,
-            sm: ha,
-            md: ha,
-            lg: ha,
-            xl: ha,
-            xxl: ha,
+            width: ma,
+            xs: ma,
+            sm: ma,
+            md: ma,
+            lg: ma,
+            xl: ma,
+            xxl: ma,
             align: u().oneOf(["start", "center", "end", "stretch", "baseline"]),
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const va = ba;
-        var _a = ["children", "is_open", "navbar", "loading_state", "className", "class_name", "tag"],
-            xa = l().forwardRef((function(t, n) {
+        const ga = pa;
+        var ba = ["children", "is_open", "navbar", "loading_state", "className", "class_name", "tag"],
+            ya = l().forwardRef((function(t, n) {
                 var r = t.children,
                     a = t.is_open,
                     s = t.navbar,
                     i = t.loading_state,
                     c = t.className,
                     u = t.class_name,
                     d = t.tag,
-                    p = o(t, _a);
+                    p = o(t, ba);
                 return l().createElement(pe, e({
                     in: a,
                     as: d,
                     className: u || c
                 }, m(["setProps"], p), {
                     "data-dash-is-loading": i && i.is_loading || void 0
                 }), l().createElement("div", {
                     ref: n,
                     className: s && "navbar-collapse"
                 }, r))
             }));
-        xa.defaultProps = {
+        ya.defaultProps = {
             dimension: "height"
-        }, xa.propTypes = {
+        }, ya.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             is_open: u().bool,
@@ -4242,117 +4186,117 @@
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             dimension: u().oneOf(["height", "width"])
         };
-        const Oa = xa,
-            wa = i.forwardRef((({
+        const ha = ya,
+            va = i.forwardRef((({
                 bsPrefix: e,
                 fluid: t = !1,
                 as: n = "div",
                 className: r,
                 ...a
             }, s) => {
                 const o = E(e, "container"),
                     i = "string" == typeof t ? `-${t}` : "-fluid";
                 return (0, _.jsx)(n, {
                     ref: s,
                     ...a,
                     className: b()(r, t ? `${o}${i}` : o)
                 })
             }));
-        wa.displayName = "Container";
-        const Na = wa;
-        var Ea = ["children", "loading_state", "className", "class_name", "tag"],
-            ja = function(t) {
+        va.displayName = "Container";
+        const _a = va;
+        var xa = ["children", "loading_state", "className", "class_name", "tag"],
+            Oa = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.tag,
-                    c = o(t, Ea);
-                return l().createElement(Na, e({
+                    c = o(t, xa);
+                return l().createElement(_a, e({
                     as: i,
                     className: s || a
                 }, m(["setProps"], c), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        ja.propTypes = {
+        Oa.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             fluid: u().oneOfType([u().bool, u().string]),
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const ka = ja;
-        var Pa = Function.prototype.bind.call(Function.prototype.call, [].slice);
+        const wa = Oa;
+        var Na = Function.prototype.bind.call(Function.prototype.call, [].slice);
 
-        function Ca(e, t) {
-            return Pa(e.querySelectorAll(t))
+        function Ea(e, t) {
+            return Na(e.querySelectorAll(t))
         }
 
-        function Ta(e, t, n) {
+        function ja(e, t, n) {
             const r = (0, i.useRef)(void 0 !== e),
                 [a, s] = (0, i.useState)(t),
                 o = void 0 !== e,
                 l = r.current;
             return r.current = o, !o && l && a !== t && s(t), [o ? e : a, (0, i.useCallback)(((...e) => {
                 const [t, ...r] = e;
                 let a = null == n ? void 0 : n(t, ...r);
                 return s(t), a
             }), [n])]
         }
 
-        function Sa() {
+        function ka() {
             const [, e] = (0, i.useReducer)((e => !e), !1);
             return e
         }
-        const Ra = i.createContext(null);
-        var Da = Object.prototype.hasOwnProperty;
+        const Pa = i.createContext(null);
+        var Ca = Object.prototype.hasOwnProperty;
 
-        function La(e, t, n) {
+        function Ta(e, t, n) {
             for (n of e.keys())
-                if ($a(n, t)) return n
+                if (Sa(n, t)) return n
         }
 
-        function $a(e, t) {
+        function Sa(e, t) {
             var n, r, a;
             if (e === t) return !0;
             if (e && t && (n = e.constructor) === t.constructor) {
                 if (n === Date) return e.getTime() === t.getTime();
                 if (n === RegExp) return e.toString() === t.toString();
                 if (n === Array) {
                     if ((r = e.length) === t.length)
-                        for (; r-- && $a(e[r], t[r]););
+                        for (; r-- && Sa(e[r], t[r]););
                     return -1 === r
                 }
                 if (n === Set) {
                     if (e.size !== t.size) return !1;
                     for (r of e) {
-                        if ((a = r) && "object" == typeof a && !(a = La(t, a))) return !1;
+                        if ((a = r) && "object" == typeof a && !(a = Ta(t, a))) return !1;
                         if (!t.has(a)) return !1
                     }
                     return !0
                 }
                 if (n === Map) {
                     if (e.size !== t.size) return !1;
                     for (r of e) {
-                        if ((a = r[0]) && "object" == typeof a && !(a = La(t, a))) return !1;
-                        if (!$a(r[1], t.get(a))) return !1
+                        if ((a = r[0]) && "object" == typeof a && !(a = Ta(t, a))) return !1;
+                        if (!Sa(r[1], t.get(a))) return !1
                     }
                     return !0
                 }
                 if (n === ArrayBuffer) e = new Uint8Array(e), t = new Uint8Array(t);
                 else if (n === DataView) {
                     if ((r = e.byteLength) === t.byteLength)
                         for (; r-- && e.getInt8(r) === t.getInt8(r););
@@ -4361,70 +4305,70 @@
                 if (ArrayBuffer.isView(e)) {
                     if ((r = e.byteLength) === t.byteLength)
                         for (; r-- && e[r] === t[r];);
                     return -1 === r
                 }
                 if (!n || "object" == typeof e) {
                     for (n in r = 0, e) {
-                        if (Da.call(e, n) && ++r && !Da.call(t, n)) return !1;
-                        if (!(n in t) || !$a(e[n], t[n])) return !1
+                        if (Ca.call(e, n) && ++r && !Ca.call(t, n)) return !1;
+                        if (!(n in t) || !Sa(e[n], t[n])) return !1
                     }
                     return Object.keys(t).length === r
                 }
             }
             return e != e && t != t
         }
 
-        function Ia(e) {
+        function Ra(e) {
             return e.split("-")[0]
         }
 
-        function Aa(e) {
+        function Da(e) {
             if (null == e) return window;
             if ("[object Window]" !== e.toString()) {
                 var t = e.ownerDocument;
                 return t && t.defaultView || window
             }
             return e
         }
 
-        function Fa(e) {
-            return e instanceof Aa(e).Element || e instanceof Element
+        function La(e) {
+            return e instanceof Da(e).Element || e instanceof Element
         }
 
-        function Ma(e) {
-            return e instanceof Aa(e).HTMLElement || e instanceof HTMLElement
+        function Ia(e) {
+            return e instanceof Da(e).HTMLElement || e instanceof HTMLElement
         }
 
-        function Ba(e) {
-            return "undefined" != typeof ShadowRoot && (e instanceof Aa(e).ShadowRoot || e instanceof ShadowRoot)
+        function $a(e) {
+            return "undefined" != typeof ShadowRoot && (e instanceof Da(e).ShadowRoot || e instanceof ShadowRoot)
         }
-        var za = Math.max,
-            Ka = Math.min,
-            Ha = Math.round;
+        var Aa = Math.max,
+            Ma = Math.min,
+            Fa = Math.round;
 
-        function Ua() {
+        function Ba() {
             var e = navigator.userAgentData;
             return null != e && e.brands && Array.isArray(e.brands) ? e.brands.map((function(e) {
                 return e.brand + "/" + e.version
             })).join(" ") : navigator.userAgent
         }
 
-        function Wa() {
-            return !/^((?!chrome|android).)*safari/i.test(Ua())
+        function za() {
+            return !/^((?!chrome|android).)*safari/i.test(Ba())
         }
 
-        function qa(e, t, n) {
+        function Ka(e, t, n) {
             void 0 === t && (t = !1), void 0 === n && (n = !1);
             var r = e.getBoundingClientRect(),
                 a = 1,
                 s = 1;
-            t && Ma(e) && (a = e.offsetWidth > 0 && Ha(r.width) / e.offsetWidth || 1, s = e.offsetHeight > 0 && Ha(r.height) / e.offsetHeight || 1);
-            var o = (Fa(e) ? Aa(e) : window).visualViewport,
-                i = !Wa() && n,
+            t && Ia(e) && (a = e.offsetWidth > 0 && Fa(r.width) / e.offsetWidth || 1, s = e.offsetHeight > 0 && Fa(r.height) / e.offsetHeight || 1);
+            var o = (La(e) ? Da(e) : window).visualViewport,
+                i = !za() && n,
                 l = (r.left + (i && o ? o.offsetLeft : 0)) / a,
                 c = (r.top + (i && o ? o.offsetTop : 0)) / s,
                 u = r.width / a,
                 d = r.height / s;
             return {
                 width: u,
                 height: d,
@@ -4433,173 +4377,173 @@
                 bottom: c + d,
                 left: l,
                 x: l,
                 y: c
             }
         }
 
-        function Va(e) {
-            var t = qa(e),
+        function Ha(e) {
+            var t = Ka(e),
                 n = e.offsetWidth,
                 r = e.offsetHeight;
             return Math.abs(t.width - n) <= 1 && (n = t.width), Math.abs(t.height - r) <= 1 && (r = t.height), {
                 x: e.offsetLeft,
                 y: e.offsetTop,
                 width: n,
                 height: r
             }
         }
 
-        function Ga(e, t) {
+        function Wa(e, t) {
             var n = t.getRootNode && t.getRootNode();
             if (e.contains(t)) return !0;
-            if (n && Ba(n)) {
+            if (n && $a(n)) {
                 var r = t;
                 do {
                     if (r && e.isSameNode(r)) return !0;
                     r = r.parentNode || r.host
                 } while (r)
             }
             return !1
         }
 
-        function Ya(e) {
+        function Ua(e) {
             return e ? (e.nodeName || "").toLowerCase() : null
         }
 
-        function Xa(e) {
-            return Aa(e).getComputedStyle(e)
+        function qa(e) {
+            return Da(e).getComputedStyle(e)
         }
 
-        function Ja(e) {
-            return ["table", "td", "th"].indexOf(Ya(e)) >= 0
+        function Va(e) {
+            return ["table", "td", "th"].indexOf(Ua(e)) >= 0
         }
 
-        function Qa(e) {
-            return ((Fa(e) ? e.ownerDocument : e.document) || window.document).documentElement
+        function Ga(e) {
+            return ((La(e) ? e.ownerDocument : e.document) || window.document).documentElement
         }
 
-        function Za(e) {
-            return "html" === Ya(e) ? e : e.assignedSlot || e.parentNode || (Ba(e) ? e.host : null) || Qa(e)
+        function Ya(e) {
+            return "html" === Ua(e) ? e : e.assignedSlot || e.parentNode || ($a(e) ? e.host : null) || Ga(e)
         }
 
-        function es(e) {
-            return Ma(e) && "fixed" !== Xa(e).position ? e.offsetParent : null
+        function Xa(e) {
+            return Ia(e) && "fixed" !== qa(e).position ? e.offsetParent : null
         }
 
-        function ts(e) {
-            for (var t = Aa(e), n = es(e); n && Ja(n) && "static" === Xa(n).position;) n = es(n);
-            return n && ("html" === Ya(n) || "body" === Ya(n) && "static" === Xa(n).position) ? t : n || function(e) {
-                var t = /firefox/i.test(Ua());
-                if (/Trident/i.test(Ua()) && Ma(e) && "fixed" === Xa(e).position) return null;
-                var n = Za(e);
-                for (Ba(n) && (n = n.host); Ma(n) && ["html", "body"].indexOf(Ya(n)) < 0;) {
-                    var r = Xa(n);
+        function Ja(e) {
+            for (var t = Da(e), n = Xa(e); n && Va(n) && "static" === qa(n).position;) n = Xa(n);
+            return n && ("html" === Ua(n) || "body" === Ua(n) && "static" === qa(n).position) ? t : n || function(e) {
+                var t = /firefox/i.test(Ba());
+                if (/Trident/i.test(Ba()) && Ia(e) && "fixed" === qa(e).position) return null;
+                var n = Ya(e);
+                for ($a(n) && (n = n.host); Ia(n) && ["html", "body"].indexOf(Ua(n)) < 0;) {
+                    var r = qa(n);
                     if ("none" !== r.transform || "none" !== r.perspective || "paint" === r.contain || -1 !== ["transform", "perspective"].indexOf(r.willChange) || t && "filter" === r.willChange || t && r.filter && "none" !== r.filter) return n;
                     n = n.parentNode
                 }
                 return null
             }(e) || t
         }
 
-        function ns(e) {
+        function Qa(e) {
             return ["top", "bottom"].indexOf(e) >= 0 ? "x" : "y"
         }
 
-        function rs(e, t, n) {
-            return za(e, Ka(t, n))
+        function Za(e, t, n) {
+            return Aa(e, Ma(t, n))
         }
 
-        function as(e) {
+        function es(e) {
             return Object.assign({}, {
                 top: 0,
                 right: 0,
                 bottom: 0,
                 left: 0
             }, e)
         }
 
-        function ss(e, t) {
+        function ts(e, t) {
             return t.reduce((function(t, n) {
                 return t[n] = e, t
             }), {})
         }
-        var os = "top",
-            is = "bottom",
-            ls = "right",
-            cs = "left",
-            us = "auto",
-            ds = [os, is, ls, cs],
-            ps = "start",
-            fs = "end",
-            ms = "viewport",
-            gs = "popper",
-            bs = ds.reduce((function(e, t) {
-                return e.concat([t + "-" + ps, t + "-" + fs])
+        var ns = "top",
+            rs = "bottom",
+            as = "right",
+            ss = "left",
+            os = "auto",
+            is = [ns, rs, as, ss],
+            ls = "start",
+            cs = "end",
+            us = "viewport",
+            ds = "popper",
+            ps = is.reduce((function(e, t) {
+                return e.concat([t + "-" + ls, t + "-" + cs])
             }), []),
-            ys = [].concat(ds, [us]).reduce((function(e, t) {
-                return e.concat([t, t + "-" + ps, t + "-" + fs])
+            fs = [].concat(is, [os]).reduce((function(e, t) {
+                return e.concat([t, t + "-" + ls, t + "-" + cs])
             }), []),
-            hs = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
-        const vs = {
+            ms = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
+        const gs = {
             name: "arrow",
             enabled: !0,
             phase: "main",
             fn: function(e) {
                 var t, n = e.state,
                     r = e.name,
                     a = e.options,
                     s = n.elements.arrow,
                     o = n.modifiersData.popperOffsets,
-                    i = Ia(n.placement),
-                    l = ns(i),
-                    c = [cs, ls].indexOf(i) >= 0 ? "height" : "width";
+                    i = Ra(n.placement),
+                    l = Qa(i),
+                    c = [ss, as].indexOf(i) >= 0 ? "height" : "width";
                 if (s && o) {
                     var u = function(e, t) {
-                            return as("number" != typeof(e = "function" == typeof e ? e(Object.assign({}, t.rects, {
+                            return es("number" != typeof(e = "function" == typeof e ? e(Object.assign({}, t.rects, {
                                 placement: t.placement
-                            })) : e) ? e : ss(e, ds))
+                            })) : e) ? e : ts(e, is))
                         }(a.padding, n),
-                        d = Va(s),
-                        p = "y" === l ? os : cs,
-                        f = "y" === l ? is : ls,
+                        d = Ha(s),
+                        p = "y" === l ? ns : ss,
+                        f = "y" === l ? rs : as,
                         m = n.rects.reference[c] + n.rects.reference[l] - o[l] - n.rects.popper[c],
                         g = o[l] - n.rects.reference[l],
-                        b = ts(s),
+                        b = Ja(s),
                         y = b ? "y" === l ? b.clientHeight || 0 : b.clientWidth || 0 : 0,
                         h = m / 2 - g / 2,
                         v = u[p],
                         _ = y - d[c] - u[f],
                         x = y / 2 - d[c] / 2 + h,
-                        O = rs(v, x, _),
+                        O = Za(v, x, _),
                         w = l;
                     n.modifiersData[r] = ((t = {})[w] = O, t.centerOffset = O - x, t)
                 }
             },
             effect: function(e) {
                 var t = e.state,
                     n = e.options.element,
                     r = void 0 === n ? "[data-popper-arrow]" : n;
-                null != r && ("string" != typeof r || (r = t.elements.popper.querySelector(r))) && Ga(t.elements.popper, r) && (t.elements.arrow = r)
+                null != r && ("string" != typeof r || (r = t.elements.popper.querySelector(r))) && Wa(t.elements.popper, r) && (t.elements.arrow = r)
             },
             requires: ["popperOffsets"],
             requiresIfExists: ["preventOverflow"]
         };
 
-        function _s(e) {
+        function bs(e) {
             return e.split("-")[1]
         }
-        var xs = {
+        var ys = {
             top: "auto",
             right: "auto",
             bottom: "auto",
             left: "auto"
         };
 
-        function Os(e) {
+        function hs(e) {
             var t, n = e.popper,
                 r = e.popperRect,
                 a = e.placement,
                 s = e.variation,
                 o = e.offsets,
                 i = e.position,
                 l = e.gpuAcceleration,
@@ -4616,480 +4560,480 @@
                 }) : {
                     x: f,
                     y: g
                 };
             f = b.x, g = b.y;
             var y = o.hasOwnProperty("x"),
                 h = o.hasOwnProperty("y"),
-                v = cs,
-                _ = os,
+                v = ss,
+                _ = ns,
                 x = window;
             if (c) {
-                var O = ts(n),
+                var O = Ja(n),
                     w = "clientHeight",
                     N = "clientWidth";
-                O === Aa(n) && "static" !== Xa(O = Qa(n)).position && "absolute" === i && (w = "scrollHeight", N = "scrollWidth"), (a === os || (a === cs || a === ls) && s === fs) && (_ = is, g -= (d && O === x && x.visualViewport ? x.visualViewport.height : O[w]) - r.height, g *= l ? 1 : -1), a !== cs && (a !== os && a !== is || s !== fs) || (v = ls, f -= (d && O === x && x.visualViewport ? x.visualViewport.width : O[N]) - r.width, f *= l ? 1 : -1)
+                O === Da(n) && "static" !== qa(O = Ga(n)).position && "absolute" === i && (w = "scrollHeight", N = "scrollWidth"), (a === ns || (a === ss || a === as) && s === cs) && (_ = rs, g -= (d && O === x && x.visualViewport ? x.visualViewport.height : O[w]) - r.height, g *= l ? 1 : -1), a !== ss && (a !== ns && a !== rs || s !== cs) || (v = as, f -= (d && O === x && x.visualViewport ? x.visualViewport.width : O[N]) - r.width, f *= l ? 1 : -1)
             }
             var E, j = Object.assign({
                     position: i
-                }, c && xs),
+                }, c && ys),
                 k = !0 === u ? function(e, t) {
                     var n = e.x,
                         r = e.y,
                         a = t.devicePixelRatio || 1;
                     return {
-                        x: Ha(n * a) / a || 0,
-                        y: Ha(r * a) / a || 0
+                        x: Fa(n * a) / a || 0,
+                        y: Fa(r * a) / a || 0
                     }
                 }({
                     x: f,
                     y: g
-                }, Aa(n)) : {
+                }, Da(n)) : {
                     x: f,
                     y: g
                 };
             return f = k.x, g = k.y, l ? Object.assign({}, j, ((E = {})[_] = h ? "0" : "", E[v] = y ? "0" : "", E.transform = (x.devicePixelRatio || 1) <= 1 ? "translate(" + f + "px, " + g + "px)" : "translate3d(" + f + "px, " + g + "px, 0)", E)) : Object.assign({}, j, ((t = {})[_] = h ? g + "px" : "", t[v] = y ? f + "px" : "", t.transform = "", t))
         }
-        const ws = {
+        const vs = {
             name: "computeStyles",
             enabled: !0,
             phase: "beforeWrite",
             fn: function(e) {
                 var t = e.state,
                     n = e.options,
                     r = n.gpuAcceleration,
                     a = void 0 === r || r,
                     s = n.adaptive,
                     o = void 0 === s || s,
                     i = n.roundOffsets,
                     l = void 0 === i || i,
                     c = {
-                        placement: Ia(t.placement),
-                        variation: _s(t.placement),
+                        placement: Ra(t.placement),
+                        variation: bs(t.placement),
                         popper: t.elements.popper,
                         popperRect: t.rects.popper,
                         gpuAcceleration: a,
                         isFixed: "fixed" === t.options.strategy
                     };
-                null != t.modifiersData.popperOffsets && (t.styles.popper = Object.assign({}, t.styles.popper, Os(Object.assign({}, c, {
+                null != t.modifiersData.popperOffsets && (t.styles.popper = Object.assign({}, t.styles.popper, hs(Object.assign({}, c, {
                     offsets: t.modifiersData.popperOffsets,
                     position: t.options.strategy,
                     adaptive: o,
                     roundOffsets: l
-                })))), null != t.modifiersData.arrow && (t.styles.arrow = Object.assign({}, t.styles.arrow, Os(Object.assign({}, c, {
+                })))), null != t.modifiersData.arrow && (t.styles.arrow = Object.assign({}, t.styles.arrow, hs(Object.assign({}, c, {
                     offsets: t.modifiersData.arrow,
                     position: "absolute",
                     adaptive: !1,
                     roundOffsets: l
                 })))), t.attributes.popper = Object.assign({}, t.attributes.popper, {
                     "data-popper-placement": t.placement
                 })
             },
             data: {}
         };
-        var Ns = {
+        var _s = {
             passive: !0
         };
-        const Es = {
+        const xs = {
             name: "eventListeners",
             enabled: !0,
             phase: "write",
             fn: function() {},
             effect: function(e) {
                 var t = e.state,
                     n = e.instance,
                     r = e.options,
                     a = r.scroll,
                     s = void 0 === a || a,
                     o = r.resize,
                     i = void 0 === o || o,
-                    l = Aa(t.elements.popper),
+                    l = Da(t.elements.popper),
                     c = [].concat(t.scrollParents.reference, t.scrollParents.popper);
                 return s && c.forEach((function(e) {
-                        e.addEventListener("scroll", n.update, Ns)
-                    })), i && l.addEventListener("resize", n.update, Ns),
+                        e.addEventListener("scroll", n.update, _s)
+                    })), i && l.addEventListener("resize", n.update, _s),
                     function() {
                         s && c.forEach((function(e) {
-                            e.removeEventListener("scroll", n.update, Ns)
-                        })), i && l.removeEventListener("resize", n.update, Ns)
+                            e.removeEventListener("scroll", n.update, _s)
+                        })), i && l.removeEventListener("resize", n.update, _s)
                     }
             },
             data: {}
         };
-        var js = {
+        var Os = {
             left: "right",
             right: "left",
             bottom: "top",
             top: "bottom"
         };
 
-        function ks(e) {
+        function ws(e) {
             return e.replace(/left|right|bottom|top/g, (function(e) {
-                return js[e]
+                return Os[e]
             }))
         }
-        var Ps = {
+        var Ns = {
             start: "end",
             end: "start"
         };
 
-        function Cs(e) {
+        function Es(e) {
             return e.replace(/start|end/g, (function(e) {
-                return Ps[e]
+                return Ns[e]
             }))
         }
 
-        function Ts(e) {
-            var t = Aa(e);
+        function js(e) {
+            var t = Da(e);
             return {
                 scrollLeft: t.pageXOffset,
                 scrollTop: t.pageYOffset
             }
         }
 
-        function Ss(e) {
-            return qa(Qa(e)).left + Ts(e).scrollLeft
+        function ks(e) {
+            return Ka(Ga(e)).left + js(e).scrollLeft
         }
 
-        function Rs(e) {
-            var t = Xa(e),
+        function Ps(e) {
+            var t = qa(e),
                 n = t.overflow,
                 r = t.overflowX,
                 a = t.overflowY;
             return /auto|scroll|overlay|hidden/.test(n + a + r)
         }
 
-        function Ds(e) {
-            return ["html", "body", "#document"].indexOf(Ya(e)) >= 0 ? e.ownerDocument.body : Ma(e) && Rs(e) ? e : Ds(Za(e))
+        function Cs(e) {
+            return ["html", "body", "#document"].indexOf(Ua(e)) >= 0 ? e.ownerDocument.body : Ia(e) && Ps(e) ? e : Cs(Ya(e))
         }
 
-        function Ls(e, t) {
+        function Ts(e, t) {
             var n;
             void 0 === t && (t = []);
-            var r = Ds(e),
+            var r = Cs(e),
                 a = r === (null == (n = e.ownerDocument) ? void 0 : n.body),
-                s = Aa(r),
-                o = a ? [s].concat(s.visualViewport || [], Rs(r) ? r : []) : r,
+                s = Da(r),
+                o = a ? [s].concat(s.visualViewport || [], Ps(r) ? r : []) : r,
                 i = t.concat(o);
-            return a ? i : i.concat(Ls(Za(o)))
+            return a ? i : i.concat(Ts(Ya(o)))
         }
 
-        function $s(e) {
+        function Ss(e) {
             return Object.assign({}, e, {
                 left: e.x,
                 top: e.y,
                 right: e.x + e.width,
                 bottom: e.y + e.height
             })
         }
 
-        function Is(e, t, n) {
-            return t === ms ? $s(function(e, t) {
-                var n = Aa(e),
-                    r = Qa(e),
+        function Rs(e, t, n) {
+            return t === us ? Ss(function(e, t) {
+                var n = Da(e),
+                    r = Ga(e),
                     a = n.visualViewport,
                     s = r.clientWidth,
                     o = r.clientHeight,
                     i = 0,
                     l = 0;
                 if (a) {
                     s = a.width, o = a.height;
-                    var c = Wa();
+                    var c = za();
                     (c || !c && "fixed" === t) && (i = a.offsetLeft, l = a.offsetTop)
                 }
                 return {
                     width: s,
                     height: o,
-                    x: i + Ss(e),
+                    x: i + ks(e),
                     y: l
                 }
-            }(e, n)) : Fa(t) ? function(e, t) {
-                var n = qa(e, !1, "fixed" === t);
+            }(e, n)) : La(t) ? function(e, t) {
+                var n = Ka(e, !1, "fixed" === t);
                 return n.top = n.top + e.clientTop, n.left = n.left + e.clientLeft, n.bottom = n.top + e.clientHeight, n.right = n.left + e.clientWidth, n.width = e.clientWidth, n.height = e.clientHeight, n.x = n.left, n.y = n.top, n
-            }(t, n) : $s(function(e) {
-                var t, n = Qa(e),
-                    r = Ts(e),
+            }(t, n) : Ss(function(e) {
+                var t, n = Ga(e),
+                    r = js(e),
                     a = null == (t = e.ownerDocument) ? void 0 : t.body,
-                    s = za(n.scrollWidth, n.clientWidth, a ? a.scrollWidth : 0, a ? a.clientWidth : 0),
-                    o = za(n.scrollHeight, n.clientHeight, a ? a.scrollHeight : 0, a ? a.clientHeight : 0),
-                    i = -r.scrollLeft + Ss(e),
+                    s = Aa(n.scrollWidth, n.clientWidth, a ? a.scrollWidth : 0, a ? a.clientWidth : 0),
+                    o = Aa(n.scrollHeight, n.clientHeight, a ? a.scrollHeight : 0, a ? a.clientHeight : 0),
+                    i = -r.scrollLeft + ks(e),
                     l = -r.scrollTop;
-                return "rtl" === Xa(a || n).direction && (i += za(n.clientWidth, a ? a.clientWidth : 0) - s), {
+                return "rtl" === qa(a || n).direction && (i += Aa(n.clientWidth, a ? a.clientWidth : 0) - s), {
                     width: s,
                     height: o,
                     x: i,
                     y: l
                 }
-            }(Qa(e)))
+            }(Ga(e)))
         }
 
-        function As(e) {
+        function Ds(e) {
             var t, n = e.reference,
                 r = e.element,
                 a = e.placement,
-                s = a ? Ia(a) : null,
-                o = a ? _s(a) : null,
+                s = a ? Ra(a) : null,
+                o = a ? bs(a) : null,
                 i = n.x + n.width / 2 - r.width / 2,
                 l = n.y + n.height / 2 - r.height / 2;
             switch (s) {
-                case os:
+                case ns:
                     t = {
                         x: i,
                         y: n.y - r.height
                     };
                     break;
-                case is:
+                case rs:
                     t = {
                         x: i,
                         y: n.y + n.height
                     };
                     break;
-                case ls:
+                case as:
                     t = {
                         x: n.x + n.width,
                         y: l
                     };
                     break;
-                case cs:
+                case ss:
                     t = {
                         x: n.x - r.width,
                         y: l
                     };
                     break;
                 default:
                     t = {
                         x: n.x,
                         y: n.y
                     }
             }
-            var c = s ? ns(s) : null;
+            var c = s ? Qa(s) : null;
             if (null != c) {
                 var u = "y" === c ? "height" : "width";
                 switch (o) {
-                    case ps:
+                    case ls:
                         t[c] = t[c] - (n[u] / 2 - r[u] / 2);
                         break;
-                    case fs:
+                    case cs:
                         t[c] = t[c] + (n[u] / 2 - r[u] / 2)
                 }
             }
             return t
         }
 
-        function Fs(e, t) {
+        function Ls(e, t) {
             void 0 === t && (t = {});
             var n = t,
                 r = n.placement,
                 a = void 0 === r ? e.placement : r,
                 s = n.strategy,
                 o = void 0 === s ? e.strategy : s,
                 i = n.boundary,
                 l = void 0 === i ? "clippingParents" : i,
                 c = n.rootBoundary,
-                u = void 0 === c ? ms : c,
+                u = void 0 === c ? us : c,
                 d = n.elementContext,
-                p = void 0 === d ? gs : d,
+                p = void 0 === d ? ds : d,
                 f = n.altBoundary,
                 m = void 0 !== f && f,
                 g = n.padding,
                 b = void 0 === g ? 0 : g,
-                y = as("number" != typeof b ? b : ss(b, ds)),
-                h = p === gs ? "reference" : gs,
+                y = es("number" != typeof b ? b : ts(b, is)),
+                h = p === ds ? "reference" : ds,
                 v = e.rects.popper,
                 _ = e.elements[m ? h : p],
                 x = function(e, t, n, r) {
                     var a = "clippingParents" === t ? function(e) {
-                            var t = Ls(Za(e)),
-                                n = ["absolute", "fixed"].indexOf(Xa(e).position) >= 0 && Ma(e) ? ts(e) : e;
-                            return Fa(n) ? t.filter((function(e) {
-                                return Fa(e) && Ga(e, n) && "body" !== Ya(e)
+                            var t = Ts(Ya(e)),
+                                n = ["absolute", "fixed"].indexOf(qa(e).position) >= 0 && Ia(e) ? Ja(e) : e;
+                            return La(n) ? t.filter((function(e) {
+                                return La(e) && Wa(e, n) && "body" !== Ua(e)
                             })) : []
                         }(e) : [].concat(t),
                         s = [].concat(a, [n]),
                         o = s[0],
                         i = s.reduce((function(t, n) {
-                            var a = Is(e, n, r);
-                            return t.top = za(a.top, t.top), t.right = Ka(a.right, t.right), t.bottom = Ka(a.bottom, t.bottom), t.left = za(a.left, t.left), t
-                        }), Is(e, o, r));
+                            var a = Rs(e, n, r);
+                            return t.top = Aa(a.top, t.top), t.right = Ma(a.right, t.right), t.bottom = Ma(a.bottom, t.bottom), t.left = Aa(a.left, t.left), t
+                        }), Rs(e, o, r));
                     return i.width = i.right - i.left, i.height = i.bottom - i.top, i.x = i.left, i.y = i.top, i
-                }(Fa(_) ? _ : _.contextElement || Qa(e.elements.popper), l, u, o),
-                O = qa(e.elements.reference),
-                w = As({
+                }(La(_) ? _ : _.contextElement || Ga(e.elements.popper), l, u, o),
+                O = Ka(e.elements.reference),
+                w = Ds({
                     reference: O,
                     element: v,
                     strategy: "absolute",
                     placement: a
                 }),
-                N = $s(Object.assign({}, v, w)),
-                E = p === gs ? N : O,
+                N = Ss(Object.assign({}, v, w)),
+                E = p === ds ? N : O,
                 j = {
                     top: x.top - E.top + y.top,
                     bottom: E.bottom - x.bottom + y.bottom,
                     left: x.left - E.left + y.left,
                     right: E.right - x.right + y.right
                 },
                 k = e.modifiersData.offset;
-            if (p === gs && k) {
+            if (p === ds && k) {
                 var P = k[a];
                 Object.keys(j).forEach((function(e) {
-                    var t = [ls, is].indexOf(e) >= 0 ? 1 : -1,
-                        n = [os, is].indexOf(e) >= 0 ? "y" : "x";
+                    var t = [as, rs].indexOf(e) >= 0 ? 1 : -1,
+                        n = [ns, rs].indexOf(e) >= 0 ? "y" : "x";
                     j[e] += P[n] * t
                 }))
             }
             return j
         }
-        const Ms = {
+        const Is = {
             name: "flip",
             enabled: !0,
             phase: "main",
             fn: function(e) {
                 var t = e.state,
                     n = e.options,
                     r = e.name;
                 if (!t.modifiersData[r]._skip) {
-                    for (var a = n.mainAxis, s = void 0 === a || a, o = n.altAxis, i = void 0 === o || o, l = n.fallbackPlacements, c = n.padding, u = n.boundary, d = n.rootBoundary, p = n.altBoundary, f = n.flipVariations, m = void 0 === f || f, g = n.allowedAutoPlacements, b = t.options.placement, y = Ia(b), h = l || (y !== b && m ? function(e) {
-                            if (Ia(e) === us) return [];
-                            var t = ks(e);
-                            return [Cs(e), t, Cs(t)]
-                        }(b) : [ks(b)]), v = [b].concat(h).reduce((function(e, n) {
-                            return e.concat(Ia(n) === us ? function(e, t) {
+                    for (var a = n.mainAxis, s = void 0 === a || a, o = n.altAxis, i = void 0 === o || o, l = n.fallbackPlacements, c = n.padding, u = n.boundary, d = n.rootBoundary, p = n.altBoundary, f = n.flipVariations, m = void 0 === f || f, g = n.allowedAutoPlacements, b = t.options.placement, y = Ra(b), h = l || (y !== b && m ? function(e) {
+                            if (Ra(e) === os) return [];
+                            var t = ws(e);
+                            return [Es(e), t, Es(t)]
+                        }(b) : [ws(b)]), v = [b].concat(h).reduce((function(e, n) {
+                            return e.concat(Ra(n) === os ? function(e, t) {
                                 void 0 === t && (t = {});
                                 var n = t,
                                     r = n.placement,
                                     a = n.boundary,
                                     s = n.rootBoundary,
                                     o = n.padding,
                                     i = n.flipVariations,
                                     l = n.allowedAutoPlacements,
-                                    c = void 0 === l ? ys : l,
-                                    u = _s(r),
-                                    d = u ? i ? bs : bs.filter((function(e) {
-                                        return _s(e) === u
-                                    })) : ds,
+                                    c = void 0 === l ? fs : l,
+                                    u = bs(r),
+                                    d = u ? i ? ps : ps.filter((function(e) {
+                                        return bs(e) === u
+                                    })) : is,
                                     p = d.filter((function(e) {
                                         return c.indexOf(e) >= 0
                                     }));
                                 0 === p.length && (p = d);
                                 var f = p.reduce((function(t, n) {
-                                    return t[n] = Fs(e, {
+                                    return t[n] = Ls(e, {
                                         placement: n,
                                         boundary: a,
                                         rootBoundary: s,
                                         padding: o
-                                    })[Ia(n)], t
+                                    })[Ra(n)], t
                                 }), {});
                                 return Object.keys(f).sort((function(e, t) {
                                     return f[e] - f[t]
                                 }))
                             }(t, {
                                 placement: n,
                                 boundary: u,
                                 rootBoundary: d,
                                 padding: c,
                                 flipVariations: m,
                                 allowedAutoPlacements: g
                             }) : n)
                         }), []), _ = t.rects.reference, x = t.rects.popper, O = new Map, w = !0, N = v[0], E = 0; E < v.length; E++) {
                         var j = v[E],
-                            k = Ia(j),
-                            P = _s(j) === ps,
-                            C = [os, is].indexOf(k) >= 0,
+                            k = Ra(j),
+                            P = bs(j) === ls,
+                            C = [ns, rs].indexOf(k) >= 0,
                             T = C ? "width" : "height",
-                            S = Fs(t, {
+                            S = Ls(t, {
                                 placement: j,
                                 boundary: u,
                                 rootBoundary: d,
                                 altBoundary: p,
                                 padding: c
                             }),
-                            R = C ? P ? ls : cs : P ? is : os;
-                        _[T] > x[T] && (R = ks(R));
-                        var D = ks(R),
+                            R = C ? P ? as : ss : P ? rs : ns;
+                        _[T] > x[T] && (R = ws(R));
+                        var D = ws(R),
                             L = [];
                         if (s && L.push(S[k] <= 0), i && L.push(S[R] <= 0, S[D] <= 0), L.every((function(e) {
                                 return e
                             }))) {
                             N = j, w = !1;
                             break
                         }
                         O.set(j, L)
                     }
                     if (w)
-                        for (var $ = function(e) {
+                        for (var I = function(e) {
                                 var t = v.find((function(t) {
                                     var n = O.get(t);
                                     if (n) return n.slice(0, e).every((function(e) {
                                         return e
                                     }))
                                 }));
                                 if (t) return N = t, "break"
-                            }, I = m ? 3 : 1; I > 0 && "break" !== $(I); I--);
+                            }, $ = m ? 3 : 1; $ > 0 && "break" !== I($); $--);
                     t.placement !== N && (t.modifiersData[r]._skip = !0, t.placement = N, t.reset = !0)
                 }
             },
             requiresIfExists: ["offset"],
             data: {
                 _skip: !1
             }
         };
 
-        function Bs(e, t, n) {
+        function $s(e, t, n) {
             return void 0 === n && (n = {
                 x: 0,
                 y: 0
             }), {
                 top: e.top - t.height - n.y,
                 right: e.right - t.width + n.x,
                 bottom: e.bottom - t.height + n.y,
                 left: e.left - t.width - n.x
             }
         }
 
-        function zs(e) {
-            return [os, ls, is, cs].some((function(t) {
+        function As(e) {
+            return [ns, as, rs, ss].some((function(t) {
                 return e[t] >= 0
             }))
         }
-        const Ks = {
+        const Ms = {
                 name: "offset",
                 enabled: !0,
                 phase: "main",
                 requires: ["popperOffsets"],
                 fn: function(e) {
                     var t = e.state,
                         n = e.options,
                         r = e.name,
                         a = n.offset,
                         s = void 0 === a ? [0, 0] : a,
-                        o = ys.reduce((function(e, n) {
+                        o = fs.reduce((function(e, n) {
                             return e[n] = function(e, t, n) {
-                                var r = Ia(e),
-                                    a = [cs, os].indexOf(r) >= 0 ? -1 : 1,
+                                var r = Ra(e),
+                                    a = [ss, ns].indexOf(r) >= 0 ? -1 : 1,
                                     s = "function" == typeof n ? n(Object.assign({}, t, {
                                         placement: e
                                     })) : n,
                                     o = s[0],
                                     i = s[1];
-                                return o = o || 0, i = (i || 0) * a, [cs, ls].indexOf(r) >= 0 ? {
+                                return o = o || 0, i = (i || 0) * a, [ss, as].indexOf(r) >= 0 ? {
                                     x: i,
                                     y: o
                                 } : {
                                     x: o,
                                     y: i
                                 }
                             }(n, t.rects, s), e
                         }), {}),
                         i = o[t.placement],
                         l = i.x,
                         c = i.y;
                     null != t.modifiersData.popperOffsets && (t.modifiersData.popperOffsets.x += l, t.modifiersData.popperOffsets.y += c), t.modifiersData[r] = o
                 }
             },
-            Hs = {
+            Fs = {
                 name: "preventOverflow",
                 enabled: !0,
                 phase: "main",
                 fn: function(e) {
                     var t = e.state,
                         n = e.options,
                         r = e.name,
@@ -5101,24 +5045,24 @@
                         c = n.rootBoundary,
                         u = n.altBoundary,
                         d = n.padding,
                         p = n.tether,
                         f = void 0 === p || p,
                         m = n.tetherOffset,
                         g = void 0 === m ? 0 : m,
-                        b = Fs(t, {
+                        b = Ls(t, {
                             boundary: l,
                             rootBoundary: c,
                             padding: d,
                             altBoundary: u
                         }),
-                        y = Ia(t.placement),
-                        h = _s(t.placement),
+                        y = Ra(t.placement),
+                        h = bs(t.placement),
                         v = !h,
-                        _ = ns(y),
+                        _ = Qa(y),
                         x = "x" === _ ? "y" : "x",
                         O = t.modifiersData.popperOffsets,
                         w = t.rects.reference,
                         N = t.rects.popper,
                         E = "function" == typeof g ? g(Object.assign({}, t.rects, {
                             placement: t.placement
                         })) : g,
@@ -5132,100 +5076,100 @@
                         k = t.modifiersData.offset ? t.modifiersData.offset[t.placement] : null,
                         P = {
                             x: 0,
                             y: 0
                         };
                     if (O) {
                         if (s) {
-                            var C, T = "y" === _ ? os : cs,
-                                S = "y" === _ ? is : ls,
+                            var C, T = "y" === _ ? ns : ss,
+                                S = "y" === _ ? rs : as,
                                 R = "y" === _ ? "height" : "width",
                                 D = O[_],
                                 L = D + b[T],
-                                $ = D - b[S],
-                                I = f ? -N[R] / 2 : 0,
-                                A = h === ps ? w[R] : N[R],
-                                F = h === ps ? -N[R] : -w[R],
-                                M = t.elements.arrow,
-                                B = f && M ? Va(M) : {
+                                I = D - b[S],
+                                $ = f ? -N[R] / 2 : 0,
+                                A = h === ls ? w[R] : N[R],
+                                M = h === ls ? -N[R] : -w[R],
+                                F = t.elements.arrow,
+                                B = f && F ? Ha(F) : {
                                     width: 0,
                                     height: 0
                                 },
                                 z = t.modifiersData["arrow#persistent"] ? t.modifiersData["arrow#persistent"].padding : {
                                     top: 0,
                                     right: 0,
                                     bottom: 0,
                                     left: 0
                                 },
                                 K = z[T],
                                 H = z[S],
-                                U = rs(0, w[R], B[R]),
-                                W = v ? w[R] / 2 - I - U - K - j.mainAxis : A - U - K - j.mainAxis,
-                                q = v ? -w[R] / 2 + I + U + H + j.mainAxis : F + U + H + j.mainAxis,
-                                V = t.elements.arrow && ts(t.elements.arrow),
+                                W = Za(0, w[R], B[R]),
+                                U = v ? w[R] / 2 - $ - W - K - j.mainAxis : A - W - K - j.mainAxis,
+                                q = v ? -w[R] / 2 + $ + W + H + j.mainAxis : M + W + H + j.mainAxis,
+                                V = t.elements.arrow && Ja(t.elements.arrow),
                                 G = V ? "y" === _ ? V.clientTop || 0 : V.clientLeft || 0 : 0,
                                 Y = null != (C = null == k ? void 0 : k[_]) ? C : 0,
                                 X = D + q - Y,
-                                J = rs(f ? Ka(L, D + W - Y - G) : L, D, f ? za($, X) : $);
+                                J = Za(f ? Ma(L, D + U - Y - G) : L, D, f ? Aa(I, X) : I);
                             O[_] = J, P[_] = J - D
                         }
                         if (i) {
-                            var Q, Z = "x" === _ ? os : cs,
-                                ee = "x" === _ ? is : ls,
+                            var Q, Z = "x" === _ ? ns : ss,
+                                ee = "x" === _ ? rs : as,
                                 te = O[x],
                                 ne = "y" === x ? "height" : "width",
                                 re = te + b[Z],
                                 ae = te - b[ee],
-                                se = -1 !== [os, cs].indexOf(y),
+                                se = -1 !== [ns, ss].indexOf(y),
                                 oe = null != (Q = null == k ? void 0 : k[x]) ? Q : 0,
                                 ie = se ? re : te - w[ne] - N[ne] - oe + j.altAxis,
                                 le = se ? te + w[ne] + N[ne] - oe - j.altAxis : ae,
                                 ce = f && se ? function(e, t, n) {
-                                    var r = rs(e, t, n);
+                                    var r = Za(e, t, n);
                                     return r > n ? n : r
-                                }(ie, te, le) : rs(f ? ie : re, te, f ? le : ae);
+                                }(ie, te, le) : Za(f ? ie : re, te, f ? le : ae);
                             O[x] = ce, P[x] = ce - te
                         }
                         t.modifiersData[r] = P
                     }
                 },
                 requiresIfExists: ["offset"]
             };
 
-        function Us(e, t, n) {
+        function Bs(e, t, n) {
             void 0 === n && (n = !1);
-            var r, a, s = Ma(t),
-                o = Ma(t) && function(e) {
+            var r, a, s = Ia(t),
+                o = Ia(t) && function(e) {
                     var t = e.getBoundingClientRect(),
-                        n = Ha(t.width) / e.offsetWidth || 1,
-                        r = Ha(t.height) / e.offsetHeight || 1;
+                        n = Fa(t.width) / e.offsetWidth || 1,
+                        r = Fa(t.height) / e.offsetHeight || 1;
                     return 1 !== n || 1 !== r
                 }(t),
-                i = Qa(t),
-                l = qa(e, o, n),
+                i = Ga(t),
+                l = Ka(e, o, n),
                 c = {
                     scrollLeft: 0,
                     scrollTop: 0
                 },
                 u = {
                     x: 0,
                     y: 0
                 };
-            return (s || !s && !n) && (("body" !== Ya(t) || Rs(i)) && (c = (r = t) !== Aa(r) && Ma(r) ? {
+            return (s || !s && !n) && (("body" !== Ua(t) || Ps(i)) && (c = (r = t) !== Da(r) && Ia(r) ? {
                 scrollLeft: (a = r).scrollLeft,
                 scrollTop: a.scrollTop
-            } : Ts(r)), Ma(t) ? ((u = qa(t, !0)).x += t.clientLeft, u.y += t.clientTop) : i && (u.x = Ss(i))), {
+            } : js(r)), Ia(t) ? ((u = Ka(t, !0)).x += t.clientLeft, u.y += t.clientTop) : i && (u.x = ks(i))), {
                 x: l.left + c.scrollLeft - u.x,
                 y: l.top + c.scrollTop - u.y,
                 width: l.width,
                 height: l.height
             }
         }
 
-        function Ws(e) {
+        function zs(e) {
             var t = new Map,
                 n = new Set,
                 r = [];
 
             function a(e) {
                 n.add(e.name), [].concat(e.requires || [], e.requiresIfExists || []).forEach((function(e) {
                     if (!n.has(e)) {
@@ -5236,39 +5180,39 @@
             }
             return e.forEach((function(e) {
                 t.set(e.name, e)
             })), e.forEach((function(e) {
                 n.has(e.name) || a(e)
             })), r
         }
-        var qs = {
+        var Ks = {
             placement: "bottom",
             modifiers: [],
             strategy: "absolute"
         };
 
-        function Vs() {
+        function Hs() {
             for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
             return !t.some((function(e) {
                 return !(e && "function" == typeof e.getBoundingClientRect)
             }))
         }
-        const Gs = function(e) {
+        const Ws = function(e) {
                 void 0 === e && (e = {});
                 var t = e,
                     n = t.defaultModifiers,
                     r = void 0 === n ? [] : n,
                     a = t.defaultOptions,
-                    s = void 0 === a ? qs : a;
+                    s = void 0 === a ? Ks : a;
                 return function(e, t, n) {
                     void 0 === n && (n = s);
                     var a, o, i = {
                             placement: "bottom",
                             orderedModifiers: [],
-                            options: Object.assign({}, qs, s),
+                            options: Object.assign({}, Ks, s),
                             modifiersData: {},
                             elements: {
                                 reference: e,
                                 popper: t
                             },
                             attributes: {},
                             styles: {}
@@ -5276,20 +5220,20 @@
                         l = [],
                         c = !1,
                         u = {
                             state: i,
                             setOptions: function(n) {
                                 var a = "function" == typeof n ? n(i.options) : n;
                                 d(), i.options = Object.assign({}, s, i.options, a), i.scrollParents = {
-                                    reference: Fa(e) ? Ls(e) : e.contextElement ? Ls(e.contextElement) : [],
-                                    popper: Ls(t)
+                                    reference: La(e) ? Ts(e) : e.contextElement ? Ts(e.contextElement) : [],
+                                    popper: Ts(t)
                                 };
                                 var o, c, p = function(e) {
-                                    var t = Ws(e);
-                                    return hs.reduce((function(e, n) {
+                                    var t = zs(e);
+                                    return ms.reduce((function(e, n) {
                                         return e.concat(t.filter((function(e) {
                                             return e.phase === n
                                         })))
                                     }), [])
                                 }((o = [].concat(r, i.options.modifiers), c = o.reduce((function(e, t) {
                                     var n = e[t.name];
                                     return e[t.name] = n ? Object.assign({}, n, t, {
@@ -5318,18 +5262,18 @@
                                 })), u.update()
                             },
                             forceUpdate: function() {
                                 if (!c) {
                                     var e = i.elements,
                                         t = e.reference,
                                         n = e.popper;
-                                    if (Vs(t, n)) {
+                                    if (Hs(t, n)) {
                                         i.rects = {
-                                            reference: Us(t, ts(n), "fixed" === i.options.strategy),
-                                            popper: Va(n)
+                                            reference: Bs(t, Ja(n), "fixed" === i.options.strategy),
+                                            popper: Ha(n)
                                         }, i.reset = !1, i.placement = i.options.placement, i.orderedModifiers.forEach((function(e) {
                                             return i.modifiersData[e.name] = Object.assign({}, e.data)
                                         }));
                                         for (var r = 0; r < i.orderedModifiers.length; r++)
                                             if (!0 !== i.reset) {
                                                 var a = i.orderedModifiers[r],
                                                     s = a.fn,
@@ -5357,15 +5301,15 @@
                                     }))
                                 }))), o
                             }),
                             destroy: function() {
                                 d(), c = !0
                             }
                         };
-                    if (!Vs(e, t)) return u;
+                    if (!Hs(e, t)) return u;
 
                     function d() {
                         l.forEach((function(e) {
                             return e()
                         })), l = []
                     }
                     return u.setOptions(n).then((function(e) {
@@ -5380,24 +5324,24 @@
                     requiresIfExists: ["preventOverflow"],
                     fn: function(e) {
                         var t = e.state,
                             n = e.name,
                             r = t.rects.reference,
                             a = t.rects.popper,
                             s = t.modifiersData.preventOverflow,
-                            o = Fs(t, {
+                            o = Ls(t, {
                                 elementContext: "reference"
                             }),
-                            i = Fs(t, {
+                            i = Ls(t, {
                                 altBoundary: !0
                             }),
-                            l = Bs(o, r),
-                            c = Bs(i, a, s),
-                            u = zs(l),
-                            d = zs(c);
+                            l = $s(o, r),
+                            c = $s(i, a, s),
+                            u = As(l),
+                            d = As(c);
                         t.modifiersData[n] = {
                             referenceClippingOffsets: l,
                             popperEscapeOffsets: c,
                             isReferenceHidden: u,
                             hasPopperEscaped: d
                         }, t.attributes.popper = Object.assign({}, t.attributes.popper, {
                             "data-popper-reference-hidden": u,
@@ -5407,32 +5351,32 @@
                 }, {
                     name: "popperOffsets",
                     enabled: !0,
                     phase: "read",
                     fn: function(e) {
                         var t = e.state,
                             n = e.name;
-                        t.modifiersData[n] = As({
+                        t.modifiersData[n] = Ds({
                             reference: t.rects.reference,
                             element: t.rects.popper,
                             strategy: "absolute",
                             placement: t.placement
                         })
                     },
                     data: {}
-                }, ws, Es, Ks, Ms, Hs, vs]
+                }, vs, xs, Ms, Is, Fs, gs]
             }),
-            Ys = ["enabled", "placement", "strategy", "modifiers"],
-            Xs = {
+            Us = ["enabled", "placement", "strategy", "modifiers"],
+            qs = {
                 name: "applyStyles",
                 enabled: !1,
                 phase: "afterWrite",
                 fn: () => {}
             },
-            Js = {
+            Vs = {
                 name: "ariaDescribedBy",
                 enabled: !0,
                 phase: "afterWrite",
                 effect: ({
                     state: e
                 }) => () => {
                     const {
@@ -5455,40 +5399,40 @@
                     if (n.id && "tooltip" === a && "setAttribute" in r) {
                         const e = r.getAttribute("aria-describedby");
                         if (e && -1 !== e.split(",").indexOf(n.id)) return;
                         r.setAttribute("aria-describedby", e ? `${e},${n.id}` : n.id)
                     }
                 }
             },
-            Qs = [],
-            Zs = function(e, t, n = {}) {
+            Gs = [],
+            Ys = function(e, t, n = {}) {
                 let {
                     enabled: r = !0,
                     placement: a = "bottom",
                     strategy: s = "absolute",
-                    modifiers: o = Qs
+                    modifiers: o = Gs
                 } = n, l = function(e, t) {
                     if (null == e) return {};
                     var n, r, a = {},
                         s = Object.keys(e);
                     for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                     return a
-                }(n, Ys);
+                }(n, Us);
                 const c = (0, i.useRef)(o),
                     u = (0, i.useRef)(),
                     d = (0, i.useCallback)((() => {
                         var e;
                         null == (e = u.current) || e.update()
                     }), []),
                     p = (0, i.useCallback)((() => {
                         var e;
                         null == (e = u.current) || e.forceUpdate()
                     }), []),
                     [f, m] = function(e) {
-                        const t = tt();
+                        const t = Ze();
                         return [e[0], (0, i.useCallback)((n => {
                             if (t()) return e[1](n)
                         }), [t, e[1]])]
                     }((0, i.useState)({
                         placement: a,
                         update: d,
                         forceUpdate: p,
@@ -5516,93 +5460,93 @@
                                 attributes: n,
                                 update: d,
                                 forceUpdate: p,
                                 placement: e.placement
                             })
                         }
                     })), [d, p, m]),
-                    b = (0, i.useMemo)((() => ($a(c.current, o) || (c.current = o), c.current)), [o]);
+                    b = (0, i.useMemo)((() => (Sa(c.current, o) || (c.current = o), c.current)), [o]);
                 return (0, i.useEffect)((() => {
                     u.current && r && u.current.setOptions({
                         placement: a,
                         strategy: s,
-                        modifiers: [...b, g, Xs]
+                        modifiers: [...b, g, qs]
                     })
                 }), [s, a, g, r, b]), (0, i.useEffect)((() => {
-                    if (r && null != e && null != t) return u.current = Gs(e, t, Object.assign({}, l, {
+                    if (r && null != e && null != t) return u.current = Ws(e, t, Object.assign({}, l, {
                         placement: a,
                         strategy: s,
-                        modifiers: [...b, Js, g]
+                        modifiers: [...b, Vs, g]
                     })), () => {
                         null != u.current && (u.current.destroy(), u.current = void 0, m((e => Object.assign({}, e, {
                             attributes: {},
                             styles: {
                                 popper: {}
                             }
                         }))))
                     }
                 }), [r, e, t]), f
             };
 
-        function eo(e, t) {
+        function Xs(e, t) {
             return e.contains ? e.contains(t) : e.compareDocumentPosition ? e === t || !!(16 & e.compareDocumentPosition(t)) : void 0
         }
-        var to = n(2),
-            no = n.n(to);
-        const ro = () => {},
-            ao = e => e && ("current" in e ? e.current : e),
-            so = {
+        var Js = n(2),
+            Qs = n.n(Js);
+        const Zs = () => {},
+            eo = e => e && ("current" in e ? e.current : e),
+            to = {
                 click: "mousedown",
                 mouseup: "mousedown",
                 pointerup: "pointerdown"
             },
-            oo = function(e, t = ro, {
+            no = function(e, t = Zs, {
                 disabled: n,
                 clickTrigger: r = "click"
             } = {}) {
                 const a = (0, i.useRef)(!1),
                     s = (0, i.useRef)(!1),
                     o = (0, i.useCallback)((t => {
-                        const n = ao(e);
+                        const n = eo(e);
                         var r;
-                        no()(!!n, "ClickOutside captured a close event but does not have a ref to compare it to. useClickOutside(), should be passed a ref that resolves to a DOM node"), a.current = !n || !!((r = t).metaKey || r.altKey || r.ctrlKey || r.shiftKey) || ! function(e) {
+                        Qs()(!!n, "ClickOutside captured a close event but does not have a ref to compare it to. useClickOutside(), should be passed a ref that resolves to a DOM node"), a.current = !n || !!((r = t).metaKey || r.altKey || r.ctrlKey || r.shiftKey) || ! function(e) {
                             return 0 === e.button
-                        }(t) || !!eo(n, t.target) || s.current, s.current = !1
+                        }(t) || !!Xs(n, t.target) || s.current, s.current = !1
                     }), [e]),
-                    l = Ye((t => {
-                        const n = ao(e);
-                        n && eo(n, t.target) && (s.current = !0)
+                    l = Ve((t => {
+                        const n = eo(e);
+                        n && Xs(n, t.target) && (s.current = !0)
                     })),
-                    c = Ye((e => {
+                    c = Ve((e => {
                         a.current || t(e)
                     }));
                 (0, i.useEffect)((() => {
                     var t, a;
                     if (n || null == e) return;
-                    const s = C(ao(e)),
+                    const s = C(eo(e)),
                         i = s.defaultView || window;
                     let u = null != (t = i.event) ? t : null == (a = i.parent) ? void 0 : a.event,
                         d = null;
-                    so[r] && (d = Z(s, so[r], l, !0));
+                    to[r] && (d = Z(s, to[r], l, !0));
                     const p = Z(s, r, o, !0),
                         f = Z(s, r, (e => {
                             e !== u ? c(e) : u = void 0
                         }));
                     let m = [];
-                    return "ontouchstart" in s.documentElement && (m = [].slice.call(s.body.children).map((e => Z(e, "mousemove", ro)))), () => {
+                    return "ontouchstart" in s.documentElement && (m = [].slice.call(s.body.children).map((e => Z(e, "mousemove", Zs)))), () => {
                         null == d || d(), p(), f(), m.forEach((e => e()))
                     }
                 }), [e, n, r, o, l, c])
             };
 
-        function io(e = {}) {
+        function ro(e = {}) {
             return Array.isArray(e) ? e : Object.keys(e).map((t => (e[t].name = t, e[t])))
         }
 
-        function lo({
+        function ao({
             enabled: e,
             enableEvents: t,
             placement: n,
             flip: r,
             offset: a,
             fixed: s,
             containerPadding: o,
@@ -5616,15 +5560,15 @@
                     t[e.name] = e
                 })), t) : e || t
             }(l.modifiers);
             return Object.assign({}, l, {
                 placement: n,
                 enabled: e,
                 strategy: s ? "fixed" : l.strategy,
-                modifiers: io(Object.assign({}, m, {
+                modifiers: ro(Object.assign({}, m, {
                     eventListeners: {
                         enabled: t,
                         options: null == (c = m.eventListeners) ? void 0 : c.options
                     },
                     preventOverflow: Object.assign({}, m.preventOverflow, {
                         options: o ? Object.assign({
                             padding: o
@@ -5643,20 +5587,20 @@
                     }),
                     flip: Object.assign({
                         enabled: !!r
                     }, m.flip)
                 }))
             })
         }
-        const co = ["children"],
-            uo = () => {};
+        const so = ["children"],
+            oo = () => {};
 
-        function po(e = {}) {
-            const t = (0, i.useContext)(Ra),
-                [n, r] = et(),
+        function io(e = {}) {
+            const t = (0, i.useContext)(Pa),
+                [n, r] = Qe(),
                 a = (0, i.useRef)(!1),
                 {
                     flip: s,
                     offset: o,
                     rootCloseEvent: l,
                     fixed: c = !1,
                     placement: u,
@@ -5667,25 +5611,25 @@
                 m = null == (null == t ? void 0 : t.show) ? !!e.show : t.show;
             m && !a.current && (a.current = !0);
             const {
                 placement: g,
                 setMenu: b,
                 menuElement: y,
                 toggleElement: h
-            } = t || {}, v = Zs(h, y, lo({
+            } = t || {}, v = Ys(h, y, ao({
                 placement: u || g || "bottom-start",
                 enabled: f,
                 enableEvents: null == p ? m : p,
                 offset: o,
                 flip: s,
                 fixed: c,
                 arrowElement: n,
                 popperConfig: d
             })), _ = Object.assign({
-                ref: b || uo,
+                ref: b || oo,
                 "aria-labelledby": null == h ? void 0 : h.id
             }, v.attributes.popper, {
                 style: v.styles.popper
             }), x = {
                 show: m,
                 placement: g,
                 hasShown: a.current,
@@ -5693,268 +5637,268 @@
                 popper: f ? v : null,
                 arrowProps: f ? Object.assign({
                     ref: r
                 }, v.attributes.arrow, {
                     style: v.styles.arrow
                 }) : {}
             };
-            return oo(y, (e => {
+            return no(y, (e => {
                 null == t || t.toggle(!1, e)
             }), {
                 clickTrigger: l,
                 disabled: !m
             }), [_, x]
         }
 
-        function fo(e) {
+        function lo(e) {
             let {
                 children: t
             } = e, n = function(e, t) {
                 if (null == e) return {};
                 var n, r, a = {},
                     s = Object.keys(e);
                 for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                 return a
-            }(e, co);
-            const [r, a] = po(n);
+            }(e, so);
+            const [r, a] = io(n);
             return (0, _.jsx)(_.Fragment, {
                 children: t(r, a)
             })
         }
-        fo.displayName = "DropdownMenu", fo.defaultProps = {
+        lo.displayName = "DropdownMenu", lo.defaultProps = {
             usePopper: !0
         };
-        const mo = fo,
-            go = {
+        const co = lo,
+            uo = {
                 prefix: String(Math.round(1e10 * Math.random())),
                 current: 0
             },
-            bo = i.createContext(go),
-            yo = i.createContext(!1);
-        let ho = Boolean("undefined" != typeof window && window.document && window.document.createElement),
-            vo = new WeakMap;
-        const _o = "function" == typeof i.useId ? function(e) {
+            po = i.createContext(uo),
+            fo = i.createContext(!1);
+        let mo = Boolean("undefined" != typeof window && window.document && window.document.createElement),
+            go = new WeakMap;
+        const bo = "function" == typeof i.useId ? function(e) {
             let t = i.useId(),
-                [n] = (0, i.useState)("function" == typeof i.useSyncExternalStore ? i.useSyncExternalStore(wo, xo, Oo) : (0, i.useContext)(yo));
-            return e || `${n?"react-aria":`react-aria${go.prefix}`}-${t}`
+                [n] = (0, i.useState)("function" == typeof i.useSyncExternalStore ? i.useSyncExternalStore(vo, yo, ho) : (0, i.useContext)(fo));
+            return e || `${n?"react-aria":`react-aria${uo.prefix}`}-${t}`
         } : function(e) {
-            let t = (0, i.useContext)(bo);
-            t !== go || ho || console.warn("When server rendering, you must wrap your application in an <SSRProvider> to ensure consistent ids are generated between the client and server.");
+            let t = (0, i.useContext)(po);
+            t !== uo || mo || console.warn("When server rendering, you must wrap your application in an <SSRProvider> to ensure consistent ids are generated between the client and server.");
             let n = function(e = !1) {
-                    let t = (0, i.useContext)(bo),
+                    let t = (0, i.useContext)(po),
                         n = (0, i.useRef)(null);
                     if (null === n.current && !e) {
                         var r, a;
                         let e = null === (a = i.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED) || void 0 === a || null === (r = a.ReactCurrentOwner) || void 0 === r ? void 0 : r.current;
                         if (e) {
-                            let n = vo.get(e);
-                            null == n ? vo.set(e, {
+                            let n = go.get(e);
+                            null == n ? go.set(e, {
                                 id: t.current,
                                 state: e.memoizedState
-                            }) : e.memoizedState !== n.state && (t.current = n.id, vo.delete(e))
+                            }) : e.memoizedState !== n.state && (t.current = n.id, go.delete(e))
                         }
                         n.current = ++t.current
                     }
                     return n.current
                 }(!!e),
                 r = `react-aria${t.prefix}`;
             return e || `${r}-${n}`
         };
 
-        function xo() {
+        function yo() {
             return !1
         }
 
-        function Oo() {
+        function ho() {
             return !0
         }
 
-        function wo(e) {
+        function vo(e) {
             return () => {}
         }
-        const No = e => {
+        const _o = e => {
                 var t;
                 return "menu" === (null == (t = e.getAttribute("role")) ? void 0 : t.toLowerCase())
             },
-            Eo = () => {};
+            xo = () => {};
 
-        function jo() {
-            const e = _o(),
+        function Oo() {
+            const e = bo(),
                 {
                     show: t = !1,
-                    toggle: n = Eo,
+                    toggle: n = xo,
                     setToggle: r,
                     menuElement: a
-                } = (0, i.useContext)(Ra) || {},
+                } = (0, i.useContext)(Pa) || {},
                 s = (0, i.useCallback)((e => {
                     n(!t, e)
                 }), [t, n]),
                 o = {
                     id: e,
-                    ref: r || Eo,
+                    ref: r || xo,
                     onClick: s,
                     "aria-expanded": !!t
                 };
-            return a && No(a) && (o["aria-haspopup"] = !0), [o, {
+            return a && _o(a) && (o["aria-haspopup"] = !0), [o, {
                 show: t,
                 toggle: n
             }]
         }
 
-        function ko({
+        function wo({
             children: e
         }) {
-            const [t, n] = jo();
+            const [t, n] = Oo();
             return (0, _.jsx)(_.Fragment, {
                 children: e(t, n)
             })
         }
-        ko.displayName = "DropdownToggle";
+        wo.displayName = "DropdownToggle";
+        const No = wo,
+            Eo = (e, t = null) => null != e ? String(e) : t || null,
+            jo = i.createContext(null),
+            ko = i.createContext(null);
+        ko.displayName = "NavContext";
         const Po = ko,
-            Co = (e, t = null) => null != e ? String(e) : t || null,
-            To = i.createContext(null),
-            So = i.createContext(null);
-        So.displayName = "NavContext";
-        const Ro = So,
-            Do = "data-rr-ui-";
+            Co = "data-rr-ui-";
 
-        function Lo(e) {
-            return `${Do}${e}`
+        function To(e) {
+            return `${Co}${e}`
         }
-        const $o = ["eventKey", "disabled", "onClick", "active", "as"];
+        const So = ["eventKey", "disabled", "onClick", "active", "as"];
 
-        function Io({
+        function Ro({
             key: e,
             href: t,
             active: n,
             disabled: r,
             onClick: a
         }) {
-            const s = (0, i.useContext)(To),
-                o = (0, i.useContext)(Ro),
+            const s = (0, i.useContext)(jo),
+                o = (0, i.useContext)(Po),
                 {
                     activeKey: l
                 } = o || {},
-                c = Co(e, t),
-                u = null == n && null != e ? Co(l) === c : n;
+                c = Eo(e, t),
+                u = null == n && null != e ? Eo(l) === c : n;
             return [{
-                onClick: Ye((e => {
+                onClick: Ve((e => {
                     r || (null == a || a(e), s && !e.isPropagationStopped() && s(c, e))
                 })),
                 "aria-disabled": r || void 0,
                 "aria-selected": u,
-                [Lo("dropdown-item")]: ""
+                [To("dropdown-item")]: ""
             }, {
                 isActive: u
             }]
         }
-        const Ao = i.forwardRef(((e, t) => {
+        const Do = i.forwardRef(((e, t) => {
             let {
                 eventKey: n,
                 disabled: r,
                 onClick: a,
                 active: s,
-                as: o = lt
+                as: o = ot
             } = e, i = function(e, t) {
                 if (null == e) return {};
                 var n, r, a = {},
                     s = Object.keys(e);
                 for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                 return a
-            }(e, $o);
-            const [l] = Io({
+            }(e, So);
+            const [l] = Ro({
                 key: n,
                 href: i.href,
                 disabled: r,
                 onClick: a,
                 active: s
             });
             return (0, _.jsx)(o, Object.assign({}, i, {
                 ref: t
             }, l))
         }));
-        Ao.displayName = "DropdownItem";
-        const Fo = Ao,
-            Mo = (0, i.createContext)(V ? window : void 0);
+        Do.displayName = "DropdownItem";
+        const Lo = Do,
+            Io = (0, i.createContext)(V ? window : void 0);
 
-        function Bo() {
-            return (0, i.useContext)(Mo)
+        function $o() {
+            return (0, i.useContext)(Io)
         }
 
-        function zo() {
-            const e = Sa(),
+        function Ao() {
+            const e = ka(),
                 t = (0, i.useRef)(null),
                 n = (0, i.useCallback)((n => {
                     t.current = n, e()
                 }), [e]);
             return [t, n]
         }
 
-        function Ko({
+        function Mo({
             defaultShow: e,
             show: t,
             onSelect: n,
             onToggle: r,
-            itemSelector: a = `* [${Lo("dropdown-item")}]`,
+            itemSelector: a = `* [${To("dropdown-item")}]`,
             focusFirstItemOnShow: s,
             placement: o = "bottom-start",
             children: l
         }) {
-            const c = Bo(),
-                [u, d] = Ta(t, e, r),
-                [p, f] = zo(),
+            const c = $o(),
+                [u, d] = ja(t, e, r),
+                [p, f] = Ao(),
                 m = p.current,
-                [g, b] = zo(),
+                [g, b] = Ao(),
                 y = g.current,
-                h = nt(u),
+                h = et(u),
                 v = (0, i.useRef)(null),
                 x = (0, i.useRef)(!1),
-                O = (0, i.useContext)(To),
+                O = (0, i.useContext)(jo),
                 w = (0, i.useCallback)(((e, t, n = (null == t ? void 0 : t.type)) => {
                     d(e, {
                         originalEvent: t,
                         source: n
                     })
                 }), [d]),
-                N = Ye(((e, t) => {
+                N = Ve(((e, t) => {
                     null == n || n(e, t), w(!1, t, "select"), t.isPropagationStopped() || null == O || O(e, t)
                 })),
                 E = (0, i.useMemo)((() => ({
                     toggle: w,
                     placement: o,
                     show: u,
                     menuElement: m,
                     toggleElement: y,
                     setMenu: f,
                     setToggle: b
                 })), [w, o, u, m, y, f, b]);
             m && h && !u && (x.current = m.contains(m.ownerDocument.activeElement));
-            const j = Ye((() => {
+            const j = Ve((() => {
                     y && y.focus && y.focus()
                 })),
-                k = Ye((() => {
+                k = Ve((() => {
                     const e = v.current;
                     let t = s;
-                    if (null == t && (t = !(!p.current || !No(p.current)) && "keyboard"), !1 === t || "keyboard" === t && !/^key.+$/.test(e)) return;
-                    const n = Ca(p.current, a)[0];
+                    if (null == t && (t = !(!p.current || !_o(p.current)) && "keyboard"), !1 === t || "keyboard" === t && !/^key.+$/.test(e)) return;
+                    const n = Ea(p.current, a)[0];
                     n && n.focus && n.focus()
                 }));
             (0, i.useEffect)((() => {
                 u ? k() : x.current && (x.current = !1, j())
             }), [u, x, j, k]), (0, i.useEffect)((() => {
                 v.current = null
             }));
             const P = (e, t) => {
                 if (!p.current) return null;
-                const n = Ca(p.current, a);
+                const n = Ea(p.current, a);
                 let r = n.indexOf(e) + t;
                 return r = Math.max(0, Math.min(r, n.length)), n[r]
             };
             return function(e, t, n, r = !1) {
-                const a = Ye(n);
+                const a = Ve(n);
                 (0, i.useEffect)((() => {
                     const n = "function" == typeof e ? e() : e;
                     return n.addEventListener(t, a, r), () => n.removeEventListener(t, a, r)
                 }), [e])
             }((0, i.useCallback)((() => c.document), [c]), "keydown", (e => {
                 var t, n;
                 const {
@@ -5986,158 +5930,158 @@
                         }), {
                             once: !0
                         });
                         break;
                     case "Escape":
                         "Escape" === r && (e.preventDefault(), e.stopPropagation()), d(!1, i)
                 }
-            })), (0, _.jsx)(To.Provider, {
+            })), (0, _.jsx)(jo.Provider, {
                 value: N,
-                children: (0, _.jsx)(Ra.Provider, {
+                children: (0, _.jsx)(Pa.Provider, {
                     value: E,
                     children: l
                 })
             })
         }
-        Mo.Provider, Ko.displayName = "Dropdown", Ko.Menu = mo, Ko.Toggle = Po, Ko.Item = Fo;
-        const Ho = Ko,
-            Uo = i.createContext({});
-        Uo.displayName = "DropdownContext";
-        const Wo = Uo,
-            qo = i.forwardRef((({
+        Io.Provider, Mo.displayName = "Dropdown", Mo.Menu = co, Mo.Toggle = No, Mo.Item = Lo;
+        const Fo = Mo,
+            Bo = i.createContext({});
+        Bo.displayName = "DropdownContext";
+        const zo = Bo,
+            Ko = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "hr",
                 role: r = "separator",
                 ...a
             }, s) => (t = E(t, "dropdown-divider"), (0, _.jsx)(n, {
                 ref: s,
                 className: b()(e, t),
                 role: r,
                 ...a
             }))));
-        qo.displayName = "DropdownDivider";
-        const Vo = qo,
-            Go = i.forwardRef((({
+        Ko.displayName = "DropdownDivider";
+        const Ho = Ko,
+            Wo = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 role: r = "heading",
                 ...a
             }, s) => (t = E(t, "dropdown-header"), (0, _.jsx)(n, {
                 ref: s,
                 className: b()(e, t),
                 role: r,
                 ...a
             }))));
-        Go.displayName = "DropdownHeader";
-        const Yo = Go,
-            Xo = i.forwardRef((({
+        Wo.displayName = "DropdownHeader";
+        const Uo = Wo,
+            qo = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 eventKey: n,
                 disabled: r = !1,
                 onClick: a,
                 active: s,
-                as: o = dt,
+                as: o = ct,
                 ...i
             }, l) => {
                 const c = E(e, "dropdown-item"),
-                    [u, d] = Io({
+                    [u, d] = Ro({
                         key: n,
                         href: i.href,
                         disabled: r,
                         onClick: a,
                         active: s
                     });
                 return (0, _.jsx)(o, {
                     ...i,
                     ...u,
                     ref: l,
                     className: b()(t, c, d.isActive && "active", r && "disabled")
                 })
             }));
-        Xo.displayName = "DropdownItem";
-        const Jo = Xo,
-            Qo = i.forwardRef((({
+        qo.displayName = "DropdownItem";
+        const Vo = qo,
+            Go = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "span",
                 ...r
             }, a) => (t = E(t, "dropdown-item-text"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        Qo.displayName = "DropdownItemText";
-        const Zo = Qo,
-            ei = i.createContext(null);
-        ei.displayName = "InputGroupContext";
-        const ti = ei,
-            ni = i.createContext(null);
-        ni.displayName = "NavbarContext";
-        const ri = ni;
+        Go.displayName = "DropdownItemText";
+        const Yo = Go,
+            Xo = i.createContext(null);
+        Xo.displayName = "InputGroupContext";
+        const Jo = Xo,
+            Qo = i.createContext(null);
+        Qo.displayName = "NavbarContext";
+        const Zo = Qo;
 
-        function ai(e, t) {
+        function ei(e, t) {
             return e
         }
 
-        function si(e, t, n) {
+        function ti(e, t, n) {
             let r = e ? n ? "bottom-start" : "bottom-end" : n ? "bottom-end" : "bottom-start";
             return "up" === t ? r = e ? n ? "top-start" : "top-end" : n ? "top-end" : "top-start" : "end" === t ? r = e ? n ? "left-end" : "right-end" : n ? "left-start" : "right-start" : "start" === t ? r = e ? n ? "right-end" : "left-end" : n ? "right-start" : "left-start" : "down-centered" === t ? r = "bottom" : "up-centered" === t && (r = "top"), r
         }
-        const oi = i.forwardRef((({
+        const ni = i.forwardRef((({
             bsPrefix: e,
             className: t,
             align: n,
             rootCloseEvent: r,
             flip: a = !0,
             show: s,
             renderOnMount: o,
             as: l = "div",
             popperConfig: c,
             variant: u,
             ...d
         }, p) => {
             let f = !1;
-            const m = (0, i.useContext)(ri),
+            const m = (0, i.useContext)(Zo),
                 g = E(e, "dropdown-menu"),
                 {
                     align: y,
                     drop: h,
                     isRTL: v
-                } = (0, i.useContext)(Wo);
+                } = (0, i.useContext)(zo);
             n = n || y;
-            const x = (0, i.useContext)(ti),
+            const x = (0, i.useContext)(Jo),
                 O = [];
             if (n)
                 if ("object" == typeof n) {
                     const e = Object.keys(n);
                     if (e.length) {
                         const t = e[0],
                             r = n[t];
                         f = "start" === r, O.push(`${g}-${t}-${r}`)
                     }
                 } else "end" === n && (f = !0);
-            const w = si(f, h, v),
+            const w = ti(f, h, v),
                 [N, {
                     hasShown: j,
                     popper: k,
                     show: P,
                     toggle: C
-                }] = po({
+                }] = io({
                     flip: a,
                     rootCloseEvent: r,
                     show: s,
                     usePopper: !m && 0 === O.length,
                     offset: [0, 2],
                     popperConfig: c,
                     placement: w
                 });
-            if (N.ref = oe(ai(p), N.ref), at((() => {
+            if (N.ref = oe(ei(p), N.ref), nt((() => {
                     P && (null == k || k.update())
                 }), [P]), !j && !o && !x) return null;
             "string" != typeof l && (N.show = P, N.close = () => null == C ? void 0 : C(!1), N.align = n);
             let T = d.style;
             return null != k && k.placement && (T = {
                 ...d.style,
                 ...N.style
@@ -6147,37 +6091,37 @@
                 style: T,
                 ...(O.length || m) && {
                     "data-bs-popper": "static"
                 },
                 className: b()(t, g, P && "show", f && `${g}-end`, u && `${g}-${u}`, ...O)
             })
         }));
-        oi.displayName = "DropdownMenu";
-        const ii = oi,
-            li = i.forwardRef((({
+        ni.displayName = "DropdownMenu";
+        const ri = ni,
+            ai = i.forwardRef((({
                 bsPrefix: e,
                 split: t,
                 className: n,
                 childBsPrefix: r,
-                as: a = nn,
+                as: a = Qt,
                 ...s
             }, o) => {
                 const l = E(e, "dropdown-toggle"),
-                    c = (0, i.useContext)(Ra);
+                    c = (0, i.useContext)(Pa);
                 void 0 !== r && (s.bsPrefix = r);
-                const [u] = jo();
-                return u.ref = oe(u.ref, ai(o)), (0, _.jsx)(a, {
+                const [u] = Oo();
+                return u.ref = oe(u.ref, ei(o)), (0, _.jsx)(a, {
                     className: b()(n, l, t && `${l}-split`, (null == c ? void 0 : c.show) && "show"),
                     ...u,
                     ...s
                 })
             }));
-        li.displayName = "DropdownToggle";
-        const ci = li,
-            ui = i.forwardRef(((e, t) => {
+        ai.displayName = "DropdownToggle";
+        const si = ai,
+            oi = i.forwardRef(((e, t) => {
                 const {
                     bsPrefix: n,
                     drop: r = "down",
                     show: a,
                     className: s,
                     align: o = "start",
                     onSelect: l,
@@ -6185,162 +6129,162 @@
                     focusFirstItemOnShow: u,
                     as: d = "div",
                     navbar: p,
                     autoClose: f = !0,
                     ...m
                 } = v(e, {
                     show: "onToggle"
-                }), g = (0, i.useContext)(ti), y = E(n, "dropdown"), h = P(), x = Ye(((e, t) => {
+                }), g = (0, i.useContext)(Jo), y = E(n, "dropdown"), h = P(), x = Ve(((e, t) => {
                     var n, r, a;
                     (null == (n = t.originalEvent) || null == (r = n.target) ? void 0 : r.classList.contains("dropdown-toggle")) && "mousedown" === t.source || (t.originalEvent.currentTarget !== document || "keydown" === t.source && "Escape" !== t.originalEvent.key || (t.source = "rootClose"), a = t.source, (!1 === f ? "click" === a : "inside" === f ? "rootClose" !== a : "outside" !== f || "select" !== a) && (null == c || c(e, t)))
-                })), O = si("end" === o, r, h), w = (0, i.useMemo)((() => ({
+                })), O = ti("end" === o, r, h), w = (0, i.useMemo)((() => ({
                     align: o,
                     drop: r,
                     isRTL: h
                 })), [o, r, h]), N = {
                     down: y,
                     "down-centered": `${y}-center`,
                     up: "dropup",
                     "up-centered": "dropup-center dropup",
                     end: "dropend",
                     start: "dropstart"
                 };
-                return (0, _.jsx)(Wo.Provider, {
+                return (0, _.jsx)(zo.Provider, {
                     value: w,
-                    children: (0, _.jsx)(Ho, {
+                    children: (0, _.jsx)(Fo, {
                         placement: O,
                         show: a,
                         onSelect: l,
                         onToggle: x,
                         focusFirstItemOnShow: u,
                         itemSelector: `.${y}-item:not(.disabled):not(:disabled)`,
                         children: g ? m.children : (0, _.jsx)(d, {
                             ...m,
                             ref: t,
                             className: b()(s, a && "show", N[r])
                         })
                     })
                 })
             }));
-        ui.displayName = "Dropdown";
-        const di = Object.assign(ui, {
-            Toggle: ci,
-            Menu: ii,
-            Item: Jo,
-            ItemText: Zo,
-            Divider: Vo,
-            Header: Yo
+        oi.displayName = "Dropdown";
+        const ii = Object.assign(oi, {
+            Toggle: si,
+            Menu: ri,
+            Item: Vo,
+            ItemText: Yo,
+            Divider: Ho,
+            Header: Uo
         });
         n(6);
-        const pi = i.createContext(null),
-            fi = ["as", "active", "eventKey"];
+        const li = i.createContext(null),
+            ci = ["as", "active", "eventKey"];
 
-        function mi({
+        function ui({
             key: e,
             onClick: t,
             active: n,
             id: r,
             role: a,
             disabled: s
         }) {
-            const o = (0, i.useContext)(To),
-                l = (0, i.useContext)(Ro),
-                c = (0, i.useContext)(pi);
+            const o = (0, i.useContext)(jo),
+                l = (0, i.useContext)(Po),
+                c = (0, i.useContext)(li);
             let u = n;
             const d = {
                 role: a
             };
             if (l) {
                 a || "tablist" !== l.role || (d.role = "tab");
                 const t = l.getControllerId(null != e ? e : null),
                     s = l.getControlledId(null != e ? e : null);
-                d[Lo("event-key")] = e, d.id = t || r, u = null == n && null != e ? l.activeKey === e : n, !u && (null != c && c.unmountOnExit || null != c && c.mountOnEnter) || (d["aria-controls"] = s)
+                d[To("event-key")] = e, d.id = t || r, u = null == n && null != e ? l.activeKey === e : n, !u && (null != c && c.unmountOnExit || null != c && c.mountOnEnter) || (d["aria-controls"] = s)
             }
-            return "tab" === d.role && (d["aria-selected"] = u, u || (d.tabIndex = -1), s && (d.tabIndex = -1, d["aria-disabled"] = !0)), d.onClick = Ye((n => {
+            return "tab" === d.role && (d["aria-selected"] = u, u || (d.tabIndex = -1), s && (d.tabIndex = -1, d["aria-disabled"] = !0)), d.onClick = Ve((n => {
                 s || (null == t || t(n), null != e && o && !n.isPropagationStopped() && o(e, n))
             })), [d, {
                 isActive: u
             }]
         }
-        const gi = i.forwardRef(((e, t) => {
+        const di = i.forwardRef(((e, t) => {
             let {
-                as: n = lt,
+                as: n = ot,
                 active: r,
                 eventKey: a
             } = e, s = function(e, t) {
                 if (null == e) return {};
                 var n, r, a = {},
                     s = Object.keys(e);
                 for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                 return a
-            }(e, fi);
-            const [o, i] = mi(Object.assign({
-                key: Co(a, s.href),
+            }(e, ci);
+            const [o, i] = ui(Object.assign({
+                key: Eo(a, s.href),
                 active: r
             }, s));
-            return o[Lo("active")] = i.isActive, (0, _.jsx)(n, Object.assign({}, s, o, {
+            return o[To("active")] = i.isActive, (0, _.jsx)(n, Object.assign({}, s, o, {
                 ref: t
             }))
         }));
-        gi.displayName = "NavItem";
-        const bi = gi,
-            yi = ["as", "onSelect", "activeKey", "role", "onKeyDown"],
-            hi = () => {},
-            vi = Lo("event-key"),
-            _i = i.forwardRef(((e, t) => {
+        di.displayName = "NavItem";
+        const pi = di,
+            fi = ["as", "onSelect", "activeKey", "role", "onKeyDown"],
+            mi = () => {},
+            gi = To("event-key"),
+            bi = i.forwardRef(((e, t) => {
                 let {
                     as: n = "div",
                     onSelect: r,
                     activeKey: a,
                     role: s,
                     onKeyDown: o
                 } = e, l = function(e, t) {
                     if (null == e) return {};
                     var n, r, a = {},
                         s = Object.keys(e);
                     for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                     return a
-                }(e, yi);
-                const c = Sa(),
+                }(e, fi);
+                const c = ka(),
                     u = (0, i.useRef)(!1),
-                    d = (0, i.useContext)(To),
-                    p = (0, i.useContext)(pi);
+                    d = (0, i.useContext)(jo),
+                    p = (0, i.useContext)(li);
                 let f, m;
                 p && (s = s || "tablist", a = p.activeKey, f = p.getControlledId, m = p.getControllerId);
                 const g = (0, i.useRef)(null),
                     b = e => {
                         const t = g.current;
                         if (!t) return null;
-                        const n = Ca(t, `[${vi}]:not([aria-disabled=true])`),
+                        const n = Ea(t, `[${gi}]:not([aria-disabled=true])`),
                             r = t.querySelector("[aria-selected=true]");
                         if (!r || r !== document.activeElement) return null;
                         const a = n.indexOf(r);
                         if (-1 === a) return null;
                         let s = a + e;
                         return s >= n.length && (s = 0), s < 0 && (s = n.length - 1), n[s]
                     },
                     y = (e, t) => {
                         null != e && (null == r || r(e, t), null == d || d(e, t))
                     };
                 (0, i.useEffect)((() => {
                     if (g.current && u.current) {
-                        const e = g.current.querySelector(`[${vi}][aria-selected=true]`);
+                        const e = g.current.querySelector(`[${gi}][aria-selected=true]`);
                         null == e || e.focus()
                     }
                     u.current = !1
                 }));
                 const h = oe(t, g);
-                return (0, _.jsx)(To.Provider, {
+                return (0, _.jsx)(jo.Provider, {
                     value: y,
-                    children: (0, _.jsx)(Ro.Provider, {
+                    children: (0, _.jsx)(Po.Provider, {
                         value: {
                             role: s,
-                            activeKey: Co(a),
-                            getControlledId: f || hi,
-                            getControllerId: m || hi
+                            activeKey: Eo(a),
+                            getControlledId: f || mi,
+                            getControllerId: m || mi
                         },
                         children: (0, _.jsx)(n, Object.assign({}, l, {
                             onKeyDown: e => {
                                 if (null == o || o(e), !p) return;
                                 let t;
                                 switch (e.key) {
                                     case "ArrowLeft":
@@ -6358,57 +6302,57 @@
                             },
                             ref: h,
                             role: s
                         }))
                     })
                 })
             }));
-        _i.displayName = "Nav";
-        const xi = Object.assign(_i, {
-                Item: bi
+        bi.displayName = "Nav";
+        const yi = Object.assign(bi, {
+                Item: pi
             }),
-            Oi = i.forwardRef((({
+            hi = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "nav-item"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        Oi.displayName = "NavItem";
-        const wi = Oi,
-            Ni = i.forwardRef((({
+        hi.displayName = "NavItem";
+        const vi = hi,
+            _i = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
-                as: n = dt,
+                as: n = ct,
                 active: r,
                 eventKey: a,
                 disabled: s = !1,
                 ...o
             }, i) => {
                 e = E(e, "nav-link");
-                const [l, c] = mi({
-                    key: Co(a, o.href),
+                const [l, c] = ui({
+                    key: Eo(a, o.href),
                     active: r,
                     disabled: s,
                     ...o
                 });
                 return (0, _.jsx)(n, {
                     ...o,
                     ...l,
                     ref: i,
                     disabled: s,
                     className: b()(t, e, s && "disabled", c.isActive && "active")
                 })
             }));
-        Ni.displayName = "NavLink";
-        const Ei = Ni,
-            ji = i.forwardRef(((e, t) => {
+        _i.displayName = "NavLink";
+        const xi = _i,
+            Oi = i.forwardRef(((e, t) => {
                 const {
                     as: n = "div",
                     bsPrefix: r,
                     variant: a,
                     fill: s = !1,
                     justify: o = !1,
                     navbar: l,
@@ -6416,19 +6360,19 @@
                     className: u,
                     activeKey: d,
                     ...p
                 } = v(e, {
                     activeKey: "onSelect"
                 }), f = E(r, "nav");
                 let m, g, y = !1;
-                const h = (0, i.useContext)(ri),
-                    x = (0, i.useContext)(yn);
+                const h = (0, i.useContext)(Zo),
+                    x = (0, i.useContext)(fn);
                 return h ? (m = h.bsPrefix, y = null == l || l) : x && ({
                     cardHeaderBsPrefix: g
-                } = x), (0, _.jsx)(xi, {
+                } = x), (0, _.jsx)(yi, {
                     as: n,
                     ref: t,
                     activeKey: d,
                     className: b()(u, {
                         [f]: !y,
                         [`${m}-nav`]: y,
                         [`${m}-nav-scroll`]: y && c,
@@ -6436,64 +6380,64 @@
                         [`${f}-${a}`]: !!a,
                         [`${f}-fill`]: s,
                         [`${f}-justified`]: o
                     }),
                     ...p
                 })
             }));
-        ji.displayName = "Nav";
-        const ki = Object.assign(ji, {
-            Item: wi,
-            Link: Ei
+        Oi.displayName = "Nav";
+        const wi = Object.assign(Oi, {
+            Item: vi,
+            Link: xi
         });
-        var Pi = l().createContext({}),
-            Ci = ["caret", "bsPrefix", "split", "className", "childBsPrefix", "as"];
-        const Ti = l().forwardRef((function(t, n) {
+        var Ni = l().createContext({}),
+            Ei = ["caret", "bsPrefix", "split", "className", "childBsPrefix", "as"];
+        const ji = l().forwardRef((function(t, n) {
             var r = t.caret,
                 a = t.bsPrefix,
                 s = t.split,
                 c = t.className,
                 u = t.childBsPrefix,
                 d = t.as,
-                p = void 0 === d ? nn : d,
-                f = o(t, Ci),
+                p = void 0 === d ? Qt : d,
+                f = o(t, Ei),
                 m = E(a, "dropdown-toggle"),
-                g = (0, i.useContext)(Ra),
-                y = (0, i.useContext)(ti);
+                g = (0, i.useContext)(Pa),
+                y = (0, i.useContext)(Jo);
             void 0 !== u && (f.bsPrefix = u);
-            var h = Se(jo(), 1)[0];
-            return h.ref = oe(h.ref, ai(n)), l().createElement(p, e({
+            var h = Se(Oo(), 1)[0];
+            return h.ref = oe(h.ref, ei(n)), l().createElement(p, e({
                 className: b()(c, r && m, s && "".concat(m, "-split"), !!y && (null == g ? void 0 : g.show) && "show")
             }, h, f))
         }));
-        var Si = ["children", "nav", "label", "disabled", "caret", "in_navbar", "addon_type", "size", "right", "align_end", "menu_variant", "direction", "loading_state", "color", "group", "toggle_style", "toggleClassName", "toggle_class_name", "className", "class_name"];
+        var ki = ["children", "nav", "label", "disabled", "caret", "in_navbar", "addon_type", "size", "right", "align_end", "menu_variant", "direction", "loading_state", "color", "group", "toggle_style", "toggleClassName", "toggle_class_name", "className", "class_name"];
 
-        function Ri(e, t) {
+        function Pi(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Di(e) {
+        function Ci(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Ri(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ri(Object(n)).forEach((function(t) {
+                t % 2 ? Pi(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Pi(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Li = function(t) {
+        var Ti = function(t) {
             var n = t.children,
                 r = t.nav,
                 a = t.label,
                 s = t.disabled,
                 c = t.caret,
                 u = t.in_navbar,
                 d = (t.addon_type, t.size),
@@ -6505,61 +6449,61 @@
                 h = t.color,
                 v = t.group,
                 _ = t.toggle_style,
                 x = t.toggleClassName,
                 O = t.toggle_class_name,
                 w = t.className,
                 N = t.class_name,
-                E = o(t, Si),
+                E = o(t, ki),
                 j = Se((0, i.useState)(!1), 2),
                 k = j[0],
                 P = j[1],
-                C = Ot.has(h) || "link" === h,
+                C = _t.has(h) || "link" === h,
                 T = function() {
                     s || P(!k)
                 };
-            return l().createElement(Pi.Provider, {
+            return l().createElement(Ni.Provider, {
                 value: {
                     toggle: T,
                     isOpen: k
                 }
-            }, l().createElement(di, e({
-                as: r ? ki.Item : v ? ln : void 0,
+            }, l().createElement(ii, e({
+                as: r ? wi.Item : v ? rn : void 0,
                 show: k,
                 disabled: s,
                 navbar: u,
                 className: N || w,
                 drop: "left" === b ? "start" : "right" === b ? "end" : b,
                 onToggle: function(e, t) {
                     t && "select" === t.source || P(e)
                 },
                 align: f || p ? "end" : "start"
             }, m(["setProps"], E), {
                 "data-dash-is-loading": y && y.is_loading || void 0
-            }), l().createElement(Ti, {
+            }), l().createElement(ji, {
                 caret: c,
-                as: r ? ki.Link : void 0,
+                as: r ? wi.Link : void 0,
                 onClick: T,
                 disabled: s,
                 size: d,
                 variant: C ? h : void 0,
-                style: C ? _ : Di({
+                style: C ? _ : Ci({
                     backgroundColor: h
                 }, _),
                 className: O || x
-            }, a), l().createElement(di.Menu, {
+            }, a), l().createElement(ii.Menu, {
                 renderOnMount: !0,
                 variant: "dark" === g ? "dark" : void 0
             }, n)))
         };
-        Li.defaultProps = {
+        Ti.defaultProps = {
             caret: !0,
             disabled: !1,
             menu_variant: "light"
-        }, Li.propTypes = {
+        }, Ti.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             label: u().node,
@@ -6580,51 +6524,50 @@
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             group: u().bool
         };
-        const $i = Li;
-        var Ii = ["children", "href", "loading_state", "target", "disabled", "n_clicks", "toggle", "setProps", "className", "class_name", "header", "divider"],
-            Ai = function(t) {
+        const Si = Ti;
+        var Ri = ["children", "href", "loading_state", "target", "disabled", "n_clicks", "toggle", "setProps", "className", "class_name", "header", "divider"],
+            Di = function(t) {
                 var n = t.children,
                     r = t.href,
                     a = t.loading_state,
                     s = t.target,
                     c = t.disabled,
                     u = t.n_clicks,
                     d = t.toggle,
                     p = t.setProps,
                     f = t.className,
                     g = t.class_name,
                     b = t.header,
                     y = t.divider,
-                    h = o(t, Ii),
-                    v = Fe(r, p),
-                    _ = (0, i.useContext)(Pi),
-                    x = v && !c;
-                return h[x ? "preOnClick" : "onClick"] = function(e) {
+                    h = o(t, Ri),
+                    v = (0, i.useContext)(Ni),
+                    _ = r && !c;
+                return h[_ ? "preOnClick" : "onClick"] = function(e) {
                     return function(e) {
                         !c && p && p({
                             n_clicks: u + 1,
                             n_clicks_timestamp: Date.now()
-                        }), d && _.isOpen && _.toggle(e)
+                        }), d && v.isOpen && v.toggle(e)
                     }(e)
-                }, b ? l().createElement(di.Header, null, n) : y ? l().createElement(di.Divider, null) : l().createElement(di.Item, e({
-                    as: x ? Bt : "button",
-                    href: x ? v : void 0,
+                }, b ? l().createElement(ii.Header, null, n) : y ? l().createElement(ii.Divider, null) : l().createElement(ii.Item, e({
+                    as: _ ? Mt : "button",
+                    href: _ ? r : void 0,
                     disabled: c,
-                    target: x ? s : void 0,
+                    target: _ ? s : void 0,
                     className: g || f
                 }, m(["setProps"], h), {
                     "data-dash-is-loading": a && a.is_loading || void 0
                 }), n)
             };
-        Ai.propTypes = {
+        Di.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             active: u().bool,
@@ -6638,59 +6581,59 @@
             n_clicks_timestamp: u().number,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             target: u().string
-        }, Ai.defaultProps = {
+        }, Di.defaultProps = {
             n_clicks: 0,
             n_clicks_timestamp: -1,
             toggle: !0
         };
-        const Fi = Ai;
-        var Mi = ["children", "is_in", "loading_state", "style", "className", "class_name", "tag"];
+        const Li = Di;
+        var Ii = ["children", "is_in", "loading_state", "style", "className", "class_name", "tag"];
 
-        function Bi(e, t) {
+        function $i(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function zi(e) {
+        function Ai(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Bi(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Bi(Object(n)).forEach((function(t) {
+                t % 2 ? $i(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : $i(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Ki = l().forwardRef((function(t, n) {
+        var Mi = l().forwardRef((function(t, n) {
             var r = t.children,
                 a = t.is_in,
                 s = t.loading_state,
                 c = t.style,
                 u = t.className,
                 d = t.class_name,
                 p = t.tag,
-                f = o(t, Mi),
+                f = o(t, Ii),
                 g = Se((0, i.useState)(!a), 2),
                 b = g[0],
                 y = g[1];
-            return l().createElement(bt, e({
+            return l().createElement(mt, e({
                 in: a,
-                style: b ? zi({
+                style: b ? Ai({
                     visibility: "hidden"
                 }, c) : c,
                 onEnter: function() {
                     return y(!1)
                 },
                 onExited: function() {
                     return y(!0)
@@ -6699,15 +6642,15 @@
                 as: p
             }, m(["setProps"], f), {
                 "data-dash-is-loading": s && s.is_loading || void 0
             }), l().createElement("div", {
                 ref: n
             }, r))
         }));
-        Ki.propTypes = {
+        Mi.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             is_in: u().bool,
@@ -6721,76 +6664,76 @@
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Hi = Ki,
-            Ui = {
+        const Fi = Mi,
+            Bi = {
                 type: u().string,
                 tooltip: u().bool,
                 as: u().elementType
             },
-            Wi = i.forwardRef((({
+            zi = i.forwardRef((({
                 as: e = "div",
                 className: t,
                 type: n = "valid",
                 tooltip: r = !1,
                 ...a
             }, s) => (0, _.jsx)(e, {
                 ...a,
                 ref: s,
                 className: b()(t, `${n}-${r?"tooltip":"feedback"}`)
             })));
-        Wi.displayName = "Feedback", Wi.propTypes = Ui;
-        const qi = Wi,
-            Vi = i.createContext({}),
-            Gi = i.forwardRef((({
+        zi.displayName = "Feedback", zi.propTypes = Bi;
+        const Ki = zi,
+            Hi = i.createContext({}),
+            Wi = i.forwardRef((({
                 id: e,
                 bsPrefix: t,
                 className: n,
                 type: r = "checkbox",
                 isValid: a = !1,
                 isInvalid: s = !1,
                 as: o = "input",
                 ...l
             }, c) => {
                 const {
                     controlId: u
-                } = (0, i.useContext)(Vi);
+                } = (0, i.useContext)(Hi);
                 return t = E(t, "form-check-input"), (0, _.jsx)(o, {
                     ...l,
                     ref: c,
                     type: r,
                     id: e || u,
                     className: b()(n, t, a && "is-valid", s && "is-invalid")
                 })
             }));
-        Gi.displayName = "FormCheckInput";
-        const Yi = Gi,
-            Xi = i.forwardRef((({
+        Wi.displayName = "FormCheckInput";
+        const Ui = Wi,
+            qi = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 htmlFor: n,
                 ...r
             }, a) => {
                 const {
                     controlId: s
-                } = (0, i.useContext)(Vi);
+                } = (0, i.useContext)(Hi);
                 return e = E(e, "form-check-label"), (0, _.jsx)("label", {
                     ...r,
                     ref: a,
                     htmlFor: n || s,
                     className: b()(t, e)
                 })
             }));
-        Xi.displayName = "FormCheckLabel";
-        const Ji = Xi,
-            Qi = i.forwardRef((({
+        qi.displayName = "FormCheckLabel";
+        const Vi = qi,
+            Gi = i.forwardRef((({
                 id: e,
                 bsPrefix: t,
                 bsSwitchPrefix: n,
                 inline: r = !1,
                 reverse: a = !1,
                 disabled: s = !1,
                 isValid: o = !1,
@@ -6806,51 +6749,51 @@
                 children: h,
                 as: v = "input",
                 ...x
             }, O) => {
                 t = E(t, "form-check"), n = E(n, "form-switch");
                 const {
                     controlId: w
-                } = (0, i.useContext)(Vi), N = (0, i.useMemo)((() => ({
+                } = (0, i.useContext)(Hi), N = (0, i.useMemo)((() => ({
                     controlId: e || w
                 })), [w, e]), j = !h && null != y && !1 !== y || function(e, t) {
                     return i.Children.toArray(e).some((e => i.isValidElement(e) && e.type === t))
-                }(h, Ji), k = (0, _.jsx)(Yi, {
+                }(h, Vi), k = (0, _.jsx)(Ui, {
                     ...x,
                     type: "switch" === g ? "checkbox" : g,
                     ref: O,
                     isValid: o,
                     isInvalid: l,
                     disabled: s,
                     as: v
                 });
-                return (0, _.jsx)(Vi.Provider, {
+                return (0, _.jsx)(Hi.Provider, {
                     value: N,
                     children: (0, _.jsx)("div", {
                         style: f,
                         className: b()(p, j && t, r && `${t}-inline`, a && `${t}-reverse`, "switch" === g && n),
                         children: h || (0, _.jsxs)(_.Fragment, {
-                            children: [k, j && (0, _.jsx)(Ji, {
+                            children: [k, j && (0, _.jsx)(Vi, {
                                 title: m,
                                 children: y
-                            }), u && (0, _.jsx)(qi, {
+                            }), u && (0, _.jsx)(Ki, {
                                 type: d,
                                 tooltip: c,
                                 children: u
                             })]
                         })
                     })
                 })
             }));
-        Qi.displayName = "FormCheck";
-        const Zi = Object.assign(Qi, {
-                Input: Yi,
-                Label: Ji
+        Gi.displayName = "FormCheck";
+        const Yi = Object.assign(Gi, {
+                Input: Ui,
+                Label: Vi
             }),
-            el = i.forwardRef((({
+            Xi = i.forwardRef((({
                 bsPrefix: e,
                 type: t,
                 size: n,
                 htmlSize: r,
                 id: a,
                 className: s,
                 isValid: o = !1,
@@ -6858,229 +6801,229 @@
                 plaintext: c,
                 readOnly: u,
                 as: d = "input",
                 ...p
             }, f) => {
                 const {
                     controlId: m
-                } = (0, i.useContext)(Vi);
+                } = (0, i.useContext)(Hi);
                 return e = E(e, "form-control"), (0, _.jsx)(d, {
                     ...p,
                     type: t,
                     size: r,
                     ref: f,
                     readOnly: u,
                     id: a || m,
                     className: b()(s, c ? `${e}-plaintext` : e, n && `${e}-${n}`, "color" === t && `${e}-color`, o && "is-valid", l && "is-invalid")
                 })
             }));
-        el.displayName = "FormControl";
-        const tl = Object.assign(el, {
-                Feedback: qi
+        Xi.displayName = "FormControl";
+        const Ji = Object.assign(Xi, {
+                Feedback: Ki
             }),
-            nl = i.forwardRef((({
+            Qi = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "form-floating"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        nl.displayName = "FormFloating";
-        const rl = nl,
-            al = i.forwardRef((({
+        Qi.displayName = "FormFloating";
+        const Zi = Qi,
+            el = i.forwardRef((({
                 controlId: e,
                 as: t = "div",
                 ...n
             }, r) => {
                 const a = (0, i.useMemo)((() => ({
                     controlId: e
                 })), [e]);
-                return (0, _.jsx)(Vi.Provider, {
+                return (0, _.jsx)(Hi.Provider, {
                     value: a,
                     children: (0, _.jsx)(t, {
                         ...n,
                         ref: r
                     })
                 })
             }));
-        al.displayName = "FormGroup";
-        const sl = al,
-            ol = i.forwardRef((({
+        el.displayName = "FormGroup";
+        const tl = el,
+            nl = i.forwardRef((({
                 as: e = "label",
                 bsPrefix: t,
                 column: n = !1,
                 visuallyHidden: r = !1,
                 className: a,
                 htmlFor: s,
                 ...o
             }, l) => {
                 const {
                     controlId: c
-                } = (0, i.useContext)(Vi);
+                } = (0, i.useContext)(Hi);
                 t = E(t, "form-label");
                 let u = "col-form-label";
                 "string" == typeof n && (u = `${u} ${u}-${n}`);
                 const d = b()(a, t, r && "visually-hidden", n && u);
-                return s = s || c, n ? (0, _.jsx)(fa, {
+                return s = s || c, n ? (0, _.jsx)(ca, {
                     ref: l,
                     as: "label",
                     className: d,
                     htmlFor: s,
                     ...o
                 }) : (0, _.jsx)(e, {
                     ref: l,
                     className: d,
                     htmlFor: s,
                     ...o
                 })
             }));
-        ol.displayName = "FormLabel";
-        const il = ol,
-            ll = i.forwardRef((({
+        nl.displayName = "FormLabel";
+        const rl = nl,
+            al = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 id: n,
                 ...r
             }, a) => {
                 const {
                     controlId: s
-                } = (0, i.useContext)(Vi);
+                } = (0, i.useContext)(Hi);
                 return e = E(e, "form-range"), (0, _.jsx)("input", {
                     ...r,
                     type: "range",
                     ref: a,
                     className: b()(t, e),
                     id: n || s
                 })
             }));
-        ll.displayName = "FormRange";
-        const cl = ll,
-            ul = i.forwardRef((({
+        al.displayName = "FormRange";
+        const sl = al,
+            ol = i.forwardRef((({
                 bsPrefix: e,
                 size: t,
                 htmlSize: n,
                 className: r,
                 isValid: a = !1,
                 isInvalid: s = !1,
                 id: o,
                 ...l
             }, c) => {
                 const {
                     controlId: u
-                } = (0, i.useContext)(Vi);
+                } = (0, i.useContext)(Hi);
                 return e = E(e, "form-select"), (0, _.jsx)("select", {
                     ...l,
                     size: n,
                     ref: c,
                     className: b()(r, e, t && `${e}-${t}`, a && "is-valid", s && "is-invalid"),
                     id: o || u
                 })
             }));
-        ul.displayName = "FormSelect";
-        const dl = ul,
-            pl = i.forwardRef((({
+        ol.displayName = "FormSelect";
+        const il = ol,
+            ll = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 as: n = "small",
                 muted: r,
                 ...a
             }, s) => (e = E(e, "form-text"), (0, _.jsx)(n, {
                 ...a,
                 ref: s,
                 className: b()(t, e, r && "text-muted")
             }))));
-        pl.displayName = "FormText";
-        const fl = pl,
-            ml = i.forwardRef(((e, t) => (0, _.jsx)(Zi, {
+        ll.displayName = "FormText";
+        const cl = ll,
+            ul = i.forwardRef(((e, t) => (0, _.jsx)(Yi, {
                 ...e,
                 ref: t,
                 type: "switch"
             })));
-        ml.displayName = "Switch";
-        const gl = Object.assign(ml, {
-                Input: Zi.Input,
-                Label: Zi.Label
+        ul.displayName = "Switch";
+        const dl = Object.assign(ul, {
+                Input: Yi.Input,
+                Label: Yi.Label
             }),
-            bl = i.forwardRef((({
+            pl = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 children: n,
                 controlId: r,
                 label: a,
                 ...s
-            }, o) => (e = E(e, "form-floating"), (0, _.jsxs)(sl, {
+            }, o) => (e = E(e, "form-floating"), (0, _.jsxs)(tl, {
                 ref: o,
                 className: b()(t, e),
                 controlId: r,
                 ...s,
                 children: [n, (0, _.jsx)("label", {
                     htmlFor: r,
                     children: a
                 })]
             }))));
-        bl.displayName = "FloatingLabel";
-        const yl = bl,
-            hl = {
+        pl.displayName = "FloatingLabel";
+        const fl = pl,
+            ml = {
                 _ref: u().any,
                 validated: u().bool,
                 as: u().elementType
             },
-            vl = i.forwardRef((({
+            gl = i.forwardRef((({
                 className: e,
                 validated: t,
                 as: n = "form",
                 ...r
             }, a) => (0, _.jsx)(n, {
                 ...r,
                 ref: a,
                 className: b()(e, t && "was-validated")
             })));
-        vl.displayName = "Form", vl.propTypes = hl;
-        const _l = Object.assign(vl, {
-            Group: sl,
-            Control: tl,
-            Floating: rl,
-            Check: Zi,
-            Switch: gl,
-            Label: il,
-            Text: fl,
-            Range: cl,
-            Select: dl,
-            FloatingLabel: yl
+        gl.displayName = "Form", gl.propTypes = ml;
+        const bl = Object.assign(gl, {
+            Group: tl,
+            Control: Ji,
+            Floating: Zi,
+            Check: Yi,
+            Switch: dl,
+            Label: rl,
+            Text: cl,
+            Range: sl,
+            Select: il,
+            FloatingLabel: fl
         });
-        var xl = ["children", "loading_state", "n_submit", "prevent_default_on_submit", "setProps", "className", "class_name"],
-            Ol = function(t) {
+        var yl = ["children", "loading_state", "n_submit", "prevent_default_on_submit", "setProps", "className", "class_name"],
+            hl = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.n_submit,
                     s = t.prevent_default_on_submit,
                     i = t.setProps,
                     c = t.className,
                     u = t.class_name,
-                    d = o(t, xl);
-                return l().createElement(_l, e({
+                    d = o(t, yl);
+                return l().createElement(bl, e({
                     onSubmit: function(e) {
                         s && e.preventDefault(), i && i({
                             n_submit: a + 1,
                             n_submit_timestamp: Date.now()
                         })
                     },
                     className: u || c
                 }, m(["n_submit_timestamp"], d), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Ol.defaultProps = {
+        hl.defaultProps = {
             prevent_default_on_submit: !0,
             n_submit: 0,
             n_submit_timestamp: -1
-        }, Ol.propTypes = {
+        }, hl.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             action: u().string,
@@ -7090,168 +7033,168 @@
             prevent_default_on_submit: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const wl = Ol;
-        var Nl = ["children", "loading_state", "className", "class_name"],
-            El = function(t) {
+        const vl = hl;
+        var _l = ["children", "loading_state", "className", "class_name"],
+            xl = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Nl);
-                return l().createElement(tl.Feedback, e({
+                    i = o(t, _l);
+                return l().createElement(Ji.Feedback, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        El.propTypes = {
+        xl.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             type: u().string,
             tooltip: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const jl = El;
-        var kl = ["children", "html_for", "className", "class_name", "loading_state"],
-            Pl = function(t) {
+        const Ol = xl;
+        var wl = ["children", "html_for", "className", "class_name", "loading_state"],
+            Nl = function(t) {
                 var n = t.children,
                     r = t.html_for,
                     a = t.className,
                     s = t.class_name,
                     i = t.loading_state,
-                    c = o(t, kl);
-                return l().createElement(rl, e({
+                    c = o(t, wl);
+                return l().createElement(Zi, e({
                     htmlFor: r,
                     className: s || a
                 }, m(["setProps"], c), {
                     "data-dash-is-loading": i && i.is_loading || void 0
                 }), n)
             };
-        Pl.propTypes = {
+        Nl.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             html_for: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Cl = Pl;
-        var Tl = ["children", "loading_state", "color", "style", "className", "class_name"];
+        const El = Nl;
+        var jl = ["children", "loading_state", "color", "style", "className", "class_name"];
 
-        function Sl(e, t) {
+        function kl(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Rl(e) {
+        function Pl(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Sl(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Sl(Object(n)).forEach((function(t) {
+                t % 2 ? kl(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : kl(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Dl = function(t) {
+        var Cl = function(t) {
             var n = t.children,
                 r = t.loading_state,
                 a = t.color,
                 s = t.style,
                 i = t.className,
                 c = t.class_name,
-                u = o(t, Tl),
-                d = wt.has(a),
+                u = o(t, jl),
+                d = xt.has(a),
                 p = b()(c || i, d && "text-".concat(a));
-            return l().createElement(fl, e({
-                style: d ? s : Rl({
+            return l().createElement(cl, e({
+                style: d ? s : Pl({
                     color: a
                 }, s),
                 className: p
             }, m(["setProps"], u), {
                 "data-dash-is-loading": r && r.is_loading || void 0
             }), n)
         };
-        Dl.propTypes = {
+        Cl.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             color: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Ll = Dl,
-            $l = p((function(e) {
+        const Tl = Cl,
+            Sl = p((function(e) {
                 return null == e
             }));
-        var Il = n(11),
-            Al = n.n(Il),
-            Fl = ["type", "value", "n_blur", "n_submit", "valid", "invalid", "plaintext", "size", "html_size", "setProps", "debounce", "loading_state", "className", "class_name", "autoComplete", "autocomplete", "autoFocus", "autofocus", "inputMode", "inputmode", "maxLength", "maxlength", "minLength", "minlength", "readonly", "tabIndex", "tabindex"];
+        var Rl = n(11),
+            Dl = n.n(Rl),
+            Ll = ["type", "value", "n_blur", "n_submit", "valid", "invalid", "plaintext", "size", "html_size", "setProps", "debounce", "loading_state", "className", "class_name", "autoComplete", "autocomplete", "autoFocus", "autofocus", "inputMode", "inputmode", "maxLength", "maxlength", "minLength", "minlength", "readonly", "tabIndex", "tabindex"];
 
-        function Ml(e, t) {
+        function Il(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Bl(e) {
+        function $l(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Ml(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ml(Object(n)).forEach((function(t) {
+                t % 2 ? Il(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Il(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var zl = function(e) {
-                return Al()(e) ? +e : NaN
+        var Al = function(e) {
+                return Dl()(e) ? +e : NaN
             },
-            Kl = function(e, t) {
+            Ml = function(e, t) {
                 return e === t || isNaN(e) && isNaN(t)
             },
-            Hl = function(t) {
+            Fl = function(t) {
                 var n = t.type,
                     r = t.value,
                     a = t.n_blur,
                     s = t.n_submit,
                     c = t.valid,
                     u = t.invalid,
                     d = t.plaintext,
@@ -7271,63 +7214,63 @@
                     k = t.maxLength,
                     P = t.maxlength,
                     C = t.minLength,
                     T = t.minlength,
                     S = t.readonly,
                     R = t.tabIndex,
                     D = t.tabindex,
-                    L = o(t, Fl),
-                    $ = (0, i.useRef)(null),
-                    I = d ? "form-control-plaintext" : "form-control",
-                    A = b()(_ || v, u && "is-invalid", c && "is-valid", !!p && "form-control-".concat(p), I);
+                    L = o(t, Ll),
+                    I = (0, i.useRef)(null),
+                    $ = d ? "form-control-plaintext" : "form-control",
+                    A = b()(_ || v, u && "is-invalid", c && "is-valid", !!p && "form-control-".concat(p), $);
                 (0, i.useEffect)((function() {
                     if ("number" === n) {
-                        var e = $.current.value,
-                            t = $.current.checkValidity() ? zl(e) : NaN,
-                            a = zl(r);
-                        Kl(a, t) || ($.current.value = $l(a) ? a : r)
+                        var e = I.current.value,
+                            t = I.current.checkValidity() ? Al(e) : NaN,
+                            a = Al(r);
+                        Ml(a, t) || (I.current.value = Sl(a) ? a : r)
                     } else {
-                        var s = $.current.value;
-                        r !== s && ($.current.value = null != r ? r : "")
+                        var s = I.current.value;
+                        r !== s && (I.current.value = null != r ? r : "")
                     }
                 }), [r]);
-                var F = function() {
+                var M = function() {
                     var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     if ("number" === n) {
-                        var t = $.current.value,
-                            a = $.current.checkValidity() ? zl(t) : NaN,
-                            s = zl(r);
-                        Kl(s, a) ? Object.keys(e).length && g(e) : g(Bl(Bl({}, e), {}, {
+                        var t = I.current.value,
+                            a = I.current.checkValidity() ? Al(t) : NaN,
+                            s = Al(r);
+                        Ml(s, a) ? Object.keys(e).length && g(e) : g($l($l({}, e), {}, {
                             value: a
                         }))
-                    } else e.value = $.current.value, g(e)
+                    } else e.value = I.current.value, g(e)
                 };
                 return l().createElement("input", e({
-                    ref: $,
+                    ref: I,
                     type: n,
                     className: A,
                     onChange: function() {
-                        y || F()
+                        y || M()
                     },
                     onBlur: function() {
                         if (g) {
                             var e = {
                                 n_blur: a + 1,
                                 n_blur_timestamp: Date.now()
                             };
-                            y ? F(e) : g(e)
+                            y ? M(e) : g(e)
                         }
                     },
                     onKeyPress: function(e) {
                         if (g && "Enter" === e.key) {
                             var t = {
                                 n_submit: s + 1,
                                 n_submit_timestamp: Date.now()
                             };
-                            y ? F(t) : g(t)
+                            y ? M(t) : g(t)
                         }
                     }
                 }, m(["n_blur_timestamp", "n_submit_timestamp", "persistence", "persistence_type", "persisted_props"], L), {
                     valid: c ? "true" : void 0,
                     invalid: u ? "true" : void 0,
                     "data-dash-is-loading": h && h.is_loading || void 0,
                     autoComplete: O || x,
@@ -7336,15 +7279,15 @@
                     maxLength: P || k,
                     minLength: T || C,
                     readOnly: S,
                     tabIndex: D || R,
                     size: f
                 }))
             };
-        Hl.propTypes = {
+        Fl.propTypes = {
             id: u().string,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             type: u().oneOf(["text", "number", "password", "email", "range", "search", "tel", "url", "hidden"]),
             value: u().oneOfType([u().string, u().number]),
@@ -7384,158 +7327,158 @@
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             tabindex: u().string,
             tabIndex: u().string
-        }, Hl.defaultProps = {
+        }, Fl.defaultProps = {
             n_blur: 0,
             n_blur_timestamp: -1,
             n_submit: 0,
             n_submit_timestamp: -1,
             debounce: !1,
             persisted_props: ["value"],
             persistence_type: "local",
             step: "any"
         };
-        const Ul = Hl,
-            Wl = i.forwardRef((({
+        const Bl = Fl,
+            zl = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "span",
                 ...r
             }, a) => (t = E(t, "input-group-text"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        Wl.displayName = "InputGroupText";
-        const ql = Wl,
-            Vl = i.forwardRef((({
+        zl.displayName = "InputGroupText";
+        const Kl = zl,
+            Hl = i.forwardRef((({
                 bsPrefix: e,
                 size: t,
                 hasValidation: n,
                 className: r,
                 as: a = "div",
                 ...s
             }, o) => {
                 e = E(e, "input-group");
                 const l = (0, i.useMemo)((() => ({})), []);
-                return (0, _.jsx)(ti.Provider, {
+                return (0, _.jsx)(Jo.Provider, {
                     value: l,
                     children: (0, _.jsx)(a, {
                         ref: o,
                         ...s,
                         className: b()(r, e, t && `${e}-${t}`, n && "has-validation")
                     })
                 })
             }));
-        Vl.displayName = "InputGroup";
-        const Gl = Object.assign(Vl, {
-            Text: ql,
-            Radio: e => (0, _.jsx)(ql, {
-                children: (0, _.jsx)(Yi, {
+        Hl.displayName = "InputGroup";
+        const Wl = Object.assign(Hl, {
+            Text: Kl,
+            Radio: e => (0, _.jsx)(Kl, {
+                children: (0, _.jsx)(Ui, {
                     type: "radio",
                     ...e
                 })
             }),
-            Checkbox: e => (0, _.jsx)(ql, {
-                children: (0, _.jsx)(Yi, {
+            Checkbox: e => (0, _.jsx)(Kl, {
+                children: (0, _.jsx)(Ui, {
                     type: "checkbox",
                     ...e
                 })
             })
         });
-        var Yl = ["children", "loading_state", "className", "class_name"],
-            Xl = function(t) {
+        var Ul = ["children", "loading_state", "className", "class_name"],
+            ql = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Yl);
-                return l().createElement(Gl, e({
+                    i = o(t, Ul);
+                return l().createElement(Wl, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Xl.propTypes = {
+        ql.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             size: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Jl = Xl;
-        var Ql = ["children", "loading_state", "className", "class_name"],
-            Zl = function(t) {
+        const Vl = ql;
+        var Gl = ["children", "loading_state", "className", "class_name"],
+            Yl = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Ql);
-                return l().createElement(Gl.Text, e({
+                    i = o(t, Gl);
+                return l().createElement(Wl.Text, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Zl.propTypes = {
+        Yl.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             key: u().string,
             class_name: u().string,
             className: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const ec = Zl;
-        var tc = ["children", "html_for", "width", "xs", "sm", "md", "lg", "xl", "xxl", "align", "size", "className", "class_name", "color", "style", "loading_state", "check"];
+        const Xl = Yl;
+        var Jl = ["children", "html_for", "width", "xs", "sm", "md", "lg", "xl", "xxl", "align", "size", "className", "class_name", "color", "style", "loading_state", "check"];
 
-        function nc(e, t) {
+        function Ql(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function rc(e) {
+        function Zl(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? nc(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : nc(Object(n)).forEach((function(t) {
+                t % 2 ? Ql(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ql(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var ac = {
+        var ec = {
                 start: "align-self-start",
                 center: "align-self-center",
                 end: "align-self-end"
             },
-            sc = ["width", "xs", "sm", "md", "lg", "xl", "xxl"],
-            oc = function(t) {
+            tc = ["width", "xs", "sm", "md", "lg", "xl", "xxl"],
+            nc = function(t) {
                 var n = t.children,
                     r = t.html_for,
                     a = t.width,
                     s = t.xs,
                     i = t.sm,
                     c = t.md,
                     u = t.lg,
@@ -7545,152 +7488,152 @@
                     g = t.size,
                     y = t.className,
                     h = t.class_name,
                     v = t.color,
                     _ = t.style,
                     x = t.loading_state,
                     O = t.check,
-                    w = o(t, tc),
-                    N = wt.has(v),
-                    E = sc.filter((function(e) {
+                    w = o(t, Jl),
+                    N = xt.has(v),
+                    E = tc.filter((function(e) {
                         return t[e]
                     }));
                 [a, s, i, c, u, d, p].forEach((function(e) {
                     "object" === Te(e) && null !== e && (e.span = e.size)
                 }));
-                var j = f && ac[f],
+                var j = f && ec[f],
                     k = b()(h || y, E.length && j, v && N && "text-".concat(v), O && "form-check-label");
-                return l().createElement(il, e({
+                return l().createElement(rl, e({
                     htmlFor: r,
                     column: g || E.length > 0,
                     xs: s || a,
                     sm: i,
                     md: c,
                     lg: u,
                     xl: d,
                     xxl: p,
                     className: k,
-                    style: N ? _ : rc({
+                    style: N ? _ : Zl({
                         color: v
                     }, _)
                 }, m(["setProps"], w), {
                     "data-dash-is-loading": x && x.is_loading || void 0
                 }), n)
             },
-            ic = u().oneOfType([u().number, u().string]),
-            lc = u().oneOfType([u().string, u().number, u().shape({
-                size: ic,
-                order: ic,
-                offset: ic
+            rc = u().oneOfType([u().number, u().string]),
+            ac = u().oneOfType([u().string, u().number, u().shape({
+                size: rc,
+                order: rc,
+                offset: rc
             })]);
-        oc.propTypes = {
+        nc.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             hidden: u().bool,
             size: u().string,
             html_for: u().string,
             check: u().bool,
-            width: lc,
-            xs: lc,
-            sm: lc,
-            md: lc,
-            lg: lc,
-            xl: lc,
+            width: ac,
+            xs: ac,
+            sm: ac,
+            md: ac,
+            lg: ac,
+            xl: ac,
             align: u().oneOf(["start", "center", "end"]),
             color: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
-        }, oc.defaultProps = {
+        }, nc.defaultProps = {
             align: "center"
         };
-        const cc = oc,
-            uc = i.forwardRef((({
+        const sc = nc,
+            oc = i.forwardRef((({
                 bsPrefix: e,
                 active: t,
                 disabled: n,
                 eventKey: r,
                 className: a,
                 variant: s,
                 action: o,
                 as: i,
                 ...l
             }, c) => {
                 e = E(e, "list-group-item");
-                const [u, d] = mi({
-                    key: Co(r, l.href),
+                const [u, d] = ui({
+                    key: Eo(r, l.href),
                     active: t,
                     ...l
-                }), p = Ye((e => {
+                }), p = Ve((e => {
                     if (n) return e.preventDefault(), void e.stopPropagation();
                     u.onClick(e)
                 }));
                 n && void 0 === l.tabIndex && (l.tabIndex = -1, l["aria-disabled"] = !0);
                 const f = i || (o ? l.href ? "a" : "button" : "div");
                 return (0, _.jsx)(f, {
                     ref: c,
                     ...l,
                     ...u,
                     onClick: p,
                     className: b()(a, e, d.isActive && "active", n && "disabled", s && `${e}-${s}`, o && `${e}-action`)
                 })
             }));
-        uc.displayName = "ListGroupItem";
-        const dc = uc,
-            pc = i.forwardRef(((e, t) => {
+        oc.displayName = "ListGroupItem";
+        const ic = oc,
+            lc = i.forwardRef(((e, t) => {
                 const {
                     className: n,
                     bsPrefix: r,
                     variant: a,
                     horizontal: s,
                     numbered: o,
                     as: i = "div",
                     ...l
                 } = v(e, {
                     activeKey: "onSelect"
                 }), c = E(r, "list-group");
                 let u;
-                return s && (u = !0 === s ? "horizontal" : `horizontal-${s}`), (0, _.jsx)(xi, {
+                return s && (u = !0 === s ? "horizontal" : `horizontal-${s}`), (0, _.jsx)(yi, {
                     ref: t,
                     ...l,
                     as: i,
                     className: b()(n, c, a && `${c}-${a}`, u && `${c}-${u}`, o && `${c}-numbered`)
                 })
             }));
-        pc.displayName = "ListGroup";
-        const fc = Object.assign(pc, {
-            Item: dc
+        lc.displayName = "ListGroup";
+        const cc = Object.assign(lc, {
+            Item: ic
         });
-        var mc = ["children", "loading_state", "className", "class_name", "flush", "tag"],
-            gc = function(t) {
+        var uc = ["children", "loading_state", "className", "class_name", "flush", "tag"],
+            dc = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.flush,
                     c = t.tag,
-                    u = o(t, mc);
-                return l().createElement(fc, e({
+                    u = o(t, uc);
+                return l().createElement(cc, e({
                     className: s || a,
                     variant: i ? "flush" : null,
                     as: c
                 }, m(["setProps"], u), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        gc.defaultProps = {
+        dc.defaultProps = {
             tag: "ul",
             numbered: !1
-        }, gc.propTypes = {
+        }, dc.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
@@ -7699,78 +7642,77 @@
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             horizontal: u().oneOfType([u().bool, u().string]),
             numbered: u().bool
         };
-        const bc = gc;
-        var yc = ["children", "disabled", "href", "loading_state", "target", "n_clicks", "setProps", "color", "style", "className", "class_name"];
+        const pc = dc;
+        var fc = ["children", "disabled", "href", "loading_state", "target", "n_clicks", "setProps", "color", "style", "className", "class_name"];
 
-        function hc(e, t) {
+        function mc(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function vc(e) {
+        function gc(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? hc(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : hc(Object(n)).forEach((function(t) {
+                t % 2 ? mc(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : mc(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var _c = function(t) {
+        var bc = function(t) {
             var n = t.children,
                 r = t.disabled,
                 a = t.href,
                 s = t.loading_state,
                 i = t.target,
                 c = t.n_clicks,
                 u = t.setProps,
                 d = t.color,
                 p = t.style,
                 f = t.className,
                 g = t.class_name,
-                b = o(t, yc),
-                y = Fe(a, u),
-                h = Ot.has(d),
-                v = y && !r;
-            return b[v ? "preOnClick" : "onClick"] = function() {
+                b = o(t, fc),
+                y = _t.has(d),
+                h = a && !r;
+            return b[h ? "preOnClick" : "onClick"] = function() {
                 !r && u && u({
                     n_clicks: c + 1,
                     n_clicks_timestamp: Date.now()
                 })
-            }, l().createElement(dc, e({
-                as: v ? Bt : "li",
-                href: y,
-                target: v ? i : void 0,
+            }, l().createElement(ic, e({
+                as: h ? Mt : "li",
+                href: a,
+                target: h ? i : void 0,
                 disabled: r,
-                variant: h ? d : null,
-                style: h ? p : vc({
+                variant: y ? d : null,
+                style: y ? p : gc({
                     backgroundColor: d
                 }, p),
                 className: g || f
             }, m(["n_clicks_timestamp"], b), {
                 "data-dash-is-loading": s && s.is_loading || void 0
             }), n)
         };
-        _c.defaultProps = {
+        bc.defaultProps = {
             n_clicks: 0,
             n_clicks_timestamp: -1
-        }, _c.propTypes = {
+        }, bc.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
@@ -7785,36 +7727,36 @@
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             target: u().string
         };
-        const xc = _c;
-        var Oc;
+        const yc = bc;
+        var hc;
 
-        function wc(e) {
-            if ((!Oc && 0 !== Oc || e) && V) {
+        function vc(e) {
+            if ((!hc && 0 !== hc || e) && V) {
                 var t = document.createElement("div");
-                t.style.position = "absolute", t.style.top = "-9999px", t.style.width = "50px", t.style.height = "50px", t.style.overflow = "scroll", document.body.appendChild(t), Oc = t.offsetWidth - t.clientWidth, document.body.removeChild(t)
+                t.style.position = "absolute", t.style.top = "-9999px", t.style.width = "50px", t.style.height = "50px", t.style.overflow = "scroll", document.body.appendChild(t), hc = t.offsetWidth - t.clientWidth, document.body.removeChild(t)
             }
-            return Oc
+            return hc
         }
 
-        function Nc(e) {
+        function _c(e) {
             void 0 === e && (e = C());
             try {
                 var t = e.activeElement;
                 return t && t.nodeName ? t : null
             } catch (t) {
                 return e.body
             }
         }
-        const Ec = Lo("modal-open"),
-            jc = class {
+        const xc = To("modal-open"),
+            Oc = class {
                 constructor({
                     ownerDocument: e,
                     handleContainerOverflow: t = !0,
                     isRTL: n = !1
                 } = {}) {
                     this.handleContainerOverflow = t, this.isRTL = n, this.modals = [], this.ownerDocument = e
                 }
@@ -7834,22 +7776,22 @@
                             overflow: "hidden"
                         },
                         n = this.isRTL ? "paddingLeft" : "paddingRight",
                         r = this.getElement();
                     e.style = {
                         overflow: r.style.overflow,
                         [n]: r.style[n]
-                    }, e.scrollBarWidth && (t[n] = `${parseInt(L(r,n)||"0",10)+e.scrollBarWidth}px`), r.setAttribute(Ec, ""), L(r, t)
+                    }, e.scrollBarWidth && (t[n] = `${parseInt(L(r,n)||"0",10)+e.scrollBarWidth}px`), r.setAttribute(xc, ""), L(r, t)
                 }
                 reset() {
                     [...this.modals].forEach((e => this.remove(e)))
                 }
                 removeContainerStyle(e) {
                     const t = this.getElement();
-                    t.removeAttribute(Ec), Object.assign(t.style, e.style)
+                    t.removeAttribute(xc), Object.assign(t.style, e.style)
                 }
                 add(e) {
                     let t = this.modals.indexOf(e);
                     return -1 !== t || (t = this.modals.length, this.modals.push(e), this.setModalAttributes(e), 0 !== t || (this.state = {
                         scrollBarWidth: this.getScrollbarWidth(),
                         style: {}
                     }, this.handleContainerOverflow && this.setContainerStyle(this.state))), t
@@ -7857,52 +7799,52 @@
                 remove(e) {
                     const t = this.modals.indexOf(e); - 1 !== t && (this.modals.splice(t, 1), !this.modals.length && this.handleContainerOverflow && this.removeContainerStyle(this.state), this.removeModalAttributes(e))
                 }
                 isTopModal(e) {
                     return !!this.modals.length && this.modals[this.modals.length - 1] === e
                 }
             },
-            kc = (e, t) => V ? null == e ? (t || C()).body : ("function" == typeof e && (e = e()), e && "current" in e && (e = e.current), e && ("nodeType" in e || e.getBoundingClientRect) ? e : null) : null;
+            wc = (e, t) => V ? null == e ? (t || C()).body : ("function" == typeof e && (e = e()), e && "current" in e && (e = e.current), e && ("nodeType" in e || e.getBoundingClientRect) ? e : null) : null;
 
-        function Pc(e, t) {
-            const n = Bo(),
-                [r, a] = (0, i.useState)((() => kc(e, null == n ? void 0 : n.document)));
+        function Nc(e, t) {
+            const n = $o(),
+                [r, a] = (0, i.useState)((() => wc(e, null == n ? void 0 : n.document)));
             if (!r) {
-                const t = kc(e);
+                const t = wc(e);
                 t && a(t)
             }
             return (0, i.useEffect)((() => {
                 t && r && t(r)
             }), [t, r]), (0, i.useEffect)((() => {
-                const t = kc(e);
+                const t = wc(e);
                 t !== r && a(t)
             }), [e, r]), r
         }
-        const Cc = function({
+        const Ec = function({
                 children: e,
                 in: t,
                 onExited: n,
                 mountOnEnter: r,
                 unmountOnExit: a
             }) {
                 const s = (0, i.useRef)(null),
                     o = (0, i.useRef)(t),
-                    l = Ye(n);
+                    l = Ve(n);
                 (0, i.useEffect)((() => {
                     t ? o.current = !0 : l(s.current)
                 }), [t, l]);
                 const c = oe(s, e.ref),
                     u = (0, i.cloneElement)(e, {
                         ref: c
                     });
                 return t ? u : a || !o.current && r ? null : u
             },
-            Tc = ["onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited", "addEndListener", "children"];
-        const Sc = ["component"],
-            Rc = i.forwardRef(((e, t) => {
+            jc = ["onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited", "addEndListener", "children"];
+        const kc = ["component"],
+            Pc = i.forwardRef(((e, t) => {
                 let {
                     component: n
                 } = e;
                 const r = function(e) {
                     let {
                         onEnter: t,
                         onEntering: n,
@@ -7914,15 +7856,15 @@
                         children: c
                     } = e, u = function(e, t) {
                         if (null == e) return {};
                         var n, r, a = {},
                             s = Object.keys(e);
                         for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                         return a
-                    }(e, Tc);
+                    }(e, jc);
                     const d = (0, i.useRef)(null),
                         p = oe(d, "function" == typeof c ? null : c.ref),
                         f = e => t => {
                             e && d.current && e(d.current, t)
                         },
                         m = (0, i.useCallback)(f(t), [t]),
                         g = (0, i.useCallback)(f(n), [n]),
@@ -7956,48 +7898,48 @@
                     })
                 }(function(e, t) {
                     if (null == e) return {};
                     var n, r, a = {},
                         s = Object.keys(e);
                     for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                     return a
-                }(e, Sc));
+                }(e, kc));
                 return (0, _.jsx)(n, Object.assign({
                     ref: t
                 }, r))
             }));
 
-        function Dc({
+        function Cc({
             children: e,
             in: t,
             onExited: n,
             onEntered: r,
             transition: a
         }) {
             const [s, o] = (0, i.useState)(!t);
             t && s && o(!1);
             const l = function({
                     in: e,
                     onTransition: t
                 }) {
                     const n = (0, i.useRef)(null),
                         r = (0, i.useRef)(!0),
-                        a = Ye(t);
-                    return at((() => {
+                        a = Ve(t);
+                    return nt((() => {
                         if (!n.current) return;
                         let t = !1;
                         return a({
                             in: e,
                             element: n.current,
                             initial: r.current,
                             isStale: () => t
                         }), () => {
                             t = !0
                         }
-                    }), [e, a]), at((() => (r.current = !1, () => {
+                    }), [e, a]), nt((() => (r.current = !1, () => {
                         r.current = !0
                     })), []), n
                 }({
                     in: !!t,
                     onTransition: e => {
                         Promise.resolve(a(e)).then((() => {
                             e.isStale() || (e.in ? null == r || r(e.element, e.initial) : (o(!0), null == n || n(e.element)))
@@ -8008,28 +7950,28 @@
                 }),
                 c = oe(l, e.ref);
             return s && !t ? null : (0, i.cloneElement)(e, {
                 ref: c
             })
         }
 
-        function Lc(e, t, n) {
-            return e ? (0, _.jsx)(Rc, Object.assign({}, n, {
+        function Tc(e, t, n) {
+            return e ? (0, _.jsx)(Pc, Object.assign({}, n, {
                 component: e
-            })) : t ? (0, _.jsx)(Dc, Object.assign({}, n, {
+            })) : t ? (0, _.jsx)(Cc, Object.assign({}, n, {
                 transition: t
-            })) : (0, _.jsx)(Cc, Object.assign({}, n))
+            })) : (0, _.jsx)(Ec, Object.assign({}, n))
         }
 
-        function $c(e) {
+        function Sc(e) {
             return "Escape" === e.code || 27 === e.keyCode
         }
-        const Ic = ["show", "role", "className", "style", "children", "backdrop", "keyboard", "onBackdropClick", "onEscapeKeyDown", "transition", "runTransition", "backdropTransition", "runBackdropTransition", "autoFocus", "enforceFocus", "restoreFocus", "restoreFocusOptions", "renderDialog", "renderBackdrop", "manager", "container", "onShow", "onHide", "onExit", "onExited", "onExiting", "onEnter", "onEntering", "onEntered"];
-        let Ac;
-        const Fc = (0, i.forwardRef)(((e, t) => {
+        const Rc = ["show", "role", "className", "style", "children", "backdrop", "keyboard", "onBackdropClick", "onEscapeKeyDown", "transition", "runTransition", "backdropTransition", "runBackdropTransition", "autoFocus", "enforceFocus", "restoreFocus", "restoreFocusOptions", "renderDialog", "renderBackdrop", "manager", "container", "onShow", "onHide", "onExit", "onExited", "onExiting", "onEnter", "onEntering", "onEntered"];
+        let Dc;
+        const Lc = (0, i.forwardRef)(((e, t) => {
             let {
                 show: n = !1,
                 role: r = "dialog",
                 className: a,
                 style: s,
                 children: o,
                 backdrop: l = !0,
@@ -8058,23 +8000,23 @@
                 onEntered: R
             } = e, D = function(e, t) {
                 if (null == e) return {};
                 var n, r, a = {},
                     s = Object.keys(e);
                 for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                 return a
-            }(e, Ic);
-            const L = Bo(),
-                $ = Pc(N),
-                I = function(e) {
-                    const t = Bo(),
+            }(e, Rc);
+            const L = $o(),
+                I = Nc(N),
+                $ = function(e) {
+                    const t = $o(),
                         n = e || function(e) {
-                            return Ac || (Ac = new jc({
+                            return Dc || (Dc = new Oc({
                                 ownerDocument: null == e ? void 0 : e.document
-                            })), Ac
+                            })), Dc
                         }(t),
                         r = (0, i.useRef)({
                             dialog: null,
                             backdrop: null
                         });
                     return Object.assign(r.current, {
                         add: () => n.add(r.current),
@@ -8084,66 +8026,66 @@
                             r.current.dialog = e
                         }), []),
                         setBackdropRef: (0, i.useCallback)((e => {
                             r.current.backdrop = e
                         }), [])
                     })
                 }(w),
-                F = tt(),
-                M = nt(n),
+                M = Ze(),
+                F = et(n),
                 [B, z] = (0, i.useState)(!n),
                 K = (0, i.useRef)(null);
-            (0, i.useImperativeHandle)(t, (() => I), [I]), V && !M && n && (K.current = Nc(null == L ? void 0 : L.document)), n && B && z(!1);
-            const H = Ye((() => {
-                    if (I.add(), X.current = Z(document, "keydown", G), Y.current = Z(document, "focus", (() => setTimeout(W)), !0), E && E(), b) {
+            (0, i.useImperativeHandle)(t, (() => $), [$]), V && !F && n && (K.current = _c(null == L ? void 0 : L.document)), n && B && z(!1);
+            const H = Ve((() => {
+                    if ($.add(), X.current = Z(document, "keydown", G), Y.current = Z(document, "focus", (() => setTimeout(U)), !0), E && E(), b) {
                         var e, t;
-                        const n = Nc(null != (e = null == (t = I.dialog) ? void 0 : t.ownerDocument) ? e : null == L ? void 0 : L.document);
-                        I.dialog && n && !eo(I.dialog, n) && (K.current = n, I.dialog.focus())
+                        const n = _c(null != (e = null == (t = $.dialog) ? void 0 : t.ownerDocument) ? e : null == L ? void 0 : L.document);
+                        $.dialog && n && !Xs($.dialog, n) && (K.current = n, $.dialog.focus())
                     }
                 })),
-                U = Ye((() => {
+                W = Ve((() => {
                     var e;
-                    I.remove(), null == X.current || X.current(), null == Y.current || Y.current(), h && (null == (e = K.current) || null == e.focus || e.focus(v), K.current = null)
+                    $.remove(), null == X.current || X.current(), null == Y.current || Y.current(), h && (null == (e = K.current) || null == e.focus || e.focus(v), K.current = null)
                 }));
             (0, i.useEffect)((() => {
-                n && $ && H()
-            }), [n, $, H]), (0, i.useEffect)((() => {
-                B && U()
-            }), [B, U]), ur((() => {
-                U()
-            }));
-            const W = Ye((() => {
-                    if (!y || !F() || !I.isTopModal()) return;
-                    const e = Nc(null == L ? void 0 : L.document);
-                    I.dialog && e && !eo(I.dialog, e) && I.dialog.focus()
+                n && I && H()
+            }), [n, I, H]), (0, i.useEffect)((() => {
+                B && W()
+            }), [B, W]), or((() => {
+                W()
+            }));
+            const U = Ve((() => {
+                    if (!y || !M() || !$.isTopModal()) return;
+                    const e = _c(null == L ? void 0 : L.document);
+                    $.dialog && e && !Xs($.dialog, e) && $.dialog.focus()
                 })),
-                q = Ye((e => {
+                q = Ve((e => {
                     e.target === e.currentTarget && (null == u || u(e), !0 === l && j())
                 })),
-                G = Ye((e => {
-                    c && $c(e) && I.isTopModal() && (null == d || d(e), e.defaultPrevented || j())
+                G = Ve((e => {
+                    c && Sc(e) && $.isTopModal() && (null == d || d(e), e.defaultPrevented || j())
                 })),
                 Y = (0, i.useRef)(),
                 X = (0, i.useRef)();
-            if (!$) return null;
+            if (!I) return null;
             const J = Object.assign({
                 role: r,
-                ref: I.setDialogRef,
+                ref: $.setDialogRef,
                 "aria-modal": "dialog" === r || void 0
             }, D, {
                 style: s,
                 className: a,
                 tabIndex: -1
             });
             let Q = x ? x(J) : (0, _.jsx)("div", Object.assign({}, J, {
                 children: i.cloneElement(o, {
                     role: "document"
                 })
             }));
-            Q = Lc(p, f, {
+            Q = Tc(p, f, {
                 unmountOnExit: !0,
                 mountOnEnter: !0,
                 appear: !0,
                 in: !!n,
                 onExit: k,
                 onExiting: C,
                 onExited: (...e) => {
@@ -8152,44 +8094,44 @@
                 onEnter: T,
                 onEntering: S,
                 onEntered: R,
                 children: Q
             });
             let ee = null;
             return l && (ee = O({
-                ref: I.setBackdropRef,
+                ref: $.setBackdropRef,
                 onClick: q
-            }), ee = Lc(m, g, {
+            }), ee = Tc(m, g, {
                 in: !!n,
                 appear: !0,
                 mountOnEnter: !0,
                 unmountOnExit: !0,
                 children: ee
             })), (0, _.jsx)(_.Fragment, {
                 children: A().createPortal((0, _.jsxs)(_.Fragment, {
                     children: [ee, Q]
-                }), $)
+                }), I)
             })
         }));
-        Fc.displayName = "Modal";
-        const Mc = Object.assign(Fc, {
-            Manager: jc
+        Lc.displayName = "Modal";
+        const Ic = Object.assign(Lc, {
+            Manager: Oc
         });
 
-        function Bc(e, t) {
+        function $c(e, t) {
             return e.classList ? !!t && e.classList.contains(t) : -1 !== (" " + (e.className.baseVal || e.className) + " ").indexOf(" " + t + " ")
         }
 
-        function zc(e, t) {
+        function Ac(e, t) {
             return e.replace(new RegExp("(^|\\s)" + t + "(?:\\s|$)", "g"), "$1").replace(/\s+/g, " ").replace(/^\s*|\s*$/g, "")
         }
-        const Kc = ".fixed-top, .fixed-bottom, .is-fixed, .sticky-top",
-            Hc = ".sticky-top",
-            Uc = ".navbar-toggler";
-        class Wc extends jc {
+        const Mc = ".fixed-top, .fixed-bottom, .is-fixed, .sticky-top",
+            Fc = ".sticky-top",
+            Bc = ".navbar-toggler";
+        class zc extends Oc {
             adjustAndStore(e, t, n) {
                 const r = t.style[e];
                 t.dataset[e] = r, L(t, {
                     [e]: `${parseFloat(L(t,e))+n}px`
                 })
             }
             restore(e, t) {
@@ -8198,293 +8140,298 @@
                     [e]: n
                 }))
             }
             setContainerStyle(e) {
                 super.setContainerStyle(e);
                 const t = this.getElement();
                 var n, r;
-                if (r = "modal-open", (n = t).classList ? n.classList.add(r) : Bc(n, r) || ("string" == typeof n.className ? n.className = n.className + " " + r : n.setAttribute("class", (n.className && n.className.baseVal || "") + " " + r)), !e.scrollBarWidth) return;
+                if (r = "modal-open", (n = t).classList ? n.classList.add(r) : $c(n, r) || ("string" == typeof n.className ? n.className = n.className + " " + r : n.setAttribute("class", (n.className && n.className.baseVal || "") + " " + r)), !e.scrollBarWidth) return;
                 const a = this.isRTL ? "paddingLeft" : "paddingRight",
                     s = this.isRTL ? "marginLeft" : "marginRight";
-                Ca(t, Kc).forEach((t => this.adjustAndStore(a, t, e.scrollBarWidth))), Ca(t, Hc).forEach((t => this.adjustAndStore(s, t, -e.scrollBarWidth))), Ca(t, Uc).forEach((t => this.adjustAndStore(s, t, e.scrollBarWidth)))
+                Ea(t, Mc).forEach((t => this.adjustAndStore(a, t, e.scrollBarWidth))), Ea(t, Fc).forEach((t => this.adjustAndStore(s, t, -e.scrollBarWidth))), Ea(t, Bc).forEach((t => this.adjustAndStore(s, t, e.scrollBarWidth)))
             }
             removeContainerStyle(e) {
                 super.removeContainerStyle(e);
                 const t = this.getElement();
                 var n, r;
-                r = "modal-open", (n = t).classList ? n.classList.remove(r) : "string" == typeof n.className ? n.className = zc(n.className, r) : n.setAttribute("class", zc(n.className && n.className.baseVal || "", r));
+                r = "modal-open", (n = t).classList ? n.classList.remove(r) : "string" == typeof n.className ? n.className = Ac(n.className, r) : n.setAttribute("class", Ac(n.className && n.className.baseVal || "", r));
                 const a = this.isRTL ? "paddingLeft" : "paddingRight",
                     s = this.isRTL ? "marginLeft" : "marginRight";
-                Ca(t, Kc).forEach((e => this.restore(a, e))), Ca(t, Hc).forEach((e => this.restore(s, e))), Ca(t, Uc).forEach((e => this.restore(s, e)))
+                Ea(t, Mc).forEach((e => this.restore(a, e))), Ea(t, Fc).forEach((e => this.restore(s, e))), Ea(t, Bc).forEach((e => this.restore(s, e)))
             }
         }
-        let qc;
+        let Kc;
 
-        function Vc(e) {
-            return qc || (qc = new Wc(e)), qc
+        function Hc(e) {
+            return Kc || (Kc = new zc(e)), Kc
         }
-        const Gc = Wc,
-            Yc = i.createContext({
+        const Wc = zc,
+            Uc = i.createContext({
                 onHide() {}
-            }),
-            Xc = i.forwardRef((({
-                bsPrefix: e,
-                className: t,
-                contentClassName: n,
-                centered: r,
-                size: a,
-                fullscreen: s,
-                children: o,
-                scrollable: i,
-                ...l
-            }, c) => {
-                const u = `${e=E(e,"modal")}-dialog`,
-                    d = "string" == typeof s ? `${e}-fullscreen-${s}` : `${e}-fullscreen`;
-                return (0, _.jsx)("div", {
-                    ...l,
-                    ref: c,
-                    className: b()(u, t, a && `${e}-${a}`, r && `${u}-centered`, i && `${u}-scrollable`, s && d),
-                    children: (0, _.jsx)("div", {
-                        className: b()(`${e}-content`, n),
-                        children: o
-                    })
-                })
-            }));
-        Xc.displayName = "ModalDialog";
-        var Jc = ["bsPrefix", "className", "style", "dialogClassName", "contentClassName", "children", "dialogAs", "aria-labelledby", "aria-describedby", "aria-label", "show", "animation", "backdrop", "keyboard", "onEscapeKeyDown", "onShow", "onHide", "container", "autoFocus", "enforceFocus", "restoreFocus", "restoreFocusOptions", "onEntered", "onExit", "onExiting", "onEnter", "onEntering", "onExited", "backdropClassName", "zIndex", "manager"];
+            });
+        var qc = ["bsPrefix", "className", "contentClassName", "centered", "size", "fullscreen", "children", "scrollable", "contentStyle"],
+            Vc = l().forwardRef((function(t, n) {
+                var r = t.bsPrefix,
+                    a = t.className,
+                    s = t.contentClassName,
+                    i = t.centered,
+                    c = t.size,
+                    u = t.fullscreen,
+                    d = t.children,
+                    p = t.scrollable,
+                    f = t.contentStyle,
+                    m = o(t, qc);
+                r = E(r, "modal");
+                var g = "".concat(r, "-dialog"),
+                    y = "string" == typeof u ? "".concat(r, "-fullscreen-").concat(u) : "".concat(r, "-fullscreen");
+                return l().createElement("div", e({}, m, {
+                    ref: n,
+                    className: b()(g, a, c && "".concat(r, "-").concat(c), i && "".concat(g, "-centered"), p && "".concat(g, "-scrollable"), u && y)
+                }), l().createElement("div", {
+                    className: b()("".concat(r, "-content"), s),
+                    style: f
+                }, d))
+            })),
+            Gc = ["bsPrefix", "className", "style", "dialogClassName", "contentClassName", "children", "dialogStyle", "contentStyle", "dialogAs", "data-bs-theme", "aria-labelledby", "aria-describedby", "aria-label", "show", "animation", "backdrop", "keyboard", "onEscapeKeyDown", "onShow", "onHide", "container", "autoFocus", "enforceFocus", "restoreFocus", "restoreFocusOptions", "onEntered", "onExit", "onExiting", "onEnter", "onEntering", "onExited", "backdropClassName", "zIndex", "manager"];
 
-        function Qc(e, t) {
+        function Yc(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Zc(e) {
+        function Xc(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Qc(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Qc(Object(n)).forEach((function(t) {
+                t % 2 ? Yc(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Yc(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var eu = {
+        var Jc = {
             show: !1,
             backdrop: !0,
             keyboard: !0,
             autoFocus: !0,
             enforceFocus: !0,
             restoreFocus: !0,
             animation: !0,
-            dialogAs: Xc
+            dialogAs: Vc
         };
 
-        function tu(t) {
-            return l().createElement(bt, e({}, t, {
+        function Qc(t) {
+            return l().createElement(mt, e({}, t, {
                 timeout: null
             }))
         }
 
-        function nu(t) {
-            return l().createElement(bt, e({}, t, {
+        function Zc(t) {
+            return l().createElement(mt, e({}, t, {
                 timeout: null
             }))
         }
-        var ru = l().forwardRef((function(t, n) {
+        var eu = l().forwardRef((function(t, n) {
             var r = t.bsPrefix,
                 a = t.className,
                 s = t.style,
                 c = t.dialogClassName,
                 u = t.contentClassName,
                 d = t.children,
-                p = t.dialogAs,
-                f = t["aria-labelledby"],
-                m = t["aria-describedby"],
-                g = t["aria-label"],
-                y = t.show,
-                h = t.animation,
-                v = t.backdrop,
-                _ = t.keyboard,
-                x = t.onEscapeKeyDown,
-                O = t.onShow,
-                w = t.onHide,
-                N = t.container,
-                j = t.autoFocus,
-                k = t.enforceFocus,
-                T = t.restoreFocus,
-                S = t.restoreFocusOptions,
-                R = t.onEntered,
-                D = t.onExit,
-                L = t.onExiting,
-                $ = t.onEnter,
-                I = t.onEntering,
-                A = t.onExited,
-                F = t.backdropClassName,
-                M = t.zIndex,
-                B = t.manager,
-                z = o(t, Jc),
-                K = Se((0, i.useState)({}), 2),
-                H = K[0],
-                U = K[1],
-                W = Se((0, i.useState)(!1), 2),
-                q = W[0],
-                G = W[1],
-                Y = (0, i.useRef)(!1),
-                X = (0, i.useRef)(!1),
-                Z = (0, i.useRef)(null),
-                te = Se(et(), 2),
-                ne = te[0],
-                re = te[1],
-                ae = oe(n, re),
-                se = Ye(w),
-                ie = P();
+                p = t.dialogStyle,
+                f = t.contentStyle,
+                m = t.dialogAs,
+                g = t["data-bs-theme"],
+                y = t["aria-labelledby"],
+                h = t["aria-describedby"],
+                v = t["aria-label"],
+                _ = t.show,
+                x = t.animation,
+                O = t.backdrop,
+                w = t.keyboard,
+                N = t.onEscapeKeyDown,
+                j = t.onShow,
+                k = t.onHide,
+                T = t.container,
+                S = t.autoFocus,
+                R = t.enforceFocus,
+                D = t.restoreFocus,
+                L = t.restoreFocusOptions,
+                I = t.onEntered,
+                $ = t.onExit,
+                A = t.onExiting,
+                M = t.onEnter,
+                F = t.onEntering,
+                B = t.onExited,
+                z = t.backdropClassName,
+                K = t.zIndex,
+                H = t.manager,
+                W = o(t, Gc),
+                U = Se((0, i.useState)({}), 2),
+                q = U[0],
+                G = U[1],
+                Y = Se((0, i.useState)(!1), 2),
+                X = Y[0],
+                Z = Y[1],
+                te = (0, i.useRef)(!1),
+                ne = (0, i.useRef)(!1),
+                re = (0, i.useRef)(null),
+                ae = Se(Qe(), 2),
+                se = ae[0],
+                ie = ae[1],
+                le = oe(n, ie),
+                ce = Ve(k),
+                ue = P();
             r = E(r, "modal");
-            var le = (0, i.useMemo)((function() {
+            var de = (0, i.useMemo)((function() {
                 return {
-                    onHide: se
+                    onHide: ce
                 }
-            }), [se]);
+            }), [ce]);
 
-            function ce() {
-                return B || Vc({
-                    isRTL: ie
+            function pe() {
+                return H || Hc({
+                    isRTL: ue
                 })
             }
 
-            function ue(e) {
+            function fe(e) {
                 if (V) {
-                    var t = ce().getScrollbarWidth() > 0,
+                    var t = pe().getScrollbarWidth() > 0,
                         n = e.scrollHeight > C(e).documentElement.clientHeight;
-                    U({
-                        paddingRight: t && !n ? wc() : void 0,
-                        paddingLeft: !t && n ? wc() : void 0
+                    G({
+                        paddingRight: t && !n ? vc() : void 0,
+                        paddingLeft: !t && n ? vc() : void 0
                     })
                 }
             }
-            var de = Ye((function() {
-                ne && ue(ne.dialog)
+            var me = Ve((function() {
+                se && fe(se.dialog)
             }));
-            ur((function() {
+            or((function() {
                 var e;
-                Q(window, "resize", de), null === (e = Z.current) || void 0 === e || e.call(Z)
+                Q(window, "resize", me), null === (e = re.current) || void 0 === e || e.call(re)
             }));
-            var pe = function() {
-                    Y.current = !0
+            var ge = function() {
+                    te.current = !0
                 },
-                fe = function(e) {
-                    Y.current && ne && e.target === ne.dialog && (X.current = !0), Y.current = !1
+                be = function(e) {
+                    te.current && se && e.target === se.dialog && (ne.current = !0), te.current = !1
                 },
-                me = function() {
-                    G(!0), Z.current = ee(ne.dialog, (function() {
-                        G(!1)
+                ye = function() {
+                    Z(!0), re.current = ee(se.dialog, (function() {
+                        Z(!1)
                     }))
                 },
-                ge = function(e) {
-                    "static" !== v ? X.current || e.target !== e.currentTarget ? X.current = !1 : null == w || w() : function(e) {
-                        e.target === e.currentTarget && me()
+                he = function(e) {
+                    "static" !== O ? ne.current || e.target !== e.currentTarget ? ne.current = !1 : null == k || k() : function(e) {
+                        e.target === e.currentTarget && ye()
                     }(e)
                 },
-                be = (0, i.useCallback)((function(t) {
+                ve = (0, i.useCallback)((function(t) {
                     return l().createElement("div", e({}, t, {
-                        className: b()("".concat(r, "-backdrop"), F, !h && "show"),
+                        className: b()("".concat(r, "-backdrop"), z, !x && "show"),
                         style: {
-                            zIndex: M
+                            zIndex: K
                         }
                     }))
-                }), [h, F, r, M]),
-                ye = Zc(Zc({}, s), H);
-            return ye.display = "block", l().createElement(Yc.Provider, {
-                value: le
-            }, l().createElement(Mc, {
-                show: y,
-                ref: ae,
-                backdrop: v,
-                container: N,
+                }), [x, z, r, K]),
+                _e = Xc(Xc({}, s), q);
+            return _e.display = "block", l().createElement(Uc.Provider, {
+                value: de
+            }, l().createElement(Ic, {
+                show: _,
+                ref: le,
+                backdrop: O,
+                container: T,
                 keyboard: !0,
-                autoFocus: j,
-                enforceFocus: k,
-                restoreFocus: T,
-                restoreFocusOptions: S,
+                autoFocus: S,
+                enforceFocus: R,
+                restoreFocus: D,
+                restoreFocusOptions: L,
                 onEscapeKeyDown: function(e) {
-                    _ || "static" !== v ? _ && x && x(e) : (e.preventDefault(), me())
+                    w ? null == N || N(e) : (e.preventDefault(), "static" === O && ye())
                 },
-                onShow: O,
-                onHide: w,
+                onShow: j,
+                onHide: k,
                 onEnter: function(e, t) {
-                    e && ue(e), null == $ || $(e, t)
+                    e && fe(e), null == M || M(e, t)
                 },
                 onEntering: function(e, t) {
-                    null == I || I(e, t), J(window, "resize", de)
+                    null == F || F(e, t), J(window, "resize", me)
                 },
-                onEntered: R,
+                onEntered: I,
                 onExit: function(e) {
                     var t;
-                    null === (t = Z.current) || void 0 === t || t.call(Z), null == D || D(e)
+                    null === (t = re.current) || void 0 === t || t.call(re), null == $ || $(e)
                 },
-                onExiting: L,
+                onExiting: A,
                 onExited: function(e) {
-                    e && (e.style.display = ""), null == A || A(e), Q(window, "resize", de)
+                    e && (e.style.display = ""), null == B || B(e), Q(window, "resize", me)
                 },
-                manager: ce(),
-                transition: h ? tu : void 0,
-                backdropTransition: h ? nu : void 0,
-                renderBackdrop: be,
+                manager: pe(),
+                transition: x ? Qc : void 0,
+                backdropTransition: x ? Zc : void 0,
+                renderBackdrop: ve,
                 renderDialog: function(t) {
                     return l().createElement("div", e({
                         role: "dialog"
                     }, t, {
-                        style: ye,
-                        className: b()(a, r, q && "".concat(r, "-static")),
-                        onClick: v ? ge : void 0,
-                        onMouseUp: fe,
-                        "aria-label": g,
-                        "aria-labelledby": f,
-                        "aria-describedby": m
-                    }), l().createElement(p, e({}, z, {
-                        onMouseDown: pe,
+                        style: _e,
+                        className: b()(a, r, X && "".concat(r, "-static"), !x && "show"),
+                        onClick: O ? he : void 0,
+                        onMouseUp: be,
+                        "data-bs-theme": g,
+                        "aria-label": v,
+                        "aria-labelledby": y,
+                        "aria-describedby": h
+                    }), l().createElement(m, e({}, W, {
+                        onMouseDown: ge,
                         className: c,
-                        contentClassName: u
+                        contentClassName: u,
+                        style: p,
+                        contentStyle: f
                     }), d))
                 }
             }))
         }));
-        ru.defaultProps = eu;
-        const au = ru;
-        var su = ["children", "is_open", "setProps", "className", "class_name", "autoFocus", "autofocus", "enforceFocus", "labelledBy", "labelledby", "modalClassName", "modal_class_name", "contentClassName", "content_class_name", "backdropClassName", "backdrop_class_name", "tag", "loading_state", "fade", "style", "zindex", "zIndex"];
+        eu.defaultProps = Jc;
+        const tu = eu;
+        var nu = ["children", "is_open", "setProps", "className", "class_name", "autoFocus", "autofocus", "enforceFocus", "labelledBy", "labelledby", "modalClassName", "modal_class_name", "contentClassName", "content_class_name", "backdropClassName", "backdrop_class_name", "tag", "loading_state", "fade", "style", "zindex", "zIndex", "dialogStyle", "dialog_style", "contentStyle", "content_style"];
 
-        function ou(e, t) {
+        function ru(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function iu(e) {
+        function au(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? ou(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ou(Object(n)).forEach((function(t) {
+                t % 2 ? ru(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ru(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var lu = function(t) {
+        var su = function(t) {
             var n = t.children,
                 r = t.is_open,
                 a = t.setProps,
                 s = t.className,
                 i = t.class_name,
                 c = t.autoFocus,
                 u = t.autofocus,
@@ -8499,43 +8446,53 @@
                 _ = t.backdrop_class_name,
                 x = t.tag,
                 O = t.loading_state,
                 w = t.fade,
                 N = t.style,
                 E = t.zindex,
                 j = t.zIndex,
-                k = o(t, su);
-            return l().createElement(au, e({
+                k = t.dialogStyle,
+                P = t.dialog_style,
+                C = t.contentStyle,
+                T = t.content_style,
+                S = o(t, nu);
+            return l().createElement(tu, e({
                 animation: w,
                 dialogAs: x,
+                dialogStyle: P || k,
+                contentStyle: T || C,
                 dialogClassName: i || s,
                 className: b || g,
                 contentClassName: h || y,
                 backdropClassName: _ || v,
                 autoFocus: u || c,
                 enforceFocus: d,
                 "aria-labelledby": f || p,
                 show: r,
                 onHide: function() {
                     a && a({
                         is_open: !1
                     })
                 },
-                style: E || j ? iu(iu({}, N), {}, {
+                style: E || j ? au(au({}, N), {}, {
                     zIndex: E || j
                 }) : N,
                 zIndex: E || j
-            }, m(["persistence", "persistence_type", "persisted_props"], k), {
+            }, m(["persistence", "persistence_type", "persisted_props"], S), {
                 "data-dash-is-loading": O && O.is_loading || void 0
             }), n)
         };
-        lu.propTypes = {
+        su.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
+            dialog_style: u().object,
+            dialogStyle: u().object,
+            content_style: u().object,
+            contentStyle: u().object,
             class_name: u().string,
             className: u().string,
             tag: u().string,
             is_open: u().bool,
             centered: u().bool,
             scrollable: u().bool,
             autofocus: u().bool,
@@ -8554,246 +8511,246 @@
             content_class_name: u().string,
             contentClassName: u().string,
             fade: u().bool,
             fullscreen: u().oneOf([u().bool, u().oneOf(["sm-down", "md-down", "lg-down", "xl-down", "xxl-down"])]),
             zindex: u().oneOfType([u().number, u().string]),
             zIndex: u().oneOfType([u().number, u().string])
         };
-        const cu = lu,
-            uu = i.forwardRef((({
+        const ou = su,
+            iu = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "modal-body"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        uu.displayName = "ModalBody";
-        const du = uu;
-        var pu = ["children", "loading_state", "className", "class_name", "tag"],
-            fu = function(t) {
+        iu.displayName = "ModalBody";
+        const lu = iu;
+        var cu = ["children", "loading_state", "className", "class_name", "tag"],
+            uu = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.tag,
-                    c = o(t, pu);
-                return l().createElement(du, e({
+                    c = o(t, cu);
+                return l().createElement(lu, e({
                     as: i,
                     className: s || a,
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }, m(["setProps"], c)), n)
             };
-        fu.propTypes = {
+        uu.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const mu = fu,
-            gu = i.forwardRef((({
+        const du = uu,
+            pu = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "modal-footer"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        gu.displayName = "ModalFooter";
-        const bu = gu;
-        var yu = ["children", "loading_state", "className", "class_name", "tag"],
-            hu = function(t) {
+        pu.displayName = "ModalFooter";
+        const fu = pu;
+        var mu = ["children", "loading_state", "className", "class_name", "tag"],
+            gu = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.tag,
-                    c = o(t, yu);
-                return l().createElement(bu, e({
+                    c = o(t, mu);
+                return l().createElement(fu, e({
                     as: i,
                     className: s || a,
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }, m(["setProps"], c)), n)
             };
-        hu.propTypes = {
+        gu.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const vu = hu,
-            _u = i.forwardRef((({
+        const bu = gu,
+            yu = i.forwardRef((({
                 closeLabel: e = "Close",
                 closeVariant: t,
                 closeButton: n = !1,
                 onHide: r,
                 children: a,
                 ...s
             }, o) => {
-                const l = (0, i.useContext)(Yc),
-                    c = Ye((() => {
+                const l = (0, i.useContext)(Uc),
+                    c = Ve((() => {
                         null == l || l.onHide(), null == r || r()
                     }));
                 return (0, _.jsxs)("div", {
                     ref: o,
                     ...s,
-                    children: [a, n && (0, _.jsx)(vt, {
+                    children: [a, n && (0, _.jsx)(yt, {
                         "aria-label": e,
                         variant: t,
                         onClick: c
                     })]
                 })
             })),
-            xu = _u,
-            Ou = i.forwardRef((({
+            hu = yu,
+            vu = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 closeLabel: n = "Close",
                 closeButton: r = !1,
                 ...a
-            }, s) => (e = E(e, "modal-header"), (0, _.jsx)(xu, {
+            }, s) => (e = E(e, "modal-header"), (0, _.jsx)(hu, {
                 ref: s,
                 ...a,
                 className: b()(t, e),
                 closeLabel: n,
                 closeButton: r
             }))));
-        Ou.displayName = "ModalHeader";
-        const wu = Ou;
-        var Nu = ["children", "loading_state", "className", "class_name", "tag", "close_button"],
-            Eu = function(t) {
+        vu.displayName = "ModalHeader";
+        const _u = vu;
+        var xu = ["children", "loading_state", "className", "class_name", "tag", "close_button"],
+            Ou = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.tag,
                     c = t.close_button,
-                    u = o(t, Nu);
-                return l().createElement(wu, e({
+                    u = o(t, xu);
+                return l().createElement(_u, e({
                     as: i,
                     className: s || a,
                     closeButton: c,
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }, m(["setProps"], u)), n)
             };
-        Eu.defaultProps = {
+        Ou.defaultProps = {
             close_button: !0
-        }, Eu.propTypes = {
+        }, Ou.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             close_button: u().bool,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const ju = Eu,
-            ku = Xe("h4"),
-            Pu = i.forwardRef((({
+        const wu = Ou,
+            Nu = Ge("h4"),
+            Eu = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
-                as: n = ku,
+                as: n = Nu,
                 ...r
             }, a) => (t = E(t, "modal-title"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        Pu.displayName = "ModalTitle";
-        const Cu = Pu;
-        var Tu = ["children", "loading_state", "className", "class_name", "tag"],
-            Su = function(t) {
+        Eu.displayName = "ModalTitle";
+        const ju = Eu;
+        var ku = ["children", "loading_state", "className", "class_name", "tag"],
+            Pu = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.tag,
-                    c = o(t, Tu);
-                return l().createElement(Cu, e({
+                    c = o(t, ku);
+                return l().createElement(ju, e({
                     as: i,
                     className: s || a,
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }, m(["setProps"], c)), n)
             };
-        Su.propTypes = {
+        Pu.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Ru = Su;
-        var Du = ["children", "loading_state", "className", "class_name", "pills", "justified", "horizontal", "vertical", "navbar_scroll"],
-            Lu = {
+        const Cu = Pu;
+        var Tu = ["children", "loading_state", "className", "class_name", "pills", "justified", "horizontal", "vertical", "navbar_scroll"],
+            Su = {
                 start: "justify-content-start",
                 center: "justify-content-center",
                 end: "justify-content-end",
                 around: "justify-content-around",
                 between: "justify-content-between"
             },
-            $u = {
+            Ru = {
                 xs: "flex-xs-column",
                 sm: "flex-sm-column",
                 md: "flex-md-column",
                 lg: "flex-lg-column",
                 xl: "flex-xl-column"
             },
-            Iu = function(t) {
+            Du = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.pills,
                     c = t.justified,
                     u = t.horizontal,
                     d = t.vertical,
                     p = t.navbar_scroll,
-                    f = o(t, Du),
-                    g = u && Lu[u],
-                    y = !0 === d ? "flex-column" : d && $u[d],
+                    f = o(t, Tu),
+                    g = u && Su[u],
+                    y = !0 === d ? "flex-column" : d && Ru[d],
                     h = b()(s || a, g, y);
-                return l().createElement(ki, e({
+                return l().createElement(wi, e({
                     className: h,
                     variant: i ? "pills" : null,
                     justify: c,
                     navbarScroll: p
                 }, m(["setProps"], f), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Iu.propTypes = {
+        Du.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             pills: u().bool,
@@ -8806,114 +8763,114 @@
             navbar_scroll: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Au = Iu,
-            Fu = i.forwardRef((({
+        const Lu = Du,
+            Iu = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 as: n,
                 ...r
             }, a) => {
                 e = E(e, "navbar-brand");
                 const s = n || (r.href ? "a" : "span");
                 return (0, _.jsx)(s, {
                     ...r,
                     ref: a,
                     className: b()(t, e)
                 })
             }));
-        Fu.displayName = "NavbarBrand";
-        const Mu = Fu,
-            Bu = i.forwardRef((({
+        Iu.displayName = "NavbarBrand";
+        const $u = Iu,
+            Au = i.forwardRef((({
                 children: e,
                 bsPrefix: t,
                 ...n
             }, r) => {
                 t = E(t, "navbar-collapse");
-                const a = (0, i.useContext)(ri);
+                const a = (0, i.useContext)(Zo);
                 return (0, _.jsx)(pe, {
                     in: !(!a || !a.expanded),
                     ...n,
                     children: (0, _.jsx)("div", {
                         ref: r,
                         className: t,
                         children: e
                     })
                 })
             }));
-        Bu.displayName = "NavbarCollapse";
-        const zu = Bu,
-            Ku = i.forwardRef((({
+        Au.displayName = "NavbarCollapse";
+        const Mu = Au,
+            Fu = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 children: n,
                 label: r = "Toggle navigation",
                 as: a = "button",
                 onClick: s,
                 ...o
             }, l) => {
                 e = E(e, "navbar-toggler");
                 const {
                     onToggle: c,
                     expanded: u
-                } = (0, i.useContext)(ri) || {}, d = Ye((e => {
+                } = (0, i.useContext)(Zo) || {}, d = Ve((e => {
                     s && s(e), c && c()
                 }));
                 return "button" === a && (o.type = "button"), (0, _.jsx)(a, {
                     ...o,
                     ref: l,
                     onClick: d,
                     "aria-label": r,
                     className: b()(t, e, !u && "collapsed"),
                     children: n || (0, _.jsx)("span", {
                         className: `${e}-icon`
                     })
                 })
             }));
-        Ku.displayName = "NavbarToggle";
-        const Hu = Ku,
-            Uu = new WeakMap,
-            Wu = (e, t) => {
+        Fu.displayName = "NavbarToggle";
+        const Bu = Fu,
+            zu = new WeakMap,
+            Ku = (e, t) => {
                 if (!e || !t) return;
-                const n = Uu.get(t) || new Map;
-                Uu.set(t, n);
+                const n = zu.get(t) || new Map;
+                zu.set(t, n);
                 let r = n.get(e);
                 return r || (r = t.matchMedia(e), r.refCount = 0, n.set(r.media, r)), r
             };
 
-        function qu(e, t = ("undefined" == typeof window ? void 0 : window)) {
-            const n = Wu(e, t),
+        function Hu(e, t = ("undefined" == typeof window ? void 0 : window)) {
+            const n = Ku(e, t),
                 [r, a] = (0, i.useState)((() => !!n && n.matches));
-            return at((() => {
-                let n = Wu(e, t);
+            return nt((() => {
+                let n = Ku(e, t);
                 if (!n) return a(!1);
-                let r = Uu.get(t);
+                let r = zu.get(t);
                 const s = () => {
                     a(n.matches)
                 };
                 return n.refCount++, n.addListener(s), s(), () => {
                     n.removeListener(s), n.refCount--, n.refCount <= 0 && (null == r || r.delete(n.media)), n = void 0
                 }
             }), [e]), r
         }
-        const Vu = function(e) {
+        const Wu = function(e) {
                 const t = Object.keys(e);
 
                 function n(e, t) {
                     return e === t ? t : e ? `${e} and ${t}` : t
                 }
                 return function(r, a, s) {
                     let o;
                     return "object" == typeof r ? (o = r, s = a, a = !0) : (a = a || !0, o = {
                         [r]: a
-                    }), qu((0, i.useMemo)((() => Object.entries(o).reduce(((r, [a, s]) => ("up" !== s && !0 !== s || (r = n(r, function(t) {
+                    }), Hu((0, i.useMemo)((() => Object.entries(o).reduce(((r, [a, s]) => ("up" !== s && !0 !== s || (r = n(r, function(t) {
                         let n = e[t];
                         return "number" == typeof n && (n = `${n}px`), `(min-width: ${n})`
                     }(a))), "down" !== s && !0 !== s || (r = n(r, function(n) {
                         const r = function(e) {
                             return t[Math.min(t.indexOf(e) + 1, t.length - 1)]
                         }(n);
                         let a = e[r];
@@ -8924,31 +8881,31 @@
                 xs: 0,
                 sm: 576,
                 md: 768,
                 lg: 992,
                 xl: 1200,
                 xxl: 1400
             }),
-            Gu = i.forwardRef((({
+            Uu = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "offcanvas-body"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        Gu.displayName = "OffcanvasBody";
-        const Yu = Gu,
-            Xu = {
+        Uu.displayName = "OffcanvasBody";
+        const qu = Uu,
+            Vu = {
                 [z]: "show",
                 [K]: "show"
             },
-            Ju = i.forwardRef((({
+            Gu = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 children: n,
                 in: r = !1,
                 mountOnEnter: a = !1,
                 unmountOnExit: s = !1,
                 appear: o = !1,
@@ -8960,60 +8917,60 @@
                 mountOnEnter: a,
                 unmountOnExit: s,
                 appear: o,
                 ...l,
                 childRef: n.ref,
                 children: (r, a) => i.cloneElement(n, {
                     ...a,
-                    className: b()(t, n.props.className, (r === z || r === H) && `${e}-toggling`, Xu[r])
+                    className: b()(t, n.props.className, (r === z || r === H) && `${e}-toggling`, Vu[r])
                 })
             }))));
-        Ju.displayName = "OffcanvasToggling";
-        const Qu = Ju,
-            Zu = i.forwardRef((({
+        Gu.displayName = "OffcanvasToggling";
+        const Yu = Gu,
+            Xu = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 closeLabel: n = "Close",
                 closeButton: r = !1,
                 ...a
-            }, s) => (e = E(e, "offcanvas-header"), (0, _.jsx)(xu, {
+            }, s) => (e = E(e, "offcanvas-header"), (0, _.jsx)(hu, {
                 ref: s,
                 ...a,
                 className: b()(t, e),
                 closeLabel: n,
                 closeButton: r
             }))));
-        Zu.displayName = "OffcanvasHeader";
-        const ed = Zu,
-            td = Xe("h5"),
-            nd = i.forwardRef((({
+        Xu.displayName = "OffcanvasHeader";
+        const Ju = Xu,
+            Qu = Ge("h5"),
+            Zu = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
-                as: n = td,
+                as: n = Qu,
                 ...r
             }, a) => (t = E(t, "offcanvas-title"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        nd.displayName = "OffcanvasTitle";
-        const rd = nd;
+        Zu.displayName = "OffcanvasTitle";
+        const ed = Zu;
 
-        function ad(e) {
-            return (0, _.jsx)(Qu, {
+        function td(e) {
+            return (0, _.jsx)(Yu, {
                 ...e
             })
         }
 
-        function sd(e) {
-            return (0, _.jsx)(bt, {
+        function nd(e) {
+            return (0, _.jsx)(mt, {
                 ...e
             })
         }
-        const od = i.forwardRef((({
+        const rd = i.forwardRef((({
             bsPrefix: e,
             className: t,
             children: n,
             "aria-labelledby": r,
             placement: a = "start",
             responsive: s,
             show: o = !1,
@@ -9039,102 +8996,102 @@
             renderStaticNode: T = !1,
             ...S
         }, R) => {
             const D = (0, i.useRef)();
             e = E(e, "offcanvas");
             const {
                 onToggle: L
-            } = (0, i.useContext)(ri) || {}, [$, I] = (0, i.useState)(!1), A = Vu(s || "xs", "up");
+            } = (0, i.useContext)(Zo) || {}, [I, $] = (0, i.useState)(!1), A = Wu(s || "xs", "up");
             (0, i.useEffect)((() => {
-                I(s ? o && !A : o)
+                $(s ? o && !A : o)
             }), [o, s, A]);
-            const F = Ye((() => {
+            const M = Ve((() => {
                     null == L || L(), null == f || f()
                 })),
-                M = (0, i.useMemo)((() => ({
-                    onHide: F
-                })), [F]),
+                F = (0, i.useMemo)((() => ({
+                    onHide: M
+                })), [M]),
                 B = (0, i.useCallback)((t => (0, _.jsx)("div", {
                     ...t,
                     className: b()(`${e}-backdrop`, P)
                 })), [P, e]),
                 z = o => (0, _.jsx)("div", {
                     ...o,
                     ...S,
                     className: b()(t, s ? `${e}-${s}` : e, `${e}-${a}`),
                     "aria-labelledby": r,
                     children: n
                 });
             return (0, _.jsxs)(_.Fragment, {
-                children: [!$ && (s || T) && z({}), (0, _.jsx)(Yc.Provider, {
-                    value: M,
-                    children: (0, _.jsx)(Mc, {
-                        show: $,
+                children: [!I && (s || T) && z({}), (0, _.jsx)(Uc.Provider, {
+                    value: F,
+                    children: (0, _.jsx)(Ic, {
+                        show: I,
                         ref: R,
                         backdrop: l,
                         container: m,
                         keyboard: c,
                         autoFocus: g,
                         enforceFocus: y && !u,
                         restoreFocus: h,
                         restoreFocusOptions: v,
                         onEscapeKeyDown: d,
                         onShow: p,
-                        onHide: F,
+                        onHide: M,
                         onEnter: (e, ...t) => {
                             e && (e.style.visibility = "visible"), null == N || N(e, ...t)
                         },
                         onEntering: j,
                         onEntered: x,
                         onExit: O,
                         onExiting: w,
                         onExited: (e, ...t) => {
                             e && (e.style.visibility = ""), null == k || k(...t)
                         },
-                        manager: C || (u ? (D.current || (D.current = new Gc({
+                        manager: C || (u ? (D.current || (D.current = new Wc({
                             handleContainerOverflow: !1
-                        })), D.current) : Vc()),
-                        transition: ad,
-                        backdropTransition: sd,
+                        })), D.current) : Hc()),
+                        transition: td,
+                        backdropTransition: nd,
                         renderBackdrop: B,
                         renderDialog: z
                     })
                 })]
             })
         }));
-        od.displayName = "Offcanvas";
-        const id = Object.assign(od, {
-                Body: Yu,
-                Header: ed,
-                Title: rd
+        rd.displayName = "Offcanvas";
+        const ad = Object.assign(rd, {
+                Body: qu,
+                Header: Ju,
+                Title: ed
             }),
-            ld = i.forwardRef(((e, t) => {
-                const n = (0, i.useContext)(ri);
-                return (0, _.jsx)(id, {
+            sd = i.forwardRef(((e, t) => {
+                const n = (0, i.useContext)(Zo);
+                return (0, _.jsx)(ad, {
                     ref: t,
                     show: !(null == n || !n.expanded),
                     ...e,
                     renderStaticNode: !0
                 })
             }));
-        ld.displayName = "NavbarOffcanvas";
-        const cd = ld,
-            ud = i.forwardRef((({
+        sd.displayName = "NavbarOffcanvas";
+        const od = sd,
+            id = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "span",
                 ...r
             }, a) => (t = E(t, "navbar-text"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        ud.displayName = "NavbarText";
-        const dd = ud,
-            pd = i.forwardRef(((e, t) => {
+        id.displayName = "NavbarText";
+        const ld = id,
+            cd = i.forwardRef(((e, t) => {
                 const {
                     bsPrefix: n,
                     expand: r = !0,
                     variant: a = "light",
                     bg: s,
                     fixed: o,
                     sticky: l,
@@ -9155,86 +9112,86 @@
                 "string" == typeof r && (x = `${x}-${r}`);
                 const O = (0, i.useMemo)((() => ({
                     onToggle: () => null == p ? void 0 : p(!d),
                     bsPrefix: y,
                     expanded: !!d,
                     expand: r
                 })), [y, d, r, p]);
-                return (0, _.jsx)(ri.Provider, {
+                return (0, _.jsx)(Zo.Provider, {
                     value: O,
-                    children: (0, _.jsx)(To.Provider, {
+                    children: (0, _.jsx)(jo.Provider, {
                         value: h,
                         children: (0, _.jsx)(u, {
                             ref: t,
                             ...g,
                             className: b()(c, y, r && x, a && `${y}-${a}`, s && `bg-${s}`, l && `sticky-${l}`, o && `fixed-${o}`)
                         })
                     })
                 })
             }));
-        pd.displayName = "Navbar";
-        const fd = Object.assign(pd, {
-            Brand: Mu,
-            Collapse: zu,
-            Offcanvas: cd,
-            Text: dd,
-            Toggle: Hu
+        cd.displayName = "Navbar";
+        const ud = Object.assign(cd, {
+            Brand: $u,
+            Collapse: Mu,
+            Offcanvas: od,
+            Text: ld,
+            Toggle: Bu
         });
-        var md = ["children", "color", "style", "loading_state", "className", "class_name", "light", "dark", "tag"];
+        var dd = ["children", "color", "style", "loading_state", "className", "class_name", "light", "dark", "tag"];
 
-        function gd(e, t) {
+        function pd(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function bd(e) {
+        function fd(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? gd(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : gd(Object(n)).forEach((function(t) {
+                t % 2 ? pd(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : pd(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var yd = function(t) {
+        var md = function(t) {
             var n = t.children,
                 r = t.color,
                 a = t.style,
                 s = t.loading_state,
                 i = t.className,
                 c = t.class_name,
                 u = (t.light, t.dark),
                 d = t.tag,
-                p = o(t, md),
-                f = Ot.has(r);
-            return l().createElement(fd, e({
+                p = o(t, dd),
+                f = _t.has(r);
+            return l().createElement(ud, e({
                 variant: u ? "dark" : "light",
                 as: d,
                 bg: f ? r : null,
-                style: bd({
+                style: fd({
                     backgroundColor: !f && r
                 }, a),
                 className: c || i
             }, m(["setProps"], p), {
                 "data-dash-is-loading": s && s.is_loading || void 0
             }), n)
         };
-        yd.defaultProps = {
+        md.defaultProps = {
             color: "light",
             light: !0,
             expand: "md"
-        }, yd.propTypes = {
+        }, md.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             light: u().bool,
@@ -9247,72 +9204,68 @@
             expand: u().oneOfType([u().bool, u().string]),
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const hd = yd;
-        var vd = ["children", "loading_state", "className", "class_name", "href", "setProps"],
-            _d = function(t) {
+        const gd = md;
+        var bd = ["children", "loading_state", "className", "class_name"],
+            yd = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = t.href,
-                    c = t.setProps,
-                    u = o(t, vd),
-                    d = Fe(i, c);
-                return l().createElement(Mu, e({
+                    i = o(t, bd);
+                return l().createElement($u, e({
                     className: s || a
-                }, u, {
-                    as: d ? Bt : "span",
-                    href: d,
+                }, m(["setProps"], i), {
+                    as: t.href ? Mt : "span",
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        _d.propTypes = {
+        yd.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             external_link: u().bool,
             href: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const xd = _d;
-        var Od = ["children", "loading_state", "className", "class_name"],
-            wd = function(t) {
+        const hd = yd;
+        var vd = ["children", "loading_state", "className", "class_name"],
+            _d = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Od);
-                return l().createElement(Hu, e({
+                    i = o(t, vd);
+                return l().createElement(Bu, e({
                     onClick: function() {
                         t.setProps && t.setProps({
                             n_clicks: t.n_clicks + 1,
                             n_clicks_timestamp: Date.now()
                         })
                     },
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        wd.defaultProps = {
+        _d.defaultProps = {
             n_clicks: 0,
             n_clicks_timestamp: -1
-        }, wd.propTypes = {
+        }, _d.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             type: u().string,
@@ -9320,93 +9273,91 @@
             n_clicks_timestamp: u().number,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Nd = wd;
-        var Ed = ["children", "brand", "brand_href", "brand_style", "brand_external_link", "links_left", "fluid", "color", "dark", "light", "style", "loading_state", "className", "class_name", "setProps"];
+        const xd = _d;
+        var Od = ["children", "brand", "brand_href", "brand_style", "brand_external_link", "links_left", "fluid", "color", "dark", "light", "style", "loading_state", "className", "class_name"];
 
-        function jd(e, t) {
+        function wd(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function kd(e) {
+        function Nd(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? jd(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : jd(Object(n)).forEach((function(t) {
+                t % 2 ? wd(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : wd(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Pd = function(t) {
+        var Ed = function(t) {
             var n = t.children,
                 r = t.brand,
                 a = t.brand_href,
                 s = t.brand_style,
                 c = t.brand_external_link,
                 u = t.links_left,
                 d = t.fluid,
                 p = t.color,
                 f = t.dark,
                 g = (t.light, t.style),
                 b = t.loading_state,
                 y = t.className,
                 h = t.class_name,
-                v = t.setProps,
-                _ = o(t, Ed),
-                x = Fe(a, v),
-                O = Ot.has(p),
-                w = Se((0, i.useState)(!1), 2),
-                N = w[0],
-                E = w[1];
-            return l().createElement(fd, e({
+                v = o(t, Od),
+                _ = _t.has(p),
+                x = Se((0, i.useState)(!1), 2),
+                O = x[0],
+                w = x[1];
+            return l().createElement(ud, e({
                 variant: f ? "dark" : "light",
-                bg: O ? p : null,
-                color: O ? p : null,
-                style: O ? g : kd({
+                bg: _ ? p : null,
+                color: _ ? p : null,
+                style: _ ? g : Nd({
                     backgroundColor: p
                 }, g),
                 className: h || y
-            }, m(["setProps"], _), {
+            }, m(["setProps"], v), {
                 "data-dash-is-loading": b && b.is_loading || void 0
-            }), l().createElement(Na, {
+            }), l().createElement(_a, {
                 fluid: d
-            }, r && l().createElement(xd, {
-                href: x,
+            }, r && l().createElement(hd, {
+                href: a,
                 style: s,
                 external_link: c
-            }, r), l().createElement(Nd, {
+            }, r), l().createElement(xd, {
                 onClick: function() {
-                    return E(!N)
+                    return w(!O)
                 }
-            }), l().createElement(fd.Collapse, {
-                in: N
-            }, l().createElement(Au, {
+            }), l().createElement(ud.Collapse, {
+                in: O
+            }, l().createElement(Lu, {
                 className: u ? "me-auto" : "ms-auto"
             }, n))))
         };
-        Pd.defaultProps = {
+        Ed.defaultProps = {
             fluid: !1,
             color: "light",
             light: !0,
             expand: "md",
             links_left: !1
-        }, Pd.propTypes = {
+        }, Ed.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             brand: u().node,
@@ -9423,91 +9374,90 @@
             expand: u().oneOfType([u().bool, u().string]),
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Cd = Pd;
-        var Td = ["children", "loading_state", "className", "class_name"],
-            Sd = function(t) {
+        const jd = Ed;
+        var kd = ["children", "loading_state", "className", "class_name"],
+            Pd = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Td);
-                return l().createElement(wi, e({
+                    i = o(t, kd);
+                return l().createElement(vi, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Sd.propTypes = {
+        Pd.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Rd = Sd;
-        var Dd = n(13),
-            Ld = ["children", "disabled", "className", "class_name", "active", "loading_state", "setProps", "n_clicks", "href"],
-            $d = function(t) {
+        const Cd = Pd;
+        var Td = n(13),
+            Sd = ["children", "disabled", "className", "class_name", "active", "loading_state", "setProps", "n_clicks", "href"],
+            Rd = function(t) {
                 var n = Se((0, i.useState)(!1), 2),
                     r = n[0],
                     a = n[1],
                     s = t.children,
                     c = t.disabled,
                     u = t.className,
                     d = t.class_name,
                     p = t.active,
                     f = t.loading_state,
                     g = t.setProps,
                     y = t.n_clicks,
                     h = t.href,
-                    v = o(t, Ld),
-                    _ = Fe(h, g),
-                    x = function(e) {
-                        a(!0 === p || "exact" === p && e === _ || "partial" === p && e.startsWith(_))
+                    v = o(t, Sd),
+                    _ = function(e) {
+                        a(!0 === p || "exact" === p && e === h || "partial" === p && e.startsWith(h))
                     };
                 (0, i.useEffect)((function() {
-                    x(window.location.pathname), "string" == typeof p && Dd.History.onChange((function() {
-                        x(window.location.pathname)
+                    _(window.location.pathname), "string" == typeof p && Td.History.onChange((function() {
+                        _(window.location.pathname)
                     }))
                 }), [p]);
-                var O = b()(d || u, "nav-link", {
+                var x = b()(d || u, "nav-link", {
                     active: r,
                     disabled: c
                 });
-                return l().createElement(Bt, e({
-                    className: O,
+                return l().createElement(Mt, e({
+                    className: x,
                     disabled: c,
                     preOnClick: function() {
                         !c && g && g({
                             n_clicks: y + 1,
                             n_clicks_timestamp: Date.now()
                         })
                     },
-                    href: _
+                    href: h
                 }, m(["n_clicks_timestamp"], v), {
                     "data-dash-is-loading": f && f.is_loading || void 0
                 }), s)
             };
-        $d.defaultProps = {
+        Rd.defaultProps = {
             active: !1,
             disabled: !1,
             n_clicks: 0,
             n_clicks_timestamp: -1
-        }, $d.propTypes = {
+        }, Rd.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             href: u().string,
@@ -9519,17 +9469,17 @@
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             target: u().string
         };
-        const Id = $d;
-        var Ad = ["is_open", "setProps", "children", "loading_state", "class_name", "className", "backdrop", "backdrop_class_name", "backdropClassName", "labelledby", "labelledBy", "scrollable", "autofocus", "autoFocus", "close_button", "title"],
-            Fd = function(t) {
+        const Dd = Rd;
+        var Ld = ["is_open", "setProps", "children", "loading_state", "class_name", "className", "backdrop", "backdrop_class_name", "backdropClassName", "labelledby", "labelledBy", "scrollable", "autofocus", "autoFocus", "close_button", "title"],
+            Id = function(t) {
                 var n = t.is_open,
                     r = t.setProps,
                     a = t.children,
                     s = t.loading_state,
                     i = t.class_name,
                     c = t.className,
                     u = t.backdrop,
@@ -9538,41 +9488,41 @@
                     f = t.labelledby,
                     m = t.labelledBy,
                     g = t.scrollable,
                     b = t.autofocus,
                     y = t.autoFocus,
                     h = t.close_button,
                     v = t.title,
-                    _ = o(t, Ad),
+                    _ = o(t, Ld),
                     x = function() {
                         r && r({
                             is_open: !n
                         })
                     },
-                    O = v || h ? l().createElement(id.Header, {
+                    O = v || h ? l().createElement(ad.Header, {
                         closeButton: h,
                         onHide: "static" === u && h ? x : null
-                    }, l().createElement(id.Title, null, v)) : null;
-                return l().createElement(id, e({
+                    }, l().createElement(ad.Title, null, v)) : null;
+                return l().createElement(ad, e({
                     autoFocus: b || y,
                     "aria-labelledby": f || m,
                     className: i || c,
                     backdropClassName: d || p,
                     scroll: g,
                     show: n,
                     onHide: "static" !== u ? x : null,
                     backdrop: u || "static" === u,
                     "data-dash-is-loading": s && s.is_loading || void 0
-                }, _), O, l().createElement(id.Body, null, a))
+                }, _), O, l().createElement(ad.Body, null, a))
             };
-        Fd.defaultProps = {
+        Id.defaultProps = {
             close_button: !0,
             is_open: !1,
             backdrop: !0
-        }, Fd.propTypes = {
+        }, Id.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             labelledby: u().string,
             labelledBy: u().string,
@@ -9589,25 +9539,25 @@
             close_button: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Md = Fd,
-            Bd = i.forwardRef((({
+        const $d = Id,
+            Ad = i.forwardRef((({
                 active: e = !1,
                 disabled: t = !1,
                 className: n,
                 style: r,
                 activeLabel: a = "(current)",
                 children: s,
                 linkStyle: o,
                 linkClassName: i,
-                as: l = dt,
+                as: l = ct,
                 ...c
             }, u) => {
                 const d = e || t ? "span" : l;
                 return (0, _.jsx)("li", {
                     ref: u,
                     style: r,
                     className: b()(n, "page-item", {
@@ -9621,143 +9571,143 @@
                         children: [s, e && a && (0, _.jsx)("span", {
                             className: "visually-hidden",
                             children: a
                         })]
                     })
                 })
             }));
-        Bd.displayName = "PageItem";
-        const zd = Bd;
+        Ad.displayName = "PageItem";
+        const Md = Ad;
 
-        function Kd(e, t, n = e) {
+        function Fd(e, t, n = e) {
             const r = i.forwardRef((({
                 children: e,
                 ...r
-            }, a) => (0, _.jsxs)(Bd, {
+            }, a) => (0, _.jsxs)(Ad, {
                 ...r,
                 ref: a,
                 children: [(0, _.jsx)("span", {
                     "aria-hidden": "true",
                     children: e || t
                 }), (0, _.jsx)("span", {
                     className: "visually-hidden",
                     children: n
                 })]
             })));
             return r.displayName = e, r
         }
-        const Hd = Kd("First", "«"),
-            Ud = Kd("Prev", "‹", "Previous"),
-            Wd = Kd("Ellipsis", "…", "More"),
-            qd = Kd("Next", "›"),
-            Vd = Kd("Last", "»"),
-            Gd = i.forwardRef((({
+        const Bd = Fd("First", "«"),
+            zd = Fd("Prev", "‹", "Previous"),
+            Kd = Fd("Ellipsis", "…", "More"),
+            Hd = Fd("Next", "›"),
+            Wd = Fd("Last", "»"),
+            Ud = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 size: n,
                 ...r
             }, a) => {
                 const s = E(e, "pagination");
                 return (0, _.jsx)("ul", {
                     ref: a,
                     ...r,
                     className: b()(t, s, n && `${s}-${n}`)
                 })
             }));
-        Gd.displayName = "Pagination";
-        const Yd = Object.assign(Gd, {
-            First: Hd,
-            Prev: Ud,
-            Ellipsis: Wd,
-            Item: zd,
-            Next: qd,
-            Last: Vd
+        Ud.displayName = "Pagination";
+        const qd = Object.assign(Ud, {
+            First: Bd,
+            Prev: zd,
+            Ellipsis: Kd,
+            Item: Md,
+            Next: Hd,
+            Last: Wd
         });
-        var Xd = ["step", "active_page", "min_value", "fully_expanded", "previous_next", "first_last", "setProps", "class_name", "className", "loading_state"],
-            Jd = function(t) {
+        var Vd = ["step", "active_page", "min_value", "fully_expanded", "previous_next", "first_last", "setProps", "class_name", "className", "loading_state"],
+            Gd = function(t) {
                 var n = t.step,
                     r = t.active_page,
                     a = t.min_value,
                     s = t.fully_expanded,
                     i = t.previous_next,
                     c = t.first_last,
                     u = t.setProps,
                     d = t.class_name,
                     p = t.className,
                     f = t.loading_state,
-                    m = o(t, Xd),
+                    m = o(t, Vd),
                     g = t.max_value;
                 (g - a) % n != 0 && (g = g + n - (g - a) % n);
                 var b = function(e) {
                         u && u({
                             active_page: e
                         })
                     },
                     y = function(e) {
-                        return l().createElement(Yd.Item, {
+                        return l().createElement(qd.Item, {
                             key: e,
                             active: e === r,
                             onClick: function() {
                                 return b(e)
                             }
                         }, e)
                     },
                     h = [];
-                if (c && h.push(l().createElement(Yd.First, {
+                if (c && h.push(l().createElement(qd.First, {
                         key: "first",
                         disabled: r === a,
                         onClick: function() {
                             return b(a)
                         }
-                    })), i && h.push(l().createElement(Yd.Prev, {
+                    })), i && h.push(l().createElement(qd.Prev, {
                         key: "previous",
                         disabled: r === a,
                         onClick: function() {
                             return b(r - n)
                         }
                     })), s || Math.floor((g - a) / n) + 1 <= 7)
                     for (var v = a; v <= g; v += n) h.push(y(v));
-                else h.push(y(a)), r <= a + 3 * n ? (h.push(y(a + n)), h.push(y(a + 2 * n)), h.push(y(a + 3 * n)), h.push(y(a + 4 * n)), h.push(l().createElement(Yd.Ellipsis, {
+                else h.push(y(a)), r <= a + 3 * n ? (h.push(y(a + n)), h.push(y(a + 2 * n)), h.push(y(a + 3 * n)), h.push(y(a + 4 * n)), h.push(l().createElement(qd.Ellipsis, {
                     disabled: !0,
                     key: "ellipsis"
-                }))) : r >= g - 3 * n ? (h.push(l().createElement(Yd.Ellipsis, {
+                }))) : r >= g - 3 * n ? (h.push(l().createElement(qd.Ellipsis, {
                     disabled: !0,
                     key: "ellipsis"
-                })), h.push(y(g - 4 * n)), h.push(y(g - 3 * n)), h.push(y(g - 2 * n)), h.push(y(g - n))) : (h.push(l().createElement(Yd.Ellipsis, {
+                })), h.push(y(g - 4 * n)), h.push(y(g - 3 * n)), h.push(y(g - 2 * n)), h.push(y(g - n))) : (h.push(l().createElement(qd.Ellipsis, {
                     disabled: !0,
                     key: "ellipsis-1"
-                })), h.push(y(r - n)), h.push(y(r)), h.push(y(r + n)), h.push(l().createElement(Yd.Ellipsis, {
+                })), h.push(y(r - n)), h.push(y(r)), h.push(y(r + n)), h.push(l().createElement(qd.Ellipsis, {
                     disabled: !0,
                     key: "ellipsis-2"
                 }))), h.push(y(g));
-                return i && h.push(l().createElement(Yd.Next, {
+                return i && h.push(l().createElement(qd.Next, {
                     key: "next",
                     disabled: r === g,
                     onClick: function() {
                         return b(r + n)
                     }
-                })), c && h.push(l().createElement(Yd.Last, {
+                })), c && h.push(l().createElement(qd.Last, {
                     key: "last",
                     disabled: r === g,
                     onClick: function() {
                         return b(g)
                     }
-                })), l().createElement(Yd, e({
+                })), l().createElement(qd, e({
                     className: d || p,
                     "data-dash-is-loading": f && f.is_loading || void 0
                 }, m), h)
             };
-        Jd.defaultProps = {
+        Gd.defaultProps = {
             min_value: 1,
             step: 1,
             active_page: 1,
             fully_expanded: !0,
             previous_next: !1,
             first_last: !1
-        }, Jd.propTypes = {
+        }, Gd.propTypes = {
             id: u().string,
             class_name: u().string,
             className: u().string,
             style: u().object,
             size: u().oneOf(["sm", "lg"]),
             min_value: u().number,
             max_value: u().number.isRequired,
@@ -9768,83 +9718,83 @@
             first_last: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Qd = Jd;
+        const Yd = Gd;
 
-        function Zd({
+        function Xd({
             animation: e,
             bg: t,
             bsPrefix: n,
             size: r,
             ...a
         }) {
             n = E(n, "placeholder");
             const [{
                 className: s,
                 ...o
-            }] = da(a);
+            }] = ia(a);
             return {
                 ...o,
                 className: b()(s, e ? `${n}-${e}` : n, r && `${n}-${r}`, t && `bg-${t}`)
             }
         }
-        const ep = i.forwardRef(((e, t) => {
-            const n = Zd(e);
-            return (0, _.jsx)(nn, {
+        const Jd = i.forwardRef(((e, t) => {
+            const n = Xd(e);
+            return (0, _.jsx)(Qt, {
                 ...n,
                 ref: t,
                 disabled: !0,
                 tabIndex: -1
             })
         }));
-        ep.displayName = "PlaceholderButton";
-        const tp = ep,
-            np = i.forwardRef((({
+        Jd.displayName = "PlaceholderButton";
+        const Qd = Jd,
+            Zd = i.forwardRef((({
                 as: e = "span",
                 ...t
             }, n) => {
-                const r = Zd(t);
+                const r = Xd(t);
                 return (0, _.jsx)(e, {
                     ...r,
                     ref: n
                 })
             }));
-        np.displayName = "Placeholder";
-        const rp = Object.assign(np, {
-            Button: tp
+        Zd.displayName = "Placeholder";
+        const ep = Object.assign(Zd, {
+            Button: Qd
         });
-        var ap = ["children", "loading_state", "className", "class_name", "color", "button", "style", "delay_hide", "delay_show", "show_initially", "animation"];
+        var tp = ["children", "loading_state", "className", "class_name", "color", "button", "style", "delay_hide", "delay_show", "show_initially", "animation"];
 
-        function sp(e, t) {
+        function np(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
-        var op = function(t) {
+        var rp = function(t) {
             var n = t.children,
                 r = t.loading_state,
                 a = t.className,
                 s = t.class_name,
                 c = t.color,
                 u = t.button,
                 d = t.style,
                 p = t.delay_hide,
                 f = t.delay_show,
                 g = t.show_initially,
                 y = t.animation,
-                h = o(t, ap),
+                h = o(t, tp),
                 v = Se((0, i.useState)(g), 2),
                 _ = v[0],
                 x = v[1],
                 O = (0, i.useRef)(),
                 w = (0, i.useRef)();
             (0, i.useEffect)((function() {
                 r && (r.is_loading ? (O.current && (O.current = clearTimeout(O.current)), _ || w.current || (w.current = setTimeout((function() {
@@ -9852,33 +9802,33 @@
                 }), f))) : (w.current && (w.current = clearTimeout(w.current)), _ && !O.current && (O.current = setTimeout((function() {
                     x(!1), O.current = null
                 }), p))))
             }), [p, f, r]);
             var N = b()(s || a, y && "placeholder"),
                 E = function(t) {
                     var n = t.finalStyle;
-                    return u ? l().createElement(rp.Button, e({
+                    return u ? l().createElement(ep.Button, e({
                         variant: c,
                         className: N,
                         style: n,
                         animation: y
-                    }, m(["setProps"], h))) : l().createElement(rp, e({
+                    }, m(["setProps"], h))) : l().createElement(ep, e({
                         bg: c,
                         className: N,
                         style: n,
                         animation: y
                     }, m(["setProps"], h)))
                 };
             if (n) {
                 var j = function(e) {
                     for (var t = 1; t < arguments.length; t++) {
                         var n = null != arguments[t] ? arguments[t] : {};
-                        t % 2 ? sp(Object(n), !0).forEach((function(t) {
-                            Ve(e, t, n[t])
-                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : sp(Object(n)).forEach((function(t) {
+                        t % 2 ? np(Object(n), !0).forEach((function(t) {
+                            Ue(e, t, n[t])
+                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : np(Object(n)).forEach((function(t) {
                             Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                         }))
                     }
                     return e
                 }({
                     display: "block",
                     margin: "1rem auto"
@@ -9903,20 +9853,20 @@
                     finalStyle: j
                 })))
             }
             return l().createElement(E, {
                 finalStyle: d
             })
         };
-        op._dashprivate_isLoadingComponent = !0, op.defaultProps = {
+        rp._dashprivate_isLoadingComponent = !0, rp.defaultProps = {
             delay_hide: 0,
             delay_show: 0,
             show_initially: !0,
             button: !1
-        }, op.propTypes = {
+        }, rp.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             loading_state: u().shape({
@@ -9934,94 +9884,94 @@
             xs: u().number,
             sm: u().number,
             md: u().number,
             lg: u().number,
             xl: u().number,
             xxl: u().number
         };
-        const ip = op,
-            lp = i.forwardRef((({
+        const ap = rp,
+            sp = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "popover-body"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        lp.displayName = "PopoverBody";
-        const cp = lp;
+        sp.displayName = "PopoverBody";
+        const op = sp;
 
-        function up(e, t, n, r, a, s, o) {
+        function ip(e, t, n, r, a, s, o) {
             try {
                 var i = e[s](o),
                     l = i.value
             } catch (e) {
                 return void n(e)
             }
             i.done ? t(l) : Promise.resolve(l).then(r, a)
         }
 
-        function dp(e) {
+        function lp(e) {
             return function() {
                 var t = this,
                     n = arguments;
                 return new Promise((function(r, a) {
                     var s = e.apply(t, n);
 
                     function o(e) {
-                        up(s, r, a, o, i, "next", e)
+                        ip(s, r, a, o, i, "next", e)
                     }
 
                     function i(e) {
-                        up(s, r, a, o, i, "throw", e)
+                        ip(s, r, a, o, i, "throw", e)
                     }
                     o(void 0)
                 }))
             }
         }
-        var pp = n(14),
-            fp = n.n(pp);
-        const mp = () => {},
-            gp = i.forwardRef(((e, t) => {
+        var cp = n(14),
+            up = n.n(cp);
+        const dp = () => {},
+            pp = i.forwardRef(((e, t) => {
                 const {
                     flip: n,
                     offset: r,
                     placement: a,
                     containerPadding: s,
                     popperConfig: o = {},
                     transition: l,
                     runTransition: c
-                } = e, [u, d] = et(), [p, f] = et(), m = oe(d, t), g = Pc(e.container), b = Pc(e.target), [y, h] = (0, i.useState)(!e.show), v = Zs(b, u, lo({
+                } = e, [u, d] = Qe(), [p, f] = Qe(), m = oe(d, t), g = Nc(e.container), b = Nc(e.target), [y, h] = (0, i.useState)(!e.show), v = Ys(b, u, ao({
                     placement: a,
                     enableEvents: !!e.show,
                     containerPadding: s || 5,
                     flip: n,
                     offset: r,
                     arrowElement: p,
                     popperConfig: o
                 }));
                 e.show && y && h(!1);
                 const _ = e.show || !y;
                 if (function(e, t, {
                         disabled: n,
                         clickTrigger: r
                     } = {}) {
-                        const a = t || mp;
-                        oo(e, a, {
+                        const a = t || dp;
+                        no(e, a, {
                             disabled: n,
                             clickTrigger: r
                         });
-                        const s = Ye((e => {
-                            $c(e) && a(e)
+                        const s = Ve((e => {
+                            Sc(e) && a(e)
                         }));
                         (0, i.useEffect)((() => {
                             if (n || null == e) return;
-                            const t = C(ao(e));
+                            const t = C(eo(e));
                             let r = (t.defaultView || window).event;
                             const a = Z(t, "keyup", (e => {
                                 e !== r ? s(e) : r = void 0
                             }));
                             return () => {
                                 a()
                             }
@@ -10045,15 +9995,15 @@
                     placement: a,
                     show: !!e.show,
                     arrowProps: Object.assign({}, v.attributes.arrow, {
                         style: v.styles.arrow,
                         ref: f
                     })
                 });
-                return j = Lc(l, c, {
+                return j = Tc(l, c, {
                     in: !!e.show,
                     appear: !0,
                     mountOnEnter: !0,
                     unmountOnExit: !0,
                     children: j,
                     onExit: x,
                     onExiting: O,
@@ -10061,45 +10011,45 @@
                         h(!0), e.onExited && e.onExited(...t)
                     },
                     onEnter: w,
                     onEntering: N,
                     onEntered: E
                 }), g ? A().createPortal(j, g) : null
             }));
-        gp.displayName = "Overlay";
-        const bp = gp,
-            yp = i.forwardRef((({
+        pp.displayName = "Overlay";
+        const fp = pp,
+            mp = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "popover-header"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        yp.displayName = "PopoverHeader";
-        const hp = yp;
+        mp.displayName = "PopoverHeader";
+        const gp = mp;
 
-        function vp(e, t) {
+        function bp(e, t) {
             let n = e;
             return "left" === e ? n = t ? "end" : "start" : "right" === e && (n = t ? "start" : "end"), n
         }
 
-        function _p(e = "absolute") {
+        function yp(e = "absolute") {
             return {
                 position: e,
                 top: "0",
                 left: "0",
                 opacity: "0",
                 pointerEvents: "none"
             }
         }
         i.Component;
-        const xp = i.forwardRef((({
+        const hp = i.forwardRef((({
                 bsPrefix: e,
                 placement: t = "right",
                 className: n,
                 style: r,
                 children: a,
                 body: s,
                 arrowProps: o,
@@ -10107,59 +10057,59 @@
                 popper: l,
                 show: c,
                 ...u
             }, d) => {
                 const p = E(e, "popover"),
                     f = P(),
                     [m] = (null == t ? void 0 : t.split("-")) || [],
-                    g = vp(m, f);
+                    g = bp(m, f);
                 let y = r;
                 return c && !i && (y = {
                     ...r,
-                    ..._p(null == l ? void 0 : l.strategy)
+                    ...yp(null == l ? void 0 : l.strategy)
                 }), (0, _.jsxs)("div", {
                     ref: d,
                     role: "tooltip",
                     style: y,
                     "x-placement": m,
                     className: b()(n, p, m && `bs-popover-${g}`),
                     ...u,
                     children: [(0, _.jsx)("div", {
                         className: "popover-arrow",
                         ...o
-                    }), s ? (0, _.jsx)(cp, {
+                    }), s ? (0, _.jsx)(op, {
                         children: a
                     }) : a]
                 })
             })),
-            Op = Object.assign(xp, {
-                Header: hp,
-                Body: cp,
+            vp = Object.assign(hp, {
+                Header: gp,
+                Body: op,
                 POPPER_OFFSET: [0, 8]
             }),
-            wp = i.forwardRef((({
+            _p = i.forwardRef((({
                 bsPrefix: e,
                 placement: t = "right",
                 className: n,
                 style: r,
                 children: a,
                 arrowProps: s,
                 hasDoneInitialMeasure: o,
                 popper: i,
                 show: l,
                 ...c
             }, u) => {
                 e = E(e, "tooltip");
                 const d = P(),
                     [p] = (null == t ? void 0 : t.split("-")) || [],
-                    f = vp(p, d);
+                    f = bp(p, d);
                 let m = r;
                 return l && !o && (m = {
                     ...r,
-                    ..._p(null == i ? void 0 : i.strategy)
+                    ...yp(null == i ? void 0 : i.strategy)
                 }), (0, _.jsxs)("div", {
                     ref: u,
                     style: m,
                     role: "tooltip",
                     "x-placement": p,
                     className: b()(n, e, `bs-tooltip-${f}`),
                     ...c,
@@ -10168,21 +10118,21 @@
                         ...s
                     }), (0, _.jsx)("div", {
                         className: `${e}-inner`,
                         children: a
                     })]
                 })
             }));
-        wp.displayName = "Tooltip";
-        const Np = Object.assign(wp, {
+        _p.displayName = "Tooltip";
+        const xp = Object.assign(_p, {
                 TOOLTIP_OFFSET: [0, 6]
             }),
-            Ep = i.forwardRef((({
+            Op = i.forwardRef((({
                 children: e,
-                transition: t = bt,
+                transition: t = mt,
                 popperConfig: n = {},
                 rootClose: r = !1,
                 placement: a = "top",
                 show: s = !1,
                 ...o
             }, l) => {
                 const c = (0, i.useRef)({}),
@@ -10193,33 +10143,33 @@
                             r = E(void 0, "tooltip"),
                             a = (0, i.useMemo)((() => ({
                                 name: "offset",
                                 options: {
                                     offset: () => {
                                         if (e) return e;
                                         if (t.current) {
-                                            if (Bc(t.current, n)) return Op.POPPER_OFFSET;
-                                            if (Bc(t.current, r)) return Np.TOOLTIP_OFFSET
+                                            if ($c(t.current, n)) return vp.POPPER_OFFSET;
+                                            if ($c(t.current, r)) return xp.TOOLTIP_OFFSET
                                         }
                                         return [0, 0]
                                     }
                                 }
                             })), [e, n, r]);
                         return [t, [a]]
                     }(o.offset),
                     m = oe(l, p),
-                    g = !0 === t ? bt : t || void 0,
-                    y = Ye((e => {
+                    g = !0 === t ? mt : t || void 0,
+                    y = Ve((e => {
                         d(e), null == n || null == n.onFirstUpdate || n.onFirstUpdate(e)
                     }));
-                return at((() => {
+                return nt((() => {
                     u && o.target && (null == c.current.scheduleUpdate || c.current.scheduleUpdate())
                 }), [u, o.target]), (0, i.useEffect)((() => {
                     s || d(null)
-                }), [s]), (0, _.jsx)(bp, {
+                }), [s]), (0, _.jsx)(fp, {
                     ...o,
                     ref: m,
                     popperConfig: {
                         ...n,
                         modifiers: f.concat(n.modifiers || []),
                         onFirstUpdate: y
                     },
@@ -10271,27 +10221,27 @@
                                 ...e.props.style,
                                 ...r.style
                             }
                         })
                     }
                 })
             }));
-        Ep.displayName = "Overlay";
-        const jp = Ep;
-        var kp = ["children", "target", "delay", "trigger", "defaultShow", "setProps", "autohide"],
-            Pp = (0, i.createContext)({});
-        const Cp = function(t) {
+        Op.displayName = "Overlay";
+        const wp = Op;
+        var Np = ["children", "target", "delay", "trigger", "defaultShow", "setProps", "autohide"],
+            Ep = (0, i.createContext)({});
+        const jp = function(t) {
             var n, r, a, s, c = t.children,
                 u = t.target,
                 d = t.delay,
                 p = t.trigger,
                 f = t.defaultShow,
                 m = t.setProps,
                 g = t.autohide,
-                b = o(t, kp),
+                b = o(t, Np),
                 y = (!1, n = Se((0, i.useState)(false), 2), r = n[0], a = n[1], s = (0, i.useRef)(r), (0, i.useEffect)((function() {
                     s.current = r
                 }), [r]), [r, a, s]),
                 h = Se(y, 3),
                 v = h[0],
                 _ = h[1],
                 x = h[2],
@@ -10322,180 +10272,180 @@
                     !x.current && N.current ? (N.current = clearTimeout(N.current), R()) : x.current && (clearTimeout(w.current), w.current = setTimeout(R, d.hide))
                 },
                 L = function() {
                     x.current || (N.current = clearTimeout(N.current), _(!0), m && E && m({
                         is_open: !0
                     }))
                 },
-                $ = function() {
+                I = function() {
                     x.current && w.current ? (w.current = clearTimeout(w.current), L()) : x.current || (clearTimeout(N.current), N.current = setTimeout(L, d.show))
                 },
-                I = function(e) {
+                $ = function(e) {
                     var t, n;
-                    t = e.target, (n = O.current) && (t === n || n.contains(t)) && (w.current && (w.current = clearTimeout(w.current)), x.current ? D() : $())
+                    t = e.target, (n = O.current) && (t === n || n.contains(t)) && (w.current && (w.current = clearTimeout(w.current)), x.current ? D() : I())
                 };
             (0, i.useEffect)((function() {
                 setTimeout((function() {
                     return _(f)
                 }), 50)
             }), [f]), (0, i.useEffect)((function() {
                 k.indexOf("legacy") > -1 ? S(!0) : S(!1)
             }), [k]);
             var A = function(e) {
                     return new Promise((function(t) {
                         return setTimeout(t, e)
                     }))
                 },
-                F = function() {
-                    var e = dp(fp().mark((function e(t) {
+                M = function() {
+                    var e = lp(up().mark((function e(t) {
                         var n, r, a = arguments;
-                        return fp().wrap((function(e) {
+                        return up().wrap((function(e) {
                             for (;;) switch (e.prev = e.next) {
                                 case 0:
                                     if (n = a.length > 1 && void 0 !== a[1] ? a[1] : 0, !(null === (r = document.getElementById(t)) && n < 4)) {
                                         e.next = 6;
                                         break
                                     }
                                     return e.next = 5, A(100 * Math.pow(2, n));
                                 case 5:
-                                    return e.abrupt("return", F(t, n + 1));
+                                    return e.abrupt("return", M(t, n + 1));
                                 case 6:
                                     return e.abrupt("return", r);
                                 case 7:
                                 case "end":
                                     return e.stop()
                             }
                         }), e)
                     })));
                     return function(t) {
                         return e.apply(this, arguments)
                     }
                 }();
             return (0, i.useEffect)((function() {
                 var e = function() {
-                    var e = dp(fp().mark((function e() {
-                        return fp().wrap((function(e) {
+                    var e = lp(up().mark((function e() {
+                        return up().wrap((function(e) {
                             for (;;) switch (e.prev = e.next) {
                                 case 0:
-                                    return e.next = 2, F(P);
+                                    return e.next = 2, M(P);
                                 case 2:
-                                    O.current = e.sent, (t = O.current) && (k.indexOf("hover") > -1 && (t.addEventListener("mouseover", $, !0), t.addEventListener("mouseout", D, !0)), k.indexOf("focus") > -1 && (t.addEventListener("focusin", $, !0), t.addEventListener("focusout", D, !0)), (k.indexOf("click") > -1 || k.indexOf("legacy") > -1) && document.addEventListener("click", I, !0), t.addEventListener("keydown", (function(e) {
+                                    O.current = e.sent, (t = O.current) && (k.indexOf("hover") > -1 && (t.addEventListener("mouseover", I, !0), t.addEventListener("mouseout", D, !0)), k.indexOf("focus") > -1 && (t.addEventListener("focusin", I, !0), t.addEventListener("focusout", D, !0)), (k.indexOf("click") > -1 || k.indexOf("legacy") > -1) && document.addEventListener("click", $, !0), t.addEventListener("keydown", (function(e) {
                                         "Escape" === e.key && R()
                                     })));
                                 case 4:
                                 case "end":
                                     return e.stop()
                             }
                             var t
                         }), e)
                     })));
                     return function() {
                         return e.apply(this, arguments)
                     }
                 }();
                 e()
-            }), [P]), l().createElement(Pp.Provider, {
+            }), [P]), l().createElement(Ep.Provider, {
                 value: {
                     handleMouseOverTooltipContent: function(e) {
                         k.indexOf("hover") > -1 && !g && (w.current && (w.current = clearTimeout(w.current)), L())
                     },
                     handleMouseLeaveTooltipContent: function(e) {
                         k.indexOf("hover") > -1 && !g && (N.current && (N.current = clearTimeout(N.current)), e.persist(), D())
                     }
                 }
-            }, l().createElement(jp, e({
+            }, l().createElement(wp, e({
                 show: v,
                 rootClose: T,
                 onHide: function() {
                     _(!1), m && E.current && m({
                         is_open: !1
                     })
                 },
                 target: O.current
             }, b), c))
         };
-        var Tp = ["placement", "className", "style", "children", "body", "arrowProps", "popper", "show", "hideArrow"],
-            Sp = ["bsPrefix", "placement", "className", "style", "children", "arrowProps", "popper", "show", "hasDoneInitialMeasure"];
+        var kp = ["placement", "className", "style", "children", "body", "arrowProps", "popper", "show", "hideArrow"],
+            Pp = ["bsPrefix", "placement", "className", "style", "children", "arrowProps", "popper", "show", "hasDoneInitialMeasure"];
 
-        function Rp(e, t) {
+        function Cp(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Dp(e) {
+        function Tp(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Rp(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Rp(Object(n)).forEach((function(t) {
+                t % 2 ? Cp(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Cp(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Lp = function(e) {
+        var Sp = function(e) {
                 var t = e;
                 return "left" === e ? t = "start" : "right" === e && (t = "end"), t
             },
-            $p = l().forwardRef((function(t, n) {
+            Rp = l().forwardRef((function(t, n) {
                 var r = t.placement,
                     a = t.className,
                     s = t.style,
                     c = t.children,
                     u = t.body,
                     d = t.arrowProps,
                     p = (t.popper, t.show, t.hideArrow),
-                    f = o(t, Tp),
+                    f = o(t, kp),
                     m = Se((null == r ? void 0 : r.split("-")) || [], 1)[0],
-                    g = Lp(m),
-                    y = (0, i.useContext)(Pp),
+                    g = Sp(m),
+                    y = (0, i.useContext)(Ep),
                     h = y.handleMouseOverTooltipContent,
                     v = y.handleMouseLeaveTooltipContent;
                 return l().createElement("div", e({
                     ref: n,
                     role: "tooltip",
                     style: s,
                     "x-placement": m,
                     className: b()(a, "popover", m && "bs-popover-".concat(g)),
                     onMouseOver: h,
                     onMouseLeave: v
                 }, f), !p && l().createElement("div", e({
                     className: "popover-arrow"
-                }, d)), u ? l().createElement(cp, null, c) : c)
+                }, d)), u ? l().createElement(op, null, c) : c)
             })),
-            Ip = l().forwardRef((function(t, n) {
+            Dp = l().forwardRef((function(t, n) {
                 t.bsPrefix;
                 var r = t.placement,
                     a = t.className,
                     s = t.style,
                     c = t.children,
                     u = t.arrowProps,
                     d = t.popper,
                     p = t.show,
                     f = t.hasDoneInitialMeasure,
-                    m = o(t, Sp),
+                    m = o(t, Pp),
                     g = Se((null == r ? void 0 : r.split("-")) || [], 1)[0],
-                    y = Lp(g),
+                    y = Sp(g),
                     h = s;
-                p && !f && (Dp(Dp({}, s), {}, {
+                p && !f && (Tp(Tp({}, s), {}, {
                     position: null == d ? void 0 : d.strategy,
                     top: "0",
                     left: "0",
                     opacity: "0",
                     pointerEvents: "none"
                 }), function(e) {
                     throw new TypeError('"computedStyle" is read-only')
                 }());
-                var v = (0, i.useContext)(Pp),
+                var v = (0, i.useContext)(Ep),
                     _ = v.handleMouseOverTooltipContent,
                     x = v.handleMouseLeaveTooltipContent;
                 return l().createElement("div", e({
                     ref: n,
                     style: h,
                     role: "tooltip",
                     "x-placement": g,
@@ -10504,60 +10454,60 @@
                     onMouseLeave: x
                 }, m), l().createElement("div", e({
                     className: "tooltip-arrow"
                 }, u)), l().createElement("div", {
                     className: "tooltip-inner"
                 }, c))
             })),
-            Ap = ["children", "is_open", "loading_state", "className", "class_name", "style", "id", "hide_arrow", "offset", "body"],
-            Fp = function(t) {
+            Lp = ["children", "is_open", "loading_state", "className", "class_name", "style", "id", "hide_arrow", "offset", "body"],
+            Ip = function(t) {
                 var n = t.children,
                     r = t.is_open,
                     a = t.loading_state,
                     s = t.className,
                     i = t.class_name,
                     c = t.style,
                     u = t.id,
                     d = t.hide_arrow,
                     p = t.offset,
                     f = t.body,
-                    g = o(t, Ap),
+                    g = o(t, Lp),
                     b = p ? {
                         modifiers: [{
                             name: "offset",
                             options: {
                                 offset: "string" == typeof p ? p.split(",").map((function(e) {
                                     return parseInt(e)
                                 })) : [0, p]
                             }
                         }]
                     } : {};
-                return l().createElement(Cp, e({
+                return l().createElement(jp, e({
                     "data-dash-is-loading": a && a.is_loading || void 0,
                     defaultShow: r,
                     popperConfig: b
-                }, m(["persistence", "persisted_props", "persistence_type"], g)), l().createElement($p, {
+                }, m(["persistence", "persisted_props", "persistence_type"], g)), l().createElement(Rp, {
                     style: c,
                     id: u,
                     className: i || s,
                     hideArrow: d,
                     body: f
                 }, n))
             };
-        Fp.defaultProps = {
+        Ip.defaultProps = {
             delay: {
                 show: 0,
                 hide: 50
             },
             placement: "right",
             flip: !0,
             autohide: !1,
             persisted_props: ["is_open"],
             persistence_type: "local"
-        }, Fp.propTypes = {
+        }, Ip.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             placement: u().oneOf(["auto", "auto-start", "auto-end", "top", "top-start", "top-end", "right", "right-start", "right-end", "bottom", "bottom-start", "bottom-end", "left", "left-start", "left-end"]),
@@ -10580,214 +10530,214 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["is_open"])),
             persistence_type: u().oneOf(["local", "session", "memory"])
         };
-        const Mp = Fp;
-        var Bp = ["children", "loading_state", "className", "class_name"],
-            zp = function(t) {
+        const $p = Ip;
+        var Ap = ["children", "loading_state", "className", "class_name"],
+            Mp = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Bp);
-                return l().createElement(cp, e({
+                    i = o(t, Ap);
+                return l().createElement(op, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        zp.propTypes = {
+        Mp.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Kp = zp;
-        var Hp = ["children", "loading_state", "className", "class_name"],
-            Up = function(t) {
+        const Fp = Mp;
+        var Bp = ["children", "loading_state", "className", "class_name"],
+            zp = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Hp);
-                return l().createElement(hp, e({
+                    i = o(t, Bp);
+                return l().createElement(gp, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Up.propTypes = {
+        zp.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Wp = Up;
-        var qp = ["min", "now", "max", "label", "visuallyHidden", "striped", "animated", "className", "style", "variant", "barStyle"],
-            Vp = ["isChild", "min", "max"],
-            Gp = ["now", "label", "visuallyHidden", "striped", "animated", "variant", "className", "children", "barStyle"],
-            Yp = ["children", "loading_state", "color", "className", "class_name", "value", "hide_label", "bar"];
+        const Kp = zp;
+        var Hp = ["min", "now", "max", "label", "visuallyHidden", "striped", "animated", "className", "style", "variant", "barStyle"],
+            Wp = ["isChild", "min", "max"],
+            Up = ["now", "label", "visuallyHidden", "striped", "animated", "variant", "className", "children", "barStyle"],
+            qp = ["children", "loading_state", "color", "className", "class_name", "value", "hide_label", "bar"];
 
-        function Xp(e, t) {
+        function Vp(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Jp(e) {
+        function Gp(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Xp(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Xp(Object(n)).forEach((function(t) {
+                t % 2 ? Vp(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Vp(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Qp = l().createContext({}),
-            Zp = 1e3;
+        var Yp = l().createContext({}),
+            Xp = 1e3;
 
-        function ef(e, t, n) {
+        function Jp(e, t, n) {
             var r = (e - t) / (n - t) * 100;
-            return Math.round(r * Zp) / Zp
+            return Math.round(r * Xp) / Xp
         }
 
-        function tf(t, n) {
+        function Qp(t, n) {
             var r = t.min,
                 a = t.now,
                 s = t.max,
                 i = t.label,
                 c = t.visuallyHidden,
                 u = t.striped,
                 d = t.animated,
                 p = t.className,
                 f = t.style,
                 m = t.variant,
                 g = t.barStyle,
-                y = o(t, qp);
+                y = o(t, Hp);
             return l().createElement("div", e({
                 ref: n
             }, y, {
                 role: "progressbar",
-                className: b()(p, "progress-bar", Ve(Ve(Ve({}, "bg-".concat(m), m), "progress-bar-animated", d), "progress-bar-striped", d || u)),
-                style: Jp(Jp({
-                    width: "".concat(ef(a, r, s), "%")
+                className: b()(p, "progress-bar", Ue(Ue(Ue({}, "bg-".concat(m), m), "progress-bar-animated", d), "progress-bar-striped", d || u)),
+                style: Gp(Gp({
+                    width: "".concat(Jp(a, r, s), "%")
                 }, f), g),
                 "aria-valuenow": a,
                 "aria-valuemin": r,
                 "aria-valuemax": s
             }), c ? l().createElement("span", {
                 className: "visually-hidden"
             }, i) : i)
         }
-        var nf = l().forwardRef((function(t, n) {
+        var Zp = l().forwardRef((function(t, n) {
             var r = t.isChild,
                 a = t.min,
                 s = t.max,
-                c = o(t, Vp);
+                c = o(t, Wp);
             if (r) {
-                var u = (0, i.useContext)(Qp);
-                return tf(Jp(Jp({}, c), {}, {
+                var u = (0, i.useContext)(Yp);
+                return Qp(Gp(Gp({}, c), {}, {
                     max: s || u.max,
                     min: a || u.min
                 }), n)
             }
             var d = c.now,
                 p = c.label,
                 f = c.visuallyHidden,
                 m = c.striped,
                 g = c.animated,
                 y = c.variant,
                 h = c.className,
                 v = c.children,
                 _ = c.barStyle,
-                x = o(c, Gp);
+                x = o(c, Up);
             return a = void 0 === a ? 0 : a, s = void 0 === s ? 100 : s, l().createElement("div", e({
                 ref: n
             }, x, {
                 className: b()(h, "progress")
-            }), l().createElement(Qp.Provider, {
+            }), l().createElement(Yp.Provider, {
                 value: {
                     min: a,
                     max: s
                 }
-            }, v ? hr(v, (function(e) {
+            }, v ? mr(v, (function(e) {
                 return (0, i.cloneElement)(e, {
                     isChild: !0
                 })
-            })) : tf({
+            })) : Qp({
                 min: a,
                 now: d,
                 max: s,
                 label: p,
                 visuallyHidden: f,
                 striped: m,
                 animated: g,
                 variant: y,
                 barStyle: _
             }, n)))
         }));
-        nf.defaultProps = {
+        Zp.defaultProps = {
             animated: !1,
             isChild: !1,
             visuallyHidden: !1,
             striped: !1
         };
-        var rf = function(t) {
+        var ef = function(t) {
             var n = t.children,
                 r = t.loading_state,
                 a = t.color,
                 s = t.className,
                 i = t.class_name,
                 c = t.value,
                 u = t.hide_label,
                 d = t.bar,
-                p = o(t, Yp),
-                f = Ot.has(a);
-            return l().createElement(nf, e({
+                p = o(t, qp),
+                f = _t.has(a);
+            return l().createElement(Zp, e({
                 className: i || s
             }, m(["setProps"], p), {
                 "data-dash-is-loading": r && r.is_loading || void 0,
                 now: c,
                 isChild: d,
                 variant: f ? a : null,
                 visuallyHidden: u,
                 barStyle: f ? {} : {
                     backgroundColor: a
                 }
             }), n)
         };
-        rf.defaultProps = {
+        ef.defaultProps = {
             hide_label: !1
-        }, rf.propTypes = {
+        }, ef.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             bar: u().bool,
@@ -10801,39 +10751,39 @@
             color: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const af = rf;
+        const tf = ef;
 
-        function sf(e, t) {
+        function nf(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function of(e) {
+        function rf(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? sf(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : sf(Object(n)).forEach((function(t) {
+                t % 2 ? nf(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : nf(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var lf = function(e) {
+        var af = function(e) {
             var t = e.id,
                 n = e.className,
                 r = e.class_name,
                 a = e.style,
                 s = e.options,
                 o = e.key,
                 i = e.loading_state,
@@ -10858,15 +10808,15 @@
                             _ = e.labelCheckedStyle,
                             x = e.label_checked_style,
                             O = e.setProps,
                             w = e.inline,
                             N = e.value,
                             E = e.switch,
                             j = t.value === N,
-                            k = j ? of(of({}, v || h), x || _) : v || h,
+                            k = j ? rf(rf({}, v || h), x || _) : v || h,
                             P = t.input_id || "_dbcprivate_radioitems_".concat(n, "_input_").concat(t.value);
                         return l().createElement("div", {
                             className: b()("form-check", w && "form-check-inline", E && "form-switch"),
                             key: t.value
                         }, l().createElement("input", {
                             id: P,
                             name: c,
@@ -10894,15 +10844,15 @@
                 id: t,
                 className: r || n,
                 style: a,
                 key: o,
                 "data-dash-is-loading": i && i.is_loading || void 0
             }, u)
         };
-        lf.propTypes = {
+        af.propTypes = {
             options: u().oneOfType([u().arrayOf(u().oneOfType([u().string, u().number])), u().object, u().arrayOf(u().exact({
                 label: u().node.isRequired,
                 value: u().oneOfType([u().string, u().number]).isRequired,
                 disabled: u().bool,
                 input_id: u().string,
                 label_id: u().string
             }))]),
@@ -10936,29 +10886,29 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             name: u().string
-        }, lf.defaultProps = {
+        }, af.defaultProps = {
             inputStyle: {},
             input_style: null,
             inputClassName: "",
             input_class_name: "",
             labelStyle: {},
             label_style: null,
             labelClassName: "",
             label_class_name: "",
             options: [],
             persisted_props: ["value"],
             persistence_type: "local"
         };
-        const cf = lf;
-        var uf = function(e) {
+        const sf = af;
+        var of = function(e) {
             var t = e.value,
                 n = e.disabled,
                 r = e.className,
                 a = e.class_name,
                 s = e.style,
                 o = e.id,
                 i = e.input_class_name,
@@ -10993,15 +10943,15 @@
             }), l().createElement("label", {
                 id: p,
                 style: f,
                 className: b()(m || g, "form-check-label", "form-label"),
                 htmlFor: o
             }, d))
         };
-        uf.propTypes = {
+        of.propTypes = {
             id: u().string,
             class_name: u().string,
             className: u().string,
             style: u().object,
             input_style: u().object,
             inputStyle: u().object,
             input_class_name: u().string,
@@ -11020,30 +10970,30 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             setProps: u().func
-        }, uf.defaultProps = {
+        }, of.defaultProps = {
             inputStyle: {},
             input_style: null,
             inputClassName: "",
             input_class_name: "",
             labelStyle: {},
             label_style: null,
             labelClassName: "",
             label_class_name: "",
             persisted_props: ["value"],
             persistence_type: "local",
             value: !1,
             disabled: !1
         };
-        const df = uf,
-            pf = i.forwardRef((({
+        const lf = of,
+            cf = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 as: n = "div",
                 ...r
             }, a) => {
                 const s = E(e, "row"),
                     o = j(),
@@ -11060,75 +11010,75 @@
                     null != n && c.push(`${l}${a}-${n}`)
                 })), (0, _.jsx)(n, {
                     ref: a,
                     ...r,
                     className: b()(t, s, ...c)
                 })
             }));
-        pf.displayName = "Row";
-        const ff = pf;
-        var mf = ["children", "className", "class_name", "align", "justify", "loading_state"],
-            gf = {
+        cf.displayName = "Row";
+        const uf = cf;
+        var df = ["children", "className", "class_name", "align", "justify", "loading_state"],
+            pf = {
                 start: "align-items-start",
                 center: "align-items-center",
                 end: "align-items-end",
                 stretch: "align-items-stretch",
                 baseline: "align-items-baseline"
             },
-            bf = {
+            ff = {
                 start: "justify-content-start",
                 center: "justify-content-center",
                 end: "justify-content-end",
                 around: "justify-content-around",
                 between: "justify-content-between",
                 evenly: "justify-content-evenly"
             },
-            yf = function(t) {
+            mf = function(t) {
                 var n = t.children,
                     r = t.className,
                     a = t.class_name,
                     s = t.align,
                     i = t.justify,
                     c = t.loading_state,
-                    u = o(t, mf),
-                    d = s && gf[s],
-                    p = i && bf[i],
+                    u = o(t, df),
+                    d = s && pf[s],
+                    p = i && ff[i],
                     f = b()(a || r, d, p);
-                return l().createElement(ff, e({
+                return l().createElement(uf, e({
                     className: f
                 }, m(["setProps"], u), {
                     "data-dash-is-loading": c && c.is_loading || void 0
                 }), n)
             };
-        yf.propTypes = {
+        mf.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             align: u().oneOf(["start", "center", "end", "stretch", "baseline"]),
             justify: u().oneOf(["start", "center", "end", "around", "between", "evenly"]),
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const hf = yf;
-        var vf = ["className", "class_name", "html_size", "valid", "invalid", "value"],
-            _f = function(t) {
+        const gf = mf;
+        var bf = ["className", "class_name", "html_size", "valid", "invalid", "value"],
+            yf = function(t) {
                 var n = t.className,
                     r = t.class_name,
                     a = t.html_size,
                     s = t.valid,
                     i = t.invalid,
                     c = t.value,
-                    u = o(t, vf);
-                return l().createElement(dl, e({}, m(["setProps", "options", "persistence", "persistence_type", "persisted_props", "loading_state"], u), {
+                    u = o(t, bf);
+                return l().createElement(il, e({}, m(["setProps", "options", "persistence", "persistence_type", "persisted_props", "loading_state"], u), {
                     isInvalid: i,
                     isValid: s,
                     onChange: function(e) {
                         t.setProps && t.setProps({
                             value: e.target.value
                         })
                     },
@@ -11144,20 +11094,20 @@
                         key: e.value,
                         value: e.value,
                         disabled: e.disabled,
                         title: e.title
                     }, e.label)
                 })))
             };
-        _f.defaultProps = {
+        yf.defaultProps = {
             value: "",
             persisted_props: ["value"],
             persistence_type: "local",
             placeholder: ""
-        }, _f.propTypes = {
+        }, yf.propTypes = {
             options: u().oneOfType([u().arrayOf(u().oneOfType([u().string, u().number])), u().object, u().arrayOf(u().exact({
                 label: u().oneOfType([u().string, u().number]).isRequired,
                 value: u().string.isRequired,
                 disabled: u().bool,
                 title: u().string
             }))]),
             value: u().oneOfType([u().string, u().number]),
@@ -11174,16 +11124,16 @@
             size: u().string,
             html_size: u().string,
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             name: u().string
         };
-        const xf = _f,
-            Of = i.forwardRef((({
+        const hf = yf,
+            vf = i.forwardRef((({
                 bsPrefix: e,
                 variant: t,
                 animation: n = "border",
                 size: r,
                 as: a = "div",
                 className: s,
                 ...o
@@ -11191,95 +11141,95 @@
                 const l = `${e=E(e,"spinner")}-${n}`;
                 return (0, _.jsx)(a, {
                     ref: i,
                     ...o,
                     className: b()(s, l, r && `${l}-${r}`, t && `text-${t}`)
                 })
             }));
-        Of.displayName = "Spinner";
-        const wf = Of;
-        var Nf = ["children", "color", "loading_state", "spinner_style", "spinnerClassName", "spinner_class_name", "fullscreen", "fullscreenClassName", "fullscreen_class_name", "fullscreen_style", "delay_hide", "delay_show", "show_initially", "type"];
+        vf.displayName = "Spinner";
+        const _f = vf;
+        var xf = ["children", "color", "loading_state", "spinner_style", "spinnerClassName", "spinner_class_name", "fullscreen", "fullscreenClassName", "fullscreen_class_name", "fullscreen_style", "delay_hide", "delay_show", "show_initially", "type"];
 
-        function Ef(e, t) {
+        function Of(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function jf(e) {
+        function wf(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Ef(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ef(Object(n)).forEach((function(t) {
+                t % 2 ? Of(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Of(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var kf = function(t) {
+        var Nf = function(t) {
             var n = t.children,
                 r = t.color,
                 a = t.loading_state,
                 s = t.spinner_style,
                 c = t.spinnerClassName,
                 u = t.spinner_class_name,
                 d = t.fullscreen,
                 p = t.fullscreenClassName,
                 f = t.fullscreen_class_name,
                 g = t.fullscreen_style,
                 b = t.delay_hide,
                 y = t.delay_show,
                 h = t.show_initially,
                 v = t.type,
-                _ = o(t, Nf),
+                _ = o(t, xf),
                 x = Se((0, i.useState)(h), 2),
                 O = x[0],
                 w = x[1],
                 N = (0, i.useRef)(),
                 E = (0, i.useRef)();
             (0, i.useEffect)((function() {
                 a && (a.is_loading ? (N.current && (N.current = clearTimeout(N.current)), O || E.current || (E.current = setTimeout((function() {
                     w(!0), E.current = null
                 }), y))) : (E.current && (E.current = clearTimeout(E.current)), O && !N.current && (N.current = setTimeout((function() {
                     w(!1), N.current = null
                 }), b))))
             }), [b, y, a]);
-            var j = Ot.has(r),
-                k = jf({
+            var j = _t.has(r),
+                k = wf({
                     position: "fixed",
                     width: "100vw",
                     height: "100vh",
                     top: 0,
                     left: 0,
                     backgroundColor: "white",
                     display: "flex",
                     justifyContent: "center",
                     alignItems: "center",
                     zIndex: 99,
                     visibility: "visible"
                 }, g),
                 P = function(t) {
                     var n = t.style;
-                    return l().createElement(wf, e({
+                    return l().createElement(_f, e({
                         variant: j ? r : null,
                         animation: v,
-                        style: jf({
+                        style: wf({
                             color: !j && r
                         }, n),
                         className: u || c
                     }, m(["setProps"], _)))
                 };
             if (n) {
-                var C = jf({
+                var C = wf({
                     display: "block",
                     margin: "1rem auto"
                 }, s);
                 return l().createElement("div", {
                     style: O ? {
                         visibility: "hidden",
                         position: "relative"
@@ -11305,20 +11255,20 @@
                 style: k
             }, l().createElement(P, {
                 style: s
             })) : l().createElement(P, {
                 style: s
             })
         };
-        kf._dashprivate_isLoadingComponent = !0, kf.defaultProps = {
+        Nf._dashprivate_isLoadingComponent = !0, Nf.defaultProps = {
             delay_hide: 0,
             delay_show: 0,
             show_initially: !0,
             type: "border"
-        }, kf.propTypes = {
+        }, Nf.propTypes = {
             id: u().string,
             children: u().node,
             fullscreen_style: u().object,
             spinner_style: u().object,
             fullscreen_class_name: u().string,
             fullscreenClassName: u().string,
             spinner_class_name: u().string,
@@ -11327,81 +11277,81 @@
             type: u().string,
             size: u().string,
             fullscreen: u().bool,
             delay_hide: u().number,
             delay_show: u().number,
             show_initially: u().bool
         };
-        const Pf = kf;
+        const Ef = Nf;
 
-        function Cf(e, t = x, n = "xs") {
+        function jf(e, t = x, n = "xs") {
             const r = [];
             return Object.entries(e).forEach((([e, a]) => {
                 null != a && ("object" == typeof a ? t.forEach((t => {
                     const s = a[t];
                     if (null != s) {
                         const a = t !== n ? `-${t}` : "";
                         r.push(`${e}${a}-${s}`)
                     }
                 })) : r.push(`${e}-${a}`))
             })), r
         }
-        const Tf = i.forwardRef((({
+        const kf = i.forwardRef((({
             as: e = "div",
             bsPrefix: t,
             className: n,
             direction: r,
             gap: a,
             ...s
         }, o) => {
             t = E(t, "horizontal" === r ? "hstack" : "vstack");
             const i = j(),
                 l = k();
             return (0, _.jsx)(e, {
                 ...s,
                 ref: o,
-                className: b()(n, t, ...Cf({
+                className: b()(n, t, ...jf({
                     gap: a
                 }, i, l))
             })
         }));
-        Tf.displayName = "Stack";
-        const Sf = Tf;
-        var Rf = ["children", "loading_state", "className", "class_name"],
-            Df = function(t) {
+        kf.displayName = "Stack";
+        const Pf = kf;
+        var Cf = ["children", "loading_state", "className", "class_name"],
+            Tf = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Rf);
-                return l().createElement(Sf, e({
+                    i = o(t, Cf);
+                return l().createElement(Pf, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Df.defaultPropTypes = {
+        Tf.defaultPropTypes = {
             direction: "vertical"
-        }, Df.propTypes = {
+        }, Tf.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             direction: u().oneOf(["vertical", "horizontal"]),
             gap: u().number
         };
-        const Lf = Df;
-        var $f = function(e) {
+        const Sf = Tf;
+        var Rf = function(e) {
             var t = e.value,
                 n = e.disabled,
                 r = e.className,
                 a = e.class_name,
                 s = e.style,
                 o = e.id,
                 i = e.input_class_name,
@@ -11435,15 +11385,15 @@
             }), l().createElement("label", {
                 id: p,
                 style: f,
                 className: b()(m || g, "form-check-label", "form-label"),
                 htmlFor: o
             }, d))
         };
-        $f.propTypes = {
+        Rf.propTypes = {
             id: u().string,
             class_name: u().string,
             className: u().string,
             style: u().object,
             input_style: u().object,
             inputStyle: u().object,
             input_class_name: u().string,
@@ -11462,35 +11412,35 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             setProps: u().func
-        }, $f.defaultProps = {
+        }, Rf.defaultProps = {
             inputStyle: {},
             input_style: null,
             inputClassName: "",
             input_class_name: "",
             labelStyle: {},
             label_style: null,
             labelClassName: "",
             label_class_name: "",
             persisted_props: ["value"],
             persistence_type: "local",
             value: !1,
             disabled: !1
         };
-        const If = $f;
-        var Af = function(e) {
+        const Df = Rf;
+        var Lf = function(e) {
             return l().createElement("div", null, e.children)
         };
-        Af.defaultProps = {
+        Lf.defaultProps = {
             disabled: !1
-        }, Af.propTypes = {
+        }, Lf.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             tab_style: u().object,
             active_tab_style: u().object,
             label_style: u().object,
             active_label_style: u().object,
@@ -11510,43 +11460,43 @@
             disabled: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Ff = Af,
-            Mf = ["active", "eventKey", "mountOnEnter", "transition", "unmountOnExit", "role", "onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited"],
-            Bf = ["activeKey", "getControlledId", "getControllerId"],
-            zf = ["as"];
+        const If = Lf,
+            $f = ["active", "eventKey", "mountOnEnter", "transition", "unmountOnExit", "role", "onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited"],
+            Af = ["activeKey", "getControlledId", "getControllerId"],
+            Mf = ["as"];
 
-        function Kf(e, t) {
+        function Ff(e, t) {
             if (null == e) return {};
             var n, r, a = {},
                 s = Object.keys(e);
             for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
             return a
         }
 
-        function Hf(e) {
+        function Bf(e) {
             let {
                 active: t,
                 eventKey: n,
                 mountOnEnter: r,
                 transition: a,
                 unmountOnExit: s,
                 role: o = "tabpanel",
                 onEnter: l,
                 onEntering: c,
                 onEntered: u,
                 onExit: d,
                 onExiting: p,
                 onExited: f
-            } = e, m = Kf(e, Mf);
-            const g = (0, i.useContext)(pi);
+            } = e, m = Ff(e, $f);
+            const g = (0, i.useContext)(li);
             if (!g) return [Object.assign({}, m, {
                 role: o
             }), {
                 eventKey: n,
                 isActive: t,
                 mountOnEnter: r,
                 transition: a,
@@ -11558,52 +11508,52 @@
                 onExiting: p,
                 onExited: f
             }];
             const {
                 activeKey: b,
                 getControlledId: y,
                 getControllerId: h
-            } = g, v = Kf(g, Bf), _ = Co(n);
+            } = g, v = Ff(g, Af), _ = Eo(n);
             return [Object.assign({}, m, {
                 role: o,
                 id: y(n),
                 "aria-labelledby": h(n)
             }), {
                 eventKey: n,
-                isActive: null == t && null != _ ? Co(b) === _ : t,
+                isActive: null == t && null != _ ? Eo(b) === _ : t,
                 transition: a || v.transition,
                 mountOnEnter: null != r ? r : v.mountOnEnter,
                 unmountOnExit: null != s ? s : v.unmountOnExit,
                 onEnter: l,
                 onEntering: c,
                 onEntered: u,
                 onExit: d,
                 onExiting: p,
                 onExited: f
             }]
         }
-        const Uf = i.forwardRef(((e, t) => {
+        const zf = i.forwardRef(((e, t) => {
             let {
                 as: n = "div"
-            } = e, r = Kf(e, zf);
+            } = e, r = Ff(e, Mf);
             const [a, {
                 isActive: s,
                 onEnter: o,
                 onEntering: i,
                 onEntered: l,
                 onExit: c,
                 onExiting: u,
                 onExited: d,
                 mountOnEnter: p,
                 unmountOnExit: f,
-                transition: m = Cc
-            }] = Hf(r);
-            return (0, _.jsx)(pi.Provider, {
+                transition: m = Ec
+            }] = Bf(r);
+            return (0, _.jsx)(li.Provider, {
                 value: null,
-                children: (0, _.jsx)(To.Provider, {
+                children: (0, _.jsx)(jo.Provider, {
                     value: null,
                     children: (0, _.jsx)(m, {
                         in: s,
                         onEnter: o,
                         onEntering: i,
                         onEntered: l,
                         onExit: c,
@@ -11616,71 +11566,71 @@
                             hidden: !s,
                             "aria-hidden": !s
                         }))
                     })
                 })
             })
         }));
-        Uf.displayName = "TabPanel";
-        const Wf = e => {
+        zf.displayName = "TabPanel";
+        const Kf = e => {
             const {
                 id: t,
                 generateChildId: n,
                 onSelect: r,
                 activeKey: a,
                 defaultActiveKey: s,
                 transition: o,
                 mountOnEnter: l,
                 unmountOnExit: c,
                 children: u
-            } = e, [d, p] = Ta(a, s, r), f = _o(t), m = (0, i.useMemo)((() => n || ((e, t) => f ? `${f}-${t}-${e}` : null)), [f, n]), g = (0, i.useMemo)((() => ({
+            } = e, [d, p] = ja(a, s, r), f = bo(t), m = (0, i.useMemo)((() => n || ((e, t) => f ? `${f}-${t}-${e}` : null)), [f, n]), g = (0, i.useMemo)((() => ({
                 onSelect: p,
                 activeKey: d,
                 transition: o,
                 mountOnEnter: l || !1,
                 unmountOnExit: c || !1,
                 getControlledId: e => m(e, "tabpane"),
                 getControllerId: e => m(e, "tab")
             })), [p, d, o, l, c, m]);
-            return (0, _.jsx)(pi.Provider, {
+            return (0, _.jsx)(li.Provider, {
                 value: g,
-                children: (0, _.jsx)(To.Provider, {
+                children: (0, _.jsx)(jo.Provider, {
                     value: p || null,
                     children: u
                 })
             })
         };
-        Wf.Panel = Uf;
-        const qf = Wf;
+        Kf.Panel = zf;
+        const Hf = Kf;
 
-        function Vf(e) {
-            return "boolean" == typeof e ? e ? bt : Cc : e
+        function Wf(e) {
+            return "boolean" == typeof e ? e ? mt : Ec : e
         }
-        const Gf = ({
+        const Uf = ({
             transition: e,
             ...t
-        }) => (0, _.jsx)(qf, {
+        }) => (0, _.jsx)(Hf, {
             ...t,
-            transition: Vf(e)
+            transition: Wf(e)
         });
-        Gf.displayName = "TabContainer";
-        const Yf = Gf,
-            Xf = i.forwardRef((({
+        Uf.displayName = "TabContainer";
+        const qf = Uf,
+            Vf = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "tab-content"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        Xf.displayName = "TabContent";
-        const Jf = Xf,
-            Qf = i.forwardRef((({
+        Vf.displayName = "TabContent";
+        const Gf = Vf,
+            Yf = i.forwardRef((({
                 bsPrefix: e,
                 transition: t,
                 ...n
             }, r) => {
                 const [{
                     className: a,
                     as: s = "div",
@@ -11691,22 +11641,22 @@
                     onEntering: c,
                     onEntered: u,
                     onExit: d,
                     onExiting: p,
                     onExited: f,
                     mountOnEnter: m,
                     unmountOnExit: g,
-                    transition: y = bt
-                }] = Hf({
+                    transition: y = mt
+                }] = Bf({
                     ...n,
-                    transition: Vf(t)
+                    transition: Wf(t)
                 }), h = E(e, "tab-pane");
-                return (0, _.jsx)(pi.Provider, {
+                return (0, _.jsx)(li.Provider, {
                     value: null,
-                    children: (0, _.jsx)(To.Provider, {
+                    children: (0, _.jsx)(jo.Provider, {
                         value: null,
                         children: (0, _.jsx)(y, {
                             in: i,
                             onEnter: l,
                             onEntering: c,
                             onEntered: u,
                             onExit: d,
@@ -11719,130 +11669,130 @@
                                 ref: r,
                                 className: b()(a, h, i && "active")
                             })
                         })
                     })
                 })
             }));
-        Qf.displayName = "TabPane";
-        const Zf = Qf,
-            em = {
+        Yf.displayName = "TabPane";
+        const Xf = Yf,
+            Jf = {
                 eventKey: u().oneOfType([u().string, u().number]),
                 title: u().node.isRequired,
                 disabled: u().bool,
                 tabClassName: u().string,
                 tabAttrs: u().object
             },
-            tm = () => {
+            Qf = () => {
                 throw new Error("ReactBootstrap: The `Tab` component is not meant to be rendered! It's an abstract component that is only valid as a direct Child of the `Tabs` Component. For custom tabs components use TabPane and TabsContainer directly")
             };
-        tm.propTypes = em;
-        const nm = Object.assign(tm, {
-            Container: Yf,
-            Content: Jf,
-            Pane: Zf
+        Qf.propTypes = Jf;
+        const Zf = Object.assign(Qf, {
+            Container: qf,
+            Content: Gf,
+            Pane: Xf
         });
-        var rm = ["children", "tab_id", "id", "label", "tab_style", "active_tab_style", "label_style", "active_label_style", "tabClassName", "tab_class_name", "activeTabClassName", "active_tab_class_name", "labelClassName", "label_class_name", "activeLabelClassName", "active_label_class_name", "loading_state"];
+        var em = ["children", "tab_id", "id", "label", "tab_style", "active_tab_style", "label_style", "active_label_style", "tabClassName", "tab_class_name", "activeTabClassName", "active_tab_class_name", "labelClassName", "label_class_name", "activeLabelClassName", "active_label_class_name", "loading_state"];
 
-        function am(e, t) {
+        function tm(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function sm(e) {
+        function nm(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? am(Object(n), !0).forEach((function(t) {
-                    Ve(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : am(Object(n)).forEach((function(t) {
+                t % 2 ? tm(Object(n), !0).forEach((function(t) {
+                    Ue(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : tm(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var om = function(t) {
+        var rm = function(t) {
             var n = t.children,
                 r = t.id,
                 a = t.className,
                 s = t.class_name,
                 c = t.style,
                 u = t.active_tab,
                 d = t.key,
                 p = t.loading_state,
                 f = t.setProps;
-            n = Le(n), (0, i.useEffect)((function() {
+            n = De(n), (0, i.useEffect)((function() {
                 f && void 0 === u && f({
-                    active_tab: n && ($e(n[0]).tab_id || "tab-0")
+                    active_tab: n && (Le(n[0]).tab_id || "tab-0")
                 })
             }), []);
             var g = n && n.map((function(e, t) {
-                    var n = $e(e),
+                    var n = Le(e),
                         r = n.key || n.tab_id || "tab-" + t,
                         a = u === r;
-                    return l().createElement(ki.Item, {
-                        id: Ae(n.id),
+                    return l().createElement(wi.Item, {
+                        id: $e(n.id),
                         key: r,
-                        style: a ? sm(sm({}, n.tab_style), n.active_tab_style) : n.tab_style,
+                        style: a ? nm(nm({}, n.tab_style), n.active_tab_style) : n.tab_style,
                         className: b()(n.tab_class_name || n.tabClassName, a && (n.active_tab_class_name || n.activeTabClassName))
-                    }, l().createElement(ki.Link, {
+                    }, l().createElement(wi.Link, {
                         className: b()(n.label_class_name || n.labelClassName, a && (n.active_label_class_name || n.activeLabelClassName), {
                             active: a
                         }),
-                        style: sm(sm(sm({}, !n.disabled && {
+                        style: nm(nm(nm({}, !n.disabled && {
                             cursor: "pointer"
                         }), n.label_style), a && n.active_label_style),
                         disabled: n.disabled,
                         onClick: function() {
                             var e;
                             n.disabled || (e = r, f && u !== e && f({
                                 active_tab: e
                             }))
                         }
                     }, n.label))
                 })),
                 y = n && n.map((function(t, n) {
-                    var r = $e(t),
+                    var r = Le(t),
                         a = (r.children, r.tab_id),
                         s = (r.id, r.label, r.tab_style, r.active_tab_style, r.label_style, r.active_label_style, r.tabClassName, r.tab_class_name, r.activeTabClassName, r.active_tab_class_name, r.labelClassName, r.label_class_name, r.activeLabelClassName, r.active_label_class_name, r.loading_state),
-                        i = o(r, rm),
+                        i = o(r, em),
                         c = a || "tab-" + n;
-                    return l().createElement(nm.Pane, e({
+                    return l().createElement(Zf.Pane, e({
                         eventKey: c,
                         key: c
                     }, m(["setProps", "persistence", "persistence_type", "persisted_props"], i), {
                         "data-dash-is-loading": s && s.is_loading || void 0
                     }), t)
                 }));
-            return l().createElement(nm.Container, {
+            return l().createElement(Zf.Container, {
                 key: d,
                 activeKey: u,
                 onSelect: function(e) {
                     return f({
                         active_tab: e
                     })
                 },
                 "data-dash-is-loading": p && p.is_loading || void 0
-            }, l().createElement(ki, {
+            }, l().createElement(wi, {
                 id: r,
                 variant: "tabs",
                 as: "ul",
                 className: s || a,
                 style: c
-            }, g), l().createElement(nm.Content, null, y))
+            }, g), l().createElement(Zf.Content, null, y))
         };
-        om.defaultProps = {
+        rm.defaultProps = {
             persisted_props: ["active_tab"],
             persistence_type: "local"
-        }, om.propTypes = {
+        }, rm.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             active_tab: u().string,
@@ -11851,16 +11801,16 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["active_tab"])),
             persistence_type: u().oneOf(["local", "session", "memory"])
         };
-        const im = om,
-            lm = i.forwardRef((({
+        const am = rm,
+            sm = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 striped: n,
                 bordered: r,
                 borderless: a,
                 hover: s,
                 size: o,
@@ -11880,32 +11830,32 @@
                     return "string" == typeof l && (e = `${e}-${l}`), (0, _.jsx)("div", {
                         className: e,
                         children: f
                     })
                 }
                 return f
             })),
-            cm = lm;
-        var um = ["children", "loading_state", "className", "class_name", "color", "dark"],
-            dm = function(t) {
+            om = sm;
+        var im = ["children", "loading_state", "className", "class_name", "color", "dark"],
+            lm = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.color,
                     c = t.dark,
-                    u = o(t, um);
-                return l().createElement(cm, e({
+                    u = o(t, im);
+                return l().createElement(om, e({
                     className: s || a,
                     variant: i || (c ? "dark" : void 0)
                 }, m(["setProps"], u), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        dm.propTypes = {
+        lm.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             size: u().string,
@@ -11918,17 +11868,17 @@
             responsive: u().oneOfType([u().bool, u().string]),
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const pm = dm;
-        var fm = ["value", "n_clicks", "n_blur", "n_submit", "setProps", "className", "class_name", "invalid", "valid", "size", "debounce", "loading_state", "autoFocus", "autofocus", "maxLength", "maxlength", "minLength", "minlength", "readOnly", "readonly", "accessKey", "accesskey", "contentEditable", "contenteditable", "contextMenu", "contextmenu", "spellCheck", "spellcheck", "tabIndex", "tabindex"],
-            mm = function(t) {
+        const cm = lm;
+        var um = ["value", "n_clicks", "n_blur", "n_submit", "setProps", "className", "class_name", "invalid", "valid", "size", "debounce", "loading_state", "autoFocus", "autofocus", "maxLength", "maxlength", "minLength", "minlength", "readOnly", "readonly", "accessKey", "accesskey", "contentEditable", "contenteditable", "contextMenu", "contextmenu", "spellCheck", "spellcheck", "tabIndex", "tabindex"],
+            dm = function(t) {
                 var n = t.value,
                     r = t.n_clicks,
                     a = t.n_blur,
                     s = t.n_submit,
                     c = t.setProps,
                     u = t.className,
                     d = t.class_name,
@@ -11949,26 +11899,26 @@
                     P = t.accesskey,
                     C = t.contentEditable,
                     T = t.contenteditable,
                     S = t.contextMenu,
                     R = t.contextmenu,
                     D = t.spellCheck,
                     L = t.spellcheck,
-                    $ = t.tabIndex,
-                    I = t.tabindex,
-                    A = o(t, fm),
-                    F = Se((0, i.useState)(n || ""), 2),
-                    M = F[0],
-                    B = F[1];
+                    I = t.tabIndex,
+                    $ = t.tabindex,
+                    A = o(t, um),
+                    M = Se((0, i.useState)(n || ""), 2),
+                    F = M[0],
+                    B = M[1];
                 (0, i.useEffect)((function() {
-                    n !== M && B(n || "")
+                    n !== F && B(n || "")
                 }), [n]);
                 var z = b()(d || u, p && "is-invalid", f && "is-valid", !!g && "form-control-".concat(g), "form-control");
                 return l().createElement("textarea", e({
-                    value: M,
+                    value: F,
                     className: z,
                     onChange: function(e) {
                         var t = e.target.value;
                         B(t), !y && c && c({
                             value: t
                         })
                     },
@@ -12001,20 +11951,20 @@
                     maxLength: O || x,
                     minLength: N || w,
                     readOnly: j || E,
                     accessKey: P || k,
                     contentEditable: T || C,
                     contextMenu: R || S,
                     spellCheck: L || D,
-                    tabIndex: I || $
+                    tabIndex: $ || I
                 }, m(["n_blur_timestamp", "n_submit_timestamp", "persistence", "persistence_type", "persisted_props"], A), {
                     "data-dash-is-loading": h && h.is_loading || void 0
                 }))
             };
-        mm.propTypes = {
+        dm.propTypes = {
             id: u().string,
             key: u().string,
             value: u().string,
             autofocus: u().string,
             autoFocus: u().string,
             cols: u().oneOfType([u().string, u().number]),
             disabled: u().oneOfType([u().string, u().bool]),
@@ -12063,85 +12013,85 @@
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"])
-        }, mm.defaultProps = {
+        }, dm.defaultProps = {
             n_blur: 0,
             n_blur_timestamp: -1,
             n_submit: 0,
             n_submit_timestamp: -1,
             n_clicks: 0,
             n_clicks_timestamp: -1,
             debounce: !1,
             persisted_props: ["value"],
             persistence_type: "local",
             value: ""
         };
-        const gm = mm,
-            bm = {
+        const pm = dm,
+            fm = {
                 [z]: "showing",
                 [H]: "showing show"
             },
-            ym = i.forwardRef(((e, t) => (0, _.jsx)(bt, {
+            mm = i.forwardRef(((e, t) => (0, _.jsx)(mt, {
                 ...e,
                 ref: t,
-                transitionClasses: bm
+                transitionClasses: fm
             })));
-        ym.displayName = "ToastFade";
-        const hm = ym,
-            vm = i.createContext({
+        mm.displayName = "ToastFade";
+        const gm = mm,
+            bm = i.createContext({
                 onClose() {}
             }),
-            _m = i.forwardRef((({
+            ym = i.forwardRef((({
                 bsPrefix: e,
                 closeLabel: t = "Close",
                 closeVariant: n,
                 closeButton: r = !0,
                 className: a,
                 children: s,
                 ...o
             }, l) => {
                 e = E(e, "toast-header");
-                const c = (0, i.useContext)(vm),
-                    u = Ye((e => {
+                const c = (0, i.useContext)(bm),
+                    u = Ve((e => {
                         null == c || null == c.onClose || c.onClose(e)
                     }));
                 return (0, _.jsxs)("div", {
                     ref: l,
                     ...o,
                     className: b()(e, a),
-                    children: [s, r && (0, _.jsx)(vt, {
+                    children: [s, r && (0, _.jsx)(yt, {
                         "aria-label": t,
                         variant: n,
                         onClick: u,
                         "data-dismiss": "toast"
                     })]
                 })
             }));
-        _m.displayName = "ToastHeader";
-        const xm = _m,
-            Om = i.forwardRef((({
+        ym.displayName = "ToastHeader";
+        const hm = ym,
+            vm = i.forwardRef((({
                 className: e,
                 bsPrefix: t,
                 as: n = "div",
                 ...r
             }, a) => (t = E(t, "toast-body"), (0, _.jsx)(n, {
                 ref: a,
                 className: b()(e, t),
                 ...r
             }))));
-        Om.displayName = "ToastBody";
-        const wm = Om,
-            Nm = i.forwardRef((({
+        vm.displayName = "ToastBody";
+        const _m = vm,
+            xm = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
-                transition: n = hm,
+                transition: n = gm,
                 show: r = !0,
                 animation: a = !0,
                 delay: s = 5e3,
                 autohide: o = !1,
                 onClose: l,
                 onEntered: c,
                 onExit: u,
@@ -12154,15 +12104,15 @@
             }, h) => {
                 e = E(e, "toast");
                 const v = (0, i.useRef)(s),
                     x = (0, i.useRef)(l);
                 (0, i.useEffect)((() => {
                     v.current = s, x.current = l
                 }), [s, l]);
-                const O = fr(),
+                const O = cr(),
                     w = !(!o || !r),
                     N = (0, i.useCallback)((() => {
                         w && (null == x.current || x.current())
                     }), [w]);
                 (0, i.useEffect)((() => {
                     O.set(N, v.current)
                 }), [O, N]);
@@ -12174,36 +12124,36 @@
                         ...y,
                         ref: h,
                         className: b()(e, t, g && `bg-${g}`, !k && (r ? "show" : "hide")),
                         role: "alert",
                         "aria-live": "assertive",
                         "aria-atomic": "true"
                     });
-                return (0, _.jsx)(vm.Provider, {
+                return (0, _.jsx)(bm.Provider, {
                     value: j,
                     children: k && n ? (0, _.jsx)(n, {
                         in: r,
                         onEnter: p,
                         onEntering: f,
                         onEntered: c,
                         onExit: u,
                         onExiting: d,
                         onExited: m,
                         unmountOnExit: !0,
                         children: P
                     }) : P
                 })
             }));
-        Nm.displayName = "Toast";
-        const Em = Object.assign(Nm, {
-            Body: wm,
-            Header: xm
+        xm.displayName = "Toast";
+        const Om = Object.assign(xm, {
+            Body: _m,
+            Header: hm
         });
-        var jm = ["children", "loading_state", "header", "icon", "header_style", "headerClassName", "header_class_name", "body_style", "bodyClassName", "body_class_name", "dismissable", "duration", "n_dismiss", "is_open", "setProps", "className", "class_name", "color"],
-            km = function(t) {
+        var wm = ["children", "loading_state", "header", "icon", "header_style", "headerClassName", "header_class_name", "body_style", "bodyClassName", "body_class_name", "dismissable", "duration", "n_dismiss", "is_open", "setProps", "className", "class_name", "color"],
+            Nm = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.header,
                     s = t.icon,
                     c = t.header_style,
                     u = t.headerClassName,
                     d = t.header_class_name,
@@ -12214,35 +12164,35 @@
                     h = t.duration,
                     v = t.n_dismiss,
                     _ = t.is_open,
                     x = t.setProps,
                     O = t.className,
                     w = t.class_name,
                     N = t.color,
-                    E = o(t, jm),
+                    E = o(t, wm),
                     j = function() {
                         x && x({
                             is_open: !1,
                             n_dismiss: v + 1,
                             n_dismiss_timestamp: Date.now()
                         })
                     },
                     k = (0, i.useRef)(null);
                 return (0, i.useEffect)((function() {
                     return h && (_ ? k.current = setTimeout(j, h) : k.current && (clearTimeout(k.current), k.current = null)),
                         function() {
                             return clearTimeout(k.current)
                         }
-                }), [_]), l().createElement(Em, e({
+                }), [_]), l().createElement(Om, e({
                     show: _,
                     onClose: y && j,
                     className: w || O,
                     bg: N,
                     "data-dash-is-loading": r && r.is_loading || void 0
-                }, m(["n_dismiss_timestamp", "persistence", "persisted_props", "persistence_type", "setProps"], E)), l().createElement(Em.Header, {
+                }, m(["n_dismiss_timestamp", "persistence", "persisted_props", "persistence_type", "setProps"], E)), l().createElement(Om.Header, {
                     style: c,
                     className: d || u,
                     closeButton: y
                 }, s && l().createElement("svg", {
                     className: "rounded text-".concat(s),
                     width: "20",
                     height: "20",
@@ -12252,27 +12202,27 @@
                     role: "img"
                 }, l().createElement("rect", {
                     fill: "currentColor",
                     width: "100%",
                     height: "100%"
                 })), l().createElement("strong", {
                     className: b()("me-auto", s && "ms-2")
-                }, a)), l().createElement(Em.Body, {
+                }, a)), l().createElement(Om.Body, {
                     style: p,
                     className: g || f
                 }, n))
             };
-        km.defaultProps = {
+        Nm.defaultProps = {
             is_open: !0,
             n_dismiss: 0,
             n_dismiss_timestamp: -1,
             dismissable: !1,
             persisted_props: ["is_open"],
             persistence_type: "local"
-        }, km.propTypes = {
+        }, Nm.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             header_style: u().object,
             header_class_name: u().string,
@@ -12295,48 +12245,48 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["is_open"])),
             persistence_type: u().oneOf(["local", "session", "memory"])
         };
-        const Pm = km;
-        var Cm = ["id", "children", "is_open", "loading_state", "className", "class_name", "style", "fade"],
-            Tm = function(t) {
+        const Em = Nm;
+        var jm = ["id", "children", "is_open", "loading_state", "className", "class_name", "style", "fade"],
+            km = function(t) {
                 var n = t.id,
                     r = t.children,
                     a = t.is_open,
                     s = t.loading_state,
                     i = t.className,
                     c = t.class_name,
                     u = t.style,
                     d = t.fade,
-                    p = o(t, Cm);
-                return l().createElement(Cp, e({
+                    p = o(t, jm);
+                return l().createElement(jp, e({
                     "data-dash-is-loading": s && s.is_loading || void 0,
                     defaultShow: a
                 }, p, {
                     transition: d
-                }), l().createElement(Ip, {
+                }), l().createElement(Dp, {
                     id: n,
                     style: u,
                     className: c || i
                 }, r))
             };
-        Tm.defaultProps = {
+        km.defaultProps = {
             delay: {
                 show: 0,
                 hide: 50
             },
             placement: "auto",
             flip: !0,
             autohide: !0,
             fade: !0,
             trigger: "hover focus"
-        }, Tm.propTypes = {
+        }, km.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             target: u().oneOfType([u().string, u().object]),
@@ -12352,10 +12302,10 @@
             is_open: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Sm = Tm
+        const Pm = km
     })(), window.dash_bootstrap_components = r
 })();
```

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/metadata.json` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989346590909091%*

 * *Differences: {"'src/components/breadcrumb/Breadcrumb.js'": "{'description': 'Use breadcrumbs to create a "*

 * *                                              "navigation breadcrumb in your app.'}",*

 * * "'src/components/modal/Modal.js'": "{'props': {'dialog_style': OrderedDict([('type', "*

 * *                                    "OrderedDict([('name', 'object')])), ('required', False), "*

 * *                                    "('description', 'Inline CSS styles to apply to the "*

 * *                                    "dialog')]), 'dialogSt […]*

```diff
@@ -597,15 +597,15 @@
                 "type": {
                     "name": "string"
                 }
             }
         }
     },
     "src/components/breadcrumb/Breadcrumb.js": {
-        "description": "",
+        "description": "Use breadcrumbs to create a navigation breadcrumb in your app.",
         "displayName": "Breadcrumb",
         "methods": [],
         "props": {
             "className": {
                 "description": "**DEPRECATED** - Use class_name instead.\n\nOften used with CSS to style elements with common properties.",
                 "required": false,
                 "type": {
@@ -7430,21 +7430,49 @@
             "contentClassName": {
                 "description": "**DEPRECATED** Use `content_class_name` instead\n\nCSS class to apply to the modal content.",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
+            "contentStyle": {
+                "description": "Inline CSS styles to apply to the content",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
             "content_class_name": {
                 "description": "CSS class to apply to the modal content.",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
+            "content_style": {
+                "description": "Inline CSS styles to apply to the content",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
+            "dialogStyle": {
+                "description": "Inline CSS styles to apply to the dialog",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
+            "dialog_style": {
+                "description": "Inline CSS styles to apply to the dialog",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
             "enforceFocus": {
                 "description": "When true The modal will prevent focus from leaving the Modal while open.",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
```

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_table.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_table.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/themes.py` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/themes.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/PKG-INFO` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-bootstrap-components
-Version: 1.6.0rc1
+Version: 1.6.1rc1
 Summary: Bootstrap themed components for use in Plotly Dash
 Home-page: https://dash-bootstrap-components.opensource.faculty.ai/
 Author: Faculty
 Author-email: opensource@faculty.ai
 License: Apache Software License
 Project-URL: Bug Reports, https://github.com/facultyai/dash-bootstrap-components/issues
 Project-URL: Source, https://github.com/facultyai/dash-bootstrap-components/
@@ -110,15 +110,15 @@
 for new features please feel free to make a [feature request][feature-request].
 If you would like to submit a pull request, please read our
 [contributing guide][contribution-guide].
 
 ## Copyright and license
 
 Code and documentation is copyright [Faculty Science Ltd.][faculty]
-2018-2022, and released under the [Apache 2.0 license](./LICENSE.txt)
+2018-2024, and released under the [Apache 2.0 license](./LICENSE.txt)
 
 [dash-homepage]: https://dash.plot.ly/
 [dash-docs-external]: https:/dash.plot.ly/external-resources
 [bootstrap-homepage]: https://getbootstrap.com/
 [dbc-repo]: https://github.com/facultyai/dash-bootstrap-components
 [reactstrap-homepage]: https://reactstrap.github.io/
 [docs-homepage]: https://dash-bootstrap-components.opensource.faculty.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.6.0rc1
+Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.6.1rc1
 Summary: Bootstrap themed components for use in Plotly Dash Home-page: https://
 dash-bootstrap-components.opensource.faculty.ai/ Author: Faculty Author-email:
 opensource@faculty.ai License: Apache Software License Project-URL: Bug
 Reports, https://github.com/facultyai/dash-bootstrap-components/issues Project-
 URL: Source, https://github.com/facultyai/dash-bootstrap-components/
 Classifier: Framework :: Dash Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -40,15 +40,15 @@
 Bootstrap components. See our [_documentation_][docs-components] for a full
 list of available components. ## Contributing We welcome contributions to
 _dash-bootstrap-components_. If you find a bug or something is unclear please
 [submit a bug report][bug-report], if you have ideas for new features please
 feel free to make a [feature request][feature-request]. If you would like to
 submit a pull request, please read our [contributing guide][contribution-
 guide]. ## Copyright and license Code and documentation is copyright [Faculty
-Science Ltd.][faculty] 2018-2022, and released under the [Apache 2.0 license]
+Science Ltd.][faculty] 2018-2024, and released under the [Apache 2.0 license]
 (./LICENSE.txt) [dash-homepage]: https://dash.plot.ly/ [dash-docs-external]:
 https:/dash.plot.ly/external-resources [bootstrap-homepage]: https://
 getbootstrap.com/ [dbc-repo]: https://github.com/facultyai/dash-bootstrap-
 components [reactstrap-homepage]: https://reactstrap.github.io/ [docs-
 homepage]: https://dash-bootstrap-components.opensource.faculty.ai [docs-
 components]: https://dash-bootstrap-components.opensource.faculty.ai/l/
 components [bootstrapcdn]: https://www.bootstrapcdn.com/ [faculty]: https://
```

### Comparing `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/SOURCES.txt` & `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -87,9 +87,8 @@
 dash_bootstrap_components/_components/metadata.json
 tests/test_alert.py
 tests/test_components_as_props.py
 tests/test_navlink.py
 tests/test_popover.py
 tests/test_positional_args.py
 tests/test_tooltip.py
-tests/test_version.py
-tests/test_xss_links.py
+tests/test_version.py
```

### Comparing `dash_bootstrap_components-1.6.0rc1/landing-page.md` & `dash_bootstrap_components-1.6.1rc1/landing-page.md`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 for new features please feel free to make a [feature request][feature-request].
 If you would like to submit a pull request, please read our
 [contributing guide][contribution-guide].
 
 ## Copyright and license
 
 Code and documentation is copyright [Faculty Science Ltd.][faculty]
-2018-2022, and released under the [Apache 2.0 license](./LICENSE.txt)
+2018-2024, and released under the [Apache 2.0 license](./LICENSE.txt)
 
 [dash-homepage]: https://dash.plot.ly/
 [dash-docs-external]: https:/dash.plot.ly/external-resources
 [bootstrap-homepage]: https://getbootstrap.com/
 [dbc-repo]: https://github.com/facultyai/dash-bootstrap-components
 [reactstrap-homepage]: https://reactstrap.github.io/
 [docs-homepage]: https://dash-bootstrap-components.opensource.faculty.ai
```

#### html2text {}

```diff
@@ -26,15 +26,15 @@
 Bootstrap components. See our [_documentation_][docs-components] for a full
 list of available components. ## Contributing We welcome contributions to
 _dash-bootstrap-components_. If you find a bug or something is unclear please
 [submit a bug report][bug-report], if you have ideas for new features please
 feel free to make a [feature request][feature-request]. If you would like to
 submit a pull request, please read our [contributing guide][contribution-
 guide]. ## Copyright and license Code and documentation is copyright [Faculty
-Science Ltd.][faculty] 2018-2022, and released under the [Apache 2.0 license]
+Science Ltd.][faculty] 2018-2024, and released under the [Apache 2.0 license]
 (./LICENSE.txt) [dash-homepage]: https://dash.plot.ly/ [dash-docs-external]:
 https:/dash.plot.ly/external-resources [bootstrap-homepage]: https://
 getbootstrap.com/ [dbc-repo]: https://github.com/facultyai/dash-bootstrap-
 components [reactstrap-homepage]: https://reactstrap.github.io/ [docs-
 homepage]: https://dash-bootstrap-components.opensource.faculty.ai [docs-
 components]: https://dash-bootstrap-components.opensource.faculty.ai/l/
 components [bootstrapcdn]: https://www.bootstrapcdn.com/ [faculty]: https://
```

### Comparing `dash_bootstrap_components-1.6.0rc1/setup.cfg` & `dash_bootstrap_components-1.6.1rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/setup.py` & `dash_bootstrap_components-1.6.1rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/tests/test_components_as_props.py` & `dash_bootstrap_components-1.6.1rc1/tests/test_components_as_props.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/tests/test_navlink.py` & `dash_bootstrap_components-1.6.1rc1/tests/test_navlink.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/tests/test_popover.py` & `dash_bootstrap_components-1.6.1rc1/tests/test_popover.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/tests/test_positional_args.py` & `dash_bootstrap_components-1.6.1rc1/tests/test_positional_args.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.0rc1/tests/test_tooltip.py` & `dash_bootstrap_components-1.6.1rc1/tests/test_tooltip.py`

 * *Files identical despite different names*

