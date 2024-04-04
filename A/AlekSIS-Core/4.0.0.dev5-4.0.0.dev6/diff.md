# Comparing `tmp/aleksis_core-4.0.0.dev5.tar.gz` & `tmp/aleksis_core-4.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_core-4.0.0.dev5.tar", max compression
+gzip compressed data, was "aleksis_core-4.0.0.dev6.tar", max compression
```

## Comparing `aleksis_core-4.0.0.dev5.tar` & `aleksis_core-4.0.0.dev6.tar`

### file list

```diff
@@ -1,565 +1,577 @@
--rw-r--r--   0        0        0    42195 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/CHANGELOG.rst
--rw-r--r--   0        0        0    14353 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/LICENCE.rst
--rw-r--r--   0        0        0     3786 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/README.rst
--rw-r--r--   0        0        0      194 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/aleksis/core/__init__.py
--rw-r--r--   0        0        0      464 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/aleksis/core/__main__.py
--rw-r--r--   0        0        0      510 2024-02-29 15:15:08.132905 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1068 2024-02-29 15:15:09.428946 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/__main__.cpython-311.pyc
--rw-r--r--   0        0        0     2168 2024-02-29 15:15:12.677051 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0    11656 2024-02-29 15:15:10.984996 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     2533 2024-02-29 15:15:08.184906 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/celery.cpython-311.pyc
--rw-r--r--   0        0        0     3716 2024-02-29 15:15:12.773054 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/checks.cpython-311.pyc
--rw-r--r--   0        0        0    23254 2024-02-29 15:15:12.321039 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/data_checks.cpython-311.pyc
--rw-r--r--   0        0        0     5154 2024-02-29 15:15:12.781054 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/health_checks.cpython-311.pyc
--rw-r--r--   0        0        0    10416 2024-02-29 15:15:12.369041 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/managers.cpython-311.pyc
--rw-r--r--   0        0        0    40344 2024-02-29 15:15:12.349040 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0        0        0   103971 2024-02-29 15:15:11.805023 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0    25271 2024-02-29 15:15:13.041062 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     1144 2024-02-29 15:15:11.004997 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/registries.cpython-311.pyc
--rw-r--r--   0        0        0    17561 2024-02-29 15:15:12.705052 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0    44148 2024-02-29 15:15:09.456947 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0     3825 2024-02-29 15:15:12.373041 aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0        0        0     1002 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/aleksis/core/admin.py
--rw-r--r--   0        0        0     8751 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/aleksis/core/apps.py
--rw-r--r--   0        0        0     1338 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/aleksis/core/celery.py
--rw-r--r--   0        0        0     2759 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/aleksis/core/checks.py
--rw-r--r--   0        0        0    14836 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/aleksis/core/data_checks.py
--rw-r--r--   0        0        0      741 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/aleksis/core/decorators.py
--rw-r--r--   0        0        0     5506 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/aleksis/core/filters.py
--rw-r--r--   0        0        0    30784 2024-02-29 15:13:34.933910 aleksis_core-4.0.0.dev5/aleksis/core/forms.py
--rw-r--r--   0        0        0     3178 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/app/apollo.js
--rw-r--r--   0        0        0     1519 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/app/dateTimeFormats.js
--rw-r--r--   0        0        0      197 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/app/i18n.js
--rw-r--r--   0        0        0      157 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/app/router.js
--rw-r--r--   0        0        0      133 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/app/sentry.js
--rw-r--r--   0        0        0     1091 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/app/vuetify.js
--rw-r--r--   0        0        0     4682 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/LegacyBaseTemplate.vue
--rw-r--r--   0        0        0      158 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/Parent.vue
--rw-r--r--   0        0        0      335 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/about/About.vue
--rw-r--r--   0        0        0     1971 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/about/AboutAleksis.vue
--rw-r--r--   0        0        0     3831 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/about/InstalledAppCard.vue
--rw-r--r--   0        0        0     1003 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/about/InstalledAppsList.vue
--rw-r--r--   0        0        0      351 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/about/installedApps.graphql
--rw-r--r--   0        0        0     2412 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/AccountMenu.vue
--rw-r--r--   0        0        0    10484 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/App.vue
--rw-r--r--   0        0        0      314 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/BrandLogo.vue
--rw-r--r--   0        0        0     1064 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/ErrorPage.vue
--rw-r--r--   0        0        0     1471 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/LanguageForm.vue
--rw-r--r--   0        0        0     4635 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/SideNav.vue
--rw-r--r--   0        0        0     1454 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/SidenavSearch.vue
--rw-r--r--   0        0        0      748 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/SnackbarItem.vue
--rw-r--r--   0        0        0     1932 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/Splash.vue
--rw-r--r--   0        0        0      124 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/customMenu.graphql
--rw-r--r--   0        0        0      205 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/dynamicRoutes.graphql
--rw-r--r--   0        0        0       42 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/messages.graphql
--rw-r--r--   0        0        0       59 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/ping.graphql
--rw-r--r--   0        0        0      139 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/searchSnippets.graphql
--rw-r--r--   0        0        0      412 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/systemProperties.graphql
--rw-r--r--   0        0        0      329 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/whoAmI.graphql
--rw-r--r--   0        0        0     2568 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue
--rw-r--r--   0        0        0     1894 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue
--rw-r--r--   0        0        0      220 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/authorized_oauth_applications/accessTokens.graphql
--rw-r--r--   0        0        0       84 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/authorized_oauth_applications/revokeOauthToken.graphql
--rw-r--r--   0        0        0     3564 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/BaseCalendarFeedDetails.vue
--rw-r--r--   0        0        0     1190 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/BaseCalendarFeedEventBar.vue
--rw-r--r--   0        0        0    13721 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/Calendar.vue
--rw-r--r--   0        0        0      624 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CalendarControlBar.vue
--rw-r--r--   0        0        0      309 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CalendarDownloadAllButton.vue
--rw-r--r--   0        0        0     5903 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CalendarOverview.vue
--rw-r--r--   0        0        0     2072 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CalendarSelect.vue
--rw-r--r--   0        0        0      364 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CalendarStatusChip.vue
--rw-r--r--   0        0        0     1521 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CalendarTypeSelect.vue
--rw-r--r--   0        0        0     1560 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CalendarWithControls.vue
--rw-r--r--   0        0        0      318 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CancelledCalendarStatusChip.vue
--rw-r--r--   0        0        0      405 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/GenericCalendarFeedDetails.vue
--rw-r--r--   0        0        0      386 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/GenericCalendarFeedEventBar.vue
--rw-r--r--   0        0        0      426 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/calendar.graphql
--rw-r--r--   0        0        0      154 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/calendarFeeds.graphql
--rw-r--r--   0        0        0      561 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/calendarMixin.js
--rw-r--r--   0        0        0     1096 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/calendarSelectedFeedsMixin.js
--rw-r--r--   0        0        0     6503 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/personal_event/PersonalEventDialog.vue
--rw-r--r--   0        0        0      961 2024-02-29 15:13:34.937910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/personal_event/personalEvent.graphql
--rw-r--r--   0        0        0       93 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/setCalendarStatus.graphql
--rw-r--r--   0        0        0      715 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar_feeds/details/BirthdaysDetails.vue
--rw-r--r--   0        0        0     5014 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar_feeds/details/PersonalDetails.vue
--rw-r--r--   0        0        0      434 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar_feeds/event_bar/BirthdaysEventBar.vue
--rw-r--r--   0        0        0     3482 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
--rw-r--r--   0        0        0     2028 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
--rw-r--r--   0        0        0      925 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
--rw-r--r--   0        0        0      432 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
--rw-r--r--   0        0        0      191 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
--rw-r--r--   0        0        0      118 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
--rw-r--r--   0        0        0     3009 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/ActionSelect.vue
--rw-r--r--   0        0        0      655 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/AvatarClickbox.vue
--rw-r--r--   0        0        0      212 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/BackButton.vue
--rw-r--r--   0        0        0      823 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/ButtonMenu.vue
--rw-r--r--   0        0        0    13517 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/CRUDBar.vue
--rw-r--r--   0        0        0     3911 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/CRUDIterator.vue
--rw-r--r--   0        0        0     6884 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/CRUDList.vue
--rw-r--r--   0        0        0     1559 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/CopyToClipboardButton.vue
--rw-r--r--   0        0        0      981 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/DetailView.vue
--rw-r--r--   0        0        0     1489 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/FilterBar.vue
--rw-r--r--   0        0        0     5294 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/InlineCRUDList.vue
--rw-r--r--   0        0        0      435 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/ListView.vue
--rw-r--r--   0        0        0      268 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/MessageBox.vue
--rw-r--r--   0        0        0     1914 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/ObjectOverview.vue
--rw-r--r--   0        0        0      269 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/SmallContainer.vue
--rw-r--r--   0        0        0     2017 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/UpdateIndicator.vue
--rw-r--r--   0        0        0      716 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/buttons/BaseButton.vue
--rw-r--r--   0        0        0      456 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/buttons/CancelButton.vue
--rw-r--r--   0        0        0      361 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/buttons/CreateButton.vue
--rw-r--r--   0        0        0      370 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/buttons/DeleteButton.vue
--rw-r--r--   0        0        0      357 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/buttons/EditButton.vue
--rw-r--r--   0        0        0     1121 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/buttons/FilterButton.vue
--rw-r--r--   0        0        0      335 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/buttons/PrimaryActionButton.vue
--rw-r--r--   0        0        0      357 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/buttons/SaveButton.vue
--rw-r--r--   0        0        0      427 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/buttons/SecondaryActionButton.vue
--rw-r--r--   0        0        0      440 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/dialogs/ClosableSnackbar.vue
--rw-r--r--   0        0        0     1273 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/dialogs/ConfirmDialog.vue
--rw-r--r--   0        0        0     3226 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue
--rw-r--r--   0        0        0     6068 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/dialogs/DialogObjectForm.vue
--rw-r--r--   0        0        0     2244 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/dialogs/FilterDialog.vue
--rw-r--r--   0        0        0     1038 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/dialogs/MobileFullscreenDialog.vue
--rw-r--r--   0        0        0     1362 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/ColorField.vue
--rw-r--r--   0        0        0     2622 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/DateField.vue
--rw-r--r--   0        0        0     2401 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/DateTimeField.vue
--rw-r--r--   0        0        0     3117 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/ForeignKeyField.vue
--rw-r--r--   0        0        0     1376 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/PositiveSmallIntegerField.vue
--rw-r--r--   0        0        0     4834 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/RecurrenceField.vue
--rw-r--r--   0        0        0     2390 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/TimeField.vue
--rw-r--r--   0        0        0     1267 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/WeekDayField.vue
--rw-r--r--   0        0        0      706 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/group/GroupCollection.vue
--rw-r--r--   0        0        0     2697 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/holiday/HolidayInlineList.vue
--rw-r--r--   0        0        0      742 2024-02-29 15:13:34.941910 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/holiday/holiday.graphql
--rw-r--r--   0        0        0     2966 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/notifications/NotificationItem.vue
--rw-r--r--   0        0        0     2616 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/notifications/NotificationList.vue
--rw-r--r--   0        0        0      107 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
--rw-r--r--   0        0        0      207 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/notifications/myNotifications.graphql
--rw-r--r--   0        0        0     1017 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/pdf/DownloadPDF.vue
--rw-r--r--   0        0        0       78 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/pdf/pdf.graphql
--rw-r--r--   0        0        0     1410 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/AdditionalImage.vue
--rw-r--r--   0        0        0     1082 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/AvatarContent.vue
--rw-r--r--   0        0        0     3340 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/PersonActions.vue
--rw-r--r--   0        0        0      527 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
--rw-r--r--   0        0        0      759 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/PersonCollection.vue
--rw-r--r--   0        0        0     7572 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/PersonOverview.vue
--rw-r--r--   0        0        0      108 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/avatarContent.graphql
--rw-r--r--   0        0        0      196 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/personActions.graphql
--rw-r--r--   0        0        0      575 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/personOverview.graphql
--rw-r--r--   0        0        0     1488 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/room/RoomInlineList.vue
--rw-r--r--   0        0        0      630 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/room/room.graphql
--rw-r--r--   0        0        0     2486 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/school_term/SchoolTermField.vue
--rw-r--r--   0        0        0     2952 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/school_term/SchoolTermInlineList.vue
--rw-r--r--   0        0        0      742 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/school_term/schoolTerm.graphql
--rw-r--r--   0        0        0     3859 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/two_factor/TwoFactor.vue
--rw-r--r--   0        0        0     1490 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
--rw-r--r--   0        0        0      589 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
--rw-r--r--   0        0        0      385 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/two_factor/twoFactor.graphql
--rw-r--r--   0        0        0      422 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/css/global.scss
--rw-r--r--   0        0        0     2807 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/index.js
--rw-r--r--   0        0        0    14714 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/messages/de.json
--rw-r--r--   0        0        0    13909 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/messages/en.json
--rw-r--r--   0        0        0    18225 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/messages/ru.json
--rw-r--r--   0        0        0    17582 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/messages/uk.json
--rw-r--r--   0        0        0     3052 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/aleksis.js
--rw-r--r--   0        0        0     1060 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/calendarFeedDetails.js
--rw-r--r--   0        0        0      386 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/calendarFeedEventBar.js
--rw-r--r--   0        0        0     2695 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/createOrPatchMixin.js
--rw-r--r--   0        0        0     1540 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/deleteMixin.js
--rw-r--r--   0        0        0      538 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/error404.js
--rw-r--r--   0        0        0     3450 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/menus.js
--rw-r--r--   0        0        0     3405 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/mutateMixin.js
--rw-r--r--   0        0        0     2256 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/offline.js
--rw-r--r--   0        0        0      762 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/permissions.js
--rw-r--r--   0        0        0     2889 2024-02-29 15:13:34.945911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/queryMixin.js
--rw-r--r--   0        0        0     2154 2024-02-29 15:13:34.949911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/routes.js
--rw-r--r--   0        0        0      766 2024-02-29 15:13:34.949911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/syncSortMixin.js
--rw-r--r--   0        0        0     1684 2024-02-29 15:13:34.949911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/useRegisterSW.js
--rw-r--r--   0        0        0     6770 2024-02-29 15:13:34.949911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/plugins/aleksis.js
--rw-r--r--   0        0        0      450 2024-02-29 15:13:34.949911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/routeValidators.js
--rw-r--r--   0        0        0    35863 2024-02-29 15:13:34.949911 aleksis_core-4.0.0.dev5/aleksis/core/frontend/routes.js
--rw-r--r--   0        0        0     2642 2024-02-29 15:13:34.949911 aleksis_core-4.0.0.dev5/aleksis/core/health_checks.py
--rw-r--r--   0        0        0      487 2024-02-29 15:15:13.393074 aleksis_core-4.0.0.dev5/aleksis/core/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74550 2024-02-29 15:13:34.949911 aleksis_core-4.0.0.dev5/aleksis/core/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      463 2024-02-29 15:15:13.381073 aleksis_core-4.0.0.dev5/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      894 2024-02-29 15:13:34.949911 aleksis_core-4.0.0.dev5/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    64425 2024-02-29 15:15:13.385073 aleksis_core-4.0.0.dev5/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   127576 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      567 2024-02-29 15:15:13.353072 aleksis_core-4.0.0.dev5/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1118 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      942 2024-02-29 15:15:13.401074 aleksis_core-4.0.0.dev5/aleksis/core/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    78337 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2024-02-29 15:15:13.417074 aleksis_core-4.0.0.dev5/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      810 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     2510 2024-02-29 15:15:13.341072 aleksis_core-4.0.0.dev5/aleksis/core/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    84014 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-02-29 15:15:13.345072 aleksis_core-4.0.0.dev5/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2024-02-29 15:15:13.361073 aleksis_core-4.0.0.dev5/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74480 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-02-29 15:15:13.365073 aleksis_core-4.0.0.dev5/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    79209 2024-02-29 15:15:13.413074 aleksis_core-4.0.0.dev5/aleksis/core/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   137668 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2024-02-29 15:15:13.341072 aleksis_core-4.0.0.dev5/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1321 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2024-02-29 15:15:13.321071 aleksis_core-4.0.0.dev5/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74420 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-02-29 15:15:13.317071 aleksis_core-4.0.0.dev5/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    78198 2024-02-29 15:15:13.425075 aleksis_core-4.0.0.dev5/aleksis/core/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   135337 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2024-02-29 15:15:13.369073 aleksis_core-4.0.0.dev5/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1331 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0        0 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/management/__init__.py
--rw-r--r--   0        0        0     3957 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/management/commands/convert_urls_to_routes.py
--rw-r--r--   0        0        0     1082 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/management/commands/vite.py
--rw-r--r--   0        0        0      439 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/management/commands/webpack_bundle.py
--rw-r--r--   0        0        0     5541 2024-02-29 15:13:34.953911 aleksis_core-4.0.0.dev5/aleksis/core/managers.py
--rw-r--r--   0        0        0    49187 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0001_initial.py
--rw-r--r--   0        0        0     2198 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0002_school_term.py
--rw-r--r--   0        0        0      531 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0003_drop_image_cropping.py
--rw-r--r--   0        0        0      796 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
--rw-r--r--   0        0        0     1252 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0005_timestamped_activity_notification.py
--rw-r--r--   0        0        0     1567 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0006_dashboard_widget_size.py
--rw-r--r--   0        0        0     1207 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0007_dashboard_widget_order.py
--rw-r--r--   0        0        0     1936 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0008_data_check_result.py
--rw-r--r--   0        0        0     1052 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0009_default_dashboard.py
--rw-r--r--   0        0        0      952 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0010_external_link_widget.py
--rw-r--r--   0        0        0      829 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0011_globalpermissions_options.py
--rw-r--r--   0        0        0      501 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0012_valid_from_announcement.py
--rw-r--r--   0        0        0     2073 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0013_pdf_file.py
--rw-r--r--   0        0        0      533 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0014_alter_pdffile_file.py
--rw-r--r--   0        0        0     1174 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0015_oauth_permissions.py
--rw-r--r--   0        0        0     1341 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0016_taskuserassignment.py
--rw-r--r--   0        0        0      426 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0017_dashboardwidget_broken.py
--rw-r--r--   0        0        0      897 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0018_pdffile_html_file.py
--rw-r--r--   0        0        0     2116 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
--rw-r--r--   0        0        0      542 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0020_pdf_file_person_optional.py
--rw-r--r--   0        0        0     1084 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
--rw-r--r--   0        0        0      923 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0022_public_favicon.py
--rw-r--r--   0        0        0     6340 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0023_oauth_application_model.py
--rw-r--r--   0        0        0      714 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0024_oauth_grant_types_optional.py
--rw-r--r--   0        0        0     1717 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0025_oauth_align_user_fk.py
--rw-r--r--   0        0        0      582 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
--rw-r--r--   0        0        0      457 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0027_person_place_of_birth.py
--rw-r--r--   0        0        0      947 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0028_char_field_not_null.py
--rw-r--r--   0        0        0     1465 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0029_invitations.py
--rw-r--r--   0        0        0     1776 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0030_user_attributes.py
--rw-r--r--   0        0        0      526 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0031_oauthapplication_icon.py
--rw-r--r--   0        0        0      340 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0032_remove_person_is_active.py
--rw-r--r--   0        0        0     2416 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0033_update_photo_avatar.py
--rw-r--r--   0        0        0      816 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0034_invite_permission.py
--rw-r--r--   0        0        0     1805 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0035_preference_model_unique.py
--rw-r--r--   0        0        0      626 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0036_additionalfields_helptext_required.py
--rw-r--r--   0        0        0      917 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0037_add_static_content_widget.py
--rw-r--r--   0        0        0      522 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0038_notification_send_at.py
--rw-r--r--   0        0        0     1029 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0039_personal_ical_url.py
--rw-r--r--   0        0        0      613 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
--rw-r--r--   0        0        0      516 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0041_update_gender_choices.py
--rw-r--r--   0        0        0      547 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0042_pdffile_empty.py
--rw-r--r--   0        0        0     2261 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0043_task_assignment_meta.py
--rw-r--r--   0        0        0      532 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0044_task_assignment_result_fetched.py
--rw-r--r--   0        0        0      486 2024-02-29 15:13:34.957911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
--rw-r--r--   0        0        0   290966 2024-02-29 15:13:34.961911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0046_notification_create_field_icon.py
--rw-r--r--   0        0        0     2510 2024-02-29 15:13:34.961911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0047_add_room_model.py
--rw-r--r--   0        0        0   893996 2024-02-29 15:13:34.965911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0048_delete_personalicalurl.py
--rw-r--r--   0        0        0      533 2024-02-29 15:13:34.965911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py
--rw-r--r--   0        0        0     6221 2024-02-29 15:13:34.965911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0050_managed_by_app_label.py
--rw-r--r--   0        0        0     5606 2024-02-29 15:13:34.965911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0051_calendarevent_and_holiday.py
--rw-r--r--   0        0        0   909270 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0052_site_related_name.py
--rw-r--r--   0        0        0      914 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0053_freebusy.py
--rw-r--r--   0        0        0     1994 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0054_create_organisation_model.py
--rw-r--r--   0        0        0     1738 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0055_customevent.py
--rw-r--r--   0        0        0      332 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0056_rename_customevent_personalevent.py
--rw-r--r--   0        0        0      505 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0057_drop_otp_yubikey.py
--rw-r--r--   0        0        0      720 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0058_migrate_preferences_to_global.py
--rw-r--r--   0        0        0     5514 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0059_drop_site.py
--rw-r--r--   0        0        0     1165 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0060_person_unique_short_name_email.py
--rw-r--r--   0        0        0      500 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/0061_remove_group_additional_fields.py
--rw-r--r--   0        0        0        0 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/migrations/__init__.py
--rw-r--r--   0        0        0    25138 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/mixins.py
--rw-r--r--   0        0        0    64469 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/models.py
--rw-r--r--   0        0        0    15497 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/preferences.py
--rw-r--r--   0        0        0      611 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/registries.py
--rw-r--r--   0        0        0    16852 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/rules.py
--rw-r--r--   0        0        0    10606 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/schema/__init__.py
--rw-r--r--   0        0        0     6400 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/schema/base.py
--rw-r--r--   0        0        0     4023 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/schema/calendar.py
--rw-r--r--   0        0        0     3049 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/schema/celery_progress.py
--rw-r--r--   0        0        0      585 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/schema/custom_menu.py
--rw-r--r--   0        0        0      459 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/schema/dynamic_routes.py
--rw-r--r--   0        0        0     2005 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/schema/group.py
--rw-r--r--   0        0        0     1606 2024-02-29 15:13:34.973911 aleksis_core-4.0.0.dev5/aleksis/core/schema/holiday.py
--rw-r--r--   0        0        0     1743 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/installed_apps.py
--rw-r--r--   0        0        0      265 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/message.py
--rw-r--r--   0        0        0     1296 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/notification.py
--rw-r--r--   0        0        0     1145 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/oauth.py
--rw-r--r--   0        0        0      554 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/pdf.py
--rw-r--r--   0        0        0      124 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/permissions.py
--rw-r--r--   0        0        0     9708 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/person.py
--rw-r--r--   0        0        0     3377 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/personal_event.py
--rw-r--r--   0        0        0     1400 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/room.py
--rw-r--r--   0        0        0     2406 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/school_term.py
--rw-r--r--   0        0        0      868 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/search.py
--rw-r--r--   0        0        0     1343 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/site_preferences.py
--rw-r--r--   0        0        0     1697 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/system_properties.py
--rw-r--r--   0        0        0     3297 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/two_factor.py
--rw-r--r--   0        0        0      829 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/schema/user.py
--rw-r--r--   0        0        0      418 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/search_indexes.py
--rw-r--r--   0        0        0    39858 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/settings.py
--rw-r--r--   0        0        0    49621 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/static/img/aleksis-banner.svg
--rw-r--r--   0        0        0     1862 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/static/img/aleksis-favicon.png
--rw-r--r--   0        0        0    17172 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/static/img/aleksis-icon-maskable.png
--rw-r--r--   0        0        0     7843 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/static/img/aleksis-icon-maskable.svg
--rw-r--r--   0        0        0    31902 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/static/img/aleksis-icon.png
--rw-r--r--   0        0        0     7346 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/static/img/aleksis-icon.svg
--rw-r--r--   0        0        0    19126 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/static/img/fallback.png
--rw-r--r--   0        0        0     2237 2024-02-29 15:13:34.977912 aleksis_core-4.0.0.dev5/aleksis/core/static/img/hero.svg
--rw-r--r--   0        0        0      490 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/js/copy_button.js
--rw-r--r--   0        0        0      521 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/js/edit_dashboard.js
--rw-r--r--   0        0        0      618 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/js/helper.js
--rw-r--r--   0        0        0      984 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/js/include_ajax_live.js
--rw-r--r--   0        0        0     4351 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/js/main.js
--rw-r--r--   0        0        0     1654 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/js/multi_select.js
--rw-r--r--   0        0        0     3495 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/js/search.js
--rw-r--r--   0        0        0     2581 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/js/serviceworker.js
--rw-r--r--   0        0        0      271 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/print-simple.css
--rw-r--r--   0        0        0     1627 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/print.css
--rw-r--r--   0        0        0      187 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/print_landscape.css
--rw-r--r--   0        0        0     1064 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/public/materialize-custom.scss
--rw-r--r--   0        0        0    15749 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/public/style.scss
--rw-r--r--   0        0        0    11345 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/static/public/theme.scss
--rw-r--r--   0        0        0     5820 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/tables.py
--rw-r--r--   0        0        0     2330 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/tasks.py
--rw-r--r--   0        0        0      838 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/403.html
--rw-r--r--   0        0        0      789 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/404.html
--rw-r--r--   0        0        0      918 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/500.html
--rw-r--r--   0        0        0       76 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/503.html
--rw-r--r--   0        0        0      851 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/account_inactive.html
--rw-r--r--   0        0        0      169 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/email/base_message.txt
--rw-r--r--   0        0        0      525 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0        0        0     1255 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/email_confirm.html
--rw-r--r--   0        0        0     1182 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/password_change.html
--rw-r--r--   0        0        0     1377 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/password_reset.html
--rw-r--r--   0        0        0      825 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/password_reset_done.html
--rw-r--r--   0        0        0     2305 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      649 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      500 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/password_set.html
--rw-r--r--   0        0        0      888 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/signup.html
--rw-r--r--   0        0        0      838 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/signup_closed.html
--rw-r--r--   0        0        0      820 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/verification_email_required.html
--rw-r--r--   0        0        0     1160 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/account/verification_sent.html
--rw-r--r--   0        0        0      979 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/components/chips.html
--rw-r--r--   0        0        0      350 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/components/materialize-chips.html
--rw-r--r--   0        0        0      225 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/components/msgbox.html
--rw-r--r--   0        0        0      958 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/components/pagination.html
--rw-r--r--   0        0        0      486 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/components/text_collapsible.html
--rw-r--r--   0        0        0     1053 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/announcement/form.html
--rw-r--r--   0        0        0     1900 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/announcement/list.html
--rw-r--r--   0        0        0     3099 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/base.html
--rw-r--r--   0        0        0     2454 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/base_print.html
--rw-r--r--   0        0        0     1212 2024-02-29 15:13:34.981912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/base_simple_print.html
--rw-r--r--   0        0        0      628 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/dashboard_widget/create.html
--rw-r--r--   0        0        0      635 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
--rw-r--r--   0        0        0      626 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/dashboard_widget/edit.html
--rw-r--r--   0        0        0      262 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
--rw-r--r--   0        0        0     1349 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/dashboard_widget/list.html
--rw-r--r--   0        0        0      226 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
--rw-r--r--   0        0        0     3879 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/data_check/list.html
--rw-r--r--   0        0        0     2233 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/edit_dashboard.html
--rw-r--r--   0        0        0        0 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/empty.html
--rw-r--r--   0        0        0     5310 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/group/child_groups.html
--rw-r--r--   0        0        0      650 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/group/edit.html
--rw-r--r--   0        0        0     3382 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/group/full.html
--rw-r--r--   0        0        0     1019 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/group/list.html
--rw-r--r--   0        0        0      465 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/group_type/edit.html
--rw-r--r--   0        0        0      564 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/group_type/list.html
--rw-r--r--   0        0        0     2504 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/index.html
--rw-r--r--   0        0        0      777 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/pages/delete.html
--rw-r--r--   0        0        0     6832 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/pages/system_status.html
--rw-r--r--   0        0        0      603 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/pages/test_pdf.html
--rw-r--r--   0        0        0       93 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/address.html
--rw-r--r--   0        0        0      189 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/admins_list.html
--rw-r--r--   0        0        0     1632 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/announcements.html
--rw-r--r--   0        0        0     1472 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/avatar_content.html
--rw-r--r--   0        0        0      319 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/copy_button.html
--rw-r--r--   0        0        0     1089 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/crud_events.html
--rw-r--r--   0        0        0      389 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/edit_dashboard_widget.html
--rw-r--r--   0        0        0     1624 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/meta.html
--rw-r--r--   0        0        0      414 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/on_page_menu.html
--rw-r--r--   0        0        0      260 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/save_button.html
--rw-r--r--   0        0        0     2358 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/splash_screen.html
--rw-r--r--   0        0        0      325 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/turnable.html
--rw-r--r--   0        0        0      915 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/perms/assign.html
--rw-r--r--   0        0        0     2478 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/perms/list.html
--rw-r--r--   0        0        0      376 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/person/collection.html
--rw-r--r--   0        0        0      649 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/person/create.html
--rw-r--r--   0        0        0      645 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/person/edit.html
--rw-r--r--   0        0        0     1165 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/person/list.html
--rw-r--r--   0        0        0      927 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/core/vue_index.html
--rw-r--r--   0        0        0     3921 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/django_tables2/materialize.html
--rw-r--r--   0        0        0      981 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/dynamic_preferences/form.html
--rw-r--r--   0        0        0      376 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/dynamic_preferences/sections.html
--rw-r--r--   0        0        0      764 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/invitations/disabled.html
--rw-r--r--   0        0        0     1281 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/invitations/enter.html
--rw-r--r--   0        0        0     1162 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/invitations/forms/_invite.html
--rw-r--r--   0        0        0      102 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/invitations/messages/invite_accepted.txt
--rw-r--r--   0        0        0      171 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/material/field_errors.html
--rw-r--r--   0        0        0     1232 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
--rw-r--r--   0        0        0     1897 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/material/fields/colorfield_colorwidget.html
--rw-r--r--   0        0        0     1009 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
--rw-r--r--   0        0        0     1009 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/material/fields/django_select2_select2widget.html
--rw-r--r--   0        0        0      253 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/material/non_field_errors.html
--rw-r--r--   0        0        0      663 2024-02-29 15:13:34.985912 aleksis_core-4.0.0.dev5/aleksis/core/templates/oauth2_provider/application/create.html
--rw-r--r--   0        0        0     2335 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/oauth2_provider/application/detail.html
--rw-r--r--   0        0        0      669 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/oauth2_provider/application/edit.html
--rw-r--r--   0        0        0     1074 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/oauth2_provider/application/list.html
--rw-r--r--   0        0        0     2686 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/oauth2_provider/authorize.html
--rw-r--r--   0        0        0      887 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/offline.html
--rw-r--r--   0        0        0       42 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/search/indexes/core/group_text.txt
--rw-r--r--   0        0        0       69 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/search/indexes/core/person_text.txt
--rw-r--r--   0        0        0       42 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/search/indexes/core/room_text.txt
--rw-r--r--   0        0        0     3171 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/search/search.html
--rw-r--r--   0        0        0      243 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/search/searchbar_snippet.html
--rw-r--r--   0        0        0      150 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/search/searchbar_snippets.html
--rw-r--r--   0        0        0      169 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/sms/notification.txt
--rw-r--r--   0        0        0      893 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0     1268 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/socialaccount/connections.html
--rw-r--r--   0        0        0     1289 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/socialaccount/login.html
--rw-r--r--   0        0        0      809 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/socialaccount/login_cancelled.html
--rw-r--r--   0        0        0     1012 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/socialaccount/signup.html
--rw-r--r--   0        0        0     1660 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0        0        0      630 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/base.email
--rw-r--r--   0        0        0     1527 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/celery_failure.email
--rw-r--r--   0        0        0      994 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/data_checks.email
--rw-r--r--   0        0        0     1014 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/email.css
--rw-r--r--   0        0        0     1102 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/invitation.email
--rw-r--r--   0        0        0     1461 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/notification.email
--rw-r--r--   0        0        0      668 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/person_changed.email
--rw-r--r--   0        0        0      219 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/_base_focus.html
--rw-r--r--   0        0        0      877 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/_wizard_actions.html
--rw-r--r--   0        0        0      119 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/_wizard_forms.html
--rw-r--r--   0        0        0     1780 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/core/backup_tokens.html
--rw-r--r--   0        0        0     6686 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/core/login.html
--rw-r--r--   0        0        0      943 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/core/otp_required.html
--rw-r--r--   0        0        0      986 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/core/phone_register.html
--rw-r--r--   0        0        0     3050 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/core/setup.html
--rw-r--r--   0        0        0     2127 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/core/setup_complete.html
--rw-r--r--   0        0        0      786 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/profile/disable.html
--rw-r--r--   0        0        0        0 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templatetags/__init__.py
--rw-r--r--   0        0        0       99 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templatetags/apps.py
--rw-r--r--   0        0        0      394 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templatetags/dashboard.py
--rw-r--r--   0        0        0     1611 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templatetags/data_helpers.py
--rw-r--r--   0        0        0     1543 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templatetags/html_helpers.py
--rw-r--r--   0        0        0      206 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/templatetags/msg_box.py
--rw-r--r--   0        0        0     3696 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/tests/browser/test_selenium.py
--rw-r--r--   0        0        0     1607 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/tests/mixins/test_registry_object.py
--rw-r--r--   0        0        0     6596 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/tests/models/test.pdf
--rw-r--r--   0        0        0     1520 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/tests/models/test_group_sync.py
--rw-r--r--   0        0        0     3049 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/tests/models/test_notification.py
--rw-r--r--   0        0        0     4003 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/tests/models/test_pdffile.py
--rw-r--r--   0        0        0      427 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/tests/models/test_person.py
--rw-r--r--   0        0        0     5503 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/tests/regression/test_regression.py
--rw-r--r--   0        0        0      683 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/tests/regression/view_oauth.py
--rw-r--r--   0        0        0     1021 2024-02-29 15:13:34.989912 aleksis_core-4.0.0.dev5/aleksis/core/tests/templatetags/test_data_helpers.py
--rw-r--r--   0        0        0     2292 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/tests/views/test_account.py
--rw-r--r--   0        0        0    18215 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/urls.py
--rw-r--r--   0        0        0        0 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/__init__.py
--rw-r--r--   0        0        0      176 2024-02-29 15:15:08.616920 aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    14949 2024-02-29 15:15:11.008997 aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0    10101 2024-02-29 15:15:12.373041 aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
--rw-r--r--   0        0        0    29144 2024-02-29 15:15:08.620920 aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     1500 2024-02-29 15:15:09.340943 aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/email.cpython-311.pyc
--rw-r--r--   0        0        0      771 2024-02-29 15:15:12.393041 aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     5811 2024-02-29 15:15:12.373041 aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
--rw-r--r--   0        0        0     9909 2024-02-29 15:15:12.705052 aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
--rw-r--r--   0        0        0     2181 2024-02-29 15:15:11.040998 aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
--rw-r--r--   0        0        0      657 2024-02-29 15:15:11.036998 aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
--rw-r--r--   0        0        0    11018 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/apps.py
--rw-r--r--   0        0        0     6343 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/auth_helpers.py
--rw-r--r--   0        0        0     7920 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/celery_progress.py
--rw-r--r--   0        0        0      197 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/context_processors.py
--rw-r--r--   0        0        0    18985 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/core_helpers.py
--rw-r--r--   0        0        0      986 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/email.py
--rw-r--r--   0        0        0     1175 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/forms.py
--rw-r--r--   0        0        0     2901 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/frontend_helpers.py
--rw-r--r--   0        0        0     2375 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/ldap.py
--rw-r--r--   0        0        0   192829 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/licenses.json
--rw-r--r--   0        0        0     2255 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/messages.py
--rw-r--r--   0        0        0     2091 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/middlewares.py
--rw-r--r--   0        0        0      850 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/model_helpers.py
--rw-r--r--   0        0        0     3818 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/notifications.py
--rw-r--r--   0        0        0     6131 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/pdf.py
--rw-r--r--   0        0        0     5801 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/predicates.py
--rw-r--r--   0        0        0      936 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/sass_helpers.py
--rw-r--r--   0        0        0      524 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/search.py
--rw-r--r--   0        0        0      125 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/spdx.py
--rw-r--r--   0        0        0     1673 2024-02-29 15:13:34.993912 aleksis_core-4.0.0.dev5/aleksis/core/util/tables.py
--rw-r--r--   0        0        0    55056 2024-02-29 15:13:34.997912 aleksis_core-4.0.0.dev5/aleksis/core/views.py
--rw-r--r--   0        0        0    12147 2024-02-29 15:13:34.997912 aleksis_core-4.0.0.dev5/aleksis/core/vite.config.js
--rw-r--r--   0        0        0      173 2024-02-29 15:13:34.997912 aleksis_core-4.0.0.dev5/aleksis/core/wsgi.py
--rw-r--r--   0        0        0       44 2024-02-29 15:13:34.997912 aleksis_core-4.0.0.dev5/conftest.py
--rw-r--r--   0        0        0      581 2024-02-29 15:13:34.997912 aleksis_core-4.0.0.dev5/docs/Makefile
--rw-r--r--   0        0        0   127432 2024-02-29 15:13:34.997912 aleksis_core-4.0.0.dev5/docs/_static/2fa.png
--rw-r--r--   0        0        0    71362 2024-02-29 15:13:34.997912 aleksis_core-4.0.0.dev5/docs/_static/accept_invite.png
--rw-r--r--   0        0        0    72621 2024-02-29 15:13:34.997912 aleksis_core-4.0.0.dev5/docs/_static/create_dashboard_widget.png
--rw-r--r--   0        0        0    41935 2024-02-29 15:13:35.001912 aleksis_core-4.0.0.dev5/docs/_static/create_social_application.png
--rw-r--r--   0        0        0    72508 2024-02-29 15:13:35.001912 aleksis_core-4.0.0.dev5/docs/_static/dashboard.png
--rw-r--r--   0        0        0    87601 2024-02-29 15:13:35.001912 aleksis_core-4.0.0.dev5/docs/_static/dashboard_widgets.png
--rw-r--r--   0        0        0   119523 2024-02-29 15:13:35.001912 aleksis_core-4.0.0.dev5/docs/_static/data_checks.png
--rw-r--r--   0        0        0    81386 2024-02-29 15:13:35.001912 aleksis_core-4.0.0.dev5/docs/_static/edit_dashboard.png
--rw-r--r--   0        0        0    85722 2024-02-29 15:13:35.005912 aleksis_core-4.0.0.dev5/docs/_static/edit_default_dashboard.png
--rw-r--r--   0        0        0   107979 2024-02-29 15:13:35.005912 aleksis_core-4.0.0.dev5/docs/_static/invitations.png
--rw-r--r--   0        0        0   177681 2024-02-29 15:13:35.005912 aleksis_core-4.0.0.dev5/docs/_static/invite_existing.png
--rw-r--r--   0        0        0    44868 2024-02-29 15:13:35.005912 aleksis_core-4.0.0.dev5/docs/_static/pwa_desktop_chromium.png
--rw-r--r--   0        0        0    69215 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/_static/pwa_mobile_chromium.png
--rw-r--r--   0        0        0   128479 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/_static/pwa_mobile_firefox.png
--rw-r--r--   0        0        0   108973 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/_static/pwa_mobile_safari.png
--rw-r--r--   0        0        0    69804 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/_static/signup.png
--rw-r--r--   0        0        0      132 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/admin/00_index.rst
--rw-r--r--   0        0        0     4231 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/admin/01_core_concepts.rst
--rw-r--r--   0        0        0     8109 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/admin/10_install.rst
--rw-r--r--   0        0        0     1872 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/admin/15_config_files.rst
--rw-r--r--   0        0        0     2086 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/admin/16_config_options.rst
--rw-r--r--   0        0        0     1648 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/admin/17_storage.rst
--rw-r--r--   0        0        0      803 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/admin/18_mail.rst
--rw-r--r--   0        0        0     1509 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/admin/21_ldap.rst
--rw-r--r--   0        0        0     3037 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/admin/22_registration.rst
--rw-r--r--   0        0        0     1467 2024-02-29 15:13:35.009913 aleksis_core-4.0.0.dev5/docs/admin/23_socialaccounts.rst
--rw-r--r--   0        0        0     3218 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/admin/31_monitoring.rst
--rw-r--r--   0        0        0     1012 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/admin/32_tasks.rst
--rw-r--r--   0        0        0     1393 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/admin/33_data_checks.rst
--rw-r--r--   0        0        0     4610 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/admin/50_dashboard.rst
--rw-r--r--   0        0        0     6392 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/conf.py
--rw-r--r--   0        0        0      132 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/dev/00_index.rst
--rw-r--r--   0        0        0     4058 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/dev/01_setup.rst
--rw-r--r--   0        0        0     1427 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/dev/02_install_apps.rst
--rw-r--r--   0        0        0     3117 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/dev/03_run_tests.rst
--rw-r--r--   0        0        0     4519 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/dev/04_materialize_templates.rst
--rw-r--r--   0        0        0      289 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/dev/05_extensible_models.rst
--rw-r--r--   0        0        0     1148 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/dev/06_merging_app_settings.rst
--rw-r--r--   0        0        0     1349 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/dev/10_dashboard_widgets.rst
--rw-r--r--   0        0        0      514 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/index.rst
--rw-r--r--   0        0        0      787 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/make.bat
--rw-r--r--   0        0        0       95 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/00_index.rst
--rw-r--r--   0        0        0       69 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/core/01_checks.rst
--rw-r--r--   0        0        0       70 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/core/02_managers.rst
--rw-r--r--   0        0        0       64 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/core/03_mixins.rst
--rw-r--r--   0        0        0       84 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/core/04_models.rst
--rw-r--r--   0        0        0      108 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/core/05_registries.rst
--rw-r--r--   0        0        0       93 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/core/06_search_indexes.rst
--rw-r--r--   0        0        0       79 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/core/07_tables.rst
--rw-r--r--   0        0        0       90 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/core/08_tasks.rst
--rw-r--r--   0        0        0     1017 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/core/09_utils.rst
--rw-r--r--   0        0        0       71 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/core/10_views.rst
--rw-r--r--   0        0        0       77 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/core/11_filters.rst
--rw-r--r--   0        0        0      373 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/ref/core/12_template_tags.rst
--rw-r--r--   0        0        0      112 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/user/00_index.rst
--rw-r--r--   0        0        0     1152 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/user/01_registration.rst
--rw-r--r--   0        0        0     3465 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/user/02_personal_account.rst
--rw-r--r--   0        0        0     1770 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/user/10_dashboard.rst
--rw-r--r--   0        0        0     2607 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/docs/user/20_pwa.rst
--rw-r--r--   0        0        0     5570 2024-02-29 15:14:02.094783 aleksis_core-4.0.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     2180 2024-02-29 15:13:35.013913 aleksis_core-4.0.0.dev5/tox.ini
--rw-r--r--   0        0        0     8737 1970-01-01 00:00:00.000000 aleksis_core-4.0.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0    42442 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/CHANGELOG.rst
+-rw-r--r--   0        0        0    14353 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/LICENCE.rst
+-rw-r--r--   0        0        0     3786 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/README.rst
+-rw-r--r--   0        0        0      194 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/__init__.py
+-rw-r--r--   0        0        0      464 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/__main__.py
+-rw-r--r--   0        0        0      510 2024-04-04 06:54:53.759696 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1068 2024-04-04 06:54:54.547687 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/__main__.cpython-311.pyc
+-rw-r--r--   0        0        0     2168 2024-04-04 06:54:56.667662 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0    11656 2024-04-04 06:54:55.499676 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     2533 2024-04-04 06:54:53.791696 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/celery.cpython-311.pyc
+-rw-r--r--   0        0        0     3716 2024-04-04 06:54:56.743662 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/checks.cpython-311.pyc
+-rw-r--r--   0        0        0    23254 2024-04-04 06:54:56.411666 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/data_checks.cpython-311.pyc
+-rw-r--r--   0        0        0     5154 2024-04-04 06:54:56.747662 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/health_checks.cpython-311.pyc
+-rw-r--r--   0        0        0    10749 2024-04-04 06:54:56.447665 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/managers.cpython-311.pyc
+-rw-r--r--   0        0        0    40416 2024-04-04 06:54:56.431665 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0        0        0   103971 2024-04-04 06:54:56.071669 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0    25279 2024-04-04 06:54:56.919660 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0     1144 2024-04-04 06:54:55.515676 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/registries.cpython-311.pyc
+-rw-r--r--   0        0        0    18563 2024-04-04 06:54:56.687662 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0    44148 2024-04-04 06:54:54.563687 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0     3825 2024-04-04 06:54:56.455665 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0        0        0     1002 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/admin.py
+-rw-r--r--   0        0        0     8751 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/apps.py
+-rw-r--r--   0        0        0     1338 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/celery.py
+-rw-r--r--   0        0        0     2759 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/checks.py
+-rw-r--r--   0        0        0    14836 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/data_checks.py
+-rw-r--r--   0        0        0      741 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/decorators.py
+-rw-r--r--   0        0        0     5506 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/filters.py
+-rw-r--r--   0        0        0    30667 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/forms.py
+-rw-r--r--   0        0        0     3178 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/apollo.js
+-rw-r--r--   0        0        0     1757 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/dateTimeFormats.js
+-rw-r--r--   0        0        0      197 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/i18n.js
+-rw-r--r--   0        0        0      157 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/router.js
+-rw-r--r--   0        0        0      133 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/sentry.js
+-rw-r--r--   0        0        0     1091 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/vuetify.js
+-rw-r--r--   0        0        0     4682 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/LegacyBaseTemplate.vue
+-rw-r--r--   0        0        0      158 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/Parent.vue
+-rw-r--r--   0        0        0      335 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/About.vue
+-rw-r--r--   0        0        0     1971 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/AboutAleksis.vue
+-rw-r--r--   0        0        0     3831 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/InstalledAppCard.vue
+-rw-r--r--   0        0        0     1003 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/InstalledAppsList.vue
+-rw-r--r--   0        0        0      351 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/installedApps.graphql
+-rw-r--r--   0        0        0     2412 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/AccountMenu.vue
+-rw-r--r--   0        0        0    10484 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/App.vue
+-rw-r--r--   0        0        0      314 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/BrandLogo.vue
+-rw-r--r--   0        0        0     1064 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/ErrorPage.vue
+-rw-r--r--   0        0        0     1471 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/LanguageForm.vue
+-rw-r--r--   0        0        0     4635 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/SideNav.vue
+-rw-r--r--   0        0        0     1454 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/SidenavSearch.vue
+-rw-r--r--   0        0        0      748 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/SnackbarItem.vue
+-rw-r--r--   0        0        0     1932 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/Splash.vue
+-rw-r--r--   0        0        0      124 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/customMenu.graphql
+-rw-r--r--   0        0        0      205 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/dynamicRoutes.graphql
+-rw-r--r--   0        0        0       42 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/messages.graphql
+-rw-r--r--   0        0        0       59 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/ping.graphql
+-rw-r--r--   0        0        0      139 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/searchSnippets.graphql
+-rw-r--r--   0        0        0      412 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/systemProperties.graphql
+-rw-r--r--   0        0        0      329 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/whoAmI.graphql
+-rw-r--r--   0        0        0     2568 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue
+-rw-r--r--   0        0        0     1894 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue
+-rw-r--r--   0        0        0      220 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/authorized_oauth_applications/accessTokens.graphql
+-rw-r--r--   0        0        0       84 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/authorized_oauth_applications/revokeOauthToken.graphql
+-rw-r--r--   0        0        0     3564 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/BaseCalendarFeedDetails.vue
+-rw-r--r--   0        0        0     1190 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/BaseCalendarFeedEventBar.vue
+-rw-r--r--   0        0        0    13721 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/Calendar.vue
+-rw-r--r--   0        0        0      624 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarControlBar.vue
+-rw-r--r--   0        0        0      309 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarDownloadAllButton.vue
+-rw-r--r--   0        0        0     5903 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarOverview.vue
+-rw-r--r--   0        0        0     2072 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarSelect.vue
+-rw-r--r--   0        0        0      364 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarStatusChip.vue
+-rw-r--r--   0        0        0     1521 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarTypeSelect.vue
+-rw-r--r--   0        0        0     1560 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarWithControls.vue
+-rw-r--r--   0        0        0      318 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CancelledCalendarStatusChip.vue
+-rw-r--r--   0        0        0      405 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/GenericCalendarFeedDetails.vue
+-rw-r--r--   0        0        0      386 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/GenericCalendarFeedEventBar.vue
+-rw-r--r--   0        0        0      426 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/calendar.graphql
+-rw-r--r--   0        0        0      154 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/calendarFeeds.graphql
+-rw-r--r--   0        0        0      561 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/calendarMixin.js
+-rw-r--r--   0        0        0     1096 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/calendarSelectedFeedsMixin.js
+-rw-r--r--   0        0        0     9850 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/personal_event/PersonalEventDialog.vue
+-rw-r--r--   0        0        0     1021 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/personal_event/personalEvent.graphql
+-rw-r--r--   0        0        0       93 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/setCalendarStatus.graphql
+-rw-r--r--   0        0        0      715 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar_feeds/details/BirthdaysDetails.vue
+-rw-r--r--   0        0        0     5242 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar_feeds/details/PersonalDetails.vue
+-rw-r--r--   0        0        0      434 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar_feeds/event_bar/BirthdaysEventBar.vue
+-rw-r--r--   0        0        0     3611 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
+-rw-r--r--   0        0        0     2806 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
+-rw-r--r--   0        0        0      925 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
+-rw-r--r--   0        0        0      432 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
+-rw-r--r--   0        0        0      191 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
+-rw-r--r--   0        0        0      118 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
+-rw-r--r--   0        0        0     3009 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ActionSelect.vue
+-rw-r--r--   0        0        0      655 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/AvatarClickbox.vue
+-rw-r--r--   0        0        0      212 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/BackButton.vue
+-rw-r--r--   0        0        0      823 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ButtonMenu.vue
+-rw-r--r--   0        0        0    13494 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CRUDBar.vue
+-rw-r--r--   0        0        0     3819 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CRUDIterator.vue
+-rw-r--r--   0        0        0     6938 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CRUDList.vue
+-rw-r--r--   0        0        0     1559 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CopyToClipboardButton.vue
+-rw-r--r--   0        0        0      981 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/DetailView.vue
+-rw-r--r--   0        0        0     1483 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/FilterBar.vue
+-rw-r--r--   0        0        0     5173 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/InlineCRUDList.vue
+-rw-r--r--   0        0        0      435 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ListView.vue
+-rw-r--r--   0        0        0      268 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/MessageBox.vue
+-rw-r--r--   0        0        0     1914 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ObjectOverview.vue
+-rw-r--r--   0        0        0      269 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/SmallContainer.vue
+-rw-r--r--   0        0        0      292 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/TableLink.vue
+-rw-r--r--   0        0        0     2017 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/UpdateIndicator.vue
+-rw-r--r--   0        0        0      716 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/BaseButton.vue
+-rw-r--r--   0        0        0      456 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/CancelButton.vue
+-rw-r--r--   0        0        0     1229 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/CollapseTriggerButton.vue
+-rw-r--r--   0        0        0      361 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/CreateButton.vue
+-rw-r--r--   0        0        0      370 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/DeleteButton.vue
+-rw-r--r--   0        0        0      357 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/EditButton.vue
+-rw-r--r--   0        0        0     1139 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/FilterButton.vue
+-rw-r--r--   0        0        0      335 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/PrimaryActionButton.vue
+-rw-r--r--   0        0        0      357 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/SaveButton.vue
+-rw-r--r--   0        0        0      427 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/SecondaryActionButton.vue
+-rw-r--r--   0        0        0      440 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/ClosableSnackbar.vue
+-rw-r--r--   0        0        0     1273 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/ConfirmDialog.vue
+-rw-r--r--   0        0        0     3269 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue
+-rw-r--r--   0        0        0     5971 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/DialogObjectForm.vue
+-rw-r--r--   0        0        0     2244 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/FilterDialog.vue
+-rw-r--r--   0        0        0     1038 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/MobileFullscreenDialog.vue
+-rw-r--r--   0        0        0     1360 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/ColorField.vue
+-rw-r--r--   0        0        0     2622 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/DateField.vue
+-rw-r--r--   0        0        0     2401 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/DateTimeField.vue
+-rw-r--r--   0        0        0     3229 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/ForeignKeyField.vue
+-rw-r--r--   0        0        0     1006 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/PositiveSmallIntegerField.vue
+-rw-r--r--   0        0        0     4834 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/RecurrenceField.vue
+-rw-r--r--   0        0        0      695 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/SexSelect.vue
+-rw-r--r--   0        0        0     2390 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/TimeField.vue
+-rw-r--r--   0        0        0     1267 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/WeekDayField.vue
+-rw-r--r--   0        0        0      355 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/group/GroupChip.vue
+-rw-r--r--   0        0        0      706 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/group/GroupCollection.vue
+-rw-r--r--   0        0        0     2125 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/group_type/GroupType.vue
+-rw-r--r--   0        0        0      696 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/group_type/groupType.graphql
+-rw-r--r--   0        0        0     2697 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/holiday/HolidayInlineList.vue
+-rw-r--r--   0        0        0      742 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/holiday/holiday.graphql
+-rw-r--r--   0        0        0     2966 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/notifications/NotificationItem.vue
+-rw-r--r--   0        0        0     2616 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/notifications/NotificationList.vue
+-rw-r--r--   0        0        0      107 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
+-rw-r--r--   0        0        0      207 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/notifications/myNotifications.graphql
+-rw-r--r--   0        0        0     1017 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/pdf/DownloadPDF.vue
+-rw-r--r--   0        0        0       78 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/pdf/pdf.graphql
+-rw-r--r--   0        0        0     1410 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/AdditionalImage.vue
+-rw-r--r--   0        0        0     1252 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/AvatarContent.vue
+-rw-r--r--   0        0        0     3389 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonActions.vue
+-rw-r--r--   0        0        0      527 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
+-rw-r--r--   0        0        0      862 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonChip.vue
+-rw-r--r--   0        0        0      759 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonCollection.vue
+-rw-r--r--   0        0        0     2482 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonList.vue
+-rw-r--r--   0        0        0     8273 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonOverview.vue
+-rw-r--r--   0        0        0      108 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/avatarContent.graphql
+-rw-r--r--   0        0        0      301 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/personActions.graphql
+-rw-r--r--   0        0        0      345 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/personList.graphql
+-rw-r--r--   0        0        0      589 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/personOverview.graphql
+-rw-r--r--   0        0        0     1488 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/room/RoomInlineList.vue
+-rw-r--r--   0        0        0      630 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/room/room.graphql
+-rw-r--r--   0        0        0     2516 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/school_term/SchoolTermField.vue
+-rw-r--r--   0        0        0     2952 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/school_term/SchoolTermInlineList.vue
+-rw-r--r--   0        0        0      742 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/school_term/schoolTerm.graphql
+-rw-r--r--   0        0        0     3859 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/TwoFactor.vue
+-rw-r--r--   0        0        0     1490 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
+-rw-r--r--   0        0        0      589 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
+-rw-r--r--   0        0        0      385 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/twoFactor.graphql
+-rw-r--r--   0        0        0      422 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/css/global.scss
+-rw-r--r--   0        0        0     2841 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/index.js
+-rw-r--r--   0        0        0    15106 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/de.json
+-rw-r--r--   0        0        0    13925 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/en.json
+-rw-r--r--   0        0        0    18225 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/ru.json
+-rw-r--r--   0        0        0    17582 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/uk.json
+-rw-r--r--   0        0        0     3052 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/aleksis.js
+-rw-r--r--   0        0        0     1060 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/calendarFeedDetails.js
+-rw-r--r--   0        0        0      386 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/calendarFeedEventBar.js
+-rw-r--r--   0        0        0     2695 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/createOrPatchMixin.js
+-rw-r--r--   0        0        0     1540 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/deleteMixin.js
+-rw-r--r--   0        0        0      538 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/error404.js
+-rw-r--r--   0        0        0     2419 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/formRulesMixin.js
+-rw-r--r--   0        0        0      490 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/loadingMixin.js
+-rw-r--r--   0        0        0     3450 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/menus.js
+-rw-r--r--   0        0        0     3296 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/mutateMixin.js
+-rw-r--r--   0        0        0     2256 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/offline.js
+-rw-r--r--   0        0        0      762 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/permissions.js
+-rw-r--r--   0        0        0     3060 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/queryMixin.js
+-rw-r--r--   0        0        0     2154 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/routes.js
+-rw-r--r--   0        0        0      524 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/sexChoiceMixin.js
+-rw-r--r--   0        0        0      766 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/syncSortMixin.js
+-rw-r--r--   0        0        0     1684 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/useRegisterSW.js
+-rw-r--r--   0        0        0     7148 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/plugins/aleksis.js
+-rw-r--r--   0        0        0      450 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/routeValidators.js
+-rw-r--r--   0        0        0    34409 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/routes.js
+-rw-r--r--   0        0        0     2642 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/health_checks.py
+-rw-r--r--   0        0        0      487 2024-04-04 06:54:57.175657 aleksis_core-4.0.0.dev6/aleksis/core/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74550 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      463 2024-04-04 06:54:57.179657 aleksis_core-4.0.0.dev6/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      894 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    64425 2024-04-04 06:54:57.179657 aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   127576 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      567 2024-04-04 06:54:57.167657 aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1118 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      942 2024-04-04 06:54:57.179657 aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    78337 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2024-04-04 06:54:57.171657 aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      810 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     2510 2024-04-04 06:54:57.187656 aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    84014 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2024-04-04 06:54:57.191656 aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2024-04-04 06:54:57.099658 aleksis_core-4.0.0.dev6/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74480 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2024-04-04 06:54:57.103658 aleksis_core-4.0.0.dev6/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    79209 2024-04-04 06:54:57.191656 aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   137668 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2024-04-04 06:54:57.179657 aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1321 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2024-04-04 06:54:57.099658 aleksis_core-4.0.0.dev6/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74420 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2024-04-04 06:54:57.095658 aleksis_core-4.0.0.dev6/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    78198 2024-04-04 06:54:57.175657 aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   135337 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2024-04-04 06:54:57.167657 aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1331 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0        0 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/management/__init__.py
+-rw-r--r--   0        0        0     3957 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/management/commands/convert_urls_to_routes.py
+-rw-r--r--   0        0        0     1082 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/management/commands/vite.py
+-rw-r--r--   0        0        0      439 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/management/commands/webpack_bundle.py
+-rw-r--r--   0        0        0     5688 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/managers.py
+-rw-r--r--   0        0        0    49187 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2198 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0002_school_term.py
+-rw-r--r--   0        0        0      531 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0003_drop_image_cropping.py
+-rw-r--r--   0        0        0      796 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
+-rw-r--r--   0        0        0     1252 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0005_timestamped_activity_notification.py
+-rw-r--r--   0        0        0     1567 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0006_dashboard_widget_size.py
+-rw-r--r--   0        0        0     1207 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0007_dashboard_widget_order.py
+-rw-r--r--   0        0        0     1936 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0008_data_check_result.py
+-rw-r--r--   0        0        0     1052 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0009_default_dashboard.py
+-rw-r--r--   0        0        0      952 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0010_external_link_widget.py
+-rw-r--r--   0        0        0      829 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0011_globalpermissions_options.py
+-rw-r--r--   0        0        0      501 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0012_valid_from_announcement.py
+-rw-r--r--   0        0        0     2073 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0013_pdf_file.py
+-rw-r--r--   0        0        0      533 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0014_alter_pdffile_file.py
+-rw-r--r--   0        0        0     1174 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0015_oauth_permissions.py
+-rw-r--r--   0        0        0     1341 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0016_taskuserassignment.py
+-rw-r--r--   0        0        0      426 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0017_dashboardwidget_broken.py
+-rw-r--r--   0        0        0      897 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0018_pdffile_html_file.py
+-rw-r--r--   0        0        0     2116 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
+-rw-r--r--   0        0        0      542 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0020_pdf_file_person_optional.py
+-rw-r--r--   0        0        0     1084 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
+-rw-r--r--   0        0        0      923 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0022_public_favicon.py
+-rw-r--r--   0        0        0     6340 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0023_oauth_application_model.py
+-rw-r--r--   0        0        0      714 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0024_oauth_grant_types_optional.py
+-rw-r--r--   0        0        0     1717 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0025_oauth_align_user_fk.py
+-rw-r--r--   0        0        0      582 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
+-rw-r--r--   0        0        0      457 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0027_person_place_of_birth.py
+-rw-r--r--   0        0        0      947 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0028_char_field_not_null.py
+-rw-r--r--   0        0        0     1465 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0029_invitations.py
+-rw-r--r--   0        0        0     1776 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0030_user_attributes.py
+-rw-r--r--   0        0        0      526 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0031_oauthapplication_icon.py
+-rw-r--r--   0        0        0      340 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0032_remove_person_is_active.py
+-rw-r--r--   0        0        0     2416 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0033_update_photo_avatar.py
+-rw-r--r--   0        0        0      816 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0034_invite_permission.py
+-rw-r--r--   0        0        0     1805 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0035_preference_model_unique.py
+-rw-r--r--   0        0        0      626 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0036_additionalfields_helptext_required.py
+-rw-r--r--   0        0        0      917 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0037_add_static_content_widget.py
+-rw-r--r--   0        0        0      522 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0038_notification_send_at.py
+-rw-r--r--   0        0        0     1029 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0039_personal_ical_url.py
+-rw-r--r--   0        0        0      613 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
+-rw-r--r--   0        0        0      516 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0041_update_gender_choices.py
+-rw-r--r--   0        0        0      547 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0042_pdffile_empty.py
+-rw-r--r--   0        0        0     2261 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0043_task_assignment_meta.py
+-rw-r--r--   0        0        0      532 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0044_task_assignment_result_fetched.py
+-rw-r--r--   0        0        0      486 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
+-rw-r--r--   0        0        0   290966 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0046_notification_create_field_icon.py
+-rw-r--r--   0        0        0     2510 2024-04-04 06:54:07.928226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0047_add_room_model.py
+-rw-r--r--   0        0        0   893996 2024-04-04 06:54:07.928226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0048_delete_personalicalurl.py
+-rw-r--r--   0        0        0      533 2024-04-04 06:54:07.928226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py
+-rw-r--r--   0        0        0     6221 2024-04-04 06:54:07.928226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0050_managed_by_app_label.py
+-rw-r--r--   0        0        0     5606 2024-04-04 06:54:07.928226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0051_calendarevent_and_holiday.py
+-rw-r--r--   0        0        0   909270 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0052_site_related_name.py
+-rw-r--r--   0        0        0      914 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0053_freebusy.py
+-rw-r--r--   0        0        0     1994 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0054_create_organisation_model.py
+-rw-r--r--   0        0        0     1738 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0055_customevent.py
+-rw-r--r--   0        0        0      332 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0056_rename_customevent_personalevent.py
+-rw-r--r--   0        0        0      505 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0057_drop_otp_yubikey.py
+-rw-r--r--   0        0        0      720 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0058_migrate_preferences_to_global.py
+-rw-r--r--   0        0        0     5514 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0059_drop_site.py
+-rw-r--r--   0        0        0     1165 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0060_person_unique_short_name_email.py
+-rw-r--r--   0        0        0      500 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0061_remove_group_additional_fields.py
+-rw-r--r--   0        0        0        0 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/__init__.py
+-rw-r--r--   0        0        0    25176 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/mixins.py
+-rw-r--r--   0        0        0    64469 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/models.py
+-rw-r--r--   0        0        0    15497 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/preferences.py
+-rw-r--r--   0        0        0      611 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/registries.py
+-rw-r--r--   0        0        0    17713 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/rules.py
+-rw-r--r--   0        0        0    11074 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/__init__.py
+-rw-r--r--   0        0        0     7649 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/base.py
+-rw-r--r--   0        0        0     4023 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/calendar.py
+-rw-r--r--   0        0        0     3049 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/celery_progress.py
+-rw-r--r--   0        0        0      585 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/custom_menu.py
+-rw-r--r--   0        0        0      459 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/dynamic_routes.py
+-rw-r--r--   0        0        0     2005 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/group.py
+-rw-r--r--   0        0        0     1309 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/group_type.py
+-rw-r--r--   0        0        0     1430 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/holiday.py
+-rw-r--r--   0        0        0     1743 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/installed_apps.py
+-rw-r--r--   0        0        0      265 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/message.py
+-rw-r--r--   0        0        0     1296 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/notification.py
+-rw-r--r--   0        0        0     1145 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/oauth.py
+-rw-r--r--   0        0        0      554 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/pdf.py
+-rw-r--r--   0        0        0      124 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/permissions.py
+-rw-r--r--   0        0        0    10060 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/person.py
+-rw-r--r--   0        0        0     3382 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/personal_event.py
+-rw-r--r--   0        0        0     1270 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/room.py
+-rw-r--r--   0        0        0     2147 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/school_term.py
+-rw-r--r--   0        0        0      868 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/search.py
+-rw-r--r--   0        0        0     1343 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/site_preferences.py
+-rw-r--r--   0        0        0     1697 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/system_properties.py
+-rw-r--r--   0        0        0     3297 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/two_factor.py
+-rw-r--r--   0        0        0      829 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/user.py
+-rw-r--r--   0        0        0      418 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/search_indexes.py
+-rw-r--r--   0        0        0    39858 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/settings.py
+-rw-r--r--   0        0        0    49621 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-banner.svg
+-rw-r--r--   0        0        0     1862 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-favicon.png
+-rw-r--r--   0        0        0    17172 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon-maskable.png
+-rw-r--r--   0        0        0     7843 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon-maskable.svg
+-rw-r--r--   0        0        0    31902 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon.png
+-rw-r--r--   0        0        0     7346 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon.svg
+-rw-r--r--   0        0        0    19126 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/fallback.png
+-rw-r--r--   0        0        0     2237 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/hero.svg
+-rw-r--r--   0        0        0      490 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/js/copy_button.js
+-rw-r--r--   0        0        0      521 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/edit_dashboard.js
+-rw-r--r--   0        0        0      618 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/helper.js
+-rw-r--r--   0        0        0      984 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/include_ajax_live.js
+-rw-r--r--   0        0        0     4351 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/main.js
+-rw-r--r--   0        0        0     1654 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/multi_select.js
+-rw-r--r--   0        0        0     3495 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/search.js
+-rw-r--r--   0        0        0     2581 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/serviceworker.js
+-rw-r--r--   0        0        0      271 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/print-simple.css
+-rw-r--r--   0        0        0     1627 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/print.css
+-rw-r--r--   0        0        0      187 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/print_landscape.css
+-rw-r--r--   0        0        0     1064 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/public/materialize-custom.scss
+-rw-r--r--   0        0        0    15749 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/public/style.scss
+-rw-r--r--   0        0        0    11345 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/public/theme.scss
+-rw-r--r--   0        0        0     5408 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/tables.py
+-rw-r--r--   0        0        0     2330 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/tasks.py
+-rw-r--r--   0        0        0      838 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/403.html
+-rw-r--r--   0        0        0      789 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/404.html
+-rw-r--r--   0        0        0      918 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/500.html
+-rw-r--r--   0        0        0       76 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/503.html
+-rw-r--r--   0        0        0      851 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/account_inactive.html
+-rw-r--r--   0        0        0      169 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/email/base_message.txt
+-rw-r--r--   0        0        0      525 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0        0        0     1255 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/email_confirm.html
+-rw-r--r--   0        0        0     1182 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_change.html
+-rw-r--r--   0        0        0     1377 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset.html
+-rw-r--r--   0        0        0      825 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0     2305 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      649 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      500 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_set.html
+-rw-r--r--   0        0        0      888 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/signup.html
+-rw-r--r--   0        0        0      838 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      820 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/verification_email_required.html
+-rw-r--r--   0        0        0     1160 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      979 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/components/chips.html
+-rw-r--r--   0        0        0      350 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/components/materialize-chips.html
+-rw-r--r--   0        0        0      225 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/components/msgbox.html
+-rw-r--r--   0        0        0      958 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/components/pagination.html
+-rw-r--r--   0        0        0      486 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/components/text_collapsible.html
+-rw-r--r--   0        0        0     1053 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/announcement/form.html
+-rw-r--r--   0        0        0     1900 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/announcement/list.html
+-rw-r--r--   0        0        0     3099 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/base.html
+-rw-r--r--   0        0        0     2454 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/base_print.html
+-rw-r--r--   0        0        0     1212 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/base_simple_print.html
+-rw-r--r--   0        0        0      628 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/create.html
+-rw-r--r--   0        0        0      635 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
+-rw-r--r--   0        0        0      626 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/edit.html
+-rw-r--r--   0        0        0      262 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
+-rw-r--r--   0        0        0     1349 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/list.html
+-rw-r--r--   0        0        0      226 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
+-rw-r--r--   0        0        0     3879 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/data_check/list.html
+-rw-r--r--   0        0        0     2233 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/edit_dashboard.html
+-rw-r--r--   0        0        0        0 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/empty.html
+-rw-r--r--   0        0        0     5310 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/child_groups.html
+-rw-r--r--   0        0        0      650 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/edit.html
+-rw-r--r--   0        0        0     3382 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/full.html
+-rw-r--r--   0        0        0     1019 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/list.html
+-rw-r--r--   0        0        0     2504 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/index.html
+-rw-r--r--   0        0        0      777 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/pages/delete.html
+-rw-r--r--   0        0        0     6832 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/pages/system_status.html
+-rw-r--r--   0        0        0      603 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/pages/test_pdf.html
+-rw-r--r--   0        0        0       93 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/address.html
+-rw-r--r--   0        0        0      189 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/admins_list.html
+-rw-r--r--   0        0        0     1632 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/announcements.html
+-rw-r--r--   0        0        0     1472 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/avatar_content.html
+-rw-r--r--   0        0        0      319 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/copy_button.html
+-rw-r--r--   0        0        0     1089 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/crud_events.html
+-rw-r--r--   0        0        0      389 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/edit_dashboard_widget.html
+-rw-r--r--   0        0        0     1624 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/meta.html
+-rw-r--r--   0        0        0      414 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/on_page_menu.html
+-rw-r--r--   0        0        0      260 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/save_button.html
+-rw-r--r--   0        0        0     2358 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/splash_screen.html
+-rw-r--r--   0        0        0      325 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/turnable.html
+-rw-r--r--   0        0        0      915 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/perms/assign.html
+-rw-r--r--   0        0        0     2478 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/perms/list.html
+-rw-r--r--   0        0        0      376 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/collection.html
+-rw-r--r--   0        0        0      649 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/create.html
+-rw-r--r--   0        0        0      645 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/edit.html
+-rw-r--r--   0        0        0     1165 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/list.html
+-rw-r--r--   0        0        0      927 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/vue_index.html
+-rw-r--r--   0        0        0     3921 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/django_tables2/materialize.html
+-rw-r--r--   0        0        0      981 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/dynamic_preferences/form.html
+-rw-r--r--   0        0        0      376 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/dynamic_preferences/sections.html
+-rw-r--r--   0        0        0      764 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/disabled.html
+-rw-r--r--   0        0        0     1281 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/enter.html
+-rw-r--r--   0        0        0     1162 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/forms/_invite.html
+-rw-r--r--   0        0        0      102 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/messages/invite_accepted.txt
+-rw-r--r--   0        0        0      171 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/material/field_errors.html
+-rw-r--r--   0        0        0     1232 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
+-rw-r--r--   0        0        0     1897 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/colorfield_colorwidget.html
+-rw-r--r--   0        0        0     1009 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
+-rw-r--r--   0        0        0     1009 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/django_select2_select2widget.html
+-rw-r--r--   0        0        0      253 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/material/non_field_errors.html
+-rw-r--r--   0        0        0      663 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/create.html
+-rw-r--r--   0        0        0     2335 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/detail.html
+-rw-r--r--   0        0        0      669 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/edit.html
+-rw-r--r--   0        0        0     1074 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/list.html
+-rw-r--r--   0        0        0     2686 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/authorize.html
+-rw-r--r--   0        0        0      887 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/offline.html
+-rw-r--r--   0        0        0       42 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/search/indexes/core/group_text.txt
+-rw-r--r--   0        0        0       69 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/search/indexes/core/person_text.txt
+-rw-r--r--   0        0        0       42 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/search/indexes/core/room_text.txt
+-rw-r--r--   0        0        0     3171 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/search/search.html
+-rw-r--r--   0        0        0      243 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/search/searchbar_snippet.html
+-rw-r--r--   0        0        0      150 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/search/searchbar_snippets.html
+-rw-r--r--   0        0        0      169 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/sms/notification.txt
+-rw-r--r--   0        0        0      893 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0     1268 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/connections.html
+-rw-r--r--   0        0        0     1289 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/login.html
+-rw-r--r--   0        0        0      809 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/login_cancelled.html
+-rw-r--r--   0        0        0     1012 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/signup.html
+-rw-r--r--   0        0        0     1660 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/snippets/provider_list.html
+-rw-r--r--   0        0        0      630 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/base.email
+-rw-r--r--   0        0        0     1527 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/celery_failure.email
+-rw-r--r--   0        0        0      994 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/data_checks.email
+-rw-r--r--   0        0        0     1014 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/email.css
+-rw-r--r--   0        0        0     1102 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/invitation.email
+-rw-r--r--   0        0        0     1461 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/notification.email
+-rw-r--r--   0        0        0      668 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/person_changed.email
+-rw-r--r--   0        0        0      219 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/_base_focus.html
+-rw-r--r--   0        0        0      877 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/_wizard_actions.html
+-rw-r--r--   0        0        0      119 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/_wizard_forms.html
+-rw-r--r--   0        0        0     1780 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/backup_tokens.html
+-rw-r--r--   0        0        0     6686 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/login.html
+-rw-r--r--   0        0        0      943 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/otp_required.html
+-rw-r--r--   0        0        0      986 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/phone_register.html
+-rw-r--r--   0        0        0     3050 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/setup.html
+-rw-r--r--   0        0        0     2127 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/setup_complete.html
+-rw-r--r--   0        0        0      786 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/profile/disable.html
+-rw-r--r--   0        0        0        0 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templatetags/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templatetags/apps.py
+-rw-r--r--   0        0        0      394 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templatetags/dashboard.py
+-rw-r--r--   0        0        0     1611 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templatetags/data_helpers.py
+-rw-r--r--   0        0        0     1543 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templatetags/html_helpers.py
+-rw-r--r--   0        0        0      206 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templatetags/msg_box.py
+-rw-r--r--   0        0        0     3696 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/tests/browser/test_selenium.py
+-rw-r--r--   0        0        0      761 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/tests/managers/test_aleksisbasemanager.py
+-rw-r--r--   0        0        0     1607 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/tests/mixins/test_registry_object.py
+-rw-r--r--   0        0        0     6596 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test.pdf
+-rw-r--r--   0        0        0     1520 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_group_sync.py
+-rw-r--r--   0        0        0     3049 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_notification.py
+-rw-r--r--   0        0        0     4003 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_pdffile.py
+-rw-r--r--   0        0        0      427 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_person.py
+-rw-r--r--   0        0        0     5503 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/regression/test_regression.py
+-rw-r--r--   0        0        0      683 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/regression/view_oauth.py
+-rw-r--r--   0        0        0     1021 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/templatetags/test_data_helpers.py
+-rw-r--r--   0        0        0     2292 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/views/test_account.py
+-rw-r--r--   0        0        0    17541 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/urls.py
+-rw-r--r--   0        0        0        0 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-04 06:54:54.083692 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    14949 2024-04-04 06:54:55.515676 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0    10101 2024-04-04 06:54:56.451665 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
+-rw-r--r--   0        0        0    29144 2024-04-04 06:54:54.083692 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     1500 2024-04-04 06:54:54.495688 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/email.cpython-311.pyc
+-rw-r--r--   0        0        0      771 2024-04-04 06:54:56.463665 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     5811 2024-04-04 06:54:56.455665 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
+-rw-r--r--   0        0        0     9909 2024-04-04 06:54:56.691662 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
+-rw-r--r--   0        0        0     2181 2024-04-04 06:54:55.535676 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0      657 2024-04-04 06:54:55.535676 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
+-rw-r--r--   0        0        0    11018 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/apps.py
+-rw-r--r--   0        0        0     6343 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/auth_helpers.py
+-rw-r--r--   0        0        0     7920 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/celery_progress.py
+-rw-r--r--   0        0        0      197 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/context_processors.py
+-rw-r--r--   0        0        0    18985 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/core_helpers.py
+-rw-r--r--   0        0        0      986 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/email.py
+-rw-r--r--   0        0        0     1175 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/forms.py
+-rw-r--r--   0        0        0     2901 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/frontend_helpers.py
+-rw-r--r--   0        0        0     2375 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/ldap.py
+-rw-r--r--   0        0        0   192829 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/licenses.json
+-rw-r--r--   0        0        0     2255 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/messages.py
+-rw-r--r--   0        0        0     2091 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/middlewares.py
+-rw-r--r--   0        0        0      850 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/model_helpers.py
+-rw-r--r--   0        0        0     3818 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/notifications.py
+-rw-r--r--   0        0        0     6131 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/pdf.py
+-rw-r--r--   0        0        0     5801 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/predicates.py
+-rw-r--r--   0        0        0      936 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/sass_helpers.py
+-rw-r--r--   0        0        0      524 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/search.py
+-rw-r--r--   0        0        0      125 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/spdx.py
+-rw-r--r--   0        0        0     1673 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/tables.py
+-rw-r--r--   0        0        0    52591 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/views.py
+-rw-r--r--   0        0        0    12147 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/vite.config.js
+-rw-r--r--   0        0        0      173 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/wsgi.py
+-rw-r--r--   0        0        0       44 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/conftest.py
+-rw-r--r--   0        0        0      581 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/docs/Makefile
+-rw-r--r--   0        0        0   127432 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/2fa.png
+-rw-r--r--   0        0        0    71362 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/accept_invite.png
+-rw-r--r--   0        0        0    72621 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/create_dashboard_widget.png
+-rw-r--r--   0        0        0    41935 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/create_social_application.png
+-rw-r--r--   0        0        0    72508 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/dashboard.png
+-rw-r--r--   0        0        0    87601 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/dashboard_widgets.png
+-rw-r--r--   0        0        0   119523 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/data_checks.png
+-rw-r--r--   0        0        0    81386 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/edit_dashboard.png
+-rw-r--r--   0        0        0    85722 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/edit_default_dashboard.png
+-rw-r--r--   0        0        0   107979 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/invitations.png
+-rw-r--r--   0        0        0   177681 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/invite_existing.png
+-rw-r--r--   0        0        0    44868 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/pwa_desktop_chromium.png
+-rw-r--r--   0        0        0    69215 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/pwa_mobile_chromium.png
+-rw-r--r--   0        0        0   128479 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/pwa_mobile_firefox.png
+-rw-r--r--   0        0        0   108973 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/pwa_mobile_safari.png
+-rw-r--r--   0        0        0    69804 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/_static/signup.png
+-rw-r--r--   0        0        0      132 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     4231 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/01_core_concepts.rst
+-rw-r--r--   0        0        0     8109 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/10_install.rst
+-rw-r--r--   0        0        0     1872 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/15_config_files.rst
+-rw-r--r--   0        0        0     2086 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/16_config_options.rst
+-rw-r--r--   0        0        0     1648 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/17_storage.rst
+-rw-r--r--   0        0        0      803 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/18_mail.rst
+-rw-r--r--   0        0        0     1509 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/21_ldap.rst
+-rw-r--r--   0        0        0     3037 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/22_registration.rst
+-rw-r--r--   0        0        0     1467 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/23_socialaccounts.rst
+-rw-r--r--   0        0        0     3218 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/31_monitoring.rst
+-rw-r--r--   0        0        0     1012 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/32_tasks.rst
+-rw-r--r--   0        0        0     1393 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/33_data_checks.rst
+-rw-r--r--   0        0        0     4610 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/50_dashboard.rst
+-rw-r--r--   0        0        0     6392 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/conf.py
+-rw-r--r--   0        0        0      132 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/00_index.rst
+-rw-r--r--   0        0        0     4058 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/01_setup.rst
+-rw-r--r--   0        0        0     1427 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/02_install_apps.rst
+-rw-r--r--   0        0        0     3117 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/03_run_tests.rst
+-rw-r--r--   0        0        0     4519 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/04_materialize_templates.rst
+-rw-r--r--   0        0        0      289 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/05_extensible_models.rst
+-rw-r--r--   0        0        0     1148 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/06_merging_app_settings.rst
+-rw-r--r--   0        0        0     1349 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/10_dashboard_widgets.rst
+-rw-r--r--   0        0        0      514 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/index.rst
+-rw-r--r--   0        0        0      787 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/make.bat
+-rw-r--r--   0        0        0       95 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/00_index.rst
+-rw-r--r--   0        0        0       69 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/01_checks.rst
+-rw-r--r--   0        0        0       70 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/02_managers.rst
+-rw-r--r--   0        0        0       64 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/03_mixins.rst
+-rw-r--r--   0        0        0       84 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/04_models.rst
+-rw-r--r--   0        0        0      108 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/05_registries.rst
+-rw-r--r--   0        0        0       93 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/06_search_indexes.rst
+-rw-r--r--   0        0        0       79 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/07_tables.rst
+-rw-r--r--   0        0        0       90 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/08_tasks.rst
+-rw-r--r--   0        0        0     1017 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/09_utils.rst
+-rw-r--r--   0        0        0       71 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/10_views.rst
+-rw-r--r--   0        0        0       77 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/11_filters.rst
+-rw-r--r--   0        0        0      373 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/12_template_tags.rst
+-rw-r--r--   0        0        0      112 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/user/00_index.rst
+-rw-r--r--   0        0        0     1152 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/user/01_registration.rst
+-rw-r--r--   0        0        0     3465 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/user/02_personal_account.rst
+-rw-r--r--   0        0        0     1770 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/user/10_dashboard.rst
+-rw-r--r--   0        0        0     2607 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/user/20_pwa.rst
+-rw-r--r--   0        0        0     5570 2024-04-04 06:54:24.344036 aleksis_core-4.0.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     2180 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/tox.ini
+-rw-r--r--   0        0        0     8737 1970-01-01 00:00:00.000000 aleksis_core-4.0.0.dev6/PKG-INFO
```

### Comparing `aleksis_core-4.0.0.dev5/CHANGELOG.rst` & `aleksis_core-4.0.0.dev6/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -47,18 +47,21 @@
 * [Dev] Child groups are exposed in the GraphQL type for groups.
 * Content width on different screen sizes is more consistent.
 * Room model icon changed from the default to a specific one.
 
 Fixed
 ~~~~~
 
+* Persons could not be edited by non-superusers with global person editing permission.
 * GraphQL mutations did not return errors in case of exceptions.
 * Make email field unique over all persons.
 * Third-party login buttons now directly open external login page.
 * Opening group details wasn't possible without permissions for all person details.
+* [Dev] Foreign keys to ExtensiblePolymorphicModel types were using the wrong manager.
+* [Dev] Allow activating more frequent polling for Celery task progress.
 
 Removed
 ~~~~~~~
 
 * Yubikey support (not WebAuthn) was removed
 * [Dev] `_recursive` methods for groups have been removed.
   Developers relying on parent groups need to account for recursion themselves.
```

### Comparing `aleksis_core-4.0.0.dev5/LICENCE.rst` & `aleksis_core-4.0.0.dev6/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/README.rst` & `aleksis_core-4.0.0.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/__main__.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/__main__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 464
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/admin.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/admin.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 1002
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/apps.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/apps.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 8751
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/celery.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/celery.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 1338
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/checks.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/checks.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 2759
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/data_checks.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/data_checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 14836
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/health_checks.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/health_checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 2642
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/managers.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/managers.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
-files sz: 5541
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+files sz: 5688
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a0401
@@ -93,108 +93,108 @@
                116 MAKE_FUNCTION            0
                118 LOAD_CONST              11 ('AlekSISBaseManager')
                120 LOAD_NAME               10 (Manager)
                122 PRECALL                  3
                126 CALL                     3
                136 STORE_NAME              18 (AlekSISBaseManager)
    
-    30         138 PUSH_NULL
+    34         138 PUSH_NULL
                140 LOAD_BUILD_CLASS
-               142 LOAD_CONST              12 (<code object AlekSISBaseManagerWithoutMigrations, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 30>)
+               142 LOAD_CONST              12 (<code object AlekSISBaseManagerWithoutMigrations, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 34>)
                144 MAKE_FUNCTION            0
                146 LOAD_CONST              13 ('AlekSISBaseManagerWithoutMigrations')
                148 LOAD_NAME               18 (AlekSISBaseManager)
                150 PRECALL                  3
                154 CALL                     3
                164 STORE_NAME              19 (AlekSISBaseManagerWithoutMigrations)
    
-    36         166 PUSH_NULL
+    40         166 PUSH_NULL
                168 LOAD_BUILD_CLASS
-               170 LOAD_CONST              14 (<code object DateRangeQuerySetMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 36>)
+               170 LOAD_CONST              14 (<code object DateRangeQuerySetMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 40>)
                172 MAKE_FUNCTION            0
                174 LOAD_CONST              15 ('DateRangeQuerySetMixin')
                176 PRECALL                  2
                180 CALL                     2
                190 STORE_NAME              20 (DateRangeQuerySetMixin)
    
-    55         192 PUSH_NULL
+    59         192 PUSH_NULL
                194 LOAD_BUILD_CLASS
-               196 LOAD_CONST              16 (<code object SchoolTermQuerySet, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 55>)
+               196 LOAD_CONST              16 (<code object SchoolTermQuerySet, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 59>)
                198 MAKE_FUNCTION            0
                200 LOAD_CONST              17 ('SchoolTermQuerySet')
                202 LOAD_NAME                8 (QuerySet)
                204 LOAD_NAME               20 (DateRangeQuerySetMixin)
                206 PRECALL                  4
                210 CALL                     4
                220 STORE_NAME              21 (SchoolTermQuerySet)
    
-    59         222 PUSH_NULL
+    63         222 PUSH_NULL
                224 LOAD_BUILD_CLASS
-               226 LOAD_CONST              18 (<code object SchoolTermRelatedQuerySet, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 59>)
+               226 LOAD_CONST              18 (<code object SchoolTermRelatedQuerySet, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 63>)
                228 MAKE_FUNCTION            0
                230 LOAD_CONST              19 ('SchoolTermRelatedQuerySet')
                232 LOAD_NAME                8 (QuerySet)
                234 PRECALL                  3
                238 CALL                     3
                248 STORE_NAME              22 (SchoolTermRelatedQuerySet)
    
-   104         250 PUSH_NULL
+   108         250 PUSH_NULL
                252 LOAD_BUILD_CLASS
-               254 LOAD_CONST              20 (<code object GroupManager, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 104>)
+               254 LOAD_CONST              20 (<code object GroupManager, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 108>)
                256 MAKE_FUNCTION            0
                258 LOAD_CONST              21 ('GroupManager')
                260 LOAD_NAME               19 (AlekSISBaseManagerWithoutMigrations)
                262 PRECALL                  3
                266 CALL                     3
                276 STORE_NAME              23 (GroupManager)
    
-   112         278 PUSH_NULL
+   116         278 PUSH_NULL
                280 LOAD_BUILD_CLASS
-               282 LOAD_CONST              22 (<code object GroupQuerySet, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 112>)
+               282 LOAD_CONST              22 (<code object GroupQuerySet, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 116>)
                284 MAKE_FUNCTION            0
                286 LOAD_CONST              23 ('GroupQuerySet')
                288 LOAD_NAME               22 (SchoolTermRelatedQuerySet)
                290 PRECALL                  3
                294 CALL                     3
                304 STORE_NAME              24 (GroupQuerySet)
    
-   116         306 PUSH_NULL
+   120         306 PUSH_NULL
                308 LOAD_BUILD_CLASS
-               310 LOAD_CONST              24 (<code object UninstallRenitentPolymorphicManager, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 116>)
+               310 LOAD_CONST              24 (<code object UninstallRenitentPolymorphicManager, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 120>)
                312 MAKE_FUNCTION            0
                314 LOAD_CONST              25 ('UninstallRenitentPolymorphicManager')
                316 LOAD_NAME               14 (PolymorphicManager)
                318 PRECALL                  3
                322 CALL                     3
                332 STORE_NAME              25 (UninstallRenitentPolymorphicManager)
    
-   128         334 PUSH_NULL
+   132         334 PUSH_NULL
                336 LOAD_BUILD_CLASS
-               338 LOAD_CONST              26 (<code object InstalledWidgetsDashboardWidgetOrderManager, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 128>)
+               338 LOAD_CONST              26 (<code object InstalledWidgetsDashboardWidgetOrderManager, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 132>)
                340 MAKE_FUNCTION            0
                342 LOAD_CONST              27 ('InstalledWidgetsDashboardWidgetOrderManager')
                344 LOAD_NAME               10 (Manager)
                346 PRECALL                  3
                350 CALL                     3
                360 STORE_NAME              26 (InstalledWidgetsDashboardWidgetOrderManager)
    
-   142         362 PUSH_NULL
+   146         362 PUSH_NULL
                364 LOAD_BUILD_CLASS
-               366 LOAD_CONST              28 (<code object PolymorphicBaseManager, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 142>)
+               366 LOAD_CONST              28 (<code object PolymorphicBaseManager, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 146>)
                368 MAKE_FUNCTION            0
                370 LOAD_CONST              29 ('PolymorphicBaseManager')
                372 LOAD_NAME               19 (AlekSISBaseManagerWithoutMigrations)
                374 LOAD_NAME               14 (PolymorphicManager)
                376 PRECALL                  4
                380 CALL                     4
                390 STORE_NAME              27 (PolymorphicBaseManager)
    
-   146         392 PUSH_NULL
+   150         392 PUSH_NULL
                394 LOAD_BUILD_CLASS
-               396 LOAD_CONST              30 (<code object HolidayQuerySet, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 146>)
+               396 LOAD_CONST              30 (<code object HolidayQuerySet, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 150>)
                398 MAKE_FUNCTION            0
                400 LOAD_CONST              31 ('HolidayQuerySet')
                402 LOAD_NAME               20 (DateRangeQuerySetMixin)
                404 LOAD_NAME               15 (PolymorphicQuerySet)
                406 PRECALL                  4
                410 CALL                     4
                420 STORE_NAME              28 (HolidayQuerySet)
@@ -214,16 +214,16 @@
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504660288006601640384
-            0c5a0564046506640265046604880066016405840c5a0764026504660264
-            0684045a08880078015a095300
+            0c5a0564046506640265046604880066016405840c5a0764026504660288
+            0066016406840c5a08640265046602640784045a09880078015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
           15           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AlekSISBaseManager')
                       10 STORE_NAME               2 (__qualname__)
@@ -250,21 +250,30 @@
                       46 LOAD_CONST               5 (<code object managed_by_app, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 22>)
                       48 MAKE_FUNCTION           12 (annotations, closure)
                       50 STORE_NAME               7 (managed_by_app)
          
           26          52 LOAD_CONST               2 ('return')
                       54 LOAD_NAME                4 (QuerySet)
                       56 BUILD_TUPLE              2
-                      58 LOAD_CONST               6 (<code object get_queryset, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 26>)
-                      60 MAKE_FUNCTION            4 (annotations)
-                      62 STORE_NAME               8 (get_queryset)
-                      64 LOAD_CLOSURE             0 (__class__)
-                      66 COPY                     1
-                      68 STORE_NAME               9 (__classcell__)
-                      70 RETURN_VALUE
+                      58 LOAD_CLOSURE             0 (__class__)
+                      60 BUILD_TUPLE              1
+                      62 LOAD_CONST               6 (<code object managed_and_unmanaged, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 26>)
+                      64 MAKE_FUNCTION           12 (annotations, closure)
+                      66 STORE_NAME               8 (managed_and_unmanaged)
+         
+          30          68 LOAD_CONST               2 ('return')
+                      70 LOAD_NAME                4 (QuerySet)
+                      72 BUILD_TUPLE              2
+                      74 LOAD_CONST               7 (<code object get_queryset, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 30>)
+                      76 MAKE_FUNCTION            4 (annotations)
+                      78 STORE_NAME               9 (get_queryset)
+                      80 LOAD_CLOSURE             0 (__class__)
+                      82 COPY                     1
+                      84 STORE_NAME              10 (__classcell__)
+                      86 RETURN_VALUE
          consts
             'AlekSISBaseManager'
             'Base manager for AlekSIS model customisation.'
             'return'
             code
                argcount  : 1
                nlocals   : 1
@@ -343,112 +352,142 @@
                lnotab 0x0402
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
+                  0x95019700740100000000000000000000a6000000ab0000000000000000
+                  00a0010000000000000000000000000000000000000000a6000000ab0000
+                  000000000000005300
+                             0 COPY_FREE_VARS           1
+               
+                26           2 RESUME                   0
+               
+                28           4 LOAD_GLOBAL              1 (NULL + super)
+                            16 PRECALL                  0
+                            20 CALL                     0
+                            30 LOAD_METHOD              1 (get_queryset)
+                            52 PRECALL                  0
+                            56 CALL                     0
+                            66 RETURN_VALUE
+               consts
+                  'Get managed and unmanaged instances managed.'
+               names      ('super', 'get_queryset')
+               varnames   ('self',)
+               freevars   ('__class__',)
+               cellvars   ()
+               filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
+               name       'managed_and_unmanaged'
+               firstlineno 26
+               lnotab 0x0402
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 2
+               flags     : 3
+               code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000005300
-                26           0 RESUME                   0
+                30           0 RESUME                   0
                
-                27           2 LOAD_FAST                0 (self)
+                31           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (unmanaged)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 RETURN_VALUE
                consts
                   None
                names      ('unmanaged',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'get_queryset'
-               firstlineno 26
+               firstlineno 30
                lnotab 0x0201
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'QuerySet', 'unmanaged', 'str', 'managed_by_app', 'get_queryset', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'QuerySet', 'unmanaged', 'str', 'managed_by_app', 'managed_and_unmanaged', 'get_queryset', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
          name       'AlekSISBaseManager'
          firstlineno 15
-         lnotab 0x0c01040210041404
+         lnotab 0x0c010402100414041004
       'AlekSISBaseManager'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025a0464035300
-          30           0 RESUME                   0
+          34           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AlekSISBaseManagerWithoutMigrations')
                        8 STORE_NAME               2 (__qualname__)
          
-          31          10 LOAD_CONST               1 ('AlekSISBaseManager for auto-generating managers just by query sets.')
+          35          10 LOAD_CONST               1 ('AlekSISBaseManager for auto-generating managers just by query sets.')
                       12 STORE_NAME               3 (__doc__)
          
-          33          14 LOAD_CONST               2 (False)
+          37          14 LOAD_CONST               2 (False)
                       16 STORE_NAME               4 (use_in_migrations)
                       18 LOAD_CONST               3 (None)
                       20 RETURN_VALUE
          consts
             'AlekSISBaseManagerWithoutMigrations'
             'AlekSISBaseManager for auto-generating managers just by query sets.'
             False
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'use_in_migrations')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
          name       'AlekSISBaseManagerWithoutMigrations'
-         firstlineno 30
+         firstlineno 34
          lnotab 0x0a010402
       'AlekSISBaseManagerWithoutMigrations'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0264015a0364026504640365046604640484045a
             05640565066602640684045a07640765046602640884045a0864095300
-          36           0 RESUME                   0
+          40           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DateRangeQuerySetMixin')
                        8 STORE_NAME               2 (__qualname__)
          
-          37          10 LOAD_CONST               1 ('QuerySet with custom query methods for models with date ranges.\n\n    Filterable fields: date_start, date_end\n    ')
+          41          10 LOAD_CONST               1 ('QuerySet with custom query methods for models with date ranges.\n\n    Filterable fields: date_start, date_end\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-          42          14 LOAD_CONST               2 ('start')
+          46          14 LOAD_CONST               2 ('start')
                       16 LOAD_NAME                4 (date)
                       18 LOAD_CONST               3 ('end')
                       20 LOAD_NAME                4 (date)
                       22 BUILD_TUPLE              4
-                      24 LOAD_CONST               4 (<code object within_dates, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 42>)
+                      24 LOAD_CONST               4 (<code object within_dates, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 46>)
                       26 MAKE_FUNCTION            4 (annotations)
                       28 STORE_NAME               5 (within_dates)
          
-          46          30 LOAD_CONST               5 ('wanted_week')
+          50          30 LOAD_CONST               5 ('wanted_week')
                       32 LOAD_NAME                6 (CalendarWeek)
                       34 BUILD_TUPLE              2
-                      36 LOAD_CONST               6 (<code object in_week, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 46>)
+                      36 LOAD_CONST               6 (<code object in_week, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 50>)
                       38 MAKE_FUNCTION            4 (annotations)
                       40 STORE_NAME               7 (in_week)
          
-          50          42 LOAD_CONST               7 ('day')
+          54          42 LOAD_CONST               7 ('day')
                       44 LOAD_NAME                4 (date)
                       46 BUILD_TUPLE              2
-                      48 LOAD_CONST               8 (<code object on_day, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 50>)
+                      48 LOAD_CONST               8 (<code object on_day, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 54>)
                       50 MAKE_FUNCTION            4 (annotations)
                       52 STORE_NAME               8 (on_day)
                       54 LOAD_CONST               9 (None)
                       56 RETURN_VALUE
          consts
             'DateRangeQuerySetMixin'
             'QuerySet with custom query methods for models with date ranges.\n\n    Filterable fields: date_start, date_end\n    '
@@ -458,17 +497,17 @@
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c027c
                   01ac01a6020000ab0200000000000000005300
-                42           0 RESUME                   0
+                46           0 RESUME                   0
                
-                44           2 LOAD_FAST                0 (self)
+                48           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (filter)
                             26 LOAD_FAST                2 (end)
                             28 LOAD_FAST                1 (start)
                             30 KW_NAMES                 1
                             32 PRECALL                  2
                             36 CALL                     2
                             46 RETURN_VALUE
@@ -477,29 +516,29 @@
                   ('date_start__lte', 'date_end__gte')
                names      ('filter',)
                varnames   ('self', 'start', 'end')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'within_dates'
-               firstlineno 42
+               firstlineno 46
                lnotab 0x0202
             'wanted_week'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c0164
                   01190000000000000000007c01640219000000000000000000a6020000ab
                   0200000000000000005300
-                46           0 RESUME                   0
+                50           0 RESUME                   0
                
-                48           2 LOAD_FAST                0 (self)
+                52           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (within_dates)
                             26 LOAD_FAST                1 (wanted_week)
                             28 LOAD_CONST               1 (0)
                             30 BINARY_SUBSCR
                             40 LOAD_FAST                1 (wanted_week)
                             42 LOAD_CONST               2 (6)
                             44 BINARY_SUBSCR
@@ -512,147 +551,147 @@
                   6
                names      ('within_dates',)
                varnames   ('self', 'wanted_week')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'in_week'
-               firstlineno 46
+               firstlineno 50
                lnotab 0x0202
             'day'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c017c
                   01a6020000ab0200000000000000005300
-                50           0 RESUME                   0
+                54           0 RESUME                   0
                
-                52           2 LOAD_FAST                0 (self)
+                56           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (within_dates)
                             26 LOAD_FAST                1 (day)
                             28 LOAD_FAST                1 (day)
                             30 PRECALL                  2
                             34 CALL                     2
                             44 RETURN_VALUE
                consts
                   'Filter for all objects on a certain day.'
                names      ('within_dates',)
                varnames   ('self', 'day')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'on_day'
-               firstlineno 50
+               firstlineno 54
                lnotab 0x0202
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'date', 'within_dates', 'CalendarWeek', 'in_week', 'on_day')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
          name       'DateRangeQuerySetMixin'
-         firstlineno 36
+         firstlineno 40
          lnotab 0x0a01040510040c04
       'DateRangeQuerySetMixin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-          55           0 RESUME                   0
+          59           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SchoolTermQuerySet')
                        8 STORE_NAME               2 (__qualname__)
          
-          56          10 LOAD_CONST               1 ('Custom query set for school terms.')
+          60          10 LOAD_CONST               1 ('Custom query set for school terms.')
                       12 STORE_NAME               3 (__doc__)
                       14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'SchoolTermQuerySet'
             'Custom query set for school terms.'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
          name       'SchoolTermQuerySet'
-         firstlineno 55
+         firstlineno 59
          lnotab 0x0a01
       'SchoolTermQuerySet'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a0264015a03640265046403650464046400660664
             0584045a0564066506640464006604640784045a07640865046404640066
             04640984045a086411640c84045a096412640d84045a0a6404650b640e19
             0000000000000000006602640f84045a0c64105300
-          59           0 RESUME                   0
+          63           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SchoolTermRelatedQuerySet')
                        8 STORE_NAME               2 (__qualname__)
          
-          60          10 LOAD_CONST               1 ('Custom query set for all models related to school terms.')
+          64          10 LOAD_CONST               1 ('Custom query set for all models related to school terms.')
                       12 STORE_NAME               3 (__doc__)
          
-          62          14 LOAD_CONST               2 ('start')
+          66          14 LOAD_CONST               2 ('start')
                       16 LOAD_NAME                4 (date)
                       18 LOAD_CONST               3 ('end')
                       20 LOAD_NAME                4 (date)
                       22 LOAD_CONST               4 ('return')
                       24 LOAD_CONST               0 ('SchoolTermRelatedQuerySet')
                       26 BUILD_TUPLE              6
-                      28 LOAD_CONST               5 (<code object within_dates, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 62>)
+                      28 LOAD_CONST               5 (<code object within_dates, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 66>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               5 (within_dates)
          
-          66          34 LOAD_CONST               6 ('wanted_week')
+          70          34 LOAD_CONST               6 ('wanted_week')
                       36 LOAD_NAME                6 (CalendarWeek)
                       38 LOAD_CONST               4 ('return')
                       40 LOAD_CONST               0 ('SchoolTermRelatedQuerySet')
                       42 BUILD_TUPLE              4
-                      44 LOAD_CONST               7 (<code object in_week, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 66>)
+                      44 LOAD_CONST               7 (<code object in_week, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 70>)
                       46 MAKE_FUNCTION            4 (annotations)
                       48 STORE_NAME               7 (in_week)
          
-          70          50 LOAD_CONST               8 ('day')
+          74          50 LOAD_CONST               8 ('day')
                       52 LOAD_NAME                4 (date)
                       54 LOAD_CONST               4 ('return')
                       56 LOAD_CONST               0 ('SchoolTermRelatedQuerySet')
                       58 BUILD_TUPLE              4
-                      60 LOAD_CONST               9 (<code object on_day, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 70>)
+                      60 LOAD_CONST               9 (<code object on_day, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 74>)
                       62 MAKE_FUNCTION            4 (annotations)
                       64 STORE_NAME               8 (on_day)
          
-          74          66 LOAD_CONST              17 (('school_term', 'SchoolTerm', 'return', 'SchoolTermRelatedQuerySet'))
-                      68 LOAD_CONST              12 (<code object for_school_term, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 74>)
+          78          66 LOAD_CONST              17 (('school_term', 'SchoolTerm', 'return', 'SchoolTermRelatedQuerySet'))
+                      68 LOAD_CONST              12 (<code object for_school_term, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 78>)
                       70 MAKE_FUNCTION            4 (annotations)
                       72 STORE_NAME               9 (for_school_term)
          
-          77          74 LOAD_CONST              18 (('return', 'SchoolTermRelatedQuerySet'))
-                      76 LOAD_CONST              13 (<code object for_current_school_term_or_all, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 77>)
+          81          74 LOAD_CONST              18 (('return', 'SchoolTermRelatedQuerySet'))
+                      76 LOAD_CONST              13 (<code object for_current_school_term_or_all, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 81>)
                       78 MAKE_FUNCTION            4 (annotations)
                       80 STORE_NAME              10 (for_current_school_term_or_all)
          
-          90          82 LOAD_CONST               4 ('return')
+          94          82 LOAD_CONST               4 ('return')
                       84 LOAD_NAME               11 (Union)
                       86 LOAD_CONST              14 (('SchoolTermRelatedQuerySet', None))
                       88 BINARY_SUBSCR
                       98 BUILD_TUPLE              2
-                     100 LOAD_CONST              15 (<code object for_current_school_term_or_none, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 90>)
+                     100 LOAD_CONST              15 (<code object for_current_school_term_or_none, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 94>)
                      102 MAKE_FUNCTION            4 (annotations)
                      104 STORE_NAME              12 (for_current_school_term_or_none)
                      106 LOAD_CONST              16 (None)
                      108 RETURN_VALUE
          consts
             'SchoolTermRelatedQuerySet'
             'Custom query set for all models related to school terms.'
@@ -663,17 +702,17 @@
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c027c
                   01ac01a6020000ab0200000000000000005300
-                62           0 RESUME                   0
+                66           0 RESUME                   0
                
-                64           2 LOAD_FAST                0 (self)
+                68           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (filter)
                             26 LOAD_FAST                2 (end)
                             28 LOAD_FAST                1 (start)
                             30 KW_NAMES                 1
                             32 PRECALL                  2
                             36 CALL                     2
                             46 RETURN_VALUE
@@ -682,29 +721,29 @@
                   ('school_term__date_start__lte', 'school_term__date_end__gte')
                names      ('filter',)
                varnames   ('self', 'start', 'end')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'within_dates'
-               firstlineno 62
+               firstlineno 66
                lnotab 0x0202
             'wanted_week'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c0164
                   01190000000000000000007c01640219000000000000000000a6020000ab
                   0200000000000000005300
-                66           0 RESUME                   0
+                70           0 RESUME                   0
                
-                68           2 LOAD_FAST                0 (self)
+                72           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (within_dates)
                             26 LOAD_FAST                1 (wanted_week)
                             28 LOAD_CONST               1 (0)
                             30 BINARY_SUBSCR
                             40 LOAD_FAST                1 (wanted_week)
                             42 LOAD_CONST               2 (6)
                             44 BINARY_SUBSCR
@@ -717,57 +756,57 @@
                   6
                names      ('within_dates',)
                varnames   ('self', 'wanted_week')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'in_week'
-               firstlineno 66
+               firstlineno 70
                lnotab 0x0202
             'day'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c017c
                   01a6020000ab0200000000000000005300
-                70           0 RESUME                   0
+                74           0 RESUME                   0
                
-                72           2 LOAD_FAST                0 (self)
+                76           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (within_dates)
                             26 LOAD_FAST                1 (day)
                             28 LOAD_FAST                1 (day)
                             30 PRECALL                  2
                             34 CALL                     2
                             44 RETURN_VALUE
                consts
                   'Filter for all objects on a certain day.'
                names      ('within_dates',)
                varnames   ('self', 'day')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'on_day'
-               firstlineno 70
+               firstlineno 74
                lnotab 0x0202
             'school_term'
             'SchoolTerm'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c01ac
                   01a6010000ab0100000000000000005300
-                74           0 RESUME                   0
+                78           0 RESUME                   0
                
-                75           2 LOAD_FAST                0 (self)
+                79           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (filter)
                             26 LOAD_FAST                1 (school_term)
                             28 KW_NAMES                 1
                             30 PRECALL                  1
                             34 CALL                     1
                             44 RETURN_VALUE
                consts
@@ -775,138 +814,138 @@
                   ('school_term',)
                names      ('filter',)
                varnames   ('self', 'school_term')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'for_school_term'
-               firstlineno 74
+               firstlineno 78
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x9700640164026c006d017d0101007c016a0200000000000000007d027c
                   0272157c00a00300000000000000000000000000000000000000007c02a6
                   010000ab01000000000000000053007c005300
-                77           0 RESUME                   0
+                81           0 RESUME                   0
                
-                82           2 LOAD_CONST               1 (0)
+                86           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('SchoolTerm',))
                              6 IMPORT_NAME              0 (aleksis.core.models)
                              8 IMPORT_FROM              1 (SchoolTerm)
                             10 STORE_FAST               1 (SchoolTerm)
                             12 POP_TOP
                
-                84          14 LOAD_FAST                1 (SchoolTerm)
+                88          14 LOAD_FAST                1 (SchoolTerm)
                             16 LOAD_ATTR                2 (current)
                             26 STORE_FAST               2 (current_school_term)
                
-                85          28 LOAD_FAST                2 (current_school_term)
+                89          28 LOAD_FAST                2 (current_school_term)
                             30 POP_JUMP_FORWARD_IF_FALSE    21 (to 74)
                
-                86          32 LOAD_FAST                0 (self)
+                90          32 LOAD_FAST                0 (self)
                             34 LOAD_METHOD              3 (for_school_term)
                             56 LOAD_FAST                2 (current_school_term)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 RETURN_VALUE
                
-                88     >>   74 LOAD_FAST                0 (self)
+                92     >>   74 LOAD_FAST                0 (self)
                             76 RETURN_VALUE
                consts
                   'Get all objects related to current school term.\n\n        If there is no current school term, it will return all objects.\n        '
                   0
                   ('SchoolTerm',)
                names      ('aleksis.core.models', 'SchoolTerm', 'current', 'for_school_term')
                varnames   ('self', 'SchoolTerm', 'current_school_term')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'for_current_school_term_or_all'
-               firstlineno 77
+               firstlineno 81
                lnotab 0x02050c020e0104012a02
             ('SchoolTermRelatedQuerySet', None)
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x9700640164026c006d017d0101007c016a0200000000000000007d027c
                   0272157c00a00300000000000000000000000000000000000000007c02a6
                   010000ab010000000000000000530064035300
-                90           0 RESUME                   0
+                94           0 RESUME                   0
                
-                95           2 LOAD_CONST               1 (0)
+                99           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('SchoolTerm',))
                              6 IMPORT_NAME              0 (aleksis.core.models)
                              8 IMPORT_FROM              1 (SchoolTerm)
                             10 STORE_FAST               1 (SchoolTerm)
                             12 POP_TOP
                
-                97          14 LOAD_FAST                1 (SchoolTerm)
+               101          14 LOAD_FAST                1 (SchoolTerm)
                             16 LOAD_ATTR                2 (current)
                             26 STORE_FAST               2 (current_school_term)
                
-                98          28 LOAD_FAST                2 (current_school_term)
+               102          28 LOAD_FAST                2 (current_school_term)
                             30 POP_JUMP_FORWARD_IF_FALSE    21 (to 74)
                
-                99          32 LOAD_FAST                0 (self)
+               103          32 LOAD_FAST                0 (self)
                             34 LOAD_METHOD              3 (for_school_term)
                             56 LOAD_FAST                2 (current_school_term)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 RETURN_VALUE
                
-               101     >>   74 LOAD_CONST               3 (None)
+               105     >>   74 LOAD_CONST               3 (None)
                             76 RETURN_VALUE
                consts
                   'Get all objects related to current school term.\n\n        If there is no current school term, it will return `None`.\n        '
                   0
                   ('SchoolTerm',)
                   None
                names      ('aleksis.core.models', 'SchoolTerm', 'current', 'for_school_term')
                varnames   ('self', 'SchoolTerm', 'current_school_term')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'for_current_school_term_or_none'
-               firstlineno 90
+               firstlineno 94
                lnotab 0x02050c020e0104012a02
             None
             ('school_term', 'SchoolTerm', 'return', 'SchoolTermRelatedQuerySet')
             ('return', 'SchoolTermRelatedQuerySet')
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'date', 'within_dates', 'CalendarWeek', 'in_week', 'on_day', 'for_school_term', 'for_current_school_term_or_all', 'Union', 'for_current_school_term_or_none')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
          name       'SchoolTermRelatedQuerySet'
-         firstlineno 59
+         firstlineno 63
          lnotab 0x0a0104021404100410040803080d
       'SchoolTermRelatedQuerySet'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a03640284005a0464035300
-         104           0 RESUME                   0
+         108           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GroupManager')
                        8 STORE_NAME               2 (__qualname__)
          
-         105          10 LOAD_CONST               1 ('Manager adding specific methods to groups.')
+         109          10 LOAD_CONST               1 ('Manager adding specific methods to groups.')
                       12 STORE_NAME               3 (__doc__)
          
-         107          14 LOAD_CONST               2 (<code object get_queryset, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 107>)
+         111          14 LOAD_CONST               2 (<code object get_queryset, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 111>)
                       16 MAKE_FUNCTION            0
                       18 STORE_NAME               4 (get_queryset)
                       20 LOAD_CONST               3 (None)
                       22 RETURN_VALUE
          consts
             'GroupManager'
             'Manager adding specific methods to groups.'
@@ -915,17 +954,17 @@
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c00a60100
                   00ab010000000000000000a0020000000000000000000000000000000000
                   0000006401a6010000ab0100000000000000005300
-               107           0 RESUME                   0
+               111           0 RESUME                   0
                
-               109           2 LOAD_GLOBAL              1 (NULL + Manager)
+               113           2 LOAD_GLOBAL              1 (NULL + Manager)
                             14 LOAD_ATTR                1 (get_queryset)
                             24 LOAD_FAST                0 (self)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 LOAD_METHOD              2 (select_related)
                             62 LOAD_CONST               1 ('school_term')
                             64 PRECALL                  1
@@ -936,74 +975,74 @@
                   'school_term'
                names      ('Manager', 'get_queryset', 'select_related')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'get_queryset'
-               firstlineno 107
+               firstlineno 111
                lnotab 0x0202
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'get_queryset')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
          name       'GroupManager'
-         firstlineno 104
+         firstlineno 108
          lnotab 0x0a010402
       'GroupManager'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015300
-         112           0 RESUME                   0
+         116           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GroupQuerySet')
                        8 STORE_NAME               2 (__qualname__)
          
-         113          10 LOAD_CONST               1 (None)
+         117          10 LOAD_CONST               1 (None)
                       12 RETURN_VALUE
          consts
             'GroupQuerySet'
             None
          names      ('__name__', '__module__', '__qualname__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
          name       'GroupQuerySet'
-         firstlineno 112
+         firstlineno 116
          lnotab 0x0a01
       'GroupQuerySet'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0388006601640284085a04880078
             015a055300
                        0 MAKE_CELL                0 (__class__)
          
-         116           2 RESUME                   0
+         120           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('UninstallRenitentPolymorphicManager')
                       10 STORE_NAME               2 (__qualname__)
          
-         117          12 LOAD_CONST               1 ('A custom manager for django-polymorphic that filters out submodels of unavailable apps.')
+         121          12 LOAD_CONST               1 ('A custom manager for django-polymorphic that filters out submodels of unavailable apps.')
                       14 STORE_NAME               3 (__doc__)
          
-         119          16 LOAD_CLOSURE             0 (__class__)
+         123          16 LOAD_CLOSURE             0 (__class__)
                       18 BUILD_TUPLE              1
-                      20 LOAD_CONST               2 (<code object get_queryset, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 119>)
+                      20 LOAD_CONST               2 (<code object get_queryset, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 123>)
                       22 MAKE_FUNCTION            8 (closure)
                       24 STORE_NAME               4 (get_queryset)
                       26 LOAD_CLOSURE             0 (__class__)
                       28 COPY                     1
                       30 STORE_NAME               5 (__classcell__)
                       32 RETURN_VALUE
          consts
@@ -1022,31 +1061,31 @@
                   0000000000000000006a0500000000000000007c006a0200000000000000
                   00a0060000000000000000000000000000000000000000a6000000ab0000
                   000000000000008e005300740700000000000000000000a6000000ab0000
                   00000000000000a0040000000000000000000000000000000000000000a6
                   000000ab0000000000000000005300
                              0 COPY_FREE_VARS           1
                
-               119           2 RESUME                   0
+               123           2 RESUME                   0
                
-               120           4 LOAD_GLOBAL              1 (NULL + apps)
+               124           4 LOAD_GLOBAL              1 (NULL + apps)
                             16 LOAD_ATTR                1 (get_model)
                             26 LOAD_CONST               1 ('core')
                             28 LOAD_CONST               2 ('DashboardWidget')
                             30 PRECALL                  2
                             34 CALL                     2
                             44 STORE_FAST               1 (DashboardWidget)
                
-               121          46 LOAD_FAST                0 (self)
+               125          46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                2 (model)
                             58 LOAD_FAST                1 (DashboardWidget)
                             60 IS_OP                    0
                             62 POP_JUMP_FORWARD_IF_FALSE    63 (to 190)
                
-               122          64 PUSH_NULL
+               126          64 PUSH_NULL
                             66 LOAD_GLOBAL              7 (NULL + super)
                             78 PRECALL                  0
                             82 CALL                     0
                             92 LOAD_METHOD              4 (get_queryset)
                            114 PRECALL                  0
                            118 CALL                     0
                            128 LOAD_ATTR                5 (instance_of)
@@ -1054,15 +1093,15 @@
                            140 LOAD_ATTR                2 (model)
                            150 LOAD_METHOD              6 (__subclasses__)
                            172 PRECALL                  0
                            176 CALL                     0
                            186 CALL_FUNCTION_EX         0
                            188 RETURN_VALUE
                
-               125     >>  190 LOAD_GLOBAL              7 (NULL + super)
+               129     >>  190 LOAD_GLOBAL              7 (NULL + super)
                            202 PRECALL                  0
                            206 CALL                     0
                            216 LOAD_METHOD              4 (get_queryset)
                            238 PRECALL                  0
                            242 CALL                     0
                            252 RETURN_VALUE
                consts
@@ -1071,47 +1110,47 @@
                   'DashboardWidget'
                names      ('apps', 'get_model', 'model', 'super', 'get_queryset', 'instance_of', '__subclasses__')
                varnames   ('self', 'DashboardWidget')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'get_queryset'
-               firstlineno 119
+               firstlineno 123
                lnotab 0x04012a0112017e03
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'get_queryset', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
          name       'UninstallRenitentPolymorphicManager'
-         firstlineno 116
+         firstlineno 120
          lnotab 0x0c010402
       'UninstallRenitentPolymorphicManager'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0388006601640284085a04880078
             015a055300
                        0 MAKE_CELL                0 (__class__)
          
-         128           2 RESUME                   0
+         132           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('InstalledWidgetsDashboardWidgetOrderManager')
                       10 STORE_NAME               2 (__qualname__)
          
-         129          12 LOAD_CONST               1 ('A manager that only returns DashboardWidgetOrder objects with an existing widget.')
+         133          12 LOAD_CONST               1 ('A manager that only returns DashboardWidgetOrder objects with an existing widget.')
                       14 STORE_NAME               3 (__doc__)
          
-         131          16 LOAD_CLOSURE             0 (__class__)
+         135          16 LOAD_CLOSURE             0 (__class__)
                       18 BUILD_TUPLE              1
-                      20 LOAD_CONST               2 (<code object get_queryset, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 131>)
+                      20 LOAD_CONST               2 (<code object get_queryset, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 135>)
                       22 MAKE_FUNCTION            8 (closure)
                       24 STORE_NAME               4 (get_queryset)
                       26 LOAD_CLOSURE             0 (__class__)
                       28 COPY                     1
                       30 STORE_NAME               5 (__classcell__)
                       32 RETURN_VALUE
          consts
@@ -1132,43 +1171,43 @@
                   0000006401a6010000ab0100000000000000007d03740100000000000000
                   000000a6000000ab000000000000000000a0010000000000000000000000
                   000000000000000000a6000000ab000000000000000000a0090000000000
                   0000000000000000000000000000007c03ac02a6010000ab010000000000
                   0000005300
                              0 COPY_FREE_VARS           1
                
-               131           2 RESUME                   0
+               135           2 RESUME                   0
                
-               132           4 LOAD_GLOBAL              1 (NULL + super)
+               136           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (get_queryset)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 STORE_FAST               1 (queryset)
                
-               135          68 LOAD_FAST                1 (queryset)
+               139          68 LOAD_FAST                1 (queryset)
                             70 LOAD_ATTR                2 (model)
                             80 LOAD_ATTR                3 (widget)
                             90 LOAD_ATTR                4 (field)
                            100 LOAD_ATTR                5 (related_model)
                            110 STORE_FAST               2 (DashboardWidget)
                
-               136         112 LOAD_FAST                2 (DashboardWidget)
+               140         112 LOAD_FAST                2 (DashboardWidget)
                            114 LOAD_ATTR                6 (objects)
                            124 LOAD_METHOD              7 (all)
                            146 PRECALL                  0
                            150 CALL                     0
                            160 LOAD_METHOD              8 (values)
                            182 LOAD_CONST               1 ('id')
                            184 PRECALL                  1
                            188 CALL                     1
                            198 STORE_FAST               3 (dashboard_widget_pks)
                
-               139         200 LOAD_GLOBAL              1 (NULL + super)
+               143         200 LOAD_GLOBAL              1 (NULL + super)
                            212 PRECALL                  0
                            216 CALL                     0
                            226 LOAD_METHOD              1 (get_queryset)
                            248 PRECALL                  0
                            252 CALL                     0
                            262 LOAD_METHOD              9 (filter)
                            284 LOAD_FAST                3 (dashboard_widget_pks)
@@ -1182,77 +1221,77 @@
                   ('widget_id__in',)
                names      ('super', 'get_queryset', 'model', 'widget', 'field', 'related_model', 'objects', 'all', 'values', 'filter')
                varnames   ('self', 'queryset', 'DashboardWidget', 'dashboard_widget_pks')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'get_queryset'
-               firstlineno 131
+               firstlineno 135
                lnotab 0x040140032c015803
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'get_queryset', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
          name       'InstalledWidgetsDashboardWidgetOrderManager'
-         firstlineno 128
+         firstlineno 132
          lnotab 0x0c010402
       'InstalledWidgetsDashboardWidgetOrderManager'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-         142           0 RESUME                   0
+         146           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PolymorphicBaseManager')
                        8 STORE_NAME               2 (__qualname__)
          
-         143          10 LOAD_CONST               1 ('Default manager for extensible, polymorphic models.')
+         147          10 LOAD_CONST               1 ('Default manager for extensible, polymorphic models.')
                       12 STORE_NAME               3 (__doc__)
                       14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'PolymorphicBaseManager'
             'Default manager for extensible, polymorphic models.'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
          name       'PolymorphicBaseManager'
-         firstlineno 142
+         firstlineno 146
          lnotab 0x0a01
       'PolymorphicBaseManager'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0264015a03640265046505190000000000000000
             006602640384045a0664045300
-         146           0 RESUME                   0
+         150           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('HolidayQuerySet')
                        8 STORE_NAME               2 (__qualname__)
          
-         147          10 LOAD_CONST               1 ('QuerySet with custom query methods for holidays.')
+         151          10 LOAD_CONST               1 ('QuerySet with custom query methods for holidays.')
                       12 STORE_NAME               3 (__doc__)
          
-         149          14 LOAD_CONST               2 ('return')
+         153          14 LOAD_CONST               2 ('return')
                       16 LOAD_NAME                4 (list)
                       18 LOAD_NAME                5 (date)
                       20 BINARY_SUBSCR
                       30 BUILD_TUPLE              2
-                      32 LOAD_CONST               3 (<code object get_all_days, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 149>)
+                      32 LOAD_CONST               3 (<code object get_all_days, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py", line 153>)
                       34 MAKE_FUNCTION            4 (annotations)
                       36 STORE_NAME               6 (get_all_days)
                       38 LOAD_CONST               4 (None)
                       40 RETURN_VALUE
          consts
             'HolidayQuerySet'
             'QuerySet with custom query methods for holidays.'
@@ -1263,62 +1302,62 @@
                stacksize : 6
                flags     : 3
                code
                   0x970067007d017c0044005d267d027c017401000000000000000000007c
                   02a0010000000000000000000000000000000000000000a6000000ab0000
                   00000000000000a6010000ab0100000000000000007a0d00007d018c277c
                   015300
-               149           0 RESUME                   0
+               153           0 RESUME                   0
                
-               151           2 BUILD_LIST               0
+               155           2 BUILD_LIST               0
                              4 STORE_FAST               1 (holiday_days)
                
-               152           6 LOAD_FAST                0 (self)
+               156           6 LOAD_FAST                0 (self)
                              8 GET_ITER
                        >>   10 FOR_ITER                38 (to 88)
                             12 STORE_FAST               2 (holiday)
                
-               153          14 LOAD_FAST                1 (holiday_days)
+               157          14 LOAD_FAST                1 (holiday_days)
                             16 LOAD_GLOBAL              1 (NULL + list)
                             28 LOAD_FAST                2 (holiday)
                             30 LOAD_METHOD              1 (get_days)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 PRECALL                  1
                             70 CALL                     1
                             80 BINARY_OP               13 (+=)
                             84 STORE_FAST               1 (holiday_days)
                             86 JUMP_BACKWARD           39 (to 10)
                
-               154     >>   88 LOAD_FAST                1 (holiday_days)
+               158     >>   88 LOAD_FAST                1 (holiday_days)
                             90 RETURN_VALUE
                consts
                   'Get all days included in the selected holidays.'
                names      ('list', 'get_days')
                varnames   ('self', 'holiday_days', 'holiday')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
                name       'get_all_days'
-               firstlineno 149
+               firstlineno 153
                lnotab 0x0202040108014a01
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'list', 'date', 'get_all_days')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
          name       'HolidayQuerySet'
-         firstlineno 146
+         firstlineno 150
          lnotab 0x0a010402
       'HolidayQuerySet'
       None
    names      ('datetime', 'date', 'typing', 'TYPE_CHECKING', 'Union', 'django.apps', 'apps', 'django.db.models', 'QuerySet', 'django.db.models.manager', 'Manager', 'calendarweek', 'CalendarWeek', 'polymorphic.managers', 'PolymorphicManager', 'PolymorphicQuerySet', 'models', 'SchoolTerm', 'AlekSISBaseManager', 'AlekSISBaseManagerWithoutMigrations', 'DateRangeQuerySetMixin', 'SchoolTermQuerySet', 'SchoolTermRelatedQuerySet', 'GroupManager', 'GroupQuerySet', 'UninstallRenitentPolymorphicManager', 'InstalledWidgetsDashboardWidgetOrderManager', 'PolymorphicBaseManager', 'HolidayQuerySet')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/managers.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c0110020c010c010c020c01100204010c031c0f1c061a131e
+      0x00ff02010c0110020c010c010c020c01100204010c031c131c061a131e
       041c2d1c081c041c0c1c0e1e04
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/mixins.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/mixins.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
-files sz: 25138
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+files sz: 25176
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d015a010100640064036c026d
@@ -345,171 +345,171 @@
                578 LOAD_NAME               83 (_ExtensiblePolymorphicModelBase)
    
    305         580 KW_NAMES                36
                582 PRECALL                  5
                586 CALL                     5
                596 STORE_NAME              84 (ExtensiblePolymorphicModel)
    
-   316         598 PUSH_NULL
+   317         598 PUSH_NULL
                600 LOAD_BUILD_CLASS
-               602 LOAD_CONST              41 (<code object PureDjangoModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 316>)
+               602 LOAD_CONST              41 (<code object PureDjangoModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 317>)
                604 MAKE_FUNCTION            0
                606 LOAD_CONST              42 ('PureDjangoModel')
                608 PRECALL                  2
                612 CALL                     2
                622 STORE_NAME              85 (PureDjangoModel)
    
-   322         624 PUSH_NULL
+   323         624 PUSH_NULL
                626 LOAD_BUILD_CLASS
-               628 LOAD_CONST              43 (<code object GlobalPermissionModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 322>)
+               628 LOAD_CONST              43 (<code object GlobalPermissionModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 323>)
                630 MAKE_FUNCTION            0
                632 LOAD_CONST              44 ('GlobalPermissionModel')
                634 LOAD_NAME               19 (models)
                636 LOAD_ATTR               81 (Model)
                646 PRECALL                  3
                650 CALL                     3
                660 STORE_NAME              86 (GlobalPermissionModel)
    
-   333         662 PUSH_NULL
+   334         662 PUSH_NULL
                664 LOAD_BUILD_CLASS
-               666 LOAD_CONST              45 (<code object _ExtensibleFormMetaclass, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 333>)
+               666 LOAD_CONST              45 (<code object _ExtensibleFormMetaclass, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 334>)
                668 MAKE_FUNCTION            0
                670 LOAD_CONST              46 ('_ExtensibleFormMetaclass')
                672 LOAD_NAME               29 (ModelFormMetaclass)
                674 PRECALL                  3
                678 CALL                     3
                688 STORE_NAME              87 (_ExtensibleFormMetaclass)
    
-   346         690 PUSH_NULL
+   347         690 PUSH_NULL
                692 LOAD_BUILD_CLASS
-               694 LOAD_CONST              47 (<code object ExtensibleForm, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 346>)
+               694 LOAD_CONST              47 (<code object ExtensibleForm, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 347>)
                696 MAKE_FUNCTION            0
                698 LOAD_CONST              48 ('ExtensibleForm')
                700 LOAD_NAME               28 (ModelForm)
                702 LOAD_NAME               87 (_ExtensibleFormMetaclass)
                704 KW_NAMES                36
                706 PRECALL                  4
                710 CALL                     4
                720 STORE_NAME              88 (ExtensibleForm)
    
-   390         722 PUSH_NULL
+   391         722 PUSH_NULL
                724 LOAD_BUILD_CLASS
-               726 LOAD_CONST              49 (<code object BaseModelAdmin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 390>)
+               726 LOAD_CONST              49 (<code object BaseModelAdmin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 391>)
                728 MAKE_FUNCTION            0
                730 LOAD_CONST              50 ('BaseModelAdmin')
                732 LOAD_NAME               54 (GuardedModelAdmin)
                734 LOAD_NAME               68 (ObjectPermissionsModelAdmin)
                736 PRECALL                  4
                740 CALL                     4
                750 STORE_NAME              89 (BaseModelAdmin)
    
-   396         752 PUSH_NULL
+   397         752 PUSH_NULL
                754 LOAD_BUILD_CLASS
-               756 LOAD_CONST              51 (<code object SuccessMessageMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 396>)
+               756 LOAD_CONST              51 (<code object SuccessMessageMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 397>)
                758 MAKE_FUNCTION            0
                760 LOAD_CONST              52 ('SuccessMessageMixin')
                762 LOAD_NAME               45 (ModelFormMixin)
                764 PRECALL                  3
                768 CALL                     3
                778 STORE_NAME              90 (SuccessMessageMixin)
    
-   405         780 PUSH_NULL
+   406         780 PUSH_NULL
                782 LOAD_BUILD_CLASS
-               784 LOAD_CONST              53 (<code object SuccessNextMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 405>)
+               784 LOAD_CONST              53 (<code object SuccessNextMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 406>)
                786 MAKE_FUNCTION            0
                788 LOAD_CONST              54 ('SuccessNextMixin')
                790 LOAD_NAME               17 (RedirectURLMixin)
                792 PRECALL                  3
                796 CALL                     3
                806 STORE_NAME              91 (SuccessNextMixin)
    
-   412         808 PUSH_NULL
+   413         808 PUSH_NULL
                810 LOAD_BUILD_CLASS
-               812 LOAD_CONST              55 (<code object AdvancedCreateView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 412>)
+               812 LOAD_CONST              55 (<code object AdvancedCreateView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 413>)
                814 MAKE_FUNCTION            0
                816 LOAD_CONST              56 ('AdvancedCreateView')
                818 LOAD_NAME               90 (SuccessMessageMixin)
                820 LOAD_NAME               41 (CreateView)
                822 PRECALL                  4
                826 CALL                     4
                836 STORE_NAME              92 (AdvancedCreateView)
    
-   416         838 PUSH_NULL
+   417         838 PUSH_NULL
                840 LOAD_BUILD_CLASS
-               842 LOAD_CONST              57 (<code object AdvancedEditView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 416>)
+               842 LOAD_CONST              57 (<code object AdvancedEditView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 417>)
                844 MAKE_FUNCTION            0
                846 LOAD_CONST              58 ('AdvancedEditView')
                848 LOAD_NAME               90 (SuccessMessageMixin)
                850 LOAD_NAME               42 (UpdateView)
                852 PRECALL                  4
                856 CALL                     4
                866 STORE_NAME              93 (AdvancedEditView)
    
-   420         868 PUSH_NULL
+   421         868 PUSH_NULL
                870 LOAD_BUILD_CLASS
-               872 LOAD_CONST              59 (<code object AdvancedDeleteView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 420>)
+               872 LOAD_CONST              59 (<code object AdvancedDeleteView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 421>)
                874 MAKE_FUNCTION            0
                876 LOAD_CONST              60 ('AdvancedDeleteView')
                878 LOAD_NAME               44 (DeleteView)
                880 PRECALL                  3
                884 CALL                     3
                894 STORE_NAME              94 (AdvancedDeleteView)
    
-   439         896 PUSH_NULL
+   440         896 PUSH_NULL
                898 LOAD_BUILD_CLASS
-               900 LOAD_CONST              61 (<code object SchoolTermRelatedExtensibleModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 439>)
+               900 LOAD_CONST              61 (<code object SchoolTermRelatedExtensibleModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 440>)
                902 MAKE_FUNCTION            0
                904 LOAD_CONST              62 ('SchoolTermRelatedExtensibleModel')
                906 LOAD_NAME               82 (ExtensibleModel)
                908 PRECALL                  3
                912 CALL                     3
                922 STORE_NAME              95 (SchoolTermRelatedExtensibleModel)
    
-   457         924 PUSH_NULL
+   458         924 PUSH_NULL
                926 LOAD_BUILD_CLASS
-               928 LOAD_CONST              63 (<code object SchoolTermRelatedExtensibleForm, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 457>)
+               928 LOAD_CONST              63 (<code object SchoolTermRelatedExtensibleForm, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 458>)
                930 MAKE_FUNCTION            0
                932 LOAD_CONST              64 ('SchoolTermRelatedExtensibleForm')
                934 LOAD_NAME               88 (ExtensibleForm)
                936 PRECALL                  3
                940 CALL                     3
                950 STORE_NAME              96 (SchoolTermRelatedExtensibleForm)
    
-   474         952 PUSH_NULL
+   475         952 PUSH_NULL
                954 LOAD_BUILD_CLASS
-               956 LOAD_CONST              65 (<code object PublicFilePreferenceMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 474>)
+               956 LOAD_CONST              65 (<code object PublicFilePreferenceMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 475>)
                958 MAKE_FUNCTION            0
                960 LOAD_CONST              66 ('PublicFilePreferenceMixin')
                962 LOAD_NAME               52 (FilePreference)
                964 PRECALL                  3
                968 CALL                     3
                978 STORE_NAME              97 (PublicFilePreferenceMixin)
    
-   485         980 PUSH_NULL
+   486         980 PUSH_NULL
                982 LOAD_BUILD_CLASS
-               984 LOAD_CONST              67 (<code object RegistryObject, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 485>)
+               984 LOAD_CONST              67 (<code object RegistryObject, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 486>)
                986 MAKE_FUNCTION            0
                988 LOAD_CONST              68 ('RegistryObject')
                990 PRECALL                  2
                994 CALL                     2
               1004 STORE_NAME              98 (RegistryObject)
    
-   520        1006 PUSH_NULL
+   521        1006 PUSH_NULL
               1008 LOAD_BUILD_CLASS
-              1010 LOAD_CONST              69 (<code object ObjectAuthenticator, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 520>)
+              1010 LOAD_CONST              69 (<code object ObjectAuthenticator, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 521>)
               1012 MAKE_FUNCTION            0
               1014 LOAD_CONST              70 ('ObjectAuthenticator')
               1016 LOAD_NAME               98 (RegistryObject)
               1018 PRECALL                  3
               1022 CALL                     3
               1032 STORE_NAME              99 (ObjectAuthenticator)
    
-   525        1034 PUSH_NULL
+   526        1034 PUSH_NULL
               1036 LOAD_BUILD_CLASS
-              1038 LOAD_CONST              71 (<code object CalendarEventMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 525>)
+              1038 LOAD_CONST              71 (<code object CalendarEventMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 526>)
               1040 MAKE_FUNCTION            0
               1042 LOAD_CONST              72 ('CalendarEventMixin')
               1044 LOAD_NAME               98 (RegistryObject)
               1046 PRECALL                  3
               1050 CALL                     3
               1060 STORE_NAME             100 (CalendarEventMixin)
               1062 LOAD_CONST               1 (None)
@@ -2118,37 +2118,41 @@
             'ExtensiblePolymorphicModel'
             'Model class for extensible, polymorphic models.'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
-               code 0x970065005a0164005a0264015a0364025300
+               code 0x970065005a0164005a0264015a0364025a0464035300
                312           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('ExtensiblePolymorphicModel.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
                313          10 LOAD_CONST               1 (True)
                             12 STORE_NAME               3 (abstract)
-                            14 LOAD_CONST               2 (None)
-                            16 RETURN_VALUE
+               
+               314          14 LOAD_CONST               2 ('objects')
+                            16 STORE_NAME               4 (base_manager_name)
+                            18 LOAD_CONST               3 (None)
+                            20 RETURN_VALUE
                consts
                   'ExtensiblePolymorphicModel.Meta'
                   True
+                  'objects'
                   None
-               names      ('__name__', '__module__', '__qualname__', 'abstract')
+               names      ('__name__', '__module__', '__qualname__', 'abstract', 'base_manager_name')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'Meta'
                firstlineno 312
-               lnotab 0x0a01
+               lnotab 0x0a010401
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'PolymorphicBaseManager', 'objects', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
@@ -2158,58 +2162,58 @@
       'ExtensiblePolymorphicModel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-         316           0 RESUME                   0
+         317           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PureDjangoModel')
                        8 STORE_NAME               2 (__qualname__)
          
-         317          10 LOAD_CONST               1 ('No-op mixin to mark a model as deliberately not using ExtensibleModel.')
+         318          10 LOAD_CONST               1 ('No-op mixin to mark a model as deliberately not using ExtensibleModel.')
                       12 STORE_NAME               3 (__doc__)
          
-         319          14 LOAD_CONST               2 (None)
+         320          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'PureDjangoModel'
             'No-op mixin to mark a model as deliberately not using ExtensibleModel.'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'PureDjangoModel'
-         firstlineno 316
+         firstlineno 317
          lnotab 0x0a010402
       'PureDjangoModel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0264015a0302004700640284006403a6020000ab
             0200000000000000005a0464045300
-         322           0 RESUME                   0
+         323           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GlobalPermissionModel')
                        8 STORE_NAME               2 (__qualname__)
          
-         323          10 LOAD_CONST               1 ('Base model for global permissions.\n\n    This base model ensures that global permissions are not managed.')
+         324          10 LOAD_CONST               1 ('Base model for global permissions.\n\n    This base model ensures that global permissions are not managed.')
                       12 STORE_NAME               3 (__doc__)
          
-         327          14 PUSH_NULL
+         328          14 PUSH_NULL
                       16 LOAD_BUILD_CLASS
-                      18 LOAD_CONST               2 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 327>)
+                      18 LOAD_CONST               2 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 328>)
                       20 MAKE_FUNCTION            0
                       22 LOAD_CONST               3 ('Meta')
                       24 PRECALL                  2
                       28 CALL                     2
                       38 STORE_NAME               4 (Meta)
                       40 LOAD_CONST               4 (None)
                       42 RETURN_VALUE
@@ -2218,27 +2222,27 @@
             'Base model for global permissions.\n\n    This base model ensures that global permissions are not managed.'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035a0564045300
-               327           0 RESUME                   0
+               328           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('GlobalPermissionModel.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               328          10 LOAD_CONST               1 (())
+               329          10 LOAD_CONST               1 (())
                             12 STORE_NAME               3 (default_permissions)
                
-               329          14 LOAD_CONST               2 (True)
+               330          14 LOAD_CONST               2 (True)
                             16 STORE_NAME               4 (abstract)
                
-               330          18 LOAD_CONST               3 (False)
+               331          18 LOAD_CONST               3 (False)
                             20 STORE_NAME               5 (managed)
                             22 LOAD_CONST               4 (None)
                             24 RETURN_VALUE
                consts
                   'GlobalPermissionModel.Meta'
                   ()
                   True
@@ -2246,46 +2250,46 @@
                   None
                names      ('__name__', '__module__', '__qualname__', 'default_permissions', 'abstract', 'managed')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'Meta'
-               firstlineno 327
+               firstlineno 328
                lnotab 0x0a0104010401
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'GlobalPermissionModel'
-         firstlineno 322
+         firstlineno 323
          lnotab 0x0a010404
       'GlobalPermissionModel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03880078015a0453
             00
                        0 MAKE_CELL                0 (__class__)
          
-         333           2 RESUME                   0
+         334           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('_ExtensibleFormMetaclass')
                       10 STORE_NAME               2 (__qualname__)
          
-         334          12 LOAD_CLOSURE             0 (__class__)
+         335          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __new__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 334>)
+                      16 LOAD_CONST               1 (<code object __new__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 335>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__new__)
                       22 LOAD_CLOSURE             0 (__class__)
                       24 COPY                     1
                       26 STORE_NAME               4 (__classcell__)
                       28 RETURN_VALUE
          consts
@@ -2301,107 +2305,107 @@
                   03a6040000ab0400000000000000007d047405000000000000000000007c
                   046401a6020000ab020000000000000000720c7c046a0300000000000000
                   006a0400000000000000006e0167007d057c057c045f0500000000000000
                   00740d000000000000000000007c058e007c045f0300000000000000007c
                   045300
                              0 COPY_FREE_VARS           1
                
-               334           2 RESUME                   0
+               335           2 RESUME                   0
                
-               335           4 LOAD_GLOBAL              1 (NULL + super)
+               336           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (__new__)
                             52 LOAD_FAST                0 (cls)
                             54 LOAD_FAST                1 (name)
                             56 LOAD_FAST                2 (bases)
                             58 LOAD_FAST                3 (dct)
                             60 PRECALL                  4
                             64 CALL                     4
                             74 STORE_FAST               4 (x)
                
-               338          76 LOAD_GLOBAL              5 (NULL + hasattr)
+               339          76 LOAD_GLOBAL              5 (NULL + hasattr)
                             88 LOAD_FAST                4 (x)
                             90 LOAD_CONST               1 ('layout')
                             92 PRECALL                  2
                             96 CALL                     2
                            106 POP_JUMP_FORWARD_IF_FALSE    12 (to 132)
                            108 LOAD_FAST                4 (x)
                            110 LOAD_ATTR                3 (layout)
                            120 LOAD_ATTR                4 (elements)
                            130 JUMP_FORWARD             1 (to 134)
                        >>  132 BUILD_LIST               0
                        >>  134 STORE_FAST               5 (base_layout)
                
-               340         136 LOAD_FAST                5 (base_layout)
+               341         136 LOAD_FAST                5 (base_layout)
                            138 LOAD_FAST                4 (x)
                            140 STORE_ATTR               5 (base_layout)
                
-               341         150 LOAD_GLOBAL             13 (NULL + Layout)
+               342         150 LOAD_GLOBAL             13 (NULL + Layout)
                            162 LOAD_FAST                5 (base_layout)
                            164 CALL_FUNCTION_EX         0
                            166 LOAD_FAST                4 (x)
                            168 STORE_ATTR               3 (layout)
                
-               343         178 LOAD_FAST                4 (x)
+               344         178 LOAD_FAST                4 (x)
                            180 RETURN_VALUE
                consts
                   None
                   'layout'
                names      ('super', '__new__', 'hasattr', 'layout', 'elements', 'base_layout', 'Layout')
                varnames   ('cls', 'name', 'bases', 'dct', 'x', 'base_layout')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       '__new__'
-               firstlineno 334
+               firstlineno 335
                lnotab 0x040148033c020e011c02
          names      ('__name__', '__module__', '__qualname__', '__new__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       '_ExtensibleFormMetaclass'
-         firstlineno 333
+         firstlineno 334
          lnotab 0x0c01
       '_ExtensibleFormMetaclass'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a0264015a03650464026505650665076602190000
             00000000000000660264038404a6000000ab0000000000000000005a0864
             045300
-         346           0 RESUME                   0
+         347           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ExtensibleForm')
                        8 STORE_NAME               2 (__qualname__)
          
-         347          10 LOAD_CONST               1 ('Base model for extensible forms.\n\n    This mixin adds functionality which allows\n    - apps to add layout nodes to the layout used by django-material\n\n    :Add layout nodes:\n\n    .. code-block:: python\n\n        from material import Fieldset\n\n        from aleksis.core.forms import ExampleForm\n\n        node = Fieldset("field_name")\n        ExampleForm.add_node_to_layout(node)\n\n    ')
+         348          10 LOAD_CONST               1 ('Base model for extensible forms.\n\n    This mixin adds functionality which allows\n    - apps to add layout nodes to the layout used by django-material\n\n    :Add layout nodes:\n\n    .. code-block:: python\n\n        from material import Fieldset\n\n        from aleksis.core.forms import ExampleForm\n\n        node = Fieldset("field_name")\n        ExampleForm.add_node_to_layout(node)\n\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         365          14 LOAD_NAME                4 (classmethod)
+         366          14 LOAD_NAME                4 (classmethod)
          
-         366          16 LOAD_CONST               2 ('node')
+         367          16 LOAD_CONST               2 ('node')
                       18 LOAD_NAME                5 (Union)
                       20 LOAD_NAME                6 (LayoutNode)
                       22 LOAD_NAME                7 (str)
                       24 BUILD_TUPLE              2
                       26 BINARY_SUBSCR
                       36 BUILD_TUPLE              2
-                      38 LOAD_CONST               3 (<code object add_node_to_layout, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 365>)
+                      38 LOAD_CONST               3 (<code object add_node_to_layout, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 366>)
                       40 MAKE_FUNCTION            4 (annotations)
          
-         365          42 PRECALL                  0
+         366          42 PRECALL                  0
                       46 CALL                     0
          
-         366          56 STORE_NAME               8 (add_node_to_layout)
+         367          56 STORE_NAME               8 (add_node_to_layout)
                       58 LOAD_CONST               4 (None)
                       60 RETURN_VALUE
          consts
             'ExtensibleForm'
             'Base model for extensible forms.\n\n    This mixin adds functionality which allows\n    - apps to add layout nodes to the layout used by django-material\n\n    :Add layout nodes:\n\n    .. code-block:: python\n\n        from material import Fieldset\n\n        from aleksis.core.forms import ExampleForm\n\n        node = Fieldset("field_name")\n        ExampleForm.add_node_to_layout(node)\n\n    '
             'node'
             code
@@ -2422,198 +2426,198 @@
                   0000000000000000007c006a0b00000000000000006a0c00000000000000
                   007c046701a6020000ab0200000000000000007c04190000000000000000
                   007d057c006a0b00000000000000006a0d0000000000000000a001000000
                   00000000000000000000000000000000007c04a6010000ab010000000000
                   00000001007c057c006a0e00000000000000007c043c000000741f000000
                   000000000000007c007c047c05a6030000ab03000000000000000001007c
                   02b0af6401530064015300
-               365           0 RESUME                   0
+               366           0 RESUME                   0
                
-               372           2 LOAD_FAST                0 (cls)
+               373           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (base_layout)
                             14 LOAD_METHOD              1 (append)
                             36 LOAD_FAST                1 (node)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               373          54 LOAD_GLOBAL              5 (NULL + Layout)
+               374          54 LOAD_GLOBAL              5 (NULL + Layout)
                             66 LOAD_FAST                0 (cls)
                             68 LOAD_ATTR                0 (base_layout)
                             78 CALL_FUNCTION_EX         0
                             80 LOAD_FAST                0 (cls)
                             82 STORE_ATTR               3 (layout)
                
-               375          92 LOAD_FAST                1 (node)
+               376          92 LOAD_FAST                1 (node)
                             94 BUILD_LIST               1
                             96 STORE_FAST               2 (visit_nodes)
                
-               376          98 LOAD_FAST                2 (visit_nodes)
+               377          98 LOAD_FAST                2 (visit_nodes)
                            100 POP_JUMP_FORWARD_IF_FALSE   177 (to 456)
                
-               377     >>  102 LOAD_FAST                2 (visit_nodes)
+               378     >>  102 LOAD_FAST                2 (visit_nodes)
                            104 LOAD_METHOD              4 (pop)
                            126 PRECALL                  0
                            130 CALL                     0
                            140 STORE_FAST               3 (current_node)
                
-               378         142 LOAD_GLOBAL             11 (NULL + isinstance)
+               379         142 LOAD_GLOBAL             11 (NULL + isinstance)
                            154 LOAD_FAST                3 (current_node)
                            156 LOAD_GLOBAL             12 (Fieldset)
                            168 PRECALL                  2
                            172 CALL                     2
                            182 POP_JUMP_FORWARD_IF_FALSE    11 (to 206)
                
-               379         184 LOAD_FAST                2 (visit_nodes)
+               380         184 LOAD_FAST                2 (visit_nodes)
                            186 LOAD_FAST                1 (node)
                            188 LOAD_ATTR                7 (elements)
                            198 BINARY_OP               13 (+=)
                            202 STORE_FAST               2 (visit_nodes)
                            204 JUMP_FORWARD           121 (to 448)
                
-               382     >>  206 LOAD_GLOBAL             11 (NULL + isinstance)
+               383     >>  206 LOAD_GLOBAL             11 (NULL + isinstance)
                            218 LOAD_FAST                3 (current_node)
                            220 LOAD_GLOBAL             16 (str)
                            232 PRECALL                  2
                            236 CALL                     2
                            246 POP_JUMP_FORWARD_IF_FALSE     2 (to 252)
                            248 LOAD_FAST                3 (current_node)
                            250 JUMP_FORWARD             6 (to 264)
                        >>  252 LOAD_FAST                3 (current_node)
                            254 LOAD_ATTR                9 (field_name)
                
-               381     >>  264 STORE_FAST               4 (field_name)
+               382     >>  264 STORE_FAST               4 (field_name)
                
-               384         266 LOAD_GLOBAL             21 (NULL + fields_for_model)
+               385         266 LOAD_GLOBAL             21 (NULL + fields_for_model)
                            278 LOAD_FAST                0 (cls)
                            280 LOAD_ATTR               11 (_meta)
                            290 LOAD_ATTR               12 (model)
                            300 LOAD_FAST                4 (field_name)
                            302 BUILD_LIST               1
                            304 PRECALL                  2
                            308 CALL                     2
                            318 LOAD_FAST                4 (field_name)
                            320 BINARY_SUBSCR
                            330 STORE_FAST               5 (field)
                
-               385         332 LOAD_FAST                0 (cls)
+               386         332 LOAD_FAST                0 (cls)
                            334 LOAD_ATTR               11 (_meta)
                            344 LOAD_ATTR               13 (fields)
                            354 LOAD_METHOD              1 (append)
                            376 LOAD_FAST                4 (field_name)
                            378 PRECALL                  1
                            382 CALL                     1
                            392 POP_TOP
                
-               386         394 LOAD_FAST                5 (field)
+               387         394 LOAD_FAST                5 (field)
                            396 LOAD_FAST                0 (cls)
                            398 LOAD_ATTR               14 (base_fields)
                            408 LOAD_FAST                4 (field_name)
                            410 STORE_SUBSCR
                
-               387         414 LOAD_GLOBAL             31 (NULL + setattr)
+               388         414 LOAD_GLOBAL             31 (NULL + setattr)
                            426 LOAD_FAST                0 (cls)
                            428 LOAD_FAST                4 (field_name)
                            430 LOAD_FAST                5 (field)
                            432 PRECALL                  3
                            436 CALL                     3
                            446 POP_TOP
                
-               376     >>  448 LOAD_FAST                2 (visit_nodes)
+               377     >>  448 LOAD_FAST                2 (visit_nodes)
                            450 POP_JUMP_BACKWARD_IF_TRUE   175 (to 102)
                            452 LOAD_CONST               1 (None)
                            454 RETURN_VALUE
                        >>  456 LOAD_CONST               1 (None)
                            458 RETURN_VALUE
                consts
                   'Add a node to `layout` attribute.\n\n        :param node: django-material layout node (Fieldset, Row etc.)\n        :type node: LayoutNode\n        '
                   None
                names      ('base_layout', 'append', 'Layout', 'layout', 'pop', 'isinstance', 'Fieldset', 'elements', 'str', 'field_name', 'fields_for_model', '_meta', 'model', 'fields', 'base_fields', 'setattr')
                varnames   ('cls', 'node', 'visit_nodes', 'current_node', 'field_name', 'field')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'add_node_to_layout'
-               firstlineno 365
+               firstlineno 366
                lnotab 0x0207340126020601040128012a0116033aff020342013e01140122f5
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'classmethod', 'Union', 'LayoutNode', 'str', 'add_node_to_layout')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'ExtensibleForm'
-         firstlineno 346
+         firstlineno 347
          lnotab 0x0a01041202011aff0e01
       'ExtensibleForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-         390           0 RESUME                   0
+         391           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BaseModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-         391          10 LOAD_CONST               1 ('A base class for ModelAdmin combining django-guardian and rules.')
+         392          10 LOAD_CONST               1 ('A base class for ModelAdmin combining django-guardian and rules.')
                       12 STORE_NAME               3 (__doc__)
          
-         393          14 LOAD_CONST               2 (None)
+         394          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'BaseModelAdmin'
             'A base class for ModelAdmin combining django-guardian and rules.'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'BaseModelAdmin'
-         firstlineno 390
+         firstlineno 391
          lnotab 0x0a010402
       'BaseModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a02550064015a036504650519000000000000
             000000650664023c00000064036507640465086604880066016405840c5a
             09880078015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
-         396           2 RESUME                   0
+         397           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('SuccessMessageMixin')
                       10 STORE_NAME               2 (__qualname__)
                       12 SETUP_ANNOTATIONS
          
-         397          14 LOAD_CONST               1 (None)
+         398          14 LOAD_CONST               1 (None)
                       16 STORE_NAME               3 (success_message)
                       18 LOAD_NAME                4 (Optional)
                       20 LOAD_NAME                5 (str)
                       22 BINARY_SUBSCR
                       32 LOAD_NAME                6 (__annotations__)
                       34 LOAD_CONST               2 ('success_message')
                       36 STORE_SUBSCR
          
-         399          40 LOAD_CONST               3 ('form')
+         400          40 LOAD_CONST               3 ('form')
                       42 LOAD_NAME                7 (BaseForm)
                       44 LOAD_CONST               4 ('return')
                       46 LOAD_NAME                8 (HttpResponse)
                       48 BUILD_TUPLE              4
                       50 LOAD_CLOSURE             0 (__class__)
                       52 BUILD_TUPLE              1
-                      54 LOAD_CONST               5 (<code object form_valid, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 399>)
+                      54 LOAD_CONST               5 (<code object form_valid, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 400>)
                       56 MAKE_FUNCTION           12 (annotations, closure)
                       58 STORE_NAME               9 (form_valid)
                       60 LOAD_CLOSURE             0 (__class__)
                       62 COPY                     1
                       64 STORE_NAME              10 (__classcell__)
                       66 RETURN_VALUE
          consts
@@ -2631,31 +2635,31 @@
                   0x950197007c006a000000000000000000721f7403000000000000000000
                   006a0200000000000000007c006a0300000000000000007c006a00000000
                   0000000000a6020000ab0200000000000000000100740900000000000000
                   000000a6000000ab000000000000000000a0050000000000000000000000
                   0000000000000000007c01a6010000ab0100000000000000005300
                              0 COPY_FREE_VARS           1
                
-               399           2 RESUME                   0
+               400           2 RESUME                   0
                
-               400           4 LOAD_FAST                0 (self)
+               401           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (success_message)
                             16 POP_JUMP_FORWARD_IF_FALSE    31 (to 80)
                
-               401          18 LOAD_GLOBAL              3 (NULL + messages)
+               402          18 LOAD_GLOBAL              3 (NULL + messages)
                             30 LOAD_ATTR                2 (success)
                             40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (request)
                             52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                0 (success_message)
                             64 PRECALL                  2
                             68 CALL                     2
                             78 POP_TOP
                
-               402     >>   80 LOAD_GLOBAL              9 (NULL + super)
+               403     >>   80 LOAD_GLOBAL              9 (NULL + super)
                             92 PRECALL                  0
                             96 CALL                     0
                            106 LOAD_METHOD              5 (form_valid)
                            128 LOAD_FAST                1 (form)
                            130 PRECALL                  1
                            134 CALL                     1
                            144 RETURN_VALUE
@@ -2663,50 +2667,50 @@
                   None
                names      ('success_message', 'messages', 'success', 'request', 'super', 'form_valid')
                varnames   ('self', 'form')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'form_valid'
-               firstlineno 399
+               firstlineno 400
                lnotab 0x04010e013e01
          names      ('__name__', '__module__', '__qualname__', 'success_message', 'Optional', 'str', '__annotations__', 'BaseForm', 'HttpResponse', 'form_valid', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'SuccessMessageMixin'
-         firstlineno 396
+         firstlineno 397
          lnotab 0x0e011a02
       'SuccessMessageMixin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504660288006601640384
             0c5a05880078015a065300
                        0 MAKE_CELL                0 (__class__)
          
-         405           2 RESUME                   0
+         406           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('SuccessNextMixin')
                       10 STORE_NAME               2 (__qualname__)
          
-         406          12 LOAD_CONST               1 ('next')
+         407          12 LOAD_CONST               1 ('next')
                       14 STORE_NAME               3 (redirect_field_name)
          
-         408          16 LOAD_CONST               2 ('return')
+         409          16 LOAD_CONST               2 ('return')
                       18 LOAD_NAME                4 (str)
                       20 BUILD_TUPLE              2
                       22 LOAD_CLOSURE             0 (__class__)
                       24 BUILD_TUPLE              1
-                      26 LOAD_CONST               3 (<code object get_success_url, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 408>)
+                      26 LOAD_CONST               3 (<code object get_success_url, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 409>)
                       28 MAKE_FUNCTION           12 (annotations, closure)
                       30 STORE_NAME               5 (get_success_url)
                       32 LOAD_CLOSURE             0 (__class__)
                       34 COPY                     1
                       36 STORE_NAME               6 (__classcell__)
                       38 RETURN_VALUE
          consts
@@ -2721,17 +2725,17 @@
                code
                   0x950197007401000000000000000000006a0100000000000000007c00a6
                   010000ab010000000000000000701f740500000000000000000000a60000
                   00ab000000000000000000a0030000000000000000000000000000000000
                   000000a6000000ab0000000000000000005300
                              0 COPY_FREE_VARS           1
                
-               408           2 RESUME                   0
+               409           2 RESUME                   0
                
-               409           4 LOAD_GLOBAL              1 (NULL + LoginView)
+               410           4 LOAD_GLOBAL              1 (NULL + LoginView)
                             16 LOAD_ATTR                1 (get_redirect_url)
                             26 LOAD_FAST                0 (self)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 JUMP_IF_TRUE_OR_POP     31 (to 106)
                             44 LOAD_GLOBAL              5 (NULL + super)
                             56 PRECALL                  0
@@ -2744,110 +2748,110 @@
                   None
                names      ('LoginView', 'get_redirect_url', 'super', 'get_success_url')
                varnames   ('self',)
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_success_url'
-               firstlineno 408
+               firstlineno 409
                lnotab 0x0401
          names      ('__name__', '__module__', '__qualname__', 'redirect_field_name', 'str', 'get_success_url', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'SuccessNextMixin'
-         firstlineno 405
+         firstlineno 406
          lnotab 0x0c010402
       'SuccessNextMixin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015300
-         412           0 RESUME                   0
+         413           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdvancedCreateView')
                        8 STORE_NAME               2 (__qualname__)
          
-         413          10 LOAD_CONST               1 (None)
+         414          10 LOAD_CONST               1 (None)
                       12 RETURN_VALUE
          consts
             'AdvancedCreateView'
             None
          names      ('__name__', '__module__', '__qualname__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'AdvancedCreateView'
-         firstlineno 412
+         firstlineno 413
          lnotab 0x0a01
       'AdvancedCreateView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015300
-         416           0 RESUME                   0
+         417           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdvancedEditView')
                        8 STORE_NAME               2 (__qualname__)
          
-         417          10 LOAD_CONST               1 (None)
+         418          10 LOAD_CONST               1 (None)
                       12 RETURN_VALUE
          consts
             'AdvancedEditView'
             None
          names      ('__name__', '__module__', '__qualname__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'AdvancedEditView'
-         firstlineno 416
+         firstlineno 417
          lnotab 0x0a01
       'AdvancedEditView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a02550064015a0364025a0465056506190000
             00000000000000650764033c00000088006601640484085a08880078015a
             095300
                        0 MAKE_CELL                0 (__class__)
          
-         420           2 RESUME                   0
+         421           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdvancedDeleteView')
                       10 STORE_NAME               2 (__qualname__)
                       12 SETUP_ANNOTATIONS
          
-         421          14 LOAD_CONST               1 ('Common confirm view for deleting.\n\n    .. warning ::\n\n        Using this view, objects are deleted permanently after confirming.\n        We recommend to include the mixin :class:`reversion.views.RevisionMixin`\n        from `django-reversion` to enable soft-delete.\n    ')
+         422          14 LOAD_CONST               1 ('Common confirm view for deleting.\n\n    .. warning ::\n\n        Using this view, objects are deleted permanently after confirming.\n        We recommend to include the mixin :class:`reversion.views.RevisionMixin`\n        from `django-reversion` to enable soft-delete.\n    ')
                       16 STORE_NAME               3 (__doc__)
          
-         430          18 LOAD_CONST               2 (None)
+         431          18 LOAD_CONST               2 (None)
                       20 STORE_NAME               4 (success_message)
                       22 LOAD_NAME                5 (Optional)
                       24 LOAD_NAME                6 (str)
                       26 BINARY_SUBSCR
                       36 LOAD_NAME                7 (__annotations__)
                       38 LOAD_CONST               3 ('success_message')
                       40 STORE_SUBSCR
          
-         432          44 LOAD_CLOSURE             0 (__class__)
+         433          44 LOAD_CLOSURE             0 (__class__)
                       46 BUILD_TUPLE              1
-                      48 LOAD_CONST               4 (<code object form_valid, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 432>)
+                      48 LOAD_CONST               4 (<code object form_valid, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 433>)
                       50 MAKE_FUNCTION            8 (closure)
                       52 STORE_NAME               8 (form_valid)
                       54 LOAD_CLOSURE             0 (__class__)
                       56 COPY                     1
                       58 STORE_NAME               9 (__classcell__)
                       60 RETURN_VALUE
          consts
@@ -2865,121 +2869,121 @@
                   00a00100000000000000000000000000000000000000007c01a6010000ab
                   0100000000000000007d027c006a020000000000000000721f7407000000
                   000000000000006a0400000000000000007c006a0500000000000000007c
                   006a020000000000000000a6020000ab02000000000000000001007c0253
                   00
                              0 COPY_FREE_VARS           1
                
-               432           2 RESUME                   0
+               433           2 RESUME                   0
                
-               433           4 LOAD_GLOBAL              1 (NULL + super)
+               434           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (form_valid)
                             52 LOAD_FAST                1 (form)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 STORE_FAST               2 (r)
                
-               434          70 LOAD_FAST                0 (self)
+               435          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                2 (success_message)
                             82 POP_JUMP_FORWARD_IF_FALSE    31 (to 146)
                
-               435          84 LOAD_GLOBAL              7 (NULL + messages)
+               436          84 LOAD_GLOBAL              7 (NULL + messages)
                             96 LOAD_ATTR                4 (success)
                            106 LOAD_FAST                0 (self)
                            108 LOAD_ATTR                5 (request)
                            118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                2 (success_message)
                            130 PRECALL                  2
                            134 CALL                     2
                            144 POP_TOP
                
-               436     >>  146 LOAD_FAST                2 (r)
+               437     >>  146 LOAD_FAST                2 (r)
                            148 RETURN_VALUE
                consts
                   None
                names      ('super', 'form_valid', 'success_message', 'messages', 'success', 'request')
                varnames   ('self', 'form', 'r')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'form_valid'
-               firstlineno 432
+               firstlineno 433
                lnotab 0x040142010e013e01
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'success_message', 'Optional', 'str', '__annotations__', 'form_valid', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'AdvancedDeleteView'
-         firstlineno 420
+         firstlineno 421
          lnotab 0x0e0104091a02
       'AdvancedDeleteView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 8
          flags     : 0
          code
             0x970065005a0164005a0264015a03020065046a05000000000000000064
             0265046a0600000000000000006403020065076404a6010000ab01000000
             000000000064056405ac06a6060000ab0600000000000000005a08020002
             0065096a0a0000000000000000650ba6010000ab010000000000000000a6
             000000ab0000000000000000005a0c02004700640784006408a6020000ab
             0200000000000000005a0d64095300
-         439           0 RESUME                   0
+         440           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SchoolTermRelatedExtensibleModel')
                        8 STORE_NAME               2 (__qualname__)
          
-         440          10 LOAD_CONST               1 ('Add relation to school term.')
+         441          10 LOAD_CONST               1 ('Add relation to school term.')
                       12 STORE_NAME               3 (__doc__)
          
-         442          14 PUSH_NULL
+         443          14 PUSH_NULL
                       16 LOAD_NAME                4 (models)
                       18 LOAD_ATTR                5 (ForeignKey)
          
-         443          28 LOAD_CONST               2 ('core.SchoolTerm')
+         444          28 LOAD_CONST               2 ('core.SchoolTerm')
          
-         444          30 LOAD_NAME                4 (models)
+         445          30 LOAD_NAME                4 (models)
                       32 LOAD_ATTR                6 (CASCADE)
          
-         445          42 LOAD_CONST               3 ('+')
+         446          42 LOAD_CONST               3 ('+')
          
-         446          44 PUSH_NULL
+         447          44 PUSH_NULL
                       46 LOAD_NAME                7 (_)
                       48 LOAD_CONST               4 ('Linked school term')
                       50 PRECALL                  1
                       54 CALL                     1
          
-         447          64 LOAD_CONST               5 (True)
+         448          64 LOAD_CONST               5 (True)
          
-         448          66 LOAD_CONST               5 (True)
+         449          66 LOAD_CONST               5 (True)
          
-         442          68 KW_NAMES                 6
+         443          68 KW_NAMES                 6
                       70 PRECALL                  6
                       74 CALL                     6
                       84 STORE_NAME               8 (school_term)
          
-         451          86 PUSH_NULL
+         452          86 PUSH_NULL
                       88 PUSH_NULL
                       90 LOAD_NAME                9 (AlekSISBaseManagerWithoutMigrations)
                       92 LOAD_ATTR               10 (from_queryset)
                      102 LOAD_NAME               11 (SchoolTermRelatedQuerySet)
                      104 PRECALL                  1
                      108 CALL                     1
                      118 PRECALL                  0
                      122 CALL                     0
                      132 STORE_NAME              12 (objects)
          
-         453         134 PUSH_NULL
+         454         134 PUSH_NULL
                      136 LOAD_BUILD_CLASS
-                     138 LOAD_CONST               7 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 453>)
+                     138 LOAD_CONST               7 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 454>)
                      140 MAKE_FUNCTION            0
                      142 LOAD_CONST               8 ('Meta')
                      144 PRECALL                  2
                      148 CALL                     2
                      158 STORE_NAME              13 (Meta)
                      160 LOAD_CONST               9 (None)
                      162 RETURN_VALUE
@@ -2993,69 +2997,69 @@
             ('on_delete', 'related_name', 'verbose_name', 'blank', 'null')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               453           0 RESUME                   0
+               454           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('SchoolTermRelatedExtensibleModel.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               454          10 LOAD_CONST               1 (True)
+               455          10 LOAD_CONST               1 (True)
                             12 STORE_NAME               3 (abstract)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'SchoolTermRelatedExtensibleModel.Meta'
                   True
                   None
                names      ('__name__', '__module__', '__qualname__', 'abstract')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'Meta'
-               firstlineno 453
+               firstlineno 454
                lnotab 0x0a01
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'ForeignKey', 'CASCADE', '_', 'school_term', 'AlekSISBaseManagerWithoutMigrations', 'from_queryset', 'SchoolTermRelatedQuerySet', 'objects', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'SchoolTermRelatedExtensibleModel'
-         firstlineno 439
+         firstlineno 440
          lnotab 0x0a0104020e0102010c0102011401020102fa12093002
       'SchoolTermRelatedExtensibleModel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0388006601640284085a04880078
             015a055300
                        0 MAKE_CELL                0 (__class__)
          
-         457           2 RESUME                   0
+         458           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('SchoolTermRelatedExtensibleForm')
                       10 STORE_NAME               2 (__qualname__)
          
-         458          12 LOAD_CONST               1 ("Extensible form for school term related data.\n\n    .. warning::\n        This doesn't automatically include the field `school_term` in `fields` or `layout`,\n        it just sets an initial value.\n    ")
+         459          12 LOAD_CONST               1 ("Extensible form for school term related data.\n\n    .. warning::\n        This doesn't automatically include the field `school_term` in `fields` or `layout`,\n        it just sets an initial value.\n    ")
                       14 STORE_NAME               3 (__doc__)
          
-         465          16 LOAD_CLOSURE             0 (__class__)
+         466          16 LOAD_CLOSURE             0 (__class__)
                       18 BUILD_TUPLE              1
-                      20 LOAD_CONST               2 (<code object __init__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 465>)
+                      20 LOAD_CONST               2 (<code object __init__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 466>)
                       22 MAKE_FUNCTION            8 (closure)
                       24 STORE_NAME               4 (__init__)
                       26 LOAD_CLOSURE             0 (__class__)
                       28 COPY                     1
                       30 STORE_NAME               5 (__classcell__)
                       32 RETURN_VALUE
          consts
@@ -3069,37 +3073,37 @@
                code
                   0x95019700640164026c006d017d03010064037c027601720c64047c036a
                   02000000000000000069017c0264053c0000000200740700000000000000
                   000000a6000000ab0000000000000000006a0400000000000000007c0169
                   007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               465           2 RESUME                   0
+               466           2 RESUME                   0
                
-               466           4 LOAD_CONST               1 (0)
+               467           4 LOAD_CONST               1 (0)
                              6 LOAD_CONST               2 (('SchoolTerm',))
                              8 IMPORT_NAME              0 (aleksis.core.models)
                             10 IMPORT_FROM              1 (SchoolTerm)
                             12 STORE_FAST               3 (SchoolTerm)
                             14 POP_TOP
                
-               468          16 LOAD_CONST               3 ('instance')
+               469          16 LOAD_CONST               3 ('instance')
                             18 LOAD_FAST                2 (kwargs)
                             20 CONTAINS_OP              1
                             22 POP_JUMP_FORWARD_IF_FALSE    12 (to 48)
                
-               469          24 LOAD_CONST               4 ('school_term')
+               470          24 LOAD_CONST               4 ('school_term')
                             26 LOAD_FAST                3 (SchoolTerm)
                             28 LOAD_ATTR                2 (current)
                             38 BUILD_MAP                1
                             40 LOAD_FAST                2 (kwargs)
                             42 LOAD_CONST               5 ('initial')
                             44 STORE_SUBSCR
                
-               471     >>   48 PUSH_NULL
+               472     >>   48 PUSH_NULL
                             50 LOAD_GLOBAL              7 (NULL + super)
                             62 PRECALL                  0
                             66 CALL                     0
                             76 LOAD_ATTR                4 (__init__)
                             86 LOAD_FAST                1 (args)
                             88 BUILD_MAP                0
                             90 LOAD_FAST                2 (kwargs)
@@ -3117,44 +3121,44 @@
                   'initial'
                names      ('aleksis.core.models', 'SchoolTerm', 'current', 'super', '__init__')
                varnames   ('self', 'args', 'kwargs', 'SchoolTerm')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       '__init__'
-               firstlineno 465
+               firstlineno 466
                lnotab 0x04010c0208011802
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'SchoolTermRelatedExtensibleForm'
-         firstlineno 457
+         firstlineno 458
          lnotab 0x0c010407
       'SchoolTermRelatedExtensibleForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025a04640384005a0564045300
-         474           0 RESUME                   0
+         475           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PublicFilePreferenceMixin')
                        8 STORE_NAME               2 (__qualname__)
          
-         475          10 LOAD_CONST               1 ('Uploads a file to the public namespace.')
+         476          10 LOAD_CONST               1 ('Uploads a file to the public namespace.')
                       12 STORE_NAME               3 (__doc__)
          
-         477          14 LOAD_CONST               2 ('public')
+         478          14 LOAD_CONST               2 ('public')
                       16 STORE_NAME               4 (upload_path)
          
-         479          18 LOAD_CONST               3 (<code object get_upload_path, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 479>)
+         480          18 LOAD_CONST               3 (<code object get_upload_path, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 480>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (get_upload_path)
                       24 LOAD_CONST               4 (None)
                       26 RETURN_VALUE
          consts
             'PublicFilePreferenceMixin'
             'Uploads a file to the public namespace.'
@@ -3166,50 +3170,50 @@
                flags     : 3
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c006a03000000000000000074
                   08000000000000000000006a0500000000000000007c00a0060000000000
                   000000000000000000000000000000a6000000ab000000000000000000a6
                   030000ab0300000000000000005300
-               479           0 RESUME                   0
+               480           0 RESUME                   0
                
-               480           2 LOAD_GLOBAL              0 (os)
+               481           2 LOAD_GLOBAL              0 (os)
                             14 LOAD_ATTR                1 (path)
                             24 LOAD_METHOD              2 (join)
                
-               481          46 LOAD_FAST                0 (self)
+               482          46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (upload_path)
                             58 LOAD_GLOBAL              8 (preferences_settings)
                             70 LOAD_ATTR                5 (FILE_PREFERENCE_UPLOAD_DIR)
                             80 LOAD_FAST                0 (self)
                             82 LOAD_METHOD              6 (identifier)
                            104 PRECALL                  0
                            108 CALL                     0
                
-               480         118 PRECALL                  3
+               481         118 PRECALL                  3
                            122 CALL                     3
                            132 RETURN_VALUE
                consts
                   None
                names      ('os', 'path', 'join', 'upload_path', 'preferences_settings', 'FILE_PREFERENCE_UPLOAD_DIR', 'identifier')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_upload_path'
-               firstlineno 479
+               firstlineno 480
                lnotab 0x02012c0148ff
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'upload_path', 'get_upload_path')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'PublicFilePreferenceMixin'
-         firstlineno 474
+         firstlineno 475
          lnotab 0x0a0104020402
       'PublicFilePreferenceMixin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
@@ -3221,25 +3225,25 @@
             09640019000000000000000000660264088404a6000000ab000000000000
             0000005a0e650f6409650765086509640019000000000000000000660219
             0000000000000000006602640a8404a6000000ab0000000000000000005a
             10650f640965116509640019000000000000000000190000000000000000
             006602640b8404a6000000ab0000000000000000005a12650d6405650864
             096506650964001900000000000000000019000000000000000000660464
             0c8404a6000000ab0000000000000000005a1364025300
-         485           0 RESUME                   0
+         486           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('RegistryObject')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         486          12 LOAD_CONST               1 ('Generic registry to allow registration of subclasses over all apps.')
+         487          12 LOAD_CONST               1 ('Generic registry to allow registration of subclasses over all apps.')
                       14 STORE_NAME               3 (__doc__)
          
-         488          16 LOAD_CONST               2 (None)
+         489          16 LOAD_CONST               2 (None)
                       18 STORE_NAME               4 (_registry)
                       20 LOAD_NAME                5 (ClassVar)
                       22 LOAD_NAME                6 (Optional)
                       24 LOAD_NAME                7 (dict)
                       26 LOAD_NAME                8 (str)
                       28 LOAD_NAME                9 (type)
                       30 LOAD_CONST               0 ('RegistryObject')
@@ -3248,96 +3252,96 @@
                       44 BINARY_SUBSCR
                       54 BINARY_SUBSCR
                       64 BINARY_SUBSCR
                       74 LOAD_NAME               10 (__annotations__)
                       76 LOAD_CONST               3 ('_registry')
                       78 STORE_SUBSCR
          
-         489          82 LOAD_CONST               4 ('')
+         490          82 LOAD_CONST               4 ('')
                       84 STORE_NAME              11 (name)
                       86 LOAD_NAME                5 (ClassVar)
                       88 LOAD_NAME                8 (str)
                       90 BINARY_SUBSCR
                      100 LOAD_NAME               10 (__annotations__)
                      102 LOAD_CONST               5 ('name')
                      104 STORE_SUBSCR
          
-         491         108 LOAD_CONST               6 (<code object __init_subclass__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 491>)
+         492         108 LOAD_CONST               6 (<code object __init_subclass__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 492>)
                      110 MAKE_FUNCTION            0
                      112 STORE_NAME              12 (__init_subclass__)
          
-         499         114 LOAD_NAME               13 (classmethod)
+         500         114 LOAD_NAME               13 (classmethod)
          
-         500         116 LOAD_CONST               7 ('cls')
+         501         116 LOAD_CONST               7 ('cls')
                      118 LOAD_NAME                9 (type)
                      120 LOAD_CONST               0 ('RegistryObject')
                      122 BINARY_SUBSCR
                      132 BUILD_TUPLE              2
-                     134 LOAD_CONST               8 (<code object _register, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 499>)
+                     134 LOAD_CONST               8 (<code object _register, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 500>)
                      136 MAKE_FUNCTION            4 (annotations)
          
-         499         138 PRECALL                  0
+         500         138 PRECALL                  0
                      142 CALL                     0
          
-         500         152 STORE_NAME              14 (_register)
+         501         152 STORE_NAME              14 (_register)
          
-         504         154 LOAD_NAME               15 (classproperty)
+         505         154 LOAD_NAME               15 (classproperty)
          
-         505         156 LOAD_CONST               9 ('return')
+         506         156 LOAD_CONST               9 ('return')
                      158 LOAD_NAME                7 (dict)
                      160 LOAD_NAME                8 (str)
                      162 LOAD_NAME                9 (type)
                      164 LOAD_CONST               0 ('RegistryObject')
                      166 BINARY_SUBSCR
                      176 BUILD_TUPLE              2
                      178 BINARY_SUBSCR
                      188 BUILD_TUPLE              2
-                     190 LOAD_CONST              10 (<code object registered_objects_dict, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 504>)
+                     190 LOAD_CONST              10 (<code object registered_objects_dict, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 505>)
                      192 MAKE_FUNCTION            4 (annotations)
          
-         504         194 PRECALL                  0
+         505         194 PRECALL                  0
                      198 CALL                     0
          
-         505         208 STORE_NAME              16 (registered_objects_dict)
+         506         208 STORE_NAME              16 (registered_objects_dict)
          
-         509         210 LOAD_NAME               15 (classproperty)
+         510         210 LOAD_NAME               15 (classproperty)
          
-         510         212 LOAD_CONST               9 ('return')
+         511         212 LOAD_CONST               9 ('return')
                      214 LOAD_NAME               17 (list)
                      216 LOAD_NAME                9 (type)
                      218 LOAD_CONST               0 ('RegistryObject')
                      220 BINARY_SUBSCR
                      230 BINARY_SUBSCR
                      240 BUILD_TUPLE              2
-                     242 LOAD_CONST              11 (<code object registered_objects_list, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 509>)
+                     242 LOAD_CONST              11 (<code object registered_objects_list, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 510>)
                      244 MAKE_FUNCTION            4 (annotations)
          
-         509         246 PRECALL                  0
+         510         246 PRECALL                  0
                      250 CALL                     0
          
-         510         260 STORE_NAME              18 (registered_objects_list)
+         511         260 STORE_NAME              18 (registered_objects_list)
          
-         514         262 LOAD_NAME               13 (classmethod)
+         515         262 LOAD_NAME               13 (classmethod)
          
-         515         264 LOAD_CONST               5 ('name')
+         516         264 LOAD_CONST               5 ('name')
                      266 LOAD_NAME                8 (str)
                      268 LOAD_CONST               9 ('return')
                      270 LOAD_NAME                6 (Optional)
                      272 LOAD_NAME                9 (type)
                      274 LOAD_CONST               0 ('RegistryObject')
                      276 BINARY_SUBSCR
                      286 BINARY_SUBSCR
                      296 BUILD_TUPLE              4
-                     298 LOAD_CONST              12 (<code object get_object_by_name, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 514>)
+                     298 LOAD_CONST              12 (<code object get_object_by_name, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 515>)
                      300 MAKE_FUNCTION            4 (annotations)
          
-         514         302 PRECALL                  0
+         515         302 PRECALL                  0
                      306 CALL                     0
          
-         515         316 STORE_NAME              19 (get_object_by_name)
+         516         316 STORE_NAME              19 (get_object_by_name)
                      318 LOAD_CONST               2 (None)
                      320 RETURN_VALUE
          consts
             'RegistryObject'
             'Generic registry to allow registration of subclasses over all apps.'
             None
             '_registry'
@@ -3350,40 +3354,40 @@
                flags     : 3
                code
                   0x97007401000000000000000000007c0064016400a6030000ab03000000
                   0000000000800969007c005f010000000000000000640053007c006a0200
                   00000000000000730c7c006a0300000000000000007c005f020000000000
                   0000007c00a0040000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               491           0 RESUME                   0
+               492           0 RESUME                   0
                
-               492           2 LOAD_GLOBAL              1 (NULL + getattr)
+               493           2 LOAD_GLOBAL              1 (NULL + getattr)
                             14 LOAD_FAST                0 (cls)
                             16 LOAD_CONST               1 ('_registry')
                             18 LOAD_CONST               0 (None)
                             20 PRECALL                  3
                             24 CALL                     3
                             34 POP_JUMP_FORWARD_IF_NOT_NONE     9 (to 54)
                
-               493          36 BUILD_MAP                0
+               494          36 BUILD_MAP                0
                             38 LOAD_FAST                0 (cls)
                             40 STORE_ATTR               1 (_registry)
                             50 LOAD_CONST               0 (None)
                             52 RETURN_VALUE
                
-               495     >>   54 LOAD_FAST                0 (cls)
+               496     >>   54 LOAD_FAST                0 (cls)
                             56 LOAD_ATTR                2 (name)
                             66 POP_JUMP_FORWARD_IF_TRUE    12 (to 92)
                
-               496          68 LOAD_FAST                0 (cls)
+               497          68 LOAD_FAST                0 (cls)
                             70 LOAD_ATTR                3 (__name__)
                             80 LOAD_FAST                0 (cls)
                             82 STORE_ATTR               2 (name)
                
-               497     >>   92 LOAD_FAST                0 (cls)
+               498     >>   92 LOAD_FAST                0 (cls)
                             94 LOAD_METHOD              4 (_register)
                            116 PRECALL                  0
                            120 CALL                     0
                            130 POP_TOP
                            132 LOAD_CONST               0 (None)
                            134 RETURN_VALUE
                consts
@@ -3391,95 +3395,95 @@
                   '_registry'
                names      ('getattr', '_registry', 'name', '__name__', '_register')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       '__init_subclass__'
-               firstlineno 491
+               firstlineno 492
                lnotab 0x0201220112020e011801
             'cls'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000721f7c006a0000000000000000007c
                   006a010000000000000000760172137c007c006a0100000000000000007c
                   006a0000000000000000003c000000640053006400530064005300
-               499           0 RESUME                   0
+               500           0 RESUME                   0
                
-               501           2 LOAD_FAST                0 (cls)
+               502           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (name)
                             14 POP_JUMP_FORWARD_IF_FALSE    31 (to 78)
                             16 LOAD_FAST                0 (cls)
                             18 LOAD_ATTR                0 (name)
                             28 LOAD_FAST                0 (cls)
                             30 LOAD_ATTR                1 (_registry)
                             40 CONTAINS_OP              1
                             42 POP_JUMP_FORWARD_IF_FALSE    19 (to 82)
                
-               502          44 LOAD_FAST                0 (cls)
+               503          44 LOAD_FAST                0 (cls)
                             46 LOAD_FAST                0 (cls)
                             48 LOAD_ATTR                1 (_registry)
                             58 LOAD_FAST                0 (cls)
                             60 LOAD_ATTR                0 (name)
                             70 STORE_SUBSCR
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                
-               501     >>   78 LOAD_CONST               0 (None)
+               502     >>   78 LOAD_CONST               0 (None)
                             80 RETURN_VALUE
                        >>   82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                names      ('name', '_registry')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       '_register'
-               firstlineno 499
+               firstlineno 500
                lnotab 0x02022a0122ff
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               504           0 RESUME                   0
+               505           0 RESUME                   0
                
-               507           2 LOAD_FAST                0 (cls)
+               508           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (_registry)
                             14 RETURN_VALUE
                consts
                   'Get dict of registered objects.'
                names      ('_registry',)
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'registered_objects_dict'
-               firstlineno 504
+               firstlineno 505
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
                   000000a6010000ab0100000000000000005300
-               509           0 RESUME                   0
+               510           0 RESUME                   0
                
-               512           2 LOAD_GLOBAL              1 (NULL + list)
+               513           2 LOAD_GLOBAL              1 (NULL + list)
                             14 LOAD_FAST                0 (cls)
                             16 LOAD_ATTR                1 (_registry)
                             26 LOAD_METHOD              2 (values)
                             48 PRECALL                  0
                             52 CALL                     0
                             62 PRECALL                  1
                             66 CALL                     1
@@ -3488,105 +3492,105 @@
                   'Get list of registered objects.'
                names      ('list', '_registry', 'values')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'registered_objects_list'
-               firstlineno 509
+               firstlineno 510
                lnotab 0x0203
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000005300
-               514           0 RESUME                   0
+               515           0 RESUME                   0
                
-               517           2 LOAD_FAST                0 (cls)
+               518           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (registered_objects_dict)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                1 (name)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 RETURN_VALUE
                consts
                   'Get registered object by name.'
                names      ('registered_objects_dict', 'get')
                varnames   ('cls', 'name')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_object_by_name'
-               firstlineno 514
+               firstlineno 515
                lnotab 0x0203
          names      ('__name__', '__module__', '__qualname__', '__doc__', '_registry', 'ClassVar', 'Optional', 'dict', 'str', 'type', '__annotations__', 'name', '__init_subclass__', 'classmethod', '_register', 'classproperty', 'registered_objects_dict', 'list', 'registered_objects_list', 'get_object_by_name')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'RegistryObject'
-         firstlineno 485
+         firstlineno 486
          lnotab
             0x0c01040242011a020608020116ff0e010204020126ff0e010204020122
             ff0e010204020126ff0e01
       'RegistryObject'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         520           0 RESUME                   0
+         521           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ObjectAuthenticator')
                        8 STORE_NAME               2 (__qualname__)
          
-         521          10 LOAD_CONST               1 (<code object authenticate, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 521>)
+         522          10 LOAD_CONST               1 (<code object authenticate, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 522>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (authenticate)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'ObjectAuthenticator'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000082
                   01
-               521           0 RESUME                   0
+               522           0 RESUME                   0
                
-               522           2 LOAD_GLOBAL              1 (NULL + NotImplementedError)
+               523           2 LOAD_GLOBAL              1 (NULL + NotImplementedError)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 RAISE_VARARGS            1
                consts
                   None
                names      ('NotImplementedError',)
                varnames   ('self', 'request', 'obj')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'authenticate'
-               firstlineno 521
+               firstlineno 522
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'authenticate')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'ObjectAuthenticator'
-         firstlineno 520
+         firstlineno 521
          lnotab 0x0a01
       'ObjectAuthenticator'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 14
          flags     : 0
@@ -3630,581 +3634,581 @@
             00000000005a276528640c6514660264258404a6000000ab000000000000
             0000005a29652864268400a6000000ab0000000000000000005a2a652864
             0c6523650519000000000000000000660264278404a6000000ab00000000
             00000000005a2b650c64288400a6000000ab0000000000000000005a2c65
             0c6429642a640c65146604642b8404a6000000ab0000000000000000005a
             2d650c642d640b650e640a7a0700006602642c8405a6000000ab00000000
             00000000005a2e640a5300
-         525           0 RESUME                   0
+         526           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CalendarEventMixin')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         526          12 LOAD_CONST               1 ("Mixin for calendar feeds.\n\n    This mixin can be used to create calendar feeds for objects. It can be used\n    by adding it to a model or another object. The basic attributes of the calendar\n    can be set by either setting the attributes of the class or by implementing\n    the corresponding class methods. Please notice that the class methods are\n    overriding the attributes. The following attributes are mandatory:\n\n    - name: Unique name for the calendar feed\n    - verbose_name: Shown name of the feed\n\n    The respective class methods have a `get_` prefix and are called without any arguments.\n    There are also some more attributes. Please refer to the class signature for more\n    information.\n\n    The list of objects used to create the calendar feed have to be provided by\n    the method `get_objects` class method. It's mandatory to implement this method.\n\n    To provide the data for the events, a certain set of class methods can be implemented.\n    The following iCal attributes are supported:\n\n    guid, title, description, link, class, created, updateddate, start_datetime, end_datetime,\n    location, geolocation, transparency, organizer, attendee, rrule, rdate, exdate, valarm, status\n\n    Additionally, the color attribute is supported. The color has to be an RGB\n    color in the format #ffffff.\n\n    To deploy extra meta data for AlekSIS' own calendar frontend, you can add a\n    dictionary for the meta attribute.\n\n    To implement a method for a certain attribute, the name of the method has to be\n    `value_<your_attribute>`. For example, to implement the `title` attribute, the\n    method `value_title` has to be implemented. The method has to return the value\n    for the attribute. The method is called with the reference object as argument.\n    ")
+         527          12 LOAD_CONST               1 ("Mixin for calendar feeds.\n\n    This mixin can be used to create calendar feeds for objects. It can be used\n    by adding it to a model or another object. The basic attributes of the calendar\n    can be set by either setting the attributes of the class or by implementing\n    the corresponding class methods. Please notice that the class methods are\n    overriding the attributes. The following attributes are mandatory:\n\n    - name: Unique name for the calendar feed\n    - verbose_name: Shown name of the feed\n\n    The respective class methods have a `get_` prefix and are called without any arguments.\n    There are also some more attributes. Please refer to the class signature for more\n    information.\n\n    The list of objects used to create the calendar feed have to be provided by\n    the method `get_objects` class method. It's mandatory to implement this method.\n\n    To provide the data for the events, a certain set of class methods can be implemented.\n    The following iCal attributes are supported:\n\n    guid, title, description, link, class, created, updateddate, start_datetime, end_datetime,\n    location, geolocation, transparency, organizer, attendee, rrule, rdate, exdate, valarm, status\n\n    Additionally, the color attribute is supported. The color has to be an RGB\n    color in the format #ffffff.\n\n    To deploy extra meta data for AlekSIS' own calendar frontend, you can add a\n    dictionary for the meta attribute.\n\n    To implement a method for a certain attribute, the name of the method has to be\n    `value_<your_attribute>`. For example, to implement the `title` attribute, the\n    method `value_title` has to be implemented. The method has to return the value\n    for the attribute. The method is called with the reference object as argument.\n    ")
                       14 STORE_NAME               3 (__doc__)
          
-         562          16 LOAD_CONST               2 ('')
+         563          16 LOAD_CONST               2 ('')
                       18 STORE_NAME               4 (name)
                       20 LOAD_NAME                5 (str)
                       22 LOAD_NAME                6 (__annotations__)
                       24 LOAD_CONST               3 ('name')
                       26 STORE_SUBSCR
          
-         563          30 LOAD_CONST               2 ('')
+         564          30 LOAD_CONST               2 ('')
                       32 STORE_NAME               7 (verbose_name)
                       34 LOAD_NAME                5 (str)
                       36 LOAD_NAME                6 (__annotations__)
                       38 LOAD_CONST               4 ('verbose_name')
                       40 STORE_SUBSCR
          
-         564          44 LOAD_CONST               2 ('')
+         565          44 LOAD_CONST               2 ('')
                       46 STORE_NAME               8 (link)
                       48 LOAD_NAME                5 (str)
                       50 LOAD_NAME                6 (__annotations__)
                       52 LOAD_CONST               5 ('link')
                       54 STORE_SUBSCR
          
-         565          58 LOAD_CONST               2 ('')
+         566          58 LOAD_CONST               2 ('')
                       60 STORE_NAME               9 (description)
                       62 LOAD_NAME                5 (str)
                       64 LOAD_NAME                6 (__annotations__)
                       66 LOAD_CONST               6 ('description')
                       68 STORE_SUBSCR
          
-         566          72 LOAD_CONST               7 ('#222222')
+         567          72 LOAD_CONST               7 ('#222222')
                       74 STORE_NAME              10 (color)
                       76 LOAD_NAME                5 (str)
                       78 LOAD_NAME                6 (__annotations__)
                       80 LOAD_CONST               8 ('color')
                       82 STORE_SUBSCR
          
-         567          86 LOAD_CONST               2 ('')
+         568          86 LOAD_CONST               2 ('')
                       88 STORE_NAME              11 (permission_required)
                       90 LOAD_NAME                5 (str)
                       92 LOAD_NAME                6 (__annotations__)
                       94 LOAD_CONST               9 ('permission_required')
                       96 STORE_SUBSCR
          
-         569         100 LOAD_NAME               12 (classmethod)
+         570         100 LOAD_NAME               12 (classmethod)
          
-         570         102 LOAD_CONST              45 ((None,))
+         571         102 LOAD_CONST              45 ((None,))
                      104 LOAD_CONST              11 ('request')
                      106 LOAD_NAME               13 (Optional)
                      108 LOAD_NAME               14 (HttpRequest)
                      110 BINARY_SUBSCR
                      120 LOAD_CONST              12 ('return')
                      122 LOAD_NAME                5 (str)
                      124 BUILD_TUPLE              4
-                     126 LOAD_CONST              13 (<code object get_verbose_name, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 569>)
+                     126 LOAD_CONST              13 (<code object get_verbose_name, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 570>)
                      128 MAKE_FUNCTION            5 (defaults, annotations)
          
-         569         130 PRECALL                  0
+         570         130 PRECALL                  0
                      134 CALL                     0
          
-         570         144 STORE_NAME              15 (get_verbose_name)
+         571         144 STORE_NAME              15 (get_verbose_name)
          
-         574         146 LOAD_NAME               12 (classmethod)
+         575         146 LOAD_NAME               12 (classmethod)
          
-         575         148 LOAD_CONST              45 ((None,))
+         576         148 LOAD_CONST              45 ((None,))
                      150 LOAD_CONST              11 ('request')
                      152 LOAD_NAME               13 (Optional)
                      154 LOAD_NAME               14 (HttpRequest)
                      156 BINARY_SUBSCR
                      166 LOAD_CONST              12 ('return')
                      168 LOAD_NAME                5 (str)
                      170 BUILD_TUPLE              4
-                     172 LOAD_CONST              14 (<code object get_link, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 574>)
+                     172 LOAD_CONST              14 (<code object get_link, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 575>)
                      174 MAKE_FUNCTION            5 (defaults, annotations)
          
-         574         176 PRECALL                  0
+         575         176 PRECALL                  0
                      180 CALL                     0
          
-         575         190 STORE_NAME              16 (get_link)
+         576         190 STORE_NAME              16 (get_link)
          
-         579         192 LOAD_NAME               12 (classmethod)
+         580         192 LOAD_NAME               12 (classmethod)
          
-         580         194 LOAD_CONST              45 ((None,))
+         581         194 LOAD_CONST              45 ((None,))
                      196 LOAD_CONST              11 ('request')
                      198 LOAD_NAME               13 (Optional)
                      200 LOAD_NAME               14 (HttpRequest)
                      202 BINARY_SUBSCR
                      212 LOAD_CONST              12 ('return')
                      214 LOAD_NAME                5 (str)
                      216 BUILD_TUPLE              4
-                     218 LOAD_CONST              15 (<code object get_description, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 579>)
+                     218 LOAD_CONST              15 (<code object get_description, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 580>)
                      220 MAKE_FUNCTION            5 (defaults, annotations)
          
-         579         222 PRECALL                  0
+         580         222 PRECALL                  0
                      226 CALL                     0
          
-         580         236 STORE_NAME              17 (get_description)
+         581         236 STORE_NAME              17 (get_description)
          
-         584         238 LOAD_NAME               12 (classmethod)
+         585         238 LOAD_NAME               12 (classmethod)
          
-         585         240 LOAD_CONST              45 ((None,))
+         586         240 LOAD_CONST              45 ((None,))
                      242 LOAD_CONST              11 ('request')
                      244 LOAD_NAME               13 (Optional)
                      246 LOAD_NAME               14 (HttpRequest)
                      248 BINARY_SUBSCR
                      258 LOAD_CONST              12 ('return')
                      260 LOAD_NAME                5 (str)
                      262 BUILD_TUPLE              4
-                     264 LOAD_CONST              16 (<code object get_language, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 584>)
+                     264 LOAD_CONST              16 (<code object get_language, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 585>)
                      266 MAKE_FUNCTION            5 (defaults, annotations)
          
-         584         268 PRECALL                  0
+         585         268 PRECALL                  0
                      272 CALL                     0
          
-         585         282 STORE_NAME              18 (get_language)
+         586         282 STORE_NAME              18 (get_language)
          
-         591         284 LOAD_NAME               12 (classmethod)
+         592         284 LOAD_NAME               12 (classmethod)
          
-         592         286 LOAD_CONST              45 ((None,))
+         593         286 LOAD_CONST              45 ((None,))
                      288 LOAD_CONST              11 ('request')
                      290 LOAD_NAME               13 (Optional)
                      292 LOAD_NAME               14 (HttpRequest)
                      294 BINARY_SUBSCR
                      304 LOAD_CONST              12 ('return')
                      306 LOAD_NAME                5 (str)
                      308 BUILD_TUPLE              4
-                     310 LOAD_CONST              17 (<code object get_color, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 591>)
+                     310 LOAD_CONST              17 (<code object get_color, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 592>)
                      312 MAKE_FUNCTION            5 (defaults, annotations)
          
-         591         314 PRECALL                  0
+         592         314 PRECALL                  0
                      318 CALL                     0
          
-         592         328 STORE_NAME              19 (get_color)
+         593         328 STORE_NAME              19 (get_color)
          
-         599         330 LOAD_NAME               12 (classmethod)
+         600         330 LOAD_NAME               12 (classmethod)
          
-         600         332 LOAD_CONST              45 ((None,))
+         601         332 LOAD_CONST              45 ((None,))
                      334 LOAD_CONST              11 ('request')
                      336 LOAD_NAME               14 (HttpRequest)
                      338 LOAD_CONST              10 (None)
                      340 BINARY_OP                7 (|)
                      344 LOAD_CONST              12 ('return')
                      346 LOAD_NAME               20 (bool)
                      348 BUILD_TUPLE              4
-                     350 LOAD_CONST              18 (<code object get_enabled, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 599>)
+                     350 LOAD_CONST              18 (<code object get_enabled, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 600>)
                      352 MAKE_FUNCTION            5 (defaults, annotations)
          
-         599         354 PRECALL                  0
+         600         354 PRECALL                  0
                      358 CALL                     0
          
-         600         368 STORE_NAME              21 (get_enabled)
+         601         368 STORE_NAME              21 (get_enabled)
          
-         606         370 LOAD_NAME               12 (classmethod)
+         607         370 LOAD_NAME               12 (classmethod)
          
-         611         372 NOP
+         612         372 NOP
          
-         612         374 NOP
+         613         374 NOP
          
-         607         376 LOAD_CONST              46 ((None, None))
+         608         376 LOAD_CONST              46 ((None, None))
                      378 LOAD_CONST              19 ('reference_object')
          
-         609         380 LOAD_NAME               22 (Any)
+         610         380 LOAD_NAME               22 (Any)
          
-         607         382 LOAD_CONST              20 ('feed')
+         608         382 LOAD_CONST              20 ('feed')
          
-         610         384 LOAD_NAME               23 (ExtendedICal20Feed)
+         611         384 LOAD_NAME               23 (ExtendedICal20Feed)
          
-         607         386 LOAD_CONST              11 ('request')
+         608         386 LOAD_CONST              11 ('request')
          
-         611         388 LOAD_NAME               13 (Optional)
+         612         388 LOAD_NAME               13 (Optional)
                      390 LOAD_NAME               14 (HttpRequest)
                      392 BINARY_SUBSCR
          
-         607         402 LOAD_CONST              21 ('params')
+         608         402 LOAD_CONST              21 ('params')
          
-         612         404 LOAD_NAME               13 (Optional)
+         613         404 LOAD_NAME               13 (Optional)
                      406 LOAD_NAME               24 (dict)
                      408 LOAD_NAME                5 (str)
                      410 LOAD_NAME               25 (any)
                      412 BUILD_TUPLE              2
                      414 BINARY_SUBSCR
                      424 BINARY_SUBSCR
          
-         607         434 LOAD_CONST              12 ('return')
+         608         434 LOAD_CONST              12 ('return')
          
-         613         436 LOAD_NAME               24 (dict)
+         614         436 LOAD_NAME               24 (dict)
                      438 LOAD_NAME                5 (str)
                      440 LOAD_NAME               22 (Any)
                      442 BUILD_TUPLE              2
                      444 BINARY_SUBSCR
          
-         607         454 BUILD_TUPLE             10
-                     456 LOAD_CONST              22 (<code object create_event, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 606>)
+         608         454 BUILD_TUPLE             10
+                     456 LOAD_CONST              22 (<code object create_event, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 607>)
                      458 MAKE_FUNCTION            5 (defaults, annotations)
          
-         606         460 PRECALL                  0
+         607         460 PRECALL                  0
                      464 CALL                     0
          
-         607         474 STORE_NAME              26 (create_event)
+         608         474 STORE_NAME              26 (create_event)
          
-         625         476 LOAD_NAME               12 (classmethod)
+         626         476 LOAD_NAME               12 (classmethod)
          
-         627         478 NOP
+         628         478 NOP
          
-         626         480 LOAD_CONST              46 ((None, None))
+         627         480 LOAD_CONST              46 ((None, None))
                      482 LOAD_CONST              11 ('request')
          
-         627         484 LOAD_NAME               13 (Optional)
+         628         484 LOAD_NAME               13 (Optional)
                      486 LOAD_NAME               14 (HttpRequest)
                      488 BINARY_SUBSCR
          
-         626         498 LOAD_CONST              21 ('params')
+         627         498 LOAD_CONST              21 ('params')
          
-         627         500 LOAD_NAME               13 (Optional)
+         628         500 LOAD_NAME               13 (Optional)
                      502 LOAD_NAME               24 (dict)
                      504 LOAD_NAME                5 (str)
                      506 LOAD_NAME               25 (any)
                      508 BUILD_TUPLE              2
                      510 BINARY_SUBSCR
                      520 BINARY_SUBSCR
          
-         626         530 LOAD_CONST              12 ('return')
+         627         530 LOAD_CONST              12 ('return')
          
-         628         532 LOAD_NAME               23 (ExtendedICal20Feed)
+         629         532 LOAD_NAME               23 (ExtendedICal20Feed)
          
-         626         534 BUILD_TUPLE              6
-                     536 LOAD_CONST              23 (<code object start_feed, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 625>)
+         627         534 BUILD_TUPLE              6
+                     536 LOAD_CONST              23 (<code object start_feed, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 626>)
                      538 MAKE_FUNCTION            5 (defaults, annotations)
          
-         625         540 PRECALL                  0
+         626         540 PRECALL                  0
                      544 CALL                     0
          
-         626         554 STORE_NAME              27 (start_feed)
+         627         554 STORE_NAME              27 (start_feed)
          
-         639         556 LOAD_NAME               12 (classmethod)
+         640         556 LOAD_NAME               12 (classmethod)
          
-         641         558 NOP
+         642         558 NOP
          
-         640         560 LOAD_CONST              46 ((None, None))
+         641         560 LOAD_CONST              46 ((None, None))
                      562 LOAD_CONST              11 ('request')
          
-         641         564 LOAD_NAME               13 (Optional)
+         642         564 LOAD_NAME               13 (Optional)
                      566 LOAD_NAME               14 (HttpRequest)
                      568 BINARY_SUBSCR
          
-         640         578 LOAD_CONST              21 ('params')
+         641         578 LOAD_CONST              21 ('params')
          
-         641         580 LOAD_NAME               13 (Optional)
+         642         580 LOAD_NAME               13 (Optional)
                      582 LOAD_NAME               24 (dict)
                      584 LOAD_NAME                5 (str)
                      586 LOAD_NAME               25 (any)
                      588 BUILD_TUPLE              2
                      590 BINARY_SUBSCR
                      600 BINARY_SUBSCR
          
-         640         610 LOAD_CONST              12 ('return')
+         641         610 LOAD_CONST              12 ('return')
          
-         642         612 LOAD_NAME               28 (Iterable)
+         643         612 LOAD_NAME               28 (Iterable)
          
-         640         614 BUILD_TUPLE              6
-                     616 LOAD_CONST              24 (<code object get_objects, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 639>)
+         641         614 BUILD_TUPLE              6
+                     616 LOAD_CONST              24 (<code object get_objects, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 640>)
                      618 MAKE_FUNCTION            5 (defaults, annotations)
          
-         639         620 PRECALL                  0
+         640         620 PRECALL                  0
                      624 CALL                     0
          
-         640         634 STORE_NAME              29 (get_objects)
+         641         634 STORE_NAME              29 (get_objects)
          
-         646         636 LOAD_NAME               12 (classmethod)
+         647         636 LOAD_NAME               12 (classmethod)
          
-         648         638 NOP
+         649         638 NOP
          
-         647         640 LOAD_CONST              46 ((None, None))
+         648         640 LOAD_CONST              46 ((None, None))
                      642 LOAD_CONST              11 ('request')
          
-         648         644 LOAD_NAME               13 (Optional)
+         649         644 LOAD_NAME               13 (Optional)
                      646 LOAD_NAME               14 (HttpRequest)
                      648 BINARY_SUBSCR
          
-         647         658 LOAD_CONST              21 ('params')
+         648         658 LOAD_CONST              21 ('params')
          
-         648         660 LOAD_NAME               13 (Optional)
+         649         660 LOAD_NAME               13 (Optional)
                      662 LOAD_NAME               24 (dict)
                      664 LOAD_NAME                5 (str)
                      666 LOAD_NAME               25 (any)
                      668 BUILD_TUPLE              2
                      670 BINARY_SUBSCR
                      680 BINARY_SUBSCR
          
-         647         690 LOAD_CONST              12 ('return')
+         648         690 LOAD_CONST              12 ('return')
          
-         649         692 LOAD_NAME               23 (ExtendedICal20Feed)
+         650         692 LOAD_NAME               23 (ExtendedICal20Feed)
          
-         647         694 BUILD_TUPLE              6
-                     696 LOAD_CONST              25 (<code object create_feed, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 646>)
+         648         694 BUILD_TUPLE              6
+                     696 LOAD_CONST              25 (<code object create_feed, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 647>)
                      698 MAKE_FUNCTION            5 (defaults, annotations)
          
-         646         700 PRECALL                  0
+         647         700 PRECALL                  0
                      704 CALL                     0
          
-         647         714 STORE_NAME              30 (create_feed)
+         648         714 STORE_NAME              30 (create_feed)
          
-         658         716 LOAD_NAME               12 (classmethod)
+         659         716 LOAD_NAME               12 (classmethod)
          
-         660         718 NOP
+         661         718 NOP
          
-         659         720 LOAD_CONST              46 ((None, None))
+         660         720 LOAD_CONST              46 ((None, None))
                      722 LOAD_CONST              11 ('request')
          
-         660         724 LOAD_NAME               13 (Optional)
+         661         724 LOAD_NAME               13 (Optional)
                      726 LOAD_NAME               14 (HttpRequest)
                      728 BINARY_SUBSCR
          
-         659         738 LOAD_CONST              21 ('params')
+         660         738 LOAD_CONST              21 ('params')
          
-         660         740 LOAD_NAME               13 (Optional)
+         661         740 LOAD_NAME               13 (Optional)
                      742 LOAD_NAME               24 (dict)
                      744 LOAD_NAME                5 (str)
                      746 LOAD_NAME               25 (any)
                      748 BUILD_TUPLE              2
                      750 BINARY_SUBSCR
                      760 BINARY_SUBSCR
          
-         659         770 LOAD_CONST              12 ('return')
+         660         770 LOAD_CONST              12 ('return')
          
-         661         772 LOAD_NAME               31 (Calendar)
+         662         772 LOAD_NAME               31 (Calendar)
          
-         659         774 BUILD_TUPLE              6
-                     776 LOAD_CONST              26 (<code object get_calendar_object, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 658>)
+         660         774 BUILD_TUPLE              6
+                     776 LOAD_CONST              26 (<code object get_calendar_object, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 659>)
                      778 MAKE_FUNCTION            5 (defaults, annotations)
          
-         658         780 PRECALL                  0
+         659         780 PRECALL                  0
                      784 CALL                     0
          
-         659         794 STORE_NAME              32 (get_calendar_object)
+         660         794 STORE_NAME              32 (get_calendar_object)
          
-         666         796 LOAD_NAME               12 (classmethod)
+         667         796 LOAD_NAME               12 (classmethod)
          
-         669         798 NOP
+         670         798 NOP
          
-         670         800 NOP
+         671         800 NOP
          
-         671         802 NOP
+         672         802 NOP
          
-         672         804 NOP
+         673         804 NOP
          
-         673         806 NOP
+         674         806 NOP
          
-         667         808 LOAD_CONST              47 ((None, None, None, None, False))
+         668         808 LOAD_CONST              47 ((None, None, None, None, False))
                      810 LOAD_CONST              28 ('start')
          
-         669         812 LOAD_NAME               33 (datetime)
+         670         812 LOAD_NAME               33 (datetime)
                      814 LOAD_CONST              10 (None)
                      816 BINARY_OP                7 (|)
          
-         667         820 LOAD_CONST              29 ('end')
+         668         820 LOAD_CONST              29 ('end')
          
-         670         822 LOAD_NAME               33 (datetime)
+         671         822 LOAD_NAME               33 (datetime)
                      824 LOAD_CONST              10 (None)
                      826 BINARY_OP                7 (|)
          
-         667         830 LOAD_CONST              11 ('request')
+         668         830 LOAD_CONST              11 ('request')
          
-         671         832 LOAD_NAME               14 (HttpRequest)
+         672         832 LOAD_NAME               14 (HttpRequest)
                      834 LOAD_CONST              10 (None)
                      836 BINARY_OP                7 (|)
          
-         667         840 LOAD_CONST              21 ('params')
+         668         840 LOAD_CONST              21 ('params')
          
-         672         842 LOAD_NAME               24 (dict)
+         673         842 LOAD_NAME               24 (dict)
                      844 LOAD_NAME                5 (str)
                      846 LOAD_NAME               25 (any)
                      848 BUILD_TUPLE              2
                      850 BINARY_SUBSCR
                      860 LOAD_CONST              10 (None)
                      862 BINARY_OP                7 (|)
          
-         667         866 LOAD_CONST              30 ('with_reference_object')
+         668         866 LOAD_CONST              30 ('with_reference_object')
          
-         673         868 LOAD_NAME               20 (bool)
+         674         868 LOAD_NAME               20 (bool)
          
-         667         870 BUILD_TUPLE             10
-                     872 LOAD_CONST              31 (<code object get_single_events, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 666>)
+         668         870 BUILD_TUPLE             10
+                     872 LOAD_CONST              31 (<code object get_single_events, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 667>)
                      874 MAKE_FUNCTION            5 (defaults, annotations)
          
-         666         876 PRECALL                  0
+         667         876 PRECALL                  0
                      880 CALL                     0
          
-         667         890 STORE_NAME              34 (get_single_events)
+         668         890 STORE_NAME              34 (get_single_events)
          
-         679         892 LOAD_NAME               12 (classmethod)
+         680         892 LOAD_NAME               12 (classmethod)
          
-         680         894 LOAD_CONST              12 ('return')
+         681         894 LOAD_CONST              12 ('return')
                      896 LOAD_NAME               35 (list)
                      898 LOAD_NAME                5 (str)
                      900 BINARY_SUBSCR
                      910 BUILD_TUPLE              2
-                     912 LOAD_CONST              32 (<code object get_event_field_names, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 679>)
+                     912 LOAD_CONST              32 (<code object get_event_field_names, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 680>)
                      914 MAKE_FUNCTION            4 (annotations)
          
-         679         916 PRECALL                  0
+         680         916 PRECALL                  0
                      920 CALL                     0
          
-         680         930 STORE_NAME              36 (get_event_field_names)
+         681         930 STORE_NAME              36 (get_event_field_names)
          
-         684         932 LOAD_NAME               12 (classmethod)
+         685         932 LOAD_NAME               12 (classmethod)
          
-         689         934 NOP
+         690         934 NOP
          
-         690         936 NOP
+         691         936 NOP
          
-         685         938 LOAD_CONST              46 ((None, None))
+         686         938 LOAD_CONST              46 ((None, None))
                      940 LOAD_CONST              33 ('field_name')
          
-         688         942 LOAD_NAME                5 (str)
+         689         942 LOAD_NAME                5 (str)
          
-         685         944 LOAD_CONST              11 ('request')
+         686         944 LOAD_CONST              11 ('request')
          
-         689         946 LOAD_NAME               14 (HttpRequest)
+         690         946 LOAD_NAME               14 (HttpRequest)
                      948 LOAD_CONST              10 (None)
                      950 BINARY_OP                7 (|)
          
-         685         954 LOAD_CONST              21 ('params')
+         686         954 LOAD_CONST              21 ('params')
          
-         690         956 LOAD_NAME               24 (dict)
+         691         956 LOAD_NAME               24 (dict)
                      958 LOAD_NAME                5 (str)
                      960 LOAD_NAME               22 (Any)
                      962 BUILD_TUPLE              2
                      964 BINARY_SUBSCR
                      974 LOAD_CONST              10 (None)
                      976 BINARY_OP                7 (|)
          
-         685         980 LOAD_CONST              12 ('return')
+         686         980 LOAD_CONST              12 ('return')
          
-         691         982 LOAD_NAME               25 (any)
+         692         982 LOAD_NAME               25 (any)
          
-         685         984 BUILD_TUPLE              8
-                     986 LOAD_CONST              34 (<code object get_event_field_value, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 684>)
+         686         984 BUILD_TUPLE              8
+                     986 LOAD_CONST              34 (<code object get_event_field_value, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 685>)
                      988 MAKE_FUNCTION            5 (defaults, annotations)
          
-         684         990 PRECALL                  0
+         685         990 PRECALL                  0
                      994 CALL                     0
          
-         685        1004 STORE_NAME              37 (get_event_field_value)
+         686        1004 STORE_NAME              37 (get_event_field_value)
          
-         698        1006 LOAD_NAME               12 (classmethod)
+         699        1006 LOAD_NAME               12 (classmethod)
          
-         699        1008 LOAD_CONST              45 ((None,))
+         700        1008 LOAD_CONST              45 ((None,))
                     1010 LOAD_CONST              11 ('request')
                     1012 LOAD_NAME               14 (HttpRequest)
                     1014 LOAD_CONST              10 (None)
                     1016 BINARY_OP                7 (|)
                     1020 LOAD_CONST              12 ('return')
                     1022 LOAD_NAME                5 (str)
                     1024 BUILD_TUPLE              4
-                    1026 LOAD_CONST              35 (<code object value_link, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 698>)
+                    1026 LOAD_CONST              35 (<code object value_link, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 699>)
                     1028 MAKE_FUNCTION            5 (defaults, annotations)
          
-         698        1030 PRECALL                  0
+         699        1030 PRECALL                  0
                     1034 CALL                     0
          
-         699        1044 STORE_NAME              38 (value_link)
+         700        1044 STORE_NAME              38 (value_link)
          
-         702        1046 LOAD_NAME               12 (classmethod)
+         703        1046 LOAD_NAME               12 (classmethod)
          
-         703        1048 LOAD_CONST              45 ((None,))
+         704        1048 LOAD_CONST              45 ((None,))
                     1050 LOAD_CONST              11 ('request')
                     1052 LOAD_NAME               14 (HttpRequest)
                     1054 LOAD_CONST              10 (None)
                     1056 BINARY_OP                7 (|)
                     1060 LOAD_CONST              12 ('return')
                     1062 LOAD_NAME                5 (str)
                     1064 BUILD_TUPLE              4
-                    1066 LOAD_CONST              36 (<code object value_color, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 702>)
+                    1066 LOAD_CONST              36 (<code object value_color, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 703>)
                     1068 MAKE_FUNCTION            5 (defaults, annotations)
          
-         702        1070 PRECALL                  0
+         703        1070 PRECALL                  0
                     1074 CALL                     0
          
-         703        1084 STORE_NAME              39 (value_color)
+         704        1084 STORE_NAME              39 (value_color)
          
-         706        1086 LOAD_NAME               40 (classproperty)
+         707        1086 LOAD_NAME               40 (classproperty)
          
-         707        1088 LOAD_CONST              12 ('return')
+         708        1088 LOAD_CONST              12 ('return')
                     1090 LOAD_NAME               20 (bool)
                     1092 BUILD_TUPLE              2
-                    1094 LOAD_CONST              37 (<code object valid_feed, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 706>)
+                    1094 LOAD_CONST              37 (<code object valid_feed, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 707>)
                     1096 MAKE_FUNCTION            4 (annotations)
          
-         706        1098 PRECALL                  0
+         707        1098 PRECALL                  0
                     1102 CALL                     0
          
-         707        1112 STORE_NAME              41 (valid_feed)
+         708        1112 STORE_NAME              41 (valid_feed)
          
-         711        1114 LOAD_NAME               40 (classproperty)
+         712        1114 LOAD_NAME               40 (classproperty)
          
-         712        1116 LOAD_CONST              38 (<code object valid_feeds, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 711>)
+         713        1116 LOAD_CONST              38 (<code object valid_feeds, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 712>)
                     1118 MAKE_FUNCTION            0
          
-         711        1120 PRECALL                  0
+         712        1120 PRECALL                  0
                     1124 CALL                     0
          
-         712        1134 STORE_NAME              42 (valid_feeds)
+         713        1134 STORE_NAME              42 (valid_feeds)
          
-         716        1136 LOAD_NAME               40 (classproperty)
+         717        1136 LOAD_NAME               40 (classproperty)
          
-         717        1138 LOAD_CONST              12 ('return')
+         718        1138 LOAD_CONST              12 ('return')
                     1140 LOAD_NAME               35 (list)
                     1142 LOAD_NAME                5 (str)
                     1144 BINARY_SUBSCR
                     1154 BUILD_TUPLE              2
-                    1156 LOAD_CONST              39 (<code object valid_feed_names, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 716>)
+                    1156 LOAD_CONST              39 (<code object valid_feed_names, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 717>)
                     1158 MAKE_FUNCTION            4 (annotations)
          
-         716        1160 PRECALL                  0
+         717        1160 PRECALL                  0
                     1164 CALL                     0
          
-         717        1174 STORE_NAME              43 (valid_feed_names)
+         718        1174 STORE_NAME              43 (valid_feed_names)
          
-         721        1176 LOAD_NAME               12 (classmethod)
+         722        1176 LOAD_NAME               12 (classmethod)
          
-         722        1178 LOAD_CONST              40 (<code object get_object_by_name, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 721>)
+         723        1178 LOAD_CONST              40 (<code object get_object_by_name, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 722>)
                     1180 MAKE_FUNCTION            0
          
-         721        1182 PRECALL                  0
+         722        1182 PRECALL                  0
                     1186 CALL                     0
          
-         722        1196 STORE_NAME              44 (get_object_by_name)
+         723        1196 STORE_NAME              44 (get_object_by_name)
          
-         725        1198 LOAD_NAME               12 (classmethod)
+         726        1198 LOAD_NAME               12 (classmethod)
          
-         726        1200 LOAD_CONST              41 ('person')
+         727        1200 LOAD_CONST              41 ('person')
                     1202 LOAD_CONST              42 ('Person')
                     1204 LOAD_CONST              12 ('return')
                     1206 LOAD_NAME               20 (bool)
                     1208 BUILD_TUPLE              4
-                    1210 LOAD_CONST              43 (<code object get_activated, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 725>)
+                    1210 LOAD_CONST              43 (<code object get_activated, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 726>)
                     1212 MAKE_FUNCTION            4 (annotations)
          
-         725        1214 PRECALL                  0
+         726        1214 PRECALL                  0
                     1218 CALL                     0
          
-         726        1228 STORE_NAME              45 (get_activated)
+         727        1228 STORE_NAME              45 (get_activated)
          
-         729        1230 LOAD_NAME               12 (classmethod)
+         730        1230 LOAD_NAME               12 (classmethod)
          
-         730        1232 LOAD_CONST              45 ((None,))
+         731        1232 LOAD_CONST              45 ((None,))
                     1234 LOAD_CONST              11 ('request')
                     1236 LOAD_NAME               14 (HttpRequest)
                     1238 LOAD_CONST              10 (None)
                     1240 BINARY_OP                7 (|)
                     1244 BUILD_TUPLE              2
-                    1246 LOAD_CONST              44 (<code object get_enabled_feeds, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 729>)
+                    1246 LOAD_CONST              44 (<code object get_enabled_feeds, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 730>)
                     1248 MAKE_FUNCTION            5 (defaults, annotations)
          
-         729        1250 PRECALL                  0
+         730        1250 PRECALL                  0
                     1254 CALL                     0
          
-         730        1264 STORE_NAME              46 (get_enabled_feeds)
+         731        1264 STORE_NAME              46 (get_enabled_feeds)
                     1266 LOAD_CONST              10 (None)
                     1268 RETURN_VALUE
          consts
             'CalendarEventMixin'
             "Mixin for calendar feeds.\n\n    This mixin can be used to create calendar feeds for objects. It can be used\n    by adding it to a model or another object. The basic attributes of the calendar\n    can be set by either setting the attributes of the class or by implementing\n    the corresponding class methods. Please notice that the class methods are\n    overriding the attributes. The following attributes are mandatory:\n\n    - name: Unique name for the calendar feed\n    - verbose_name: Shown name of the feed\n\n    The respective class methods have a `get_` prefix and are called without any arguments.\n    There are also some more attributes. Please refer to the class signature for more\n    information.\n\n    The list of objects used to create the calendar feed have to be provided by\n    the method `get_objects` class method. It's mandatory to implement this method.\n\n    To provide the data for the events, a certain set of class methods can be implemented.\n    The following iCal attributes are supported:\n\n    guid, title, description, link, class, created, updateddate, start_datetime, end_datetime,\n    location, geolocation, transparency, organizer, attendee, rrule, rdate, exdate, valarm, status\n\n    Additionally, the color attribute is supported. The color has to be an RGB\n    color in the format #ffffff.\n\n    To deploy extra meta data for AlekSIS' own calendar frontend, you can add a\n    dictionary for the meta attribute.\n\n    To implement a method for a certain attribute, the name of the method has to be\n    `value_<your_attribute>`. For example, to implement the `title` attribute, the\n    method `value_title` has to be implemented. The method has to return the value\n    for the attribute. The method is called with the reference object as argument.\n    "
             ''
             'name'
@@ -4219,160 +4223,160 @@
             'return'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               569           0 RESUME                   0
+               570           0 RESUME                   0
                
-               572           2 LOAD_FAST                0 (cls)
+               573           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (verbose_name)
                             14 RETURN_VALUE
                consts
                   'Return the verbose name of the calendar feed.'
                names      ('verbose_name',)
                varnames   ('cls', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_verbose_name'
-               firstlineno 569
+               firstlineno 570
                lnotab 0x0203
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               574           0 RESUME                   0
+               575           0 RESUME                   0
                
-               577           2 LOAD_FAST                0 (cls)
+               578           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (link)
                             14 RETURN_VALUE
                consts
                   'Return the link of the calendar feed.'
                names      ('link',)
                varnames   ('cls', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_link'
-               firstlineno 574
+               firstlineno 575
                lnotab 0x0203
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               579           0 RESUME                   0
+               580           0 RESUME                   0
                
-               582           2 LOAD_FAST                0 (cls)
+               583           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (description)
                             14 RETURN_VALUE
                consts
                   'Return the description of the calendar feed.'
                names      ('description',)
                varnames   ('cls', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_description'
-               firstlineno 579
+               firstlineno 580
                lnotab 0x0203
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code
                   0x97007c0172077c016a0000000000000000005300740200000000000000
                   0000006a0000000000000000005300
-               584           0 RESUME                   0
+               585           0 RESUME                   0
                
-               587           2 LOAD_FAST                1 (request)
+               588           2 LOAD_FAST                1 (request)
                              4 POP_JUMP_FORWARD_IF_FALSE     7 (to 20)
                
-               588           6 LOAD_FAST                1 (request)
+               589           6 LOAD_FAST                1 (request)
                              8 LOAD_ATTR                0 (LANGUAGE_CODE)
                             18 RETURN_VALUE
                
-               589     >>   20 LOAD_GLOBAL              2 (settings)
+               590     >>   20 LOAD_GLOBAL              2 (settings)
                             32 LOAD_ATTR                0 (LANGUAGE_CODE)
                             42 RETURN_VALUE
                consts
                   'Return the language of the calendar feed.'
                names      ('LANGUAGE_CODE', 'settings')
                varnames   ('cls', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_language'
-               firstlineno 584
+               firstlineno 585
                lnotab 0x020304010e01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               591           0 RESUME                   0
+               592           0 RESUME                   0
                
-               597           2 LOAD_FAST                0 (cls)
+               598           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (color)
                             14 RETURN_VALUE
                consts
                   'Return the color of the calendar feed.\n\n        The color has to be an RGB color in the format #ffffff.\n        '
                names      ('color',)
                varnames   ('cls', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_color'
-               firstlineno 591
+               firstlineno 592
                lnotab 0x0206
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a00000000000000000072217c01721f7c016a010000000000
                   000000a00200000000000000000000000000000000000000007c006a0000
                   00000000000000a6010000ab010000000000000000530064015300
-               599           0 RESUME                   0
+               600           0 RESUME                   0
                
-               602           2 LOAD_FAST                0 (cls)
+               603           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (permission_required)
                             14 POP_JUMP_FORWARD_IF_FALSE    33 (to 82)
                             16 LOAD_FAST                1 (request)
                             18 POP_JUMP_FORWARD_IF_FALSE    31 (to 82)
                
-               603          20 LOAD_FAST                1 (request)
+               604          20 LOAD_FAST                1 (request)
                             22 LOAD_ATTR                1 (user)
                             32 LOAD_METHOD              2 (has_perm)
                             54 LOAD_FAST                0 (cls)
                             56 LOAD_ATTR                0 (permission_required)
                             66 PRECALL                  1
                             70 CALL                     1
                             80 RETURN_VALUE
                
-               604     >>   82 LOAD_CONST               1 (True)
+               605     >>   82 LOAD_CONST               1 (True)
                             84 RETURN_VALUE
                consts
                   'Return whether the calendar is visible in the frontend.'
                   True
                names      ('permission_required', 'user', 'has_perm')
                varnames   ('cls', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_enabled'
-               firstlineno 599
+               firstlineno 600
                lnotab 0x020312013e01
             'reference_object'
             'feed'
             'params'
             code
                argcount  : 5
                nlocals   : 8
@@ -4380,73 +4384,73 @@
                flags     : 3
                code
                   0x970069007d057c00a00000000000000000000000000000000000000000
                   00a6000000ab00000000000000000044005d227d067c00a0010000000000
                   0000000000000000000000000000007c017c067c037c04ac01a6040000ab
                   0400000000000000007d077c0781057c077c057c063c0000008c2302007c
                   026a020000000000000000640369007c05a4018e0101007c055300
-               606           0 RESUME                   0
+               607           0 RESUME                   0
                
-               615           2 BUILD_MAP                0
+               616           2 BUILD_MAP                0
                              4 STORE_FAST               5 (values)
                
-               616           6 LOAD_FAST                0 (cls)
+               617           6 LOAD_FAST                0 (cls)
                              8 LOAD_METHOD              0 (get_event_field_names)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 GET_ITER
                        >>   46 FOR_ITER                34 (to 116)
                             48 STORE_FAST               6 (field)
                
-               617          50 LOAD_FAST                0 (cls)
+               618          50 LOAD_FAST                0 (cls)
                             52 LOAD_METHOD              1 (get_event_field_value)
                
-               618          74 LOAD_FAST                1 (reference_object)
+               619          74 LOAD_FAST                1 (reference_object)
                             76 LOAD_FAST                6 (field)
                             78 LOAD_FAST                3 (request)
                             80 LOAD_FAST                4 (params)
                
-               617          82 KW_NAMES                 1
+               618          82 KW_NAMES                 1
                             84 PRECALL                  4
                             88 CALL                     4
                             98 STORE_FAST               7 (field_value)
                
-               620         100 LOAD_FAST                7 (field_value)
+               621         100 LOAD_FAST                7 (field_value)
                            102 POP_JUMP_FORWARD_IF_NONE     5 (to 114)
                
-               621         104 LOAD_FAST                7 (field_value)
+               622         104 LOAD_FAST                7 (field_value)
                            106 LOAD_FAST                5 (values)
                            108 LOAD_FAST                6 (field)
                            110 STORE_SUBSCR
                        >>  114 JUMP_BACKWARD           35 (to 46)
                
-               622     >>  116 PUSH_NULL
+               623     >>  116 PUSH_NULL
                            118 LOAD_FAST                2 (feed)
                            120 LOAD_ATTR                2 (add_item)
                            130 LOAD_CONST               3 (())
                            132 BUILD_MAP                0
                            134 LOAD_FAST                5 (values)
                            136 DICT_MERGE               1
                            138 CALL_FUNCTION_EX         1
                            140 POP_TOP
                
-               623         142 LOAD_FAST                5 (values)
+               624         142 LOAD_FAST                5 (values)
                            144 RETURN_VALUE
                consts
                   'Create an event for the given reference object and add it to the feed.'
                   ('request', 'params')
                   None
                   ()
                names      ('get_event_field_names', 'get_event_field_value', 'add_item')
                varnames   ('cls', 'reference_object', 'feed', 'request', 'params', 'values', 'field', 'field_value')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'create_event'
-               firstlineno 606
+               firstlineno 607
                lnotab 0x020904012c01180108ff120304010c011a01
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 9
                flags     : 3
                code
@@ -4455,186 +4459,186 @@
                   0200000000000000000000000000000000000000007c01ac01a6010000ab
                   0100000000000000007c00a0030000000000000000000000000000000000
                   0000007c01ac01a6010000ab0100000000000000007c00a0040000000000
                   0000000000000000000000000000007c01ac01a6010000ab010000000000
                   0000007c00a00500000000000000000000000000000000000000007c01ac
                   01a6010000ab010000000000000000ac02a6050000ab0500000000000000
                   007d037c035300
-               625           0 RESUME                   0
+               626           0 RESUME                   0
                
-               630           2 LOAD_GLOBAL              1 (NULL + ExtendedICal20Feed)
+               631           2 LOAD_GLOBAL              1 (NULL + ExtendedICal20Feed)
                
-               631          14 LOAD_FAST                0 (cls)
+               632          14 LOAD_FAST                0 (cls)
                             16 LOAD_METHOD              1 (get_verbose_name)
                             38 LOAD_FAST                1 (request)
                             40 KW_NAMES                 1
                             42 PRECALL                  1
                             46 CALL                     1
                
-               632          56 LOAD_FAST                0 (cls)
+               633          56 LOAD_FAST                0 (cls)
                             58 LOAD_METHOD              2 (get_link)
                             80 LOAD_FAST                1 (request)
                             82 KW_NAMES                 1
                             84 PRECALL                  1
                             88 CALL                     1
                
-               633          98 LOAD_FAST                0 (cls)
+               634          98 LOAD_FAST                0 (cls)
                            100 LOAD_METHOD              3 (get_description)
                            122 LOAD_FAST                1 (request)
                            124 KW_NAMES                 1
                            126 PRECALL                  1
                            130 CALL                     1
                
-               634         140 LOAD_FAST                0 (cls)
+               635         140 LOAD_FAST                0 (cls)
                            142 LOAD_METHOD              4 (get_language)
                            164 LOAD_FAST                1 (request)
                            166 KW_NAMES                 1
                            168 PRECALL                  1
                            172 CALL                     1
                
-               635         182 LOAD_FAST                0 (cls)
+               636         182 LOAD_FAST                0 (cls)
                            184 LOAD_METHOD              5 (get_color)
                            206 LOAD_FAST                1 (request)
                            208 KW_NAMES                 1
                            210 PRECALL                  1
                            214 CALL                     1
                
-               630         224 KW_NAMES                 2
+               631         224 KW_NAMES                 2
                            226 PRECALL                  5
                            230 CALL                     5
                            240 STORE_FAST               3 (feed)
                
-               637         242 LOAD_FAST                3 (feed)
+               638         242 LOAD_FAST                3 (feed)
                            244 RETURN_VALUE
                consts
                   'Start the feed and return it.'
                   ('request',)
                   ('title', 'link', 'description', 'language', 'color')
                names      ('ExtendedICal20Feed', 'get_verbose_name', 'get_link', 'get_description', 'get_language', 'get_color')
                varnames   ('cls', 'request', 'params', 'feed')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'start_feed'
-               firstlineno 625
+               firstlineno 626
                lnotab 0x02050c012a012a012a012a012afb1207
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x97007400000000000000000000008201
-               639           0 RESUME                   0
+               640           0 RESUME                   0
                
-               644           2 LOAD_GLOBAL              0 (NotImplementedError)
+               645           2 LOAD_GLOBAL              0 (NotImplementedError)
                             14 RAISE_VARARGS            1
                consts
                   'Return the objects to create the calendar feed for.'
                names      ('NotImplementedError',)
                varnames   ('cls', 'request', 'params')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_objects'
-               firstlineno 639
+               firstlineno 640
                lnotab 0x0205
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 7
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c017c
                   02ac01a6020000ab0200000000000000007d037c00a00100000000000000
                   000000000000000000000000007c017c02ac01a6020000ab020000000000
                   00000044005d1b7d047c00a0020000000000000000000000000000000000
                   0000007c047c037c017c02ac01a6040000ab04000000000000000001008c
                   1c7c035300
-               646           0 RESUME                   0
+               647           0 RESUME                   0
                
-               651           2 LOAD_FAST                0 (cls)
+               652           2 LOAD_FAST                0 (cls)
                              4 LOAD_METHOD              0 (start_feed)
                             26 LOAD_FAST                1 (request)
                             28 LOAD_FAST                2 (params)
                             30 KW_NAMES                 1
                             32 PRECALL                  2
                             36 CALL                     2
                             46 STORE_FAST               3 (feed)
                
-               653          48 LOAD_FAST                0 (cls)
+               654          48 LOAD_FAST                0 (cls)
                             50 LOAD_METHOD              1 (get_objects)
                             72 LOAD_FAST                1 (request)
                             74 LOAD_FAST                2 (params)
                             76 KW_NAMES                 1
                             78 PRECALL                  2
                             82 CALL                     2
                             92 GET_ITER
                        >>   94 FOR_ITER                27 (to 150)
                             96 STORE_FAST               4 (reference_object)
                
-               654          98 LOAD_FAST                0 (cls)
+               655          98 LOAD_FAST                0 (cls)
                            100 LOAD_METHOD              2 (create_event)
                            122 LOAD_FAST                4 (reference_object)
                            124 LOAD_FAST                3 (feed)
                            126 LOAD_FAST                1 (request)
                            128 LOAD_FAST                2 (params)
                            130 KW_NAMES                 1
                            132 PRECALL                  4
                            136 CALL                     4
                            146 POP_TOP
                            148 JUMP_BACKWARD           28 (to 94)
                
-               656     >>  150 LOAD_FAST                3 (feed)
+               657     >>  150 LOAD_FAST                3 (feed)
                            152 RETURN_VALUE
                consts
                   'Create the calendar feed with all events.'
                   ('request', 'params')
                names      ('start_feed', 'get_objects', 'create_event')
                varnames   ('cls', 'request', 'params', 'feed', 'reference_object')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'create_feed'
-               firstlineno 646
+               firstlineno 647
                lnotab 0x02052e0232013402
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c017c
                   02ac01a6020000ab0200000000000000007d037c03a00100000000000000
                   00000000000000000000000000a6000000ab0000000000000000005300
-               658           0 RESUME                   0
+               659           0 RESUME                   0
                
-               663           2 LOAD_FAST                0 (cls)
+               664           2 LOAD_FAST                0 (cls)
                              4 LOAD_METHOD              0 (create_feed)
                             26 LOAD_FAST                1 (request)
                             28 LOAD_FAST                2 (params)
                             30 KW_NAMES                 1
                             32 PRECALL                  2
                             36 CALL                     2
                             46 STORE_FAST               3 (feed)
                
-               664          48 LOAD_FAST                3 (feed)
+               665          48 LOAD_FAST                3 (feed)
                             50 LOAD_METHOD              1 (get_calendar_object)
                             72 PRECALL                  0
                             76 CALL                     0
                             86 RETURN_VALUE
                consts
                   'Return the calendar object.'
                   ('request', 'params')
                names      ('create_feed', 'get_calendar_object')
                varnames   ('cls', 'request', 'params', 'feed')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_calendar_object'
-               firstlineno 658
+               firstlineno 659
                lnotab 0x02052e01
             False
             'start'
             'end'
             'with_reference_object'
             code
                argcount  : 6
@@ -4642,26 +4646,26 @@
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c037c
                   04ac01a6020000ab0200000000000000007d067c06a00100000000000000
                   000000000000000000000000007c017c027c05ac02a6030000ab03000000
                   00000000005300
-               666           0 RESUME                   0
+               667           0 RESUME                   0
                
-               676           2 LOAD_FAST                0 (cls)
+               677           2 LOAD_FAST                0 (cls)
                              4 LOAD_METHOD              0 (create_feed)
                             26 LOAD_FAST                3 (request)
                             28 LOAD_FAST                4 (params)
                             30 KW_NAMES                 1
                             32 PRECALL                  2
                             36 CALL                     2
                             46 STORE_FAST               6 (feed)
                
-               677          48 LOAD_FAST                6 (feed)
+               678          48 LOAD_FAST                6 (feed)
                             50 LOAD_METHOD              1 (get_single_events)
                             72 LOAD_FAST                1 (start)
                             74 LOAD_FAST                2 (end)
                             76 LOAD_FAST                5 (with_reference_object)
                             78 KW_NAMES                 2
                             80 PRECALL                  3
                             84 CALL                     3
@@ -4672,27 +4676,27 @@
                   ('with_reference_object',)
                names      ('create_feed', 'get_single_events')
                varnames   ('cls', 'start', 'end', 'request', 'params', 'with_reference_object', 'feed')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_single_events'
-               firstlineno 666
+               firstlineno 667
                lnotab 0x020a2e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x9700640184007400000000000000000000004400a6000000ab00000000
                   00000000005300
-               679           0 RESUME                   0
+               680           0 RESUME                   0
                
-               682           2 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 682>)
+               683           2 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 683>)
                              4 MAKE_FUNCTION            0
                              6 LOAD_GLOBAL              0 (ITEM_ELEMENT_FIELD_MAP)
                             18 GET_ITER
                             20 PRECALL                  0
                             24 CALL                     0
                             34 RETURN_VALUE
                consts
@@ -4701,15 +4705,15 @@
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d0a7d017c0164001900000000000000000091028c0b53
                         00
-                     682           0 RESUME                   0
+                     683           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                10 (to 28)
                                    8 STORE_FAST               1 (field_map)
                                   10 LOAD_FAST                1 (field_map)
                                   12 LOAD_CONST               0 (0)
                                   14 BINARY_SUBSCR
@@ -4720,46 +4724,46 @@
                         0
                      names      ()
                      varnames   ('.0', 'field_map')
                      freevars   ()
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                      name       '<listcomp>'
-                     firstlineno 682
+                     firstlineno 683
                      lnotab 0x
                names      ('ITEM_ELEMENT_FIELD_MAP',)
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_event_field_names'
-               firstlineno 679
+               firstlineno 680
                lnotab 0x0203
             'field_name'
             code
                argcount  : 5
                nlocals   : 6
                stacksize : 6
                flags     : 3
                code
                   0x970064017c029b009d027d057401000000000000000000007c007c05a6
                   020000ab0200000000000000007238740300000000000000000000740500
                   0000000000000000007c007c05a6020000ab020000000000000000a60100
                   00ab010000000000000000721b02007405000000000000000000007c007c
                   05a6020000ab0200000000000000007c017c03ac02a6020000ab02000000
                   0000000000530064035300
-               684           0 RESUME                   0
+               685           0 RESUME                   0
                
-               693           2 LOAD_CONST               1 ('value_')
+               694           2 LOAD_CONST               1 ('value_')
                              4 LOAD_FAST                2 (field_name)
                              6 FORMAT_VALUE             0
                              8 BUILD_STRING             2
                             10 STORE_FAST               5 (method_name)
                
-               694          12 LOAD_GLOBAL              1 (NULL + hasattr)
+               695          12 LOAD_GLOBAL              1 (NULL + hasattr)
                             24 LOAD_FAST                0 (cls)
                             26 LOAD_FAST                5 (method_name)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_FALSE    56 (to 156)
                             44 LOAD_GLOBAL              3 (NULL + callable)
                             56 LOAD_GLOBAL              5 (NULL + getattr)
@@ -4767,74 +4771,74 @@
                             70 LOAD_FAST                5 (method_name)
                             72 PRECALL                  2
                             76 CALL                     2
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    27 (to 156)
                
-               695         102 PUSH_NULL
+               696         102 PUSH_NULL
                            104 LOAD_GLOBAL              5 (NULL + getattr)
                            116 LOAD_FAST                0 (cls)
                            118 LOAD_FAST                5 (method_name)
                            120 PRECALL                  2
                            124 CALL                     2
                            134 LOAD_FAST                1 (reference_object)
                            136 LOAD_FAST                3 (request)
                            138 KW_NAMES                 2
                            140 PRECALL                  2
                            144 CALL                     2
                            154 RETURN_VALUE
                
-               696     >>  156 LOAD_CONST               3 (None)
+               697     >>  156 LOAD_CONST               3 (None)
                            158 RETURN_VALUE
                consts
                   'Return the value for the given field name.'
                   'value_'
                   ('request',)
                   None
                names      ('hasattr', 'callable', 'getattr')
                varnames   ('cls', 'reference_object', 'field_name', 'request', 'params', 'method_name')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_event_field_value'
-               firstlineno 684
+               firstlineno 685
                lnotab 0x02090a015a013601
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x970064015300
-               698           0 RESUME                   0
+               699           0 RESUME                   0
                
-               700           2 LOAD_CONST               1 ('')
+               701           2 LOAD_CONST               1 ('')
                              4 RETURN_VALUE
                consts
                   None
                   ''
                names      ()
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'value_link'
-               firstlineno 698
+               firstlineno 699
                lnotab 0x0202
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c02ac
                   01a6010000ab0100000000000000005300
-               702           0 RESUME                   0
+               703           0 RESUME                   0
                
-               704           2 LOAD_FAST                0 (cls)
+               705           2 LOAD_FAST                0 (cls)
                              4 LOAD_METHOD              0 (get_color)
                             26 LOAD_FAST                2 (request)
                             28 KW_NAMES                 1
                             30 PRECALL                  1
                             34 CALL                     1
                             44 RETURN_VALUE
                consts
@@ -4842,53 +4846,53 @@
                   ('request',)
                names      ('get_color',)
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'value_color'
-               firstlineno 702
+               firstlineno 703
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a0000000000000000007c006a0100000000000000006b0300
                   0000005300
-               706           0 RESUME                   0
+               707           0 RESUME                   0
                
-               709           2 LOAD_FAST                0 (cls)
+               710           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (name)
                             14 LOAD_FAST                0 (cls)
                             16 LOAD_ATTR                1 (__name__)
                             26 COMPARE_OP               3 (!=)
                             32 RETURN_VALUE
                consts
                   'Return if the feed is valid.'
                names      ('name', '__name__')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'valid_feed'
-               firstlineno 706
+               firstlineno 707
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x9700640184007c006a0000000000000000004400a6000000ab00000000
                   00000000005300
-               711           0 RESUME                   0
+               712           0 RESUME                   0
                
-               714           2 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 714>)
+               715           2 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 715>)
                              4 MAKE_FUNCTION            0
                              6 LOAD_FAST                0 (cls)
                              8 LOAD_ATTR                0 (registered_objects_list)
                             18 GET_ITER
                             20 PRECALL                  0
                             24 CALL                     0
                             34 RETURN_VALUE
@@ -4898,15 +4902,15 @@
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code
                         0x970067007c005d0b7d017c016a000000000000000000af097c0191028c
                         0c5300
-                     714           0 RESUME                   0
+                     715           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                11 (to 30)
                                    8 STORE_FAST               1 (feed)
                                   10 LOAD_FAST                1 (feed)
                                   12 LOAD_ATTR                0 (valid_feed)
                                   22 POP_JUMP_BACKWARD_IF_FALSE     9 (to 6)
@@ -4917,35 +4921,35 @@
                      consts
                      names      ('valid_feed',)
                      varnames   ('.0', 'feed')
                      freevars   ()
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                      name       '<listcomp>'
-                     firstlineno 714
+                     firstlineno 715
                      lnotab 0x
                names      ('registered_objects_list',)
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'valid_feeds'
-               firstlineno 711
+               firstlineno 712
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x9700640184007c006a0000000000000000004400a6000000ab00000000
                   00000000005300
-               716           0 RESUME                   0
+               717           0 RESUME                   0
                
-               719           2 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 719>)
+               720           2 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 720>)
                              4 MAKE_FUNCTION            0
                              6 LOAD_FAST                0 (cls)
                              8 LOAD_ATTR                0 (valid_feeds)
                             18 GET_ITER
                             20 PRECALL                  0
                             24 CALL                     0
                             34 RETURN_VALUE
@@ -4953,15 +4957,15 @@
                   'Return a list of valid feed names.'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                     719           0 RESUME                   0
+                     720           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 STORE_FAST               1 (feed)
                                   10 LOAD_FAST                1 (feed)
                                   12 LOAD_ATTR                0 (name)
                                   22 LIST_APPEND              2
@@ -4970,64 +4974,64 @@
                      consts
                      names      ('name',)
                      varnames   ('.0', 'feed')
                      freevars   ()
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                      name       '<listcomp>'
-                     firstlineno 719
+                     firstlineno 720
                      lnotab 0x
                names      ('valid_feeds',)
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'valid_feed_names'
-               firstlineno 716
+               firstlineno 717
                lnotab 0x0203
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000005300
-               721           0 RESUME                   0
+               722           0 RESUME                   0
                
-               723           2 LOAD_FAST                0 (cls)
+               724           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (registered_objects_dict)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                1 (name)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 RETURN_VALUE
                consts
                   None
                names      ('registered_objects_dict', 'get')
                varnames   ('cls', 'name')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_object_by_name'
-               firstlineno 721
+               firstlineno 722
                lnotab 0x0202
             'person'
             'Person'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c016a010000000000000000640119
                   00000000000000000076005300
-               725           0 RESUME                   0
+               726           0 RESUME                   0
                
-               727           2 LOAD_FAST                0 (cls)
+               728           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (name)
                             14 LOAD_FAST                1 (person)
                             16 LOAD_ATTR                1 (preferences)
                             26 LOAD_CONST               1 ('calendar__activated_calendars')
                             28 BINARY_SUBSCR
                             38 CONTAINS_OP              0
                             40 RETURN_VALUE
@@ -5036,31 +5040,31 @@
                   'calendar__activated_calendars'
                names      ('name', 'preferences')
                varnames   ('cls', 'person')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_activated'
-               firstlineno 725
+               firstlineno 726
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x8701970088016601640184087c006a0000000000000000004400a60000
                   00ab0000000000000000005300
                              0 MAKE_CELL                1 (request)
                
-               729           2 RESUME                   0
+               730           2 RESUME                   0
                
-               731           4 LOAD_CLOSURE             1 (request)
+               732           4 LOAD_CLOSURE             1 (request)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 731>)
+                             8 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 732>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 LOAD_FAST                0 (cls)
                             14 LOAD_ATTR                0 (valid_feeds)
                             24 GET_ITER
                             26 PRECALL                  0
                             30 CALL                     0
                             40 RETURN_VALUE
@@ -5073,15 +5077,15 @@
                      flags     : 19
                      code
                         0x9501970067007c005d197d017c01a00000000000000000000000000000
                         000000000000008902a6010000ab010000000000000000af177c0191028c
                         1a5300
                                    0 COPY_FREE_VARS           1
                      
-                     731           2 RESUME                   0
+                     732           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                25 (to 60)
                                   10 STORE_FAST               1 (feed)
                                   12 LOAD_FAST                1 (feed)
                                   14 LOAD_METHOD              0 (get_enabled)
                                   36 LOAD_DEREF               2 (request)
@@ -5095,34 +5099,34 @@
                      consts
                      names      ('get_enabled',)
                      varnames   ('.0', 'feed')
                      freevars   ('request',)
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                      name       '<listcomp>'
-                     firstlineno 731
+                     firstlineno 732
                      lnotab 0x
                names      ('valid_feeds',)
                varnames   ('cls', 'request')
                freevars   ()
                cellvars   ('request',)
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_enabled_feeds'
-               firstlineno 729
+               firstlineno 730
                lnotab 0x0402
             (None,)
             (None, None)
             (None, None, None, None, False)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'name', 'str', '__annotations__', 'verbose_name', 'link', 'description', 'color', 'permission_required', 'classmethod', 'Optional', 'HttpRequest', 'get_verbose_name', 'get_link', 'get_description', 'get_language', 'get_color', 'bool', 'get_enabled', 'Any', 'ExtendedICal20Feed', 'dict', 'any', 'create_event', 'start_feed', 'Iterable', 'get_objects', 'create_feed', 'Calendar', 'get_calendar_object', 'datetime', 'get_single_events', 'list', 'get_event_field_names', 'get_event_field_value', 'value_link', 'value_color', 'classproperty', 'valid_feed', 'valid_feeds', 'valid_feed_names', 'get_object_by_name', 'get_activated', 'get_enabled_feeds')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'CalendarEventMixin'
-         firstlineno 525
+         firstlineno 526
          lnotab
             0x0c0104240e010e010e010e010e010e0202011cff0e01020402011cff0e
             01020402011cff0e01020402011cff0e01020602011cff0e010207020116
             ff0e0102060205020102fb040202fe020302fd02040efc02051efb020612
             fa06ff0e010212020202ff04010eff02011eff020202fe06ff0e01020d02
             0202ff04010eff02011eff020202fe06ff0e010206020202ff04010eff02
             011eff020202fe06ff0e01020b020202ff04010eff02011eff020202fe06
@@ -5138,9 +5142,9 @@
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020308010c0128020c010c0110010c010c0110010c011401100110
       010c011001100208010c010c010c010c010c010c0114010c010c010c0218
-      070c0204010c03301406162a7f00561e040a0106ff120b1a06260b1c0d20
+      070c0204010c03301406162a7f00561e040a0106ff120c1a06260b1c0d20
       2c1e061c091c071e041e041c131c121c111c0b1a231c05
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/models.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/models.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 64469
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 16
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/preferences.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/preferences.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 15497
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
@@ -3539,15 +3539,15 @@
          
          488          14 LOAD_NAME                4 (calendar)
                       16 STORE_NAME               5 (section)
          
          489          18 LOAD_CONST               2 ('birthday_color')
                       20 STORE_NAME               6 (name)
          
-         490          22 LOAD_CONST               3 ('#0d5eaf')
+         490          22 LOAD_CONST               3 ('#f39c12')
                       24 STORE_NAME               7 (default)
          
          491          26 PUSH_NULL
                       28 LOAD_NAME                8 (_)
                       30 LOAD_CONST               4 ('Birthday calendar feed color')
                       32 PRECALL                  1
                       36 CALL                     1
@@ -3560,15 +3560,15 @@
                       54 STORE_NAME              12 (required)
                       56 LOAD_CONST               6 (None)
                       58 RETURN_VALUE
          consts
             'BirthdayFeedColor'
             'Color for the birthdays calendar feed.'
             'birthday_color'
-            '#0d5eaf'
+            '#f39c12'
             'Birthday calendar feed color'
             True
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'calendar', 'section', 'name', 'default', '_', 'verbose_name', 'ColorWidget', 'widget', 'required')
          varnames   ()
          freevars   ()
          cellvars   ()
@@ -3597,15 +3597,15 @@
          
          500          14 LOAD_NAME                4 (calendar)
                       16 STORE_NAME               5 (section)
          
          501          18 LOAD_CONST               2 ('holiday_color')
                       20 STORE_NAME               6 (name)
          
-         502          22 LOAD_CONST               3 ('#0d5eaf')
+         502          22 LOAD_CONST               3 ('#00b894')
                       24 STORE_NAME               7 (default)
          
          503          26 PUSH_NULL
                       28 LOAD_NAME                8 (_)
                       30 LOAD_CONST               4 ('Holiday calendar feed color')
                       32 PRECALL                  1
                       36 CALL                     1
@@ -3618,15 +3618,15 @@
                       54 STORE_NAME              12 (required)
                       56 LOAD_CONST               6 (None)
                       58 RETURN_VALUE
          consts
             'HolidayFeedColor'
             'Color for the holidays calendar feed.'
             'holiday_color'
-            '#0d5eaf'
+            '#00b894'
             'Holiday calendar feed color'
             True
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'calendar', 'section', 'name', 'default', '_', 'verbose_name', 'ColorWidget', 'widget', 'required')
          varnames   ()
          freevars   ()
          cellvars   ()
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/registries.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/registries.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 611
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/rules.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/rules.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
-files sz: 16852
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+files sz: 17713
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064026c006d015a010100640364046c026d
@@ -201,15 +201,29 @@
       63020065006a14000000000000000064986563a6020000ab020000000000
       0000000100650c0200650a6499a6010000ab0100000000000000007a0100
       005a64020065006a140000000000000000649a6564a6020000ab02000000
       00000000000100650c0200650a649ba6010000ab01000000000000000065
       127a0700007a0100005a65020065006a140000000000000000649c6565a6
       020000ab0200000000000000000100650c0200650a649da6010000ab0100
       0000000000000065127a0700007a0100005a66020065006a140000000000
-      000000649e6566a6020000ab020000000000000000010064015300
+      000000649e6566a6020000ab0200000000000000000100650c0200650a64
+      9fa6010000ab0100000000000000000200650b649fa6010000ab01000000
+      00000000007a0700007a0100005a67020065006a14000000000000000064
+      a06567a6020000ab0200000000000000000100650c0200650a649fa60100
+      00ab01000000000000000002006509649f6506a6020000ab020000000000
+      0000007a0700007a0100005a68020065006a14000000000000000064a165
+      68a6020000ab0200000000000000000100650c0200650a64a2a6010000ab
+      0100000000000000000200650b64a2a6010000ab0100000000000000007a
+      0700007a0100005a69020065006a14000000000000000064a36569a60200
+      00ab0200000000000000000100650c0200650a64a4a6010000ab01000000
+      00000000007a0100005a6a020065006a14000000000000000064a5656aa6
+      020000ab0200000000000000000100650c0200650a64a6a6010000ab0100
+      000000000000000200650b64a6a6010000ab0100000000000000007a0700
+      007a0100005a6b020065006a14000000000000000064a7656ba6020000ab
+      020000000000000000010064015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (rules)
                  8 STORE_NAME               0 (rules)
    
@@ -2082,16 +2096,139 @@
               5930 LOAD_NAME                0 (rules)
               5932 LOAD_ATTR               20 (add_perm)
               5942 LOAD_CONST             158 ('core.delete_personal_event_rule')
               5944 LOAD_NAME              102 (delete_personal_event_predicate)
               5946 PRECALL                  2
               5950 CALL                     2
               5960 POP_TOP
-              5962 LOAD_CONST               1 (None)
-              5964 RETURN_VALUE
+   
+   442        5962 LOAD_NAME               12 (has_person)
+   
+   443        5964 PUSH_NULL
+              5966 LOAD_NAME               10 (has_global_perm)
+              5968 LOAD_CONST             159 ('core.view_room')
+              5970 PRECALL                  1
+              5974 CALL                     1
+              5984 PUSH_NULL
+              5986 LOAD_NAME               11 (has_object_perm)
+              5988 LOAD_CONST             159 ('core.view_room')
+              5990 PRECALL                  1
+              5994 CALL                     1
+              6004 BINARY_OP                7 (|)
+   
+   442        6008 BINARY_OP                1 (&)
+              6012 STORE_NAME             103 (view_room_predicate)
+   
+   445        6014 PUSH_NULL
+              6016 LOAD_NAME                0 (rules)
+              6018 LOAD_ATTR               20 (add_perm)
+              6028 LOAD_CONST             160 ('core.view_room_rule')
+              6030 LOAD_NAME              103 (view_room_predicate)
+              6032 PRECALL                  2
+              6036 CALL                     2
+              6046 POP_TOP
+   
+   447        6048 LOAD_NAME               12 (has_person)
+   
+   448        6050 PUSH_NULL
+              6052 LOAD_NAME               10 (has_global_perm)
+              6054 LOAD_CONST             159 ('core.view_room')
+              6056 PRECALL                  1
+              6060 CALL                     1
+              6070 PUSH_NULL
+              6072 LOAD_NAME                9 (has_any_object)
+              6074 LOAD_CONST             159 ('core.view_room')
+              6076 LOAD_NAME                6 (Holiday)
+              6078 PRECALL                  2
+              6082 CALL                     2
+              6092 BINARY_OP                7 (|)
+   
+   447        6096 BINARY_OP                1 (&)
+              6100 STORE_NAME             104 (view_rooms_predicate)
+   
+   450        6102 PUSH_NULL
+              6104 LOAD_NAME                0 (rules)
+              6106 LOAD_ATTR               20 (add_perm)
+              6116 LOAD_CONST             161 ('core.view_rooms_rule')
+              6118 LOAD_NAME              104 (view_rooms_predicate)
+              6120 PRECALL                  2
+              6124 CALL                     2
+              6134 POP_TOP
+   
+   452        6136 LOAD_NAME               12 (has_person)
+   
+   453        6138 PUSH_NULL
+              6140 LOAD_NAME               10 (has_global_perm)
+              6142 LOAD_CONST             162 ('core.change_room')
+              6144 PRECALL                  1
+              6148 CALL                     1
+              6158 PUSH_NULL
+              6160 LOAD_NAME               11 (has_object_perm)
+              6162 LOAD_CONST             162 ('core.change_room')
+              6164 PRECALL                  1
+              6168 CALL                     1
+              6178 BINARY_OP                7 (|)
+   
+   452        6182 BINARY_OP                1 (&)
+              6186 STORE_NAME             105 (edit_room_predicate)
+   
+   455        6188 PUSH_NULL
+              6190 LOAD_NAME                0 (rules)
+              6192 LOAD_ATTR               20 (add_perm)
+              6202 LOAD_CONST             163 ('core.edit_room_rule')
+              6204 LOAD_NAME              105 (edit_room_predicate)
+              6206 PRECALL                  2
+              6210 CALL                     2
+              6220 POP_TOP
+   
+   457        6222 LOAD_NAME               12 (has_person)
+              6224 PUSH_NULL
+              6226 LOAD_NAME               10 (has_global_perm)
+              6228 LOAD_CONST             164 ('core.add_room')
+              6230 PRECALL                  1
+              6234 CALL                     1
+              6244 BINARY_OP                1 (&)
+              6248 STORE_NAME             106 (create_room_predicate)
+   
+   458        6250 PUSH_NULL
+              6252 LOAD_NAME                0 (rules)
+              6254 LOAD_ATTR               20 (add_perm)
+              6264 LOAD_CONST             165 ('core.create_room_rule')
+              6266 LOAD_NAME              106 (create_room_predicate)
+              6268 PRECALL                  2
+              6272 CALL                     2
+              6282 POP_TOP
+   
+   460        6284 LOAD_NAME               12 (has_person)
+   
+   461        6286 PUSH_NULL
+              6288 LOAD_NAME               10 (has_global_perm)
+              6290 LOAD_CONST             166 ('core.delete_room')
+              6292 PRECALL                  1
+              6296 CALL                     1
+              6306 PUSH_NULL
+              6308 LOAD_NAME               11 (has_object_perm)
+              6310 LOAD_CONST             166 ('core.delete_room')
+              6312 PRECALL                  1
+              6316 CALL                     1
+              6326 BINARY_OP                7 (|)
+   
+   460        6330 BINARY_OP                1 (&)
+              6334 STORE_NAME             107 (delete_room_predicate)
+   
+   463        6336 PUSH_NULL
+              6338 LOAD_NAME                0 (rules)
+              6340 LOAD_ATTR               20 (add_perm)
+              6350 LOAD_CONST             167 ('core.delete_room_rule')
+              6352 LOAD_NAME              107 (delete_room_predicate)
+              6354 PRECALL                  2
+              6358 CALL                     2
+              6368 POP_TOP
+              6370 LOAD_CONST               1 (None)
+              6372 RETURN_VALUE
    consts
       0
       None
       ('is_superuser',)
       1
       ('Announcement', 'Group', 'GroupType', 'Holiday', 'Person')
       ('has_any_object', 'has_global_perm', 'has_object_perm', 'has_person', 'is_anonymous', 'is_current_person', 'is_group_owner', 'is_notification_recipient', 'is_own_celery_task', 'is_personal_event_owner', 'is_site_preference_set')
@@ -2244,15 +2381,24 @@
       'core.create_personal_event_rule'
       'core.create_personalevent'
       'core.create_personal_event_with_invitations_rule'
       'core.change_personalevent'
       'core.edit_personal_event_rule'
       'core.delete_personalevent'
       'core.delete_personal_event_rule'
-   names      ('rules', 'is_superuser', 'models', 'Announcement', 'Group', 'GroupType', 'Holiday', 'Person', 'util.predicates', 'has_any_object', 'has_global_perm', 'has_object_perm', 'has_person', 'is_anonymous', 'is_current_person', 'is_group_owner', 'is_notification_recipient', 'is_own_celery_task', 'is_personal_event_owner', 'is_site_preference_set', 'add_perm', 'always_allow', 'login_predicate', 'logout_predicate', 'view_account_predicate', 'manage_2fa_predicate', 'manage_social_connections_predicate', 'manage_authorized_tokens_predicate', 'view_dashboard_predicate', 'search_predicate', 'view_persons_predicate', 'view_person_predicate', 'view_address_predicate', 'view_contact_details_predicate', 'view_photo_predicate', 'view_avatar_predicate', 'view_groups_predicate', 'edit_person_predicate', 'delete_person_predicate', 'view_group_predicate', 'edit_group_predicate', 'delete_group_predicate', 'assign_child_groups_to_groups_predicate', 'edit_school_information_predicate', 'manage_data_predicate', 'mark_notification_as_read_predicate', 'view_announcements_predicate', 'create_or_edit_announcement_predicate', 'delete_announcement_predicate', 'impersonate_predicate', 'view_system_status_predicate', 'view_personal_details_predicate', 'change_site_preferences', 'change_person_preferences', 'change_account_preferences', 'change_group_preferences', 'view_group_type_predicate', 'change_group_type_predicate', 'create_group_type_predicate', 'delete_group_type_predicate', 'view_group_types_predicate', 'create_person_predicate', 'create_group_predicate', 'view_school_term_predicate', 'create_school_term_predicate', 'edit_school_term_predicate', 'view_group_stats_predicate', 'view_data_check_results_predicate', 'run_data_checks_predicate', 'solve_data_problem_predicate', 'view_dashboard_widget_predicate', 'create_dashboard_widget_predicate', 'edit_dashboard_widget_predicate', 'delete_dashboard_widget_predicate', 'edit_dashboard_predicate', 'edit_default_dashboard_predicate', 'signup_predicate', 'change_password_predicate', 'reset_password_predicate', 'invite_enabled_predicate', 'accept_invite_predicate', 'invite_predicate', 'create_oauthapplication_predicate', 'view_oauth_applications_predicate', 'view_oauth_application_predicate', 'edit_oauth_application_predicate', 'delete_oauth_applications_predicate', 'view_django_admin_predicate', 'view_admin_menu_predicate', 'upload_files_ckeditor_predicate', 'manage_person_permissions_predicate', 'test_pdf_generation_predicate', 'view_progress_predicate', 'view_calendar_feed_predicate', 'view_holiday_predicate', 'view_holidays_predicate', 'edit_holiday_predicate', 'create_holiday_predicate', 'delete_holiday_predicate', 'create_personal_event_predicate', 'create_personal_event_with_invitations_predicate', 'edit_personal_event_predicate', 'delete_personal_event_predicate')
+      'core.view_room'
+      'core.view_room_rule'
+      'core.view_rooms_rule'
+      'core.change_room'
+      'core.edit_room_rule'
+      'core.add_room'
+      'core.create_room_rule'
+      'core.delete_room'
+      'core.delete_room_rule'
+   names      ('rules', 'is_superuser', 'models', 'Announcement', 'Group', 'GroupType', 'Holiday', 'Person', 'util.predicates', 'has_any_object', 'has_global_perm', 'has_object_perm', 'has_person', 'is_anonymous', 'is_current_person', 'is_group_owner', 'is_notification_recipient', 'is_own_celery_task', 'is_personal_event_owner', 'is_site_preference_set', 'add_perm', 'always_allow', 'login_predicate', 'logout_predicate', 'view_account_predicate', 'manage_2fa_predicate', 'manage_social_connections_predicate', 'manage_authorized_tokens_predicate', 'view_dashboard_predicate', 'search_predicate', 'view_persons_predicate', 'view_person_predicate', 'view_address_predicate', 'view_contact_details_predicate', 'view_photo_predicate', 'view_avatar_predicate', 'view_groups_predicate', 'edit_person_predicate', 'delete_person_predicate', 'view_group_predicate', 'edit_group_predicate', 'delete_group_predicate', 'assign_child_groups_to_groups_predicate', 'edit_school_information_predicate', 'manage_data_predicate', 'mark_notification_as_read_predicate', 'view_announcements_predicate', 'create_or_edit_announcement_predicate', 'delete_announcement_predicate', 'impersonate_predicate', 'view_system_status_predicate', 'view_personal_details_predicate', 'change_site_preferences', 'change_person_preferences', 'change_account_preferences', 'change_group_preferences', 'view_group_type_predicate', 'change_group_type_predicate', 'create_group_type_predicate', 'delete_group_type_predicate', 'view_group_types_predicate', 'create_person_predicate', 'create_group_predicate', 'view_school_term_predicate', 'create_school_term_predicate', 'edit_school_term_predicate', 'view_group_stats_predicate', 'view_data_check_results_predicate', 'run_data_checks_predicate', 'solve_data_problem_predicate', 'view_dashboard_widget_predicate', 'create_dashboard_widget_predicate', 'edit_dashboard_widget_predicate', 'delete_dashboard_widget_predicate', 'edit_dashboard_predicate', 'edit_default_dashboard_predicate', 'signup_predicate', 'change_password_predicate', 'reset_password_predicate', 'invite_enabled_predicate', 'accept_invite_predicate', 'invite_predicate', 'create_oauthapplication_predicate', 'view_oauth_applications_predicate', 'view_oauth_application_predicate', 'edit_oauth_application_predicate', 'delete_oauth_applications_predicate', 'view_django_admin_predicate', 'view_admin_menu_predicate', 'upload_files_ckeditor_predicate', 'manage_person_permissions_predicate', 'test_pdf_generation_predicate', 'view_progress_predicate', 'view_calendar_feed_predicate', 'view_holiday_predicate', 'view_holidays_predicate', 'edit_holiday_predicate', 'create_holiday_predicate', 'delete_holiday_predicate', 'create_personal_event_predicate', 'create_personal_event_with_invitations_predicate', 'edit_personal_event_predicate', 'delete_personal_event_predicate', 'view_room_predicate', 'view_rooms_predicate', 'edit_room_predicate', 'create_room_predicate', 'delete_room_predicate')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/rules.py'
    name       '<module>'
    firstlineno 1
    lnotab
@@ -2272,8 +2418,9 @@
       01220420ff0203220420ff020322021c0122021c0122021c0122021c0122
       021e0122021c0122031a012202060104ff160322021a0122031a0122020a
       012202220122031c0122021c0122021c0122021c0122021c0122020a0122
       030201020102ff040202fe040302fd040402fc040502fb040602fa040702
       f9040802f804ff060b22031c0122020a0122021c0122020a012202040122
       0402012cff0603220202012eff0603220202012cff060322021c01220202
       012cff0603220404012202060102ff14030e01020102fe100502011aff06
-      03220202011aff0603
+      03220202011aff0603220302012cff0603220202012eff0603220202012c
+      ff060322021c01220202012cff0603
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/settings.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/settings.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 39858
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 18
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/__pycache__/tasks.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/tasks.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 2330
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/admin.py` & `aleksis_core-4.0.0.dev6/aleksis/core/admin.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/apps.py` & `aleksis_core-4.0.0.dev6/aleksis/core/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/celery.py` & `aleksis_core-4.0.0.dev6/aleksis/core/celery.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/checks.py` & `aleksis_core-4.0.0.dev6/aleksis/core/checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/data_checks.py` & `aleksis_core-4.0.0.dev6/aleksis/core/data_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/decorators.py` & `aleksis_core-4.0.0.dev6/aleksis/core/decorators.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/filters.py` & `aleksis_core-4.0.0.dev6/aleksis/core/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/forms.py` & `aleksis_core-4.0.0.dev6/aleksis/core/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from material import Fieldset, Layout, Row
 
 from .mixins import ExtensibleForm, SchoolTermRelatedExtensibleForm
 from .models import (
     Announcement,
     DashboardWidget,
     Group,
-    GroupType,
     OAuthApplication,
     Person,
     PersonInvitation,
 )
 from .registries import (
     group_preferences_registry,
     person_preferences_registry,
@@ -109,14 +108,15 @@
     def __init__(self, *args, **kwargs):
         request = kwargs.pop("request", None)
         super().__init__(*args, **kwargs)
 
         if (
             request
             and self.instance
+            and not request.user.has_perm("core.change_person")
             and not request.user.has_perm("core.change_person", self.instance)
         ):
             # Disable non-editable fields
             allowed_person_fields = get_site_preferences()["account__editable_fields_person"]
             for field in self.fields:
                 if field not in allowed_person_fields:
                     self.fields[field].disabled = True
@@ -350,22 +350,14 @@
 
 class GroupPreferenceForm(PreferenceForm):
     """Form to edit preferences valid for members of a group."""
 
     registry = group_preferences_registry
 
 
-class EditGroupTypeForm(forms.ModelForm):
-    """Form to manage group types."""
-
-    class Meta:
-        model = GroupType
-        fields = ["name", "description"]
-
-
 class DashboardWidgetOrderForm(ExtensibleForm):
     pk = forms.ModelChoiceField(
         queryset=None,
         widget=forms.HiddenInput(attrs={"class": "pk-input"}),
     )
     order = forms.IntegerField(initial=0, widget=forms.HiddenInput(attrs={"class": "order-input"}))
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/app/apollo.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/apollo.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/app/dateTimeFormats.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/dateTimeFormats.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -33,14 +33,20 @@
             hour: "numeric",
             minute: "numeric",
         },
         shortTime: {
             hour: "numeric",
             minute: "numeric",
         },
+        dateWithWeekday: {
+            year: "numeric",
+            month: "long",
+            day: "numeric",
+            weekday: "long",
+        },
     },
     de: {
         short: {
             year: "numeric",
             month: "short",
             day: "numeric",
         },
@@ -71,11 +77,17 @@
             hour: "numeric",
             minute: "numeric",
         },
         shortTime: {
             hour: "numeric",
             minute: "numeric",
         },
+        dateWithWeekday: {
+            year: "numeric",
+            month: "long",
+            day: "numeric",
+            weekday: "long",
+        },
     },
 };
 
 export default dateTimeFormats;
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/app/vuetify.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/vuetify.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/LegacyBaseTemplate.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/LegacyBaseTemplate.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/about/AboutAleksis.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/AboutAleksis.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/about/InstalledAppCard.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/InstalledAppCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/about/InstalledAppsList.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/InstalledAppsList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/AccountMenu.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/AccountMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/App.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/App.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/ErrorPage.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/ErrorPage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/LanguageForm.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/LanguageForm.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/SideNav.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/SideNav.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/SidenavSearch.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/SidenavSearch.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/SnackbarItem.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/SnackbarItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/app/Splash.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/Splash.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/BaseCalendarFeedDetails.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/BaseCalendarFeedDetails.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/BaseCalendarFeedEventBar.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/BaseCalendarFeedEventBar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/Calendar.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/Calendar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CalendarControlBar.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarControlBar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CalendarOverview.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CalendarSelect.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarSelect.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CalendarTypeSelect.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarTypeSelect.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/CalendarWithControls.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarWithControls.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/calendarMixin.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/calendarMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/calendarSelectedFeedsMixin.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/calendarSelectedFeedsMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar/personal_event/personalEvent.graphql` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/personal_event/personalEvent.graphql`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,16 @@
       id
       title
       description
       location
 
       datetimeStart
       datetimeEnd
+      dateStart
+      dateEnd
       recurrences
 
       persons {
         id
         fullName
       }
       groups {
@@ -34,14 +36,16 @@
       id
       title
       description
       location
 
       datetimeStart
       datetimeEnd
+      dateStart
+      dateEnd
       recurrences
 
       persons {
         id
         fullName
       }
       groups {
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar_feeds/details/BirthdaysDetails.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar_feeds/details/BirthdaysDetails.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/calendar_feeds/details/PersonalDetails.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar_feeds/details/PersonalDetails.vue`

 * *Files 4% similar despite different names*

```diff
@@ -156,13 +156,17 @@
         persons: this.selectedEvent.meta.persons.map((p) => p.id.toString()),
         groups: this.selectedEvent.meta.groups.map((g) => g.id.toString()),
         title: this.selectedEvent.name,
         description: this.selectedEvent.meta.description,
         location: this.selectedEvent.location,
         datetimeStart: this.selectedEvent.startDateTime.toISO(),
         datetimeEnd: this.selectedEvent.endDateTime.toISO(),
+        dateStart: this.selectedEvent.startDateTime.toISODate(),
+        dateEnd: this.selectedEvent.endDateTime.toISODate(),
+        fullDay: this.selectedEvent.allDay,
         recurrences: this.selectedEvent.meta.recurrences,
+        recurring: !!this.selectedEvent.meta.recurrences,
       };
     },
   },
 };
 </script>
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,19 @@
       </v-card-text>
       <v-card-actions
         v-if="
           progress &&
           (progress.state === 'FAILURE' || progress.state === 'SUCCESS')
         "
       >
-        <back-button :href="progress.meta.backUrl" text />
+        <back-button
+          v-if="progress.meta.backUrl"
+          :href="progress.meta.backUrl"
+          text
+        />
         <v-spacer />
         <v-btn
           v-if="progress.meta.additionalButton && progress.state === 'SUCCESS'"
           :href="progress.meta.additionalButton.url"
           text
           color="primary"
         >
@@ -112,14 +116,16 @@
         this.$apollo.queries.celeryProgressByTaskId.stopPolling();
         this.$apollo.mutate({
           mutation: gqlCeleryProgressFetched,
           variables: {
             taskId: this.$route.params.taskId,
           },
         });
+      } else {
+        this.$activateFrequentCeleryPolling();
       }
       if (newState === "SUCCESS" && this.progress.meta.redirectOnSuccessUrl) {
         this.$router.push(this.progress.meta.redirectOnSuccessUrl);
       }
     },
   },
 };
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue`

 * *Files 19% similar despite different names*

```diff
@@ -32,39 +32,60 @@
   </v-bottom-sheet>
 </template>
 
 <script>
 import TaskListItem from "./TaskListItem.vue";
 import gqlCeleryProgressButton from "./celeryProgressBottom.graphql";
 
+const NORMAL_INTERVAL = 30000;
+const FREQUENT_INTERVAL = 1000;
+
 export default {
   name: "CeleryProgressBottom",
   components: { TaskListItem },
   data() {
     return { open: 0 };
   },
   mounted() {
     // Vuetify uses the hideScroll method to disable scrolling by setting an event listener
     // to the window. As event listeners can only be removed by referencing the listener
     // method and because vuetify this method is called on every state change of the dialog,
     // we simply replace the method in this component instance
     this.$refs.sheet.hideScroll = this.$refs.sheet.showScroll;
   },
+  watch: {
+    "$root.frequentCeleryPolling": function (newValue) {
+      // Watch for activation of frequent polling and update poll interval accordingly
+
+      const newInterval = newValue ? FREQUENT_INTERVAL : NORMAL_INTERVAL;
+      if (
+        this.$apollo.queries.celeryProgressByUser.options.pollInterval !==
+        newInterval
+      ) {
+        this.$apollo.queries.celeryProgressByUser.stopPolling();
+        this.$apollo.queries.celeryProgressByUser.startPolling(newInterval);
+      }
+    },
+  },
   computed: {
     show() {
       return this.celeryProgressByUser && this.celeryProgressByUser.length > 0;
     },
     numberOfTasks() {
       if (!this.celeryProgressByUser) {
         return 0;
       }
       return this.celeryProgressByUser.length;
     },
   },
   apollo: {
     celeryProgressByUser: {
       query: gqlCeleryProgressButton,
-      pollInterval: 30000,
+      pollInterval: NORMAL_INTERVAL,
+      result({ data }) {
+        // Deactivate frequent polling if there is not at least one running task
+        this.$root.frequentCeleryPolling = data.celeryProgressByUser.length > 0;
+      },
     },
   },
 };
 </script>
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/celery_progress/TaskListItem.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/TaskListItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/ActionSelect.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ActionSelect.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/AvatarClickbox.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/AvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/ButtonMenu.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ButtonMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/CRUDBar.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CRUDBar.vue`

 * *Files 3% similar despite different names*

```diff
@@ -82,34 +82,36 @@
           getPatchData: $attrs['get-patch-data'],
           createItemI18nKey: $attrs['create-item-i18n-key'],
           editItemI18nKey: $attrs['edit-item-i18n-key'],
           itemId: $attrs['item-id'],
         }"
         :on="{
           input: (i) => (i ? (createMode = true) : null),
-          loading: (state) => $emit('loading', state),
+          loading: (loading) => handleLoading(loading),
         }"
         :create-mode="createMode"
         :form-field-slot-name="fieldSlot"
         :disabled="createMode || loading || lock"
       >
         <dialog-object-form
           v-model="createMode"
           :affected-query="lastQuery"
           :get-create-data="$attrs['get-create-data']"
+          :get-patch-data="$attrs['get-patch-data']"
           :default-item="defaultItem"
           :gql-create-mutation="$attrs['gql-create-mutation']"
           :edit-item="editItem"
           :gql-patch-mutation="$attrs['gql-patch-mutation']"
           :is-create="isCreate"
           :fields="editableHeaders"
           :create-item-i18n-key="$attrs['create-item-i18n-key']"
           :edited-item-i18n-key="$attrs['edit-item-i18n-key']"
           :item-id="$attrs['item-id']"
-          @loading="$emit('loading', $event)"
+          :force-model-item-update="!isCreate"
+          @loading="handleLoading($event)"
         >
           <template #activator="{ props }">
             <create-button
               v-show="showCreate"
               color="secondary"
               @click="handleCreate"
               :disabled="createMode || loading || lock"
@@ -142,29 +144,29 @@
           itemId: $attrs['item-id'],
           itemAttribute: $attrs['item-attribute'],
           deleteSuccessMessageI18nKey:
             $attrs['delete-success-message-i18n-key'],
         }"
         :on="{
           input: (i) => (i ? (createMode = true) : null),
-          loading: (state) => $emit('loading', state),
+          loading: (loading) => handleLoading(loading),
         }"
         :disabled="deleteMode || loading || lock"
       >
         <delete-dialog
           v-model="deleteMode"
           :affected-query="lastQuery"
           :gql-delete-mutation="$attrs['gql-delete-mutation']"
           :items="itemsToDelete"
           :item-id="$attrs['item-id']"
           :item-attribute="$attrs['item-attribute']"
           :delete-success-message-i18n-key="
             $attrs['delete-success-message-i18n-key']
           "
-          @loading="$emit('loading', $event)"
+          @loading="handleLoading($event)"
         />
       </slot>
       <!-- @slot Insert additional things - actions/buttons - in the table header -->
       <slot name="additionalActions" />
     </v-row>
   </v-toolbar>
 </template>
@@ -339,16 +341,14 @@
       required: false,
       default: true,
     },
   },
   emits: ["search", "selectable", "selection", "deletable", "mode"],
   data() {
     return {
-      // Loading state
-      loading: false,
       // Use create component for creation
       isCreate: true,
       // Toggle for create component
       createMode: false,
       // Used to pass item for editing
       editItem: {},
       // Show delete component
@@ -446,18 +446,14 @@
        */
       this.$emit("mode", this.createMode || this.deleteMode);
     },
   },
   mounted() {
     this.$setToolBarTitle(this.$t(`${this.i18nKey}.title_plural`), null);
 
-    this.$on("loading", (state) => {
-      this.loading = state;
-    });
-
     this.$watch("createMode", this.handleMode);
     this.$watch("deleteMode", this.handleMode);
   },
 };
 </script>
 
 <style>
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/CRUDIterator.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CRUDIterator.vue`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 <template>
   <v-data-iterator
+    v-bind="$attrs"
+    v-on="$listeners"
     :items="items"
     :items-per-page="itemsPerPage"
     :loading="loading"
     :class="elevated ? 'elevation-2' : ''"
     :search="search"
     :sort-by.sync="sortBy"
     :sort-desc.sync="sortDesc"
@@ -65,24 +67,25 @@
     </template>
   </v-data-iterator>
 </template>
 
 <script>
 import CRUDBar from "./CRUDBar.vue";
 
+import loadingMixin from "../../mixins/loadingMixin.js";
 import syncSortMixin from "../../mixins/syncSortMixin.js";
 
 // TODO: props, data & methods are a subset of CRUDList's -> share?
 
 export default {
   name: "CRUDIterator",
   components: {
     CRUDBar,
   },
-  mixins: [syncSortMixin],
+  mixins: [loadingMixin, syncSortMixin],
   props: {
     /**
      * Elevate the iterator?
      * @values true, false
      */
     elevated: {
       type: Boolean,
@@ -95,20 +98,18 @@
      */
     itemsPerPage: {
       type: Number,
       required: false,
       default: 15,
     },
   },
-  emits: ["mode", "lastQuery", "deletable", "loading", "items", "selection"],
+  emits: ["mode", "lastQuery", "deletable", "items", "selection"],
   data() {
     return {
       items: [],
-      // Loading state
-      loading: false,
       // Search
       search: "",
       // Item selection
       showSelect: false,
       selection: [],
       allSelected: false,
     };
@@ -117,19 +118,14 @@
     computedHeaders() {
       return "headers" in this.$attrs
         ? this.$attrs.headers.filter((header) => !header.disableEdit)
         : [];
     },
   },
   methods: {
-    handleLoading(state) {
-      this.loading = state;
-      // Pass on; documented in query/mutateMixin.
-      this.$emit("loading", state);
-    },
     handleItems(items) {
       this.items = items;
       // Pass on; documented in queryMixin.
       this.$emit("items", items);
     },
     handleSelection(selection) {
       this.selection = selection;
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/CRUDList.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CRUDList.vue`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,17 @@
             :item="item"
             :is-create="isCreate"
           />
         </template>
         <template #additionalActions="{ attrs, on }">
           <slot name="additionalActions" :attrs="attrs" :on="on" />
         </template>
+        <template #createComponent="createComponentProps">
+          <slot name="createComponent" v-bind="createComponentProps" />
+        </template>
       </c-r-u-d-bar>
     </template>
 
     <!-- Row template -->
     <template
       v-for="(header, idx) in $attrs.headers"
       #[rowSlot(header)]="{ item }"
@@ -69,15 +72,15 @@
 
     <!-- Add a action (= btn) column -->
     <!-- eslint-disable-next-line vue/valid-v-slot -->
     <template #item.actions="{ item }">
       <!-- @slot Add additional action to action column -->
       <slot name="actions" :item="item" />
       <edit-button
-        v-if="$attrs['enable-edit']"
+        v-if="$attrs['enable-edit'] && 'canEdit' in item && item.canEdit"
         icon
         color="secondary"
         @click="$refs.bar.handleEdit(item)"
         :disabled="mode || loading || $attrs.lock"
       />
       <delete-button
         v-if="showDelete && 'canDelete' in item && item.canDelete"
@@ -108,24 +111,25 @@
 </template>
 
 <script>
 import CRUDBar from "./CRUDBar.vue";
 import EditButton from "./buttons/EditButton.vue";
 import DeleteButton from "./buttons/DeleteButton.vue";
 
+import loadingMixin from "../../mixins/loadingMixin.js";
 import syncSortMixin from "../../mixins/syncSortMixin.js";
 
 export default {
   name: "CRUDList",
   components: {
     CRUDBar,
     EditButton,
     DeleteButton,
   },
-  mixins: [syncSortMixin],
+  mixins: [loadingMixin, syncSortMixin],
   props: {
     /**
      * Elevate the table?
      * @values true, false
      */
     elevated: {
       type: Boolean,
@@ -165,21 +169,19 @@
      */
     showExpand: {
       type: Boolean,
       required: false,
       default: false,
     },
   },
-  emits: ["lastQuery", "mode", "loading", "items"],
+  emits: ["lastQuery", "mode", "items"],
   data() {
     return {
       // Items shown in List = items with added selectable key
       items: [],
-      // Loading state
-      loading: false,
       // Search
       search: "",
       // Item selection
       selectable: false,
       selection: [],
       allSelected: false,
       // Delete
@@ -211,19 +213,14 @@
   },
   methods: {
     handleMode(mode) {
       this.mode = mode;
       // Pass on; documented in CRUDBar.
       this.$emit("mode", mode);
     },
-    handleLoading(state) {
-      this.loading = state;
-      // Pass on; documented in query/mutateMixin.
-      this.$emit("loading", state);
-    },
     handleItems(items) {
       this.items = items;
       // Pass on; documented in queryMixin.
       this.$emit("items", items);
     },
     // Item selection
     handleItemSelected({ item, value }) {
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/CopyToClipboardButton.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CopyToClipboardButton.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/DetailView.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/DetailView.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/FilterBar.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/FilterBar.vue`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       class="my-1 button-40"
       :num-filters="numFilters"
       @click="filterDialog = true"
       @clear="updateFilters({})"
     />
     <filter-dialog
       v-model="filterDialog"
-      :filters="filters"
+      :filters="value"
       @filters="updateFilters"
     >
       <template #filters="{ attrs, on }">
         <slot name="filters" :attrs="attrs" :on="on" />
       </template>
     </filter-dialog>
   </div>
@@ -42,23 +42,23 @@
   props: {
     /**
      * Active filters
      * Use this to supply initial filters and receive updated filters
      * (via v-model)
      * @model
      */
-    filters: {
+    value: {
       type: Object,
       required: false,
       default: () => ({}),
     },
   },
   data() {
     return {
-      numFilters: Object.keys(this.filters).length,
+      numFilters: Object.keys(this.value).length,
       filterDialog: false,
     };
   },
   methods: {
     updateFilters(filters) {
       this.numFilters = Object.keys(filters).length;
       this.$emit("input", filters);
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/InlineCRUDList.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/InlineCRUDList.vue`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       :show-create="isCreate"
       :enable-edit="false"
       :show-select="isCreate"
       :show-action-column="isCreate"
       :lock="!isCreate"
       @lastQuery="affectedQuery = $event"
       @mode="handleMode"
-      @loading="$emit('loading', $event)"
+      @loading="handleLoading($event)"
       @items="$emit('items', $event)"
     >
       <template #filters="{ attrs, on }">
         <slot name="filters" :attrs="attrs" :on="on" />
       </template>
 
       <template
@@ -127,16 +127,14 @@
     CancelButton,
     SaveButton,
   },
   mixins: [createOrPatchMixin],
   data() {
     return {
       valid: false,
-      // Loading state
-      loading: false,
       // Modal state
       mode: false,
       // Store inline edits
       inlineEdits: {},
     };
   },
   methods: {
@@ -172,17 +170,14 @@
     },
     // Template names
     fieldSlot(header) {
       return header.value + ".field";
     },
   },
   mounted() {
-    this.$on("loading", (state) => {
-      this.loading = state;
-    });
     this.$on("save", (_data) => {
       if (this.inlineEdits) {
         this.cancelInlineEdit();
       }
     });
   },
 };
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/ObjectOverview.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ObjectOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/UpdateIndicator.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/UpdateIndicator.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/buttons/BaseButton.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/BaseButton.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/buttons/FilterButton.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/FilterButton.vue`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <template>
   <secondary-action-button
     v-bind="$attrs"
     v-on="$listeners"
     :i18n-key="i18nKey"
   >
-    <v-icon v-if="icon" left>{{ icon }}</v-icon>
+    <v-icon v-if="filterIcon" left>{{ filterIcon }}</v-icon>
     <v-badge color="secondary" :value="numFilters" :content="numFilters" inline>
       <span v-t="i18nKey" />
     </v-badge>
     <v-btn
       icon
       @click.stop="$emit('clear')"
       small
@@ -24,15 +24,15 @@
 import SecondaryActionButton from "./SecondaryActionButton.vue";
 
 export default {
   name: "FilterButton",
   components: { SecondaryActionButton },
   extends: SecondaryActionButton,
   computed: {
-    icon() {
+    filterIcon() {
       return this.hasFilters || this.numFilters > 0
         ? "$filterSet"
         : "$filterEmpty";
     },
   },
   props: {
     i18nKey: {
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/dialogs/ConfirmDialog.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/ConfirmDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
       </slot>
     </template>
     <template #content>
       <!-- @slot Delete dialog body slot -->
       <slot name="body">
         <ul class="text-body-1">
           <li v-for="(item, idx) in items" :key="idx">
-            {{ nameOfItem(item) }}
+            {{ getNameOfItem(item) }}
           </li>
         </ul>
       </slot>
     </template>
     <template #actions>
       <cancel-button @click="handleCancel" :disabled="loading">
         <!-- @slot Delete dialog cancel button slot -->
@@ -65,22 +65,34 @@
      */
     items: {
       type: Array,
       required: false,
       default: () => [],
     },
     /**
-     * The item's name property displayed in confirm delete dialog.
+     * The item's name property displayed (per default) in confirm delete dialog.
      */
     itemAttribute: {
       type: String,
       required: false,
       default: "name",
     },
     /**
+     * Method to get the text displayed per item in confirm delete dialog.
+     */
+    getNameOfItem: {
+      type: Function,
+      required: false,
+      default: function (item) {
+        return this.itemAttribute in item || {}
+          ? item[this.itemAttribute]
+          : item.toString();
+      },
+    },
+    /**
      * Message shown after successful delete.
      */
     deleteSuccessMessageI18nKey: {
       type: String,
       required: false,
       default: "status.object_delete_success",
     },
@@ -97,42 +109,28 @@
     },
     confirmI18nKey() {
       return this.items.length > 1
         ? "actions.confirm_deletion_multiple"
         : "actions.confirm_deletion";
     },
   },
-  data() {
-    return {
-      // Loading state
-      loading: false,
-    };
-  },
   methods: {
-    nameOfItem(item) {
-      return this.itemAttribute in item || {}
-        ? item[this.itemAttribute]
-        : item.toString();
-    },
     handleDelete() {
       this.delete(this.items);
       this.dialog = false;
     },
     handleCancel() {
       this.dialog = false;
       /**
        * Emitted when user cancels
        */
       this.$emit("cancel");
     },
   },
   mounted() {
-    this.$on("loading", (status) => {
-      this.loading = status;
-    });
     this.$on("save", () => {
       this.dialog = false;
       this.$toastSuccess(this.deleteSuccessMessageI18nKey);
     });
   },
 };
 </script>
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/dialogs/DialogObjectForm.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/DialogObjectForm.vue`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,14 @@
     /**
      * Also inherited props from createOrPatchMixin
      */
   },
   emits: ["cancel"],
   data() {
     return {
-      loading: false,
       valid: false,
       firstInitDone: false,
       itemModel: {},
     };
   },
   computed: {
     dialog: {
@@ -222,17 +221,14 @@
       // Only update the model if the dialog is hidden or has just been mounted
       if (this.forceModelItemUpdate || !this.firstInitDone || !this.dialog) {
         this.resetModel();
       }
     },
   },
   mounted() {
-    this.$on("loading", (status) => {
-      this.loading = status;
-    });
     this.$on("save", this.handleSuccess);
 
     this.updateModel();
     this.firstInitDone = true;
 
     this.$watch("isCreate", this.updateModel);
     this.$watch("defaultItem", this.updateModel, { deep: true });
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/dialogs/FilterDialog.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/FilterDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/dialogs/MobileFullscreenDialog.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/MobileFullscreenDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/ColorField.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/ColorField.vue`

 * *Files 14% similar despite different names*

```diff
@@ -10,29 +10,32 @@
   >
     <template #activator="{ on, attrs }">
       <v-text-field
         v-model="color"
         v-bind="$attrs"
         v-on="$listeners"
         placeholder="#AABBCC"
-        :rules="mergedRules"
+        :rules="$rules().isHexColor(allowAlpha).build(rules)"
       >
         <template #prepend-inner>
           <v-icon :color="color" v-bind="attrs" v-on="on"> mdi-circle </v-icon>
         </template>
       </v-text-field>
     </template>
     <v-color-picker v-if="menu" v-model="color" ref="picker"></v-color-picker>
   </v-menu>
 </template>
 
 <script>
+import formRulesMixin from "../../../mixins/formRulesMixin";
+
 export default {
-  name: "DateField",
+  name: "ColorField",
   extends: "v-text-field",
+  mixins: [formRulesMixin],
   data() {
     return {
       menu: false,
     };
   },
   props: {
     value: {
@@ -40,30 +43,27 @@
       default: undefined,
     },
     rules: {
       type: Array,
       required: false,
       default: () => [],
     },
+    allowAlpha: {
+      type: Boolean,
+      required: false,
+      default: true,
+    },
   },
   computed: {
     color: {
       get() {
         return this.value;
       },
       set(newValue) {
         this.$emit("input", newValue);
       },
     },
-    mergedRules() {
-      return [
-        (value) =>
-          /^(#([0-9a-f]{3,4}|[0-9a-f]{6}|[0-9a-f]{8}))?$/i.test(value) ||
-          this.$t("forms.errors.invalid_color"),
-        ...this.rules,
-      ];
-    },
   },
 };
 </script>
 
 <style scoped></style>
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/DateField.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/DateField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/DateTimeField.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/DateTimeField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/ForeignKeyField.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/ForeignKeyField.vue`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     class="fc-my-auto"
   >
     <template #item="item">
       <slot name="item" v-bind="item">
         {{ item.item[itemName] }}
       </slot>
     </template>
-    <template #append-outer>
+    <template #append-outer v-if="enableCreate">
       <v-btn icon @click="createMode = true">
         <v-icon>$plus</v-icon>
       </v-btn>
 
       <slot
         name="createComponent"
         :attrs="{
@@ -103,14 +103,19 @@
   },
   props: {
     itemName: {
       type: [String, Function],
       required: false,
       default: "name",
     },
+    enableCreate: {
+      type: Boolean,
+      required: false,
+      default: true,
+    },
   },
 };
 </script>
 
 <style scoped>
 .fc-my-auto > :first-child {
   margin-block: auto;
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/PositiveSmallIntegerField.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/PositiveSmallIntegerField.vue`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 <template>
   <v-text-field
     v-bind="$attrs"
     v-on="on"
-    :rules="mergedRules"
+    :rules="
+      $rules()
+        .isANumber.isAWholeNumber.isGreaterThan(0)
+        .isSmallerThan(32767)
+        .build(rules)
+    "
     type="number"
     inputmode="decimal"
   ></v-text-field>
 </template>
 
 <script>
+import formRulesMixin from "../../../mixins/formRulesMixin";
+
 export default {
   name: "PositiveSmallIntegerField",
   extends: "v-text-field",
+  mixins: [formRulesMixin],
   props: {
     rules: {
       type: Array,
       required: false,
       default: () => [],
     },
   },
@@ -23,35 +31,14 @@
     on() {
       return {
         ...this.$listeners,
         input: this.inputHandler("input"),
         change: this.inputHandler("change"),
       };
     },
-    mergedRules() {
-      return [
-        (value) =>
-          !value ||
-          !isNaN(parseInt(value)) ||
-          this.$t("forms.errors.not_a_number"),
-        (value) =>
-          !value ||
-          value % 1 === 0 ||
-          this.$t("forms.errors.not_a_whole_number"),
-        (value) =>
-          !value ||
-          parseInt(value) >= 0 ||
-          this.$t("forms.errors.number_too_small"),
-        (value) =>
-          !value ||
-          parseInt(value) <= 32767 ||
-          this.$t("forms.errors.number_too_big"),
-        ...this.rules,
-      ];
-    },
   },
   methods: {
     inputHandler(name) {
       return (event) => {
         const num = parseInt(event);
         if (!isNaN(num) && num >= 0 && num <= 32767 && num % 1 === 0) {
           this.$emit(name, num);
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/RecurrenceField.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/RecurrenceField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/TimeField.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/TimeField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/generic/forms/WeekDayField.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/WeekDayField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/group/GroupCollection.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/group/GroupCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/holiday/HolidayInlineList.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/holiday/HolidayInlineList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/holiday/holiday.graphql` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/holiday/holiday.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/notifications/NotificationItem.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/notifications/NotificationItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/notifications/NotificationList.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/notifications/NotificationList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/pdf/DownloadPDF.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/pdf/DownloadPDF.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/AdditionalImage.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/AdditionalImage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/AvatarContent.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/AvatarContent.vue`

 * *Files 19% similar despite different names*

```diff
@@ -5,23 +5,23 @@
         <v-progress-circular
           indeterminate
           color="grey lighten-5"
         ></v-progress-circular>
       </v-row>
     </template>
     <v-img
-      v-if="person && person.image"
-      :src="person.image"
+      v-if="person?.image || imageUrl"
+      :src="person?.image || imageUrl"
       :alt="$t('person.avatar')"
       max-width="100%"
       max-height="100%"
       :contain="contain"
       class="fullsize"
     />
-    <v-icon class="grey lighten-1" dark v-else>mdi-folder</v-icon>
+    <v-icon class="grey lighten-1" dark v-else>mdi-image-off-outline</v-icon>
   </div>
 </template>
 
 <script>
 import gqlAvatarContent from "./avatarContent.graphql";
 export default {
   name: "AvatarContent",
@@ -32,22 +32,30 @@
       default: "",
     },
     contain: {
       type: Boolean,
       required: false,
       default: false,
     },
+    imageUrl: {
+      type: String,
+      required: false,
+      default: null,
+    },
   },
   apollo: {
     person: {
       query: gqlAvatarContent,
       variables() {
         return {
           id: this.id,
         };
       },
+      skip() {
+        return !!this.imageUrl;
+      },
     },
   },
 };
 </script>
 
 <style scoped></style>
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/PersonActions.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonActions.vue`

 * *Files 10% similar despite different names*

```diff
@@ -78,56 +78,58 @@
             <v-list-item-title>
               {{ $t("person.delete") }}
             </v-list-item-title>
           </v-list-item-content>
         </v-list-item>
       </button-menu>
     </template>
-    <confirm-dialog
+    <delete-dialog
       v-model="showDeleteConfirm"
+      :gql-delete-mutation="deleteMutation"
+      item-attribute="fullName"
+      :items="[person]"
       @confirm="
         $router.push({
-          name: 'core.deletePerson',
-          params: { id: person.id },
+          name: 'core.persons',
         })
       "
-      @cancel="showDeleteConfirm = false"
     >
       <template #title>
         {{ $t("person.confirm_delete") }}
       </template>
-    </confirm-dialog>
+    </delete-dialog>
   </div>
 </template>
 
 <script>
-import gqlPersonActions from "./personActions.graphql";
-import ConfirmDialog from "../generic/dialogs/ConfirmDialog.vue";
+import { actions, deletePersons } from "./personActions.graphql";
+import DeleteDialog from "../generic/dialogs/DeleteDialog.vue";
 
 export default {
   name: "PersonActions",
-  components: { ConfirmDialog },
+  components: { DeleteDialog },
   props: {
     id: {
       type: String,
       required: true,
     },
   },
   apollo: {
     person: {
-      query: gqlPersonActions,
+      query: actions,
       variables() {
         return {
           id: this.id,
         };
       },
     },
   },
   data() {
     return {
       showDeleteConfirm: false,
+      deleteMutation: deletePersons,
     };
   },
 };
 </script>
 
 <style scoped></style>
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/PersonCollection.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/PersonOverview.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonOverview.vue`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,31 @@
         </template>
 
         <template #title>
           {{ person.firstName }} {{ person.lastName }}
         </template>
 
         <template #subtitle>
-          {{ person.username }}
+          <span v-if="person.shortName">
+            <v-tooltip bottom>
+              <template v-slot:activator="{ on, attrs }">
+                <span v-bind="attrs" v-on="on">{{ person.shortName }}</span>
+              </template>
+              <span>{{ $t("person.short_name") }}</span>
+            </v-tooltip>
+          </span>
+          <span v-if="person.shortName && person.username"> · </span>
+          <span v-if="person.username">
+            <v-tooltip bottom>
+              <template v-slot:activator="{ on, attrs }">
+                <span v-bind="attrs" v-on="on">{{ person.username }}</span>
+              </template>
+              <span>{{ $t("person.username") }}</span>
+            </v-tooltip>
+          </span>
         </template>
 
         <template #actions="{ classes }">
           <person-actions :class="classes" :id="person.id" />
         </template>
 
         <div class="text-center my-5" v-text="person.description"></div>
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/person/personOverview.graphql` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/personOverview.graphql`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
   object: personByIdOrMe(id: $id) {
     id
     username
     firstName
     additionalName
     lastName
     fullName
+    shortName
 
     description
 
     sex
     street
     housenumber
     postalCode
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/room/RoomInlineList.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/room/RoomInlineList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/room/room.graphql` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/room/room.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/school_term/SchoolTermField.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/school_term/SchoolTermField.vue`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 <script>
 import ForeignKeyField from "../generic/forms/ForeignKeyField.vue";
 import { createSchoolTerms, schoolTerms } from "./schoolTerm.graphql";
 
 export default {
   name: "SchoolTermField",
   components: { ForeignKeyField },
+  extends: [ForeignKeyField],
   data() {
     return {
       gqlQuery: schoolTerms,
       gqlCreateMutation: createSchoolTerms,
       fields: [
         {
           text: this.$t("school_term.name"),
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/school_term/SchoolTermInlineList.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/school_term/SchoolTermInlineList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/school_term/schoolTerm.graphql` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/school_term/schoolTerm.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/two_factor/TwoFactor.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/TwoFactor.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/index.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -74,14 +74,15 @@
         offline: false,
         backgroundActive: true,
         invalidation: false,
         snackbarItems: [],
         toolbarTitle: "AlekSIS®",
         permissions: [],
         permissionNames: [],
+        frequentCeleryPolling: false,
     }),
     computed: {
         matchedComponents() {
             if (this.$route.matched.length > 0) {
                 return this.$route.matched.map(
                     (route) => route.components.default.name,
                 );
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/messages/de.json` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/de.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'group'": "{'group_type': {'create': 'Gruppentyp erstellen', 'name': 'Name', 'description': "*

 * *            "'Beschreibung'}}",*

 * * "'person'": "{'sex': {'field': 'Geschlecht'}, 'first_name': 'Vorname', 'last_name': 'Nachname', "*

 * *             "'short_name': 'Kürzel', 'name': 'Name'}",*

 * * "'personal_events'": "{'date_start': 'Start', 'date_end': 'Ende', 'is_full_day': 'Ganztägig', "*

 * *                      "'is_recurring': 'Wiederkehrend', 'is_not_recurring': 'Einmalig'}"}*

```diff
@@ -197,15 +197,18 @@
     },
     "graphql": {
         "snackbar_error_message": "Beim Abrufen der Seitendaten ist ein Fehler aufgetreten. Bitte versuchen Sie es erneut.",
         "snackbar_success_message": "Der Vorgang wurde erfolgreich beendet."
     },
     "group": {
         "group_type": {
+            "create": "Gruppentyp erstellen",
+            "description": "Beschreibung",
             "menu_title": "Gruppentypen",
+            "name": "Name",
             "title": "Gruppentyp",
             "title_plural": "Gruppentypen"
         },
         "groups_and_child_groups": "Gruppen und Kindgruppen",
         "menu_title": "Gruppen",
         "ownership": "Gruppen-Eigent\u00fcmerschaft",
         "title": "Gruppe",
@@ -270,44 +273,54 @@
         "account_menu_title": "Konto",
         "additional_image": "Weiteres Bild",
         "avatar": "Avatar",
         "children": "Kinder",
         "confirm_delete": "Wollen Sie wirklich diese Person l\u00f6schen?",
         "delete": "L\u00f6schen",
         "details": "Kontaktdaten",
+        "first_name": "Vorname",
         "guardians": "Erziehungsberechtigte / Eltern",
         "home": "Festnetz",
         "impersonation": {
             "impersonate": "Verkleiden",
             "impersonating": "Verkleidet als",
             "stop": "Verkleidung beenden"
         },
         "invite": "Einladen",
+        "last_name": "Nachname",
         "logged_in_as": "Angemeldet als",
         "menu_title": "Personen",
         "mobile": "Handy",
+        "name": "Name",
         "no_additional_image": "Diese Person hat kein weiteres Bild hochgeladen",
         "no_persons": "Keine Personen",
         "page_title": "Person",
         "sex": {
             "f": "Weiblich",
+            "field": "Geschlecht",
             "m": "M\u00e4nnlich",
             "x": "Divers"
         },
+        "short_name": "K\u00fcrzel",
         "title": "Person",
         "title_plural": "Personen"
     },
     "personal_events": {
         "create_button": "Termin erstellen",
         "create_title": "Pers\u00f6nlichen Termin erstellen",
+        "date_end": "Ende",
+        "date_start": "Start",
         "datetime_end": "Ende",
         "datetime_start": "Start",
         "description": "Beschreibung",
         "edit_title": "Pers\u00f6nlichen Termin bearbeiten",
         "groups": "Teilnehmende Gruppen",
+        "is_full_day": "Ganzt\u00e4gig",
+        "is_not_recurring": "Einmalig",
+        "is_recurring": "Wiederkehrend",
         "location": "Ort",
         "persons": "Teilnehmende Personen",
         "title": "Titel"
     },
     "preferences": {
         "person": {
             "change_preferences": "Einstellungen",
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/messages/en.json` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/en.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891941391941393%*

 * *Differences: {"'group'": "{'group_type': {'create': 'Create Group Type', 'name': 'Name', 'description': "*

 * *            "'Description'}}",*

 * * "'person'": "{'sex': {'field': 'Sex'}, 'first_name': 'First Name', 'last_name': 'Last Name', "*

 * *             "'short_name': 'Short Name', 'name': 'Name', 'username': 'Username', 'primary_group': "*

 * *             "'Primary Group'}",*

 * * "'personal_events'": "{'date_start': 'Start', 'date_end': 'End', 'is_full_day': 'Full day event', "*

 * *                      "'is_recurring': 'Recurring', 'is_n […]*

```diff
@@ -197,15 +197,18 @@
     },
     "graphql": {
         "snackbar_error_message": "There was an error retrieving the page data. Please try again.",
         "snackbar_success_message": "The operation has been finished successfully."
     },
     "group": {
         "group_type": {
+            "create": "Create Group Type",
+            "description": "Description",
             "menu_title": "Group Types",
+            "name": "Name",
             "title": "Group Type",
             "title_plural": "Group Types"
         },
         "groups_and_child_groups": "Groups and Child Groups",
         "menu_title": "Groups",
         "ownership": "Group ownership",
         "title": "Group",
@@ -270,44 +273,56 @@
         "account_menu_title": "Account",
         "additional_image": "Additional Image",
         "avatar": "Avatar",
         "children": "Children",
         "confirm_delete": "Do you really want to delete this person?",
         "delete": "Delete",
         "details": "Contact details",
+        "first_name": "First Name",
         "guardians": "Guardians / Parents",
         "home": "home phone",
         "impersonation": {
             "impersonate": "Impersonate",
             "impersonating": "Impersonating",
             "stop": "Stop Impersonation"
         },
         "invite": "Invite",
+        "last_name": "Last Name",
         "logged_in_as": "Logged in as",
         "menu_title": "Persons",
         "mobile": "mobile phone",
+        "name": "Name",
         "no_additional_image": "The person didn't upload an additional Image",
         "no_persons": "No Persons",
         "page_title": "Person",
+        "primary_group": "Primary Group",
         "sex": {
             "f": "Female",
+            "field": "Sex",
             "m": "Male",
             "x": "Other"
         },
+        "short_name": "Short Name",
         "title": "Person",
-        "title_plural": "Persons"
+        "title_plural": "Persons",
+        "username": "Username"
     },
     "personal_events": {
         "create_button": "Create event",
         "create_title": "Create personal event",
+        "date_end": "End",
+        "date_start": "Start",
         "datetime_end": "End",
         "datetime_start": "Start",
         "description": "Description",
         "edit_title": "Edit personal event",
         "groups": "Participating groups",
+        "is_full_day": "Full day event",
+        "is_not_recurring": "One-time",
+        "is_recurring": "Recurring",
         "location": "Location",
         "persons": "Participating people",
         "recurrences": "Repeat",
         "title": "Title"
     },
     "preferences": {
         "person": {
@@ -345,14 +360,15 @@
         "update": "Update"
     },
     "status": {
         "changes": "You have unsaved changes.",
         "error": "There has been an error while saving the latest changes.",
         "object_create_success": "The object was created successfully.",
         "object_delete_success": "The object was deleted successfully.",
+        "object_edit_success": "The object was updated successfully.",
         "objects_delete_success": "The objects were deleted successfully."
     },
     "weekdays": {
         "A_0": "Monday",
         "A_1": "Tuesday",
         "A_2": "Wednesday",
         "A_3": "Thursday",
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/messages/ru.json` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/ru.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/messages/uk.json` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/uk.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/aleksis.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/calendarFeedDetails.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/calendarFeedDetails.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/createOrPatchMixin.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/createOrPatchMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/deleteMixin.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/deleteMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/error404.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/error404.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/menus.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/menus.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/mutateMixin.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/mutateMixin.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,14 @@
+import loadingMixin from "./loadingMixin.js";
+
 /**
  * This mixin provides generic graphQL mutation handling.
  */
 export default {
+    mixins: [loadingMixin],
     props: {
         /**
          * The graphQL query this mutation affects.
          * If provided the cached query will be updated.
          * Either use lastQuery from the queryMixin or
          * $apollo.queries[lastQueryName].
          */
@@ -24,15 +27,15 @@
             required: false,
             default: "id",
         },
     },
     // update & save come from DialogObjectForm
     // save could be success as well but keeping it backwards compatible
     // for now
-    emits: ["loading", "update", "save"],
+    emits: ["update", "save"],
     computed: {
         // Expand the affectedQuery
         expandedQuery() {
             if (!this.affectedQuery) {
                 return false;
             }
             return {
@@ -49,21 +52,15 @@
          * the incoming data.
          *
          * @param {Object} mutation
          * @param {Object} variables
          * @param {Function} updateStore
          */
         mutate(mutation, variables, updateStore = (cached, incoming) => {}) {
-            /**
-             * Emitted when the graphQL mutation starts or finishes loading
-             *
-             * @property {boolean} status shows whether loading or not
-             */
-            this.$emit("loading", true);
-
+            this.handleLoading(true);
             this.$apollo
                 .mutate({
                     mutation: mutation,
                     variables: variables,
                     update: (store, data) => {
                         // TODO: Is data transformed properly?
                         // Current implemented for create | patch
@@ -108,12 +105,12 @@
                      */
                     this.$emit("save", data);
                 })
                 .catch((error) => {
                     this.handleError(error);
                 })
                 .finally(() => {
-                    this.$emit("loading", false);
+                    this.handleLoading(false);
                 });
         },
     },
 };
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/offline.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/offline.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/permissions.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/permissions.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/queryMixin.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/queryMixin.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,15 @@
+import loadingMixin from "./loadingMixin.js";
+
 /**
  * This mixin provides generic item query via graphQL.
  * The query result is available in items.
  */
 export default {
+    mixins: [loadingMixin],
     props: {
         /**
          * The graphQL query
          */
         gqlQuery: {
             type: Object,
             required: true,
@@ -41,59 +44,73 @@
          */
         getGqlData: {
             type: Function,
             required: false,
             default: (item) => item,
         },
     },
-    emits: ["loading", "items", "lastQuery"],
+    emits: ["items", "lastQuery"],
     data() {
         return {
-            additionalFilters: {},
+            internalAdditionalFilters: {},
+            filterString: "{}",
             lastQuery: {},
         };
     },
+    computed: {
+        additionalFilters: {
+            get() {
+                return this.internalAdditionalFilters;
+            },
+            set(filters) {
+                this.internalAdditionalFilters = filters;
+                this.updateFilterString();
+            },
+        },
+    },
+    watch: {
+        gqlFilters: {
+            handler() {
+                this.updateFilterString();
+            },
+            deep: true,
+        },
+    },
     methods: {
         handleItems(items) {
             return items;
         },
+        updateFilterString() {
+            this.filterString = JSON.stringify({
+                ...this.gqlFilters,
+                ...this.internalAdditionalFilters,
+            });
+        },
     },
     apollo: {
         items() {
             return {
                 query: this.gqlQuery,
                 variables() {
                     const orderBy = this.gqlOrderBy.length ?
                         {
                             orderBy: this.gqlOrderBy
                         } :
                         {};
-                    const filters =
-                        Object.keys(this.gqlFilters).length ||
-                        Object.keys(this.additionalFilters).length ?
-                        {
-                            filters: JSON.stringify({
-                                ...this.gqlFilters,
-                                ...this.additionalFilters,
-                            }),
-                        } :
-                        {};
+                    const filters = {
+                        filters: this.filterString,
+                    };
                     return {
                         ...this.gqlAdditionalQueryArgs,
                         ...orderBy,
                         ...filters,
                     };
                 },
                 watchLoading(loading) {
-                    /**
-                     * Emitted when graphQL query starts or finishes loading
-                     *
-                     * @property {boolean} status shows whether loading or not
-                     */
-                    this.$emit("loading", loading);
+                    this.handleLoading(loading);
                 },
                 error: (error) => {
                     this.handleError(error);
                 },
                 update: (data) => {
                     this.lastQuery = this.$apollo.queries.items;
                     /**
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/routes.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/syncSortMixin.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/syncSortMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/mixins/useRegisterSW.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/useRegisterSW.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/plugins/aleksis.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/plugins/aleksis.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -236,12 +236,24 @@
     Vue.prototype.$d = function(value, ...args) {
         if (typeof value === DateTime) {
             value = value.toJSDate();
         }
         return this.$i18n.d(value, ...args);
     };
 
+    /**
+     * Activate frequent polling for celery task progress.
+     *
+     * This can be used to notify the frontend about a currently running task that
+     * should be monitored more closely.
+     *
+     */
+    Vue.prototype.$activateFrequentCeleryPolling = function() {
+        console.debug("Activate frequent polling for Celery tasks");
+        this.$root.frequentCeleryPolling = true;
+    };
+
     // Add default behaviour for all components
     Vue.mixin(aleksisMixin);
 };
 
 export default AleksisVue;
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/frontend/routes.js` & `aleksis_core-4.0.0.dev6/aleksis/core/frontend/routes.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -83,183 +83,146 @@
             inMenu: true,
             titleKey: "people",
             icon: "mdi-account-group-outline",
             iconActive: "mdi-account-group",
             permission: "core.view_people_menu_rule",
         },
         children: [{
-                path: "/persons",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.persons",
-                meta: {
-                    inMenu: true,
-                    titleKey: "person.menu_title",
-                    icon: "mdi-account-outline",
-                    iconActive: "mdi-account",
-                    permission: "core.view_persons_rule",
-                },
-            }, {
-                path: "/persons/create/",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.createPerson",
-            }, {
-                path: "/persons/:id(\\d+)/",
-                component: () => import("./components/person/PersonOverview.vue"),
-                name: "core.personById",
-                props: true,
-                meta: {
-                    titleKey: "person.page_title",
-                },
-            }, {
-                path: "/persons/:id(\\d+)/edit/",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.editPerson",
-            }, {
-                path: "/persons/:id(\\d+)/delete/",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.deletePerson",
-            }, {
-                path: "/persons/:id(\\d+)/invite/",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.invitePerson",
-            }, {
-                path: "/groups",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.groups",
-                meta: {
-                    inMenu: true,
-                    titleKey: "group.menu_title",
-                    icon: "mdi-account-multiple-outline",
-                    iconActive: "mdi-account-multiple",
-                    permission: "core.view_groups_rule",
-                },
-            }, {
-                path: "/groups/create",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.createGroup",
-            }, {
-                path: "/groups/:id(\\d+)",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.group",
-            }, {
-                path: "/groups/:id(\\d+)/edit",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.editGroup",
-            }, {
-                path: "/groups/:id(\\d+)/delete",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.deleteGroup",
-            }, {
-                path: "/groups/group_types",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.groupTypes",
-                meta: {
-                    inMenu: true,
-                    titleKey: "group.group_type.menu_title",
-                    icon: "mdi-shape-outline",
-                    iconActive: "mdi-shape",
-                    permission: "core.view_grouptypes_rule",
-                },
-            }, {
-                path: "/groups/group_types/create",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.createGroupType",
-            }, {
-                path: "/groups/group_types/:id(\\d+)/delete",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.deleteGroupType,",
-            }, {
-                path: "/groups/group_types/:id(\\d+)/edit",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.editGroupType",
-            },
-
-            {
-                path: "/groups/child_groups/",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.groupsChildGroups",
-                meta: {
-                    inMenu: true,
-                    titleKey: "group.groups_and_child_groups",
-                    icon: "mdi-account-multiple-plus-outline",
-                    iconActive: "mdi-account-multiple-plus",
-                    permission: "core.assign_child_groups_to_groups_rule",
-                },
-            }, {
-                path: "/invitations/send-invite",
-                component: () => import("./components/LegacyBaseTemplate.vue"),
-                props: {
-                    byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-                },
-                name: "core.invite_person",
-                meta: {
-                    inMenu: true,
-                    titleKey: "accounts.invitation.invite_person.menu_title",
-                    icon: "mdi-account-plus-outline",
-                    iconActive: "mdi-account-plus",
-                    permission: "core.invite_rule",
-                },
-            }, {
-                path: "/rooms/",
-                component: () => import("./components/room/RoomInlineList.vue"),
-                name: "core.rooms",
-                meta: {
-                    inMenu: true,
-                    titleKey: "rooms.menu_title",
-                    toolbarTitle: "rooms.menu_title",
-                    icon: "mdi-floor-plan",
-                    permission: "core.view_rooms_rule",
-                },
+            path: "/persons",
+            component: () => import("./components/person/PersonList.vue"),
+            name: "core.persons",
+            meta: {
+                inMenu: true,
+                titleKey: "person.menu_title",
+                icon: "mdi-account-outline",
+                iconActive: "mdi-account",
+                permission: "core.view_persons_rule",
             },
-        ],
+        }, {
+            path: "/persons/create/",
+            component: () => import("./components/LegacyBaseTemplate.vue"),
+            props: {
+                byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+            },
+            name: "core.createPerson",
+        }, {
+            path: "/persons/:id(\\d+)/",
+            component: () => import("./components/person/PersonOverview.vue"),
+            name: "core.personById",
+            props: true,
+            meta: {
+                titleKey: "person.page_title",
+            },
+        }, {
+            path: "/persons/:id(\\d+)/edit/",
+            component: () => import("./components/LegacyBaseTemplate.vue"),
+            props: {
+                byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+            },
+            name: "core.editPerson",
+        }, {
+            path: "/persons/:id(\\d+)/invite/",
+            component: () => import("./components/LegacyBaseTemplate.vue"),
+            props: {
+                byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+            },
+            name: "core.invitePerson",
+        }, {
+            path: "/groups",
+            component: () => import("./components/LegacyBaseTemplate.vue"),
+            props: {
+                byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+            },
+            name: "core.groups",
+            meta: {
+                inMenu: true,
+                titleKey: "group.menu_title",
+                icon: "mdi-account-multiple-outline",
+                iconActive: "mdi-account-multiple",
+                permission: "core.view_groups_rule",
+            },
+        }, {
+            path: "/groups/create",
+            component: () => import("./components/LegacyBaseTemplate.vue"),
+            props: {
+                byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+            },
+            name: "core.createGroup",
+        }, {
+            path: "/groups/:id(\\d+)",
+            component: () => import("./components/LegacyBaseTemplate.vue"),
+            props: {
+                byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+            },
+            name: "core.group",
+        }, {
+            path: "/groups/:id(\\d+)/edit",
+            component: () => import("./components/LegacyBaseTemplate.vue"),
+            props: {
+                byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+            },
+            name: "core.editGroup",
+        }, {
+            path: "/groups/:id(\\d+)/delete",
+            component: () => import("./components/LegacyBaseTemplate.vue"),
+            props: {
+                byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+            },
+            name: "core.deleteGroup",
+        }, {
+            path: "/groups/group_types",
+            component: () => import("./components/group_type/GroupType.vue"),
+            name: "core.groupTypes",
+            meta: {
+                inMenu: true,
+                titleKey: "group.group_type.menu_title",
+                icon: "mdi-shape-outline",
+                iconActive: "mdi-shape",
+                permission: "core.view_grouptypes_rule",
+            },
+        }, {
+            path: "/groups/child_groups/",
+            component: () => import("./components/LegacyBaseTemplate.vue"),
+            props: {
+                byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+            },
+            name: "core.groupsChildGroups",
+            meta: {
+                inMenu: true,
+                titleKey: "group.groups_and_child_groups",
+                icon: "mdi-account-multiple-plus-outline",
+                iconActive: "mdi-account-multiple-plus",
+                permission: "core.assign_child_groups_to_groups_rule",
+            },
+        }, {
+            path: "/invitations/send-invite",
+            component: () => import("./components/LegacyBaseTemplate.vue"),
+            props: {
+                byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+            },
+            name: "core.invite_person",
+            meta: {
+                inMenu: true,
+                titleKey: "accounts.invitation.invite_person.menu_title",
+                icon: "mdi-account-plus-outline",
+                iconActive: "mdi-account-plus",
+                permission: "core.invite_rule",
+            },
+        }, {
+            path: "/rooms/",
+            component: () => import("./components/room/RoomInlineList.vue"),
+            name: "core.rooms",
+            meta: {
+                inMenu: true,
+                titleKey: "rooms.menu_title",
+                toolbarTitle: "rooms.menu_title",
+                icon: "mdi-floor-plan",
+                permission: "core.view_rooms_rule",
+            },
+        }, ],
     }, {
         path: "#",
         component: () => import("./components/Parent.vue"),
         name: "core.administration",
         meta: {
             inMenu: true,
             titleKey: "administration.menu_title",
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/health_checks.py` & `aleksis_core-4.0.0.dev6/aleksis/core/health_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/ar/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/fr/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/fr/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/la/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/la/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/la/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/ru/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/ru/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/uk/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/uk/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/management/commands/convert_urls_to_routes.py` & `aleksis_core-4.0.0.dev6/aleksis/core/management/commands/convert_urls_to_routes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/management/commands/vite.py` & `aleksis_core-4.0.0.dev6/aleksis/core/management/commands/vite.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/managers.py` & `aleksis_core-4.0.0.dev6/aleksis/core/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,18 @@
         """Get instances that are not managed by any particular app."""
         return super().get_queryset().filter(managed_by_app_label="")
 
     def managed_by_app(self, app_label: str) -> QuerySet:
         """Get instances managed by a particular app."""
         return super().get_queryset().filter(managed_by_app_label=app_label)
 
+    def managed_and_unmanaged(self) -> QuerySet:
+        """Get managed and unmanaged instances managed."""
+        return super().get_queryset()
+
     def get_queryset(self) -> QuerySet:
         return self.unmanaged()
 
 
 class AlekSISBaseManagerWithoutMigrations(AlekSISBaseManager):
     """AlekSISBaseManager for auto-generating managers just by query sets."""
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0001_initial.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0002_school_term.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0002_school_term.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0003_drop_image_cropping.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0003_drop_image_cropping.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0004_add_permissions_for_group_stats.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0004_add_permissions_for_group_stats.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0005_timestamped_activity_notification.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0005_timestamped_activity_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0006_dashboard_widget_size.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0006_dashboard_widget_size.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0007_dashboard_widget_order.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0007_dashboard_widget_order.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0008_data_check_result.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0008_data_check_result.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0009_default_dashboard.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0009_default_dashboard.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0010_external_link_widget.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0010_external_link_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0011_globalpermissions_options.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0011_globalpermissions_options.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0013_pdf_file.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0013_pdf_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0014_alter_pdffile_file.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0014_alter_pdffile_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0015_oauth_permissions.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0015_oauth_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0016_taskuserassignment.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0016_taskuserassignment.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0018_pdffile_html_file.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0018_pdffile_html_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0019_fix_uniqueness_per_site.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0019_fix_uniqueness_per_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0020_pdf_file_person_optional.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0020_pdf_file_person_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0021_drop_persons_accounts_perm.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0021_drop_persons_accounts_perm.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0022_public_favicon.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0022_public_favicon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0023_oauth_application_model.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0023_oauth_application_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0024_oauth_grant_types_optional.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0024_oauth_grant_types_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0025_oauth_align_user_fk.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0025_oauth_align_user_fk.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0028_char_field_not_null.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0028_char_field_not_null.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0029_invitations.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0029_invitations.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0030_user_attributes.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0030_user_attributes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0031_oauthapplication_icon.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0031_oauthapplication_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0033_update_photo_avatar.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0033_update_photo_avatar.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0034_invite_permission.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0034_invite_permission.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0035_preference_model_unique.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0035_preference_model_unique.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0036_additionalfields_helptext_required.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0036_additionalfields_helptext_required.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0037_add_static_content_widget.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0037_add_static_content_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0038_notification_send_at.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0038_notification_send_at.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0039_personal_ical_url.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0039_personal_ical_url.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0041_update_gender_choices.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0041_update_gender_choices.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0042_pdffile_empty.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0042_pdffile_empty.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0043_task_assignment_meta.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0043_task_assignment_meta.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0044_task_assignment_result_fetched.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0044_task_assignment_result_fetched.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0046_notification_create_field_icon.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0046_notification_create_field_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0047_add_room_model.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0047_add_room_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0048_delete_personalicalurl.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0048_delete_personalicalurl.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0050_managed_by_app_label.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0050_managed_by_app_label.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0051_calendarevent_and_holiday.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0051_calendarevent_and_holiday.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0052_site_related_name.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0052_site_related_name.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0053_freebusy.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0053_freebusy.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0054_create_organisation_model.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0054_create_organisation_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0055_customevent.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0055_customevent.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0058_migrate_preferences_to_global.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0058_migrate_preferences_to_global.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0059_drop_site.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0059_drop_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/migrations/0060_person_unique_short_name_email.py` & `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0060_person_unique_short_name_email.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/mixins.py` & `aleksis_core-4.0.0.dev6/aleksis/core/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,14 +307,15 @@
 ):
     """Model class for extensible, polymorphic models."""
 
     objects = PolymorphicBaseManager()
 
     class Meta:
         abstract = True
+        base_manager_name = "objects"
 
 
 class PureDjangoModel:
     """No-op mixin to mark a model as deliberately not using ExtensibleModel."""
 
     pass
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/models.py` & `aleksis_core-4.0.0.dev6/aleksis/core/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/preferences.py` & `aleksis_core-4.0.0.dev6/aleksis/core/preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -483,27 +483,27 @@
 
 @site_preferences_registry.register
 class BirthdayFeedColor(StringPreference):
     """Color for the birthdays calendar feed."""
 
     section = calendar
     name = "birthday_color"
-    default = "#0d5eaf"
+    default = "#f39c12"
     verbose_name = _("Birthday calendar feed color")
     widget = ColorWidget
     required = True
 
 
 @site_preferences_registry.register
 class HolidayFeedColor(StringPreference):
     """Color for the holidays calendar feed."""
 
     section = calendar
     name = "holiday_color"
-    default = "#0d5eaf"
+    default = "#00b894"
     verbose_name = _("Holiday calendar feed color")
     widget = ColorWidget
     required = True
 
 
 @site_preferences_registry.register
 class PersonalEventFeedColor(StringPreference):
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/registries.py` & `aleksis_core-4.0.0.dev6/aleksis/core/registries.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/rules.py` & `aleksis_core-4.0.0.dev6/aleksis/core/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
 
 # Create group
 create_group_predicate = has_person & (
     has_global_perm("core.add_group") | has_object_perm("core.add_group")
 )
 rules.add_perm("core.create_group_rule", create_group_predicate)
 
-# School years
+# School terms
 view_school_term_predicate = has_person & has_global_perm("core.view_schoolterm")
 rules.add_perm("core.view_schoolterm_rule", view_school_term_predicate)
 
 create_school_term_predicate = has_person & has_global_perm("core.add_schoolterm")
 rules.add_perm("core.create_schoolterm_rule", create_school_term_predicate)
 
 edit_school_term_predicate = has_person & has_global_perm("core.change_schoolterm")
@@ -433,7 +433,31 @@
 )
 rules.add_perm("core.edit_personal_event_rule", edit_personal_event_predicate)
 
 delete_personal_event_predicate = has_person & (
     has_global_perm("core.delete_personalevent") | is_personal_event_owner
 )
 rules.add_perm("core.delete_personal_event_rule", delete_personal_event_predicate)
+
+# Rooms
+view_room_predicate = has_person & (
+    has_global_perm("core.view_room") | has_object_perm("core.view_room")
+)
+rules.add_perm("core.view_room_rule", view_room_predicate)
+
+view_rooms_predicate = has_person & (
+    has_global_perm("core.view_room") | has_any_object("core.view_room", Holiday)
+)
+rules.add_perm("core.view_rooms_rule", view_rooms_predicate)
+
+edit_room_predicate = has_person & (
+    has_global_perm("core.change_room") | has_object_perm("core.change_room")
+)
+rules.add_perm("core.edit_room_rule", edit_room_predicate)
+
+create_room_predicate = has_person & (has_global_perm("core.add_room"))
+rules.add_perm("core.create_room_rule", create_room_predicate)
+
+delete_room_predicate = has_person & (
+    has_global_perm("core.delete_room") | has_object_perm("core.delete_room")
+)
+rules.add_perm("core.delete_room_rule", delete_room_predicate)
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/__init__.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,26 +24,32 @@
 from ..util.core_helpers import get_allowed_object_ids, get_app_module, get_app_packages, has_person
 from .base import FilterOrderList
 from .calendar import CalendarBaseType, SetCalendarStatusMutation
 from .celery_progress import CeleryProgressFetchedMutation, CeleryProgressType
 from .custom_menu import CustomMenuType
 from .dynamic_routes import DynamicRouteType
 from .group import GroupType
+from .group_type import (
+    GroupTypeBatchCreateMutation,
+    GroupTypeBatchDeleteMutation,
+    GroupTypeBatchPatchMutation,
+    GroupTypeType,
+)
 from .holiday import (
     HolidayBatchCreateMutation,
     HolidayBatchDeleteMutation,
     HolidayBatchPatchMutation,
     HolidayType,
 )
 from .installed_apps import AppType
 from .message import MessageType
 from .notification import MarkNotificationReadMutation, NotificationType
 from .oauth import OAuthAccessTokenType, OAuthBatchRevokeTokenMutation
 from .pdf import PDFFileType
-from .person import PersonMutation, PersonType
+from .person import PersonBatchDeleteMutation, PersonMutation, PersonType
 from .personal_event import (
     PersonalEventBatchCreateMutation,
     PersonalEventBatchDeleteMutation,
     PersonalEventBatchPatchMutation,
 )
 from .room import (
     RoomBatchCreateMutation,
@@ -64,15 +70,15 @@
 
 
 class Query(graphene.ObjectType):
     ping = graphene.String(payload=graphene.String())
 
     notifications = graphene.List(NotificationType)
 
-    persons = graphene.List(PersonType)
+    persons = FilterOrderList(PersonType)
     person_by_id = graphene.Field(PersonType, id=graphene.ID())
     person_by_id_or_me = graphene.Field(PersonType, id=graphene.ID())
 
     groups = graphene.List(GroupType)
     group_by_id = graphene.Field(GroupType, id=graphene.ID())
     groups_by_owner = FilterOrderList(GroupType, owner=graphene.ID())
 
@@ -104,14 +110,16 @@
     room_by_id = graphene.Field(RoomType, id=graphene.ID())
 
     school_terms = FilterOrderList(SchoolTermType)
 
     holidays = FilterOrderList(HolidayType)
     calendar = graphene.Field(CalendarBaseType)
 
+    group_types = FilterOrderList(GroupTypeType)
+
     def resolve_ping(root, info, payload) -> str:
         return payload
 
     def resolve_notifications(root, info, **kwargs):
         return Notification.objects.filter(
             Q(
                 pk__in=get_objects_for_user(
@@ -252,14 +260,15 @@
     @staticmethod
     def resolve_calendar(root, info, **kwargs):
         return True
 
 
 class Mutation(graphene.ObjectType):
     update_person = PersonMutation.Field()
+    delete_persons = PersonBatchDeleteMutation.Field()
 
     mark_notification_read = MarkNotificationReadMutation.Field()
 
     celery_progress_fetched = CeleryProgressFetchedMutation.Field()
 
     revoke_oauth_tokens = OAuthBatchRevokeTokenMutation.Field()
 
@@ -277,14 +286,18 @@
 
     create_personal_events = PersonalEventBatchCreateMutation.Field()
     delete_personal_events = PersonalEventBatchDeleteMutation.Field()
     update_personal_events = PersonalEventBatchPatchMutation.Field()
 
     set_calendar_status = SetCalendarStatusMutation.Field()
 
+    create_group_types = GroupTypeBatchCreateMutation.Field()
+    delete_group_types = GroupTypeBatchDeleteMutation.Field()
+    update_group_types = GroupTypeBatchPatchMutation.Field()
+
 
 def build_global_schema():
     """Build global GraphQL schema from all apps."""
     query_bases = [Query]
     mutation_bases = [Mutation]
 
     for app in get_app_packages():
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/base.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import json
 
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import PermissionDenied
 from django.db.models import Model
 
 import graphene
+import reversion
 from django_filters.filterset import FilterSet, filterset_factory
 from graphene_django import DjangoListField, DjangoObjectType
+from graphene_django_cud.mutations.batch_create import DjangoBatchCreateMutation
+from graphene_django_cud.mutations.batch_delete import DjangoBatchDeleteMutation
+from graphene_django_cud.mutations.batch_patch import DjangoBatchPatchMutation
+from reversion import set_comment, set_user
 
 from ..util.core_helpers import queryset_rules_filter
 
 
 class RulesObjectType(DjangoObjectType):
     class Meta:
         abstract = True
@@ -90,38 +95,44 @@
     `is_optimistic` can be set to true in the frontend.
     """
 
     is_optimistic = graphene.Boolean(default_value=False)
 
 
 class PermissionBatchPatchMixin:
+    """Mixin for permission checking during batch patch mutations."""
+
     class Meta:
         login_required = True
 
     @classmethod
     def check_permissions(cls, root, info, input):  # noqa
         if info.context.user.has_perms(cls._meta.permissions, root):
             return
 
         raise PermissionDenied()
 
 
 class PermissionBatchDeleteMixin:
+    """Mixin for permission checking during batch delete mutations."""
+
     class Meta:
         login_required = True
 
     @classmethod
     def check_permissions(cls, root, info, input):  # noqa
         if info.context.user.has_perms(cls._meta.permissions, root):
             return
 
         raise PermissionDenied()
 
 
 class PermissionPatchMixin:
+    """Mixin for permission checking during patch mutations."""
+
     class Meta:
         login_required = True
 
     @classmethod
     def check_permissions(cls, root, info, input, id, obj):  # noqa
         if info.context.user.has_perms(cls._meta.permissions, root):
             return
@@ -208,10 +219,38 @@
 
         if order_by is not None:
             if isinstance(order_by, str):
                 order_by = [order_by]
 
             qs = qs.order_by(*order_by)
 
-        print(f"{filters=}")
-
         return qs
+
+
+class MutateWithRevisionMixin:
+    """Mixin for creating revision for mutation."""
+
+    @classmethod
+    def mutate(cls, root, info, *args, **kwargs):
+        with reversion.create_revision():
+            set_user(info.context.user)
+            set_comment(cls.__name__)
+            super().mutate(root, info, *args, **kwargs)
+
+
+class BaseBatchCreateMutation(MutateWithRevisionMixin, DjangoBatchCreateMutation):
+    class Meta:
+        abstract = True
+
+
+class BaseBatchPatchMutation(
+    MutateWithRevisionMixin, PermissionBatchPatchMixin, DjangoBatchPatchMutation
+):
+    class Meta:
+        abstract = True
+
+
+class BaseBatchDeleteMutation(
+    MutateWithRevisionMixin, PermissionBatchDeleteMixin, DjangoBatchDeleteMutation
+):
+    class Meta:
+        abstract = True
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/calendar.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/calendar.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/celery_progress.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/custom_menu.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/custom_menu.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/group.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/group.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/holiday.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/holiday.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from graphene_django import DjangoObjectType
-from graphene_django_cud.mutations import (
-    DjangoBatchCreateMutation,
-    DjangoBatchDeleteMutation,
-    DjangoBatchPatchMutation,
-)
 from guardian.shortcuts import get_objects_for_user
 
 from ..models import Holiday
 from .base import (
+    BaseBatchCreateMutation,
+    BaseBatchDeleteMutation,
+    BaseBatchPatchMutation,
     DjangoFilterMixin,
-    PermissionBatchDeleteMixin,
-    PermissionBatchPatchMixin,
     PermissionsTypeMixin,
 )
 
 
 class HolidayType(PermissionsTypeMixin, DjangoFilterMixin, DjangoObjectType):
     class Meta:
         model = Holiday
@@ -27,25 +23,25 @@
         }
 
     @classmethod
     def get_queryset(cls, queryset, info):
         return get_objects_for_user(info.context.user, "core.view_holiday", queryset)
 
 
-class HolidayBatchCreateMutation(DjangoBatchCreateMutation):
+class HolidayBatchCreateMutation(BaseBatchCreateMutation):
     class Meta:
         model = Holiday
         permissions = ("core.create_holiday_rule",)
         only_fields = ("holiday_name", "date_start", "date_end")
 
 
-class HolidayBatchDeleteMutation(PermissionBatchDeleteMixin, DjangoBatchDeleteMutation):
+class HolidayBatchDeleteMutation(BaseBatchDeleteMutation):
     class Meta:
         model = Holiday
         permissions = ("core.delete_holiday_rule",)
 
 
-class HolidayBatchPatchMutation(PermissionBatchPatchMixin, DjangoBatchPatchMutation):
+class HolidayBatchPatchMutation(BaseBatchPatchMutation):
     class Meta:
         model = Holiday
         permissions = ("core.edit_holiday_rule",)
         only_fields = ("id", "holiday_name", "date_start", "date_end")
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/installed_apps.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/installed_apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/notification.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/oauth.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/pdf.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/person.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/person.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 from django.utils import timezone
 
 import graphene
 from graphene_django import DjangoObjectType
 from graphene_django.forms.mutation import DjangoModelFormMutation
 from guardian.shortcuts import get_objects_for_user
 
+from ..filters import PersonFilter
 from ..forms import PersonForm
 from ..models import DummyPerson, Person
 from ..util.core_helpers import get_site_preferences, has_person
-from .base import FieldFileType
+from .base import (
+    BaseBatchDeleteMutation,
+    DjangoFilterMixin,
+    FieldFileType,
+    PermissionsTypeMixin,
+)
 from .notification import NotificationType
 
 
 class PersonPreferencesType(graphene.ObjectType):
     theme_design_mode = graphene.String()
 
     def resolve_theme_design_mode(parent, info, **kwargs):
         return parent["theme__design"]
 
 
-class PersonType(DjangoObjectType):
+class PersonType(PermissionsTypeMixin, DjangoFilterMixin, DjangoObjectType):
     class Meta:
         model = Person
         fields = [
             "id",
             "user",
             "first_name",
             "last_name",
@@ -47,14 +53,15 @@
             "guardians",
             "primary_group",
             "description",
             "children",
             "owner_of",
             "member_of",
         ]
+        filterset_class = PersonFilter
 
     full_name = graphene.String()
     username = graphene.String()
     userid = graphene.ID()
     photo = graphene.Field(FieldFileType, required=False)
     avatar = graphene.Field(FieldFileType, required=False)
     avatar_url = graphene.String()
@@ -248,7 +255,13 @@
         if not form.initial:
             if not info.context.user.has_perm("core.create_person_rule"):
                 raise PermissionDenied()
         else:
             if not info.context.user.has_perm("core.edit_person_rule", form.instance):
                 raise PermissionDenied()
         return super().perform_mutate(form, info)
+
+
+class PersonBatchDeleteMutation(BaseBatchDeleteMutation):
+    class Meta:
+        model = Person
+        permissions = ("core.delete_person_rule",)
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/personal_event.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/personal_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from typing import Iterable
 
 from django.utils import timezone
 
 import graphene
 from graphene_django import DjangoObjectType
-from graphene_django_cud.mutations import (
-    DjangoBatchCreateMutation,
-    DjangoBatchDeleteMutation,
-    DjangoBatchPatchMutation,
-)
 
 from ..models import PersonalEvent
 from .base import (
-    PermissionBatchDeleteMixin,
+    BaseBatchCreateMutation,
+    BaseBatchDeleteMutation,
+    BaseBatchPatchMutation,
     PermissionBatchPatchMixin,
 )
 
 
 class PersonalEventType(DjangoObjectType):
     class Meta:
         model = PersonalEvent
         fields = (
             "id",
             "title",
             "description",
             "location",
             "datetime_start",
             "datetime_end",
+            "date_start",
+            "date_end",
             "owner",
             "persons",
             "groups",
         )
 
     recurrences = graphene.String()
 
 
-class PersonalEventBatchCreateMutation(PermissionBatchPatchMixin, DjangoBatchCreateMutation):
+class PersonalEventBatchCreateMutation(PermissionBatchPatchMixin, BaseBatchCreateMutation):
     class Meta:
         model = PersonalEvent
         permissions = ("core.create_personal_event_with_invitations_rule",)
         only_fields = (
             "title",
             "description",
             "location",
             "datetime_start",
             "datetime_end",
+            "date_start",
+            "date_end",
             "recurrences",
             "persons",
             "groups",
         )
         field_types = {"recurrences": graphene.String(), "location": graphene.String()}
 
     @classmethod
@@ -70,31 +71,33 @@
 
     @classmethod
     def handle_datetime_end(cls, value, name, info):
         value = value.replace(tzinfo=timezone.get_default_timezone())
         return value
 
 
-class PersonalEventBatchDeleteMutation(PermissionBatchDeleteMixin, DjangoBatchDeleteMutation):
+class PersonalEventBatchDeleteMutation(BaseBatchDeleteMutation):
     class Meta:
         model = PersonalEvent
         permissions = ("core.delete_personal_event_rule",)
 
 
-class PersonalEventBatchPatchMutation(PermissionBatchPatchMixin, DjangoBatchPatchMutation):
+class PersonalEventBatchPatchMutation(BaseBatchPatchMutation):
     class Meta:
         model = PersonalEvent
         permissions = ("core.change_personalevent",)
         only_fields = (
             "id",
             "title",
             "description",
             "location",
             "datetime_start",
             "datetime_end",
+            "date_start",
+            "date_end",
             "recurrences",
             "persons",
             "groups",
         )
         field_types = {"recurrences": graphene.String(), "location": graphene.String()}
 
     @classmethod
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/search.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/site_preferences.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/site_preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/system_properties.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/system_properties.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/two_factor.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/two_factor.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/schema/user.py` & `aleksis_core-4.0.0.dev6/aleksis/core/schema/user.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/settings.py` & `aleksis_core-4.0.0.dev6/aleksis/core/settings.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/img/aleksis-banner.svg` & `aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-banner.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/img/aleksis-favicon.png` & `aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-favicon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/img/aleksis-icon-maskable.png` & `aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon-maskable.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/img/aleksis-icon-maskable.svg` & `aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon-maskable.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/img/aleksis-icon.png` & `aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/img/aleksis-icon.svg` & `aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/img/fallback.png` & `aleksis_core-4.0.0.dev6/aleksis/core/static/img/fallback.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/img/hero.svg` & `aleksis_core-4.0.0.dev6/aleksis/core/static/img/hero.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/js/edit_dashboard.js` & `aleksis_core-4.0.0.dev6/aleksis/core/static/js/edit_dashboard.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/js/helper.js` & `aleksis_core-4.0.0.dev6/aleksis/core/static/js/helper.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/js/include_ajax_live.js` & `aleksis_core-4.0.0.dev6/aleksis/core/static/js/include_ajax_live.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/js/main.js` & `aleksis_core-4.0.0.dev6/aleksis/core/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/js/multi_select.js` & `aleksis_core-4.0.0.dev6/aleksis/core/static/js/multi_select.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/js/search.js` & `aleksis_core-4.0.0.dev6/aleksis/core/static/js/search.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/js/serviceworker.js` & `aleksis_core-4.0.0.dev6/aleksis/core/static/js/serviceworker.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/print.css` & `aleksis_core-4.0.0.dev6/aleksis/core/static/print.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/public/materialize-custom.scss` & `aleksis_core-4.0.0.dev6/aleksis/core/static/public/materialize-custom.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/public/style.scss` & `aleksis_core-4.0.0.dev6/aleksis/core/static/public/style.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/static/public/theme.scss` & `aleksis_core-4.0.0.dev6/aleksis/core/static/public/theme.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/tables.py` & `aleksis_core-4.0.0.dev6/aleksis/core/tables.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,27 +77,14 @@
         attrs = {"class": "highlight"}
 
     name = tables.LinkColumn("group_by_id", args=[A("id")])
     short_name = tables.LinkColumn("group_by_id", args=[A("id")])
     school_term = tables.Column()
 
 
-class GroupTypesTable(tables.Table):
-    """Table to list group types."""
-
-    class Meta:
-        attrs = {"class": "highlight"}
-
-    name = tables.LinkColumn("edit_group_type_by_id", args=[A("id")])
-    description = tables.LinkColumn("edit_group_type_by_id", args=[A("id")])
-    delete = tables.LinkColumn(
-        "delete_group_type_by_id", args=[A("id")], verbose_name=_("Delete"), text=_("Delete")
-    )
-
-
 class DashboardWidgetTable(tables.Table):
     """Table to list dashboard widgets."""
 
     class Meta:
         attrs = {"class": "highlight"}
 
     widget_name = tables.Column(accessor="pk")
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/tasks.py` & `aleksis_core-4.0.0.dev6/aleksis/core/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/403.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/403.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/404.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/404.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/500.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/500.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/account/account_inactive.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/account_inactive.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/account/email/email_confirmation_message.txt` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/email/email_confirmation_message.txt`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/account/email_confirm.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/account/password_change.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_change.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/account/password_reset.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/account/password_reset_done.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/account/password_reset_from_key.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/account/password_reset_from_key_done.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset_from_key_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/account/signup.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/account/signup_closed.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/signup_closed.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/account/verification_email_required.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/verification_email_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/account/verification_sent.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/components/chips.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/components/chips.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/components/pagination.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/components/pagination.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/announcement/form.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/announcement/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/announcement/list.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/announcement/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/base.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/base.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/base_print.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/base_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/base_simple_print.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/base_simple_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/dashboard_widget/create.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/dashboard_widget/edit.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/dashboard_widget/list.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/data_check/list.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/data_check/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/edit_dashboard.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/edit_dashboard.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/group/child_groups.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/child_groups.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/group/edit.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/group/full.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/group/list.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/group_type/list.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/disabled.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,48 @@
-00000000: 7b23 202d 2a2d 2065 6e67 696e 653a 646a  {# -*- engine:dj
-00000010: 616e 676f 202d 2a2d 2023 7d0a 0a7b 2520  ango -*- #}..{% 
-00000020: 6578 7465 6e64 7320 2263 6f72 652f 6261  extends "core/ba
-00000030: 7365 2e68 746d 6c22 2025 7d0a 0a7b 2520  se.html" %}..{% 
-00000040: 6c6f 6164 2069 3138 6e20 257d 0a7b 2520  load i18n %}.{% 
-00000050: 6c6f 6164 2072 656e 6465 725f 7461 626c  load render_tabl
-00000060: 6520 6672 6f6d 2064 6a61 6e67 6f5f 7461  e from django_ta
-00000070: 626c 6573 3220 257d 0a0a 7b25 2062 6c6f  bles2 %}..{% blo
-00000080: 636b 2062 726f 7773 6572 5f74 6974 6c65  ck browser_title
-00000090: 2025 7d7b 2520 626c 6f63 6b74 7261 6e73   %}{% blocktrans
-000000a0: 2025 7d47 726f 7570 2074 7970 6573 7b25   %}Group types{%
-000000b0: 2065 6e64 626c 6f63 6b74 7261 6e73 2025   endblocktrans %
-000000c0: 7d7b 2520 656e 6462 6c6f 636b 2025 7d0a  }{% endblock %}.
-000000d0: 7b25 2062 6c6f 636b 2070 6167 655f 7469  {% block page_ti
-000000e0: 746c 6520 257d 7b25 2062 6c6f 636b 7472  tle %}{% blocktr
-000000f0: 616e 7320 257d 4772 6f75 7020 7479 7065  ans %}Group type
-00000100: 737b 2520 656e 6462 6c6f 636b 7472 616e  s{% endblocktran
-00000110: 7320 257d 7b25 2065 6e64 626c 6f63 6b20  s %}{% endblock 
-00000120: 257d 0a0a 7b25 2062 6c6f 636b 2063 6f6e  %}..{% block con
-00000130: 7465 6e74 2025 7d0a 2020 3c61 2063 6c61  tent %}.  <a cla
-00000140: 7373 3d22 6274 6e20 6772 6565 6e20 7761  ss="btn green wa
-00000150: 7665 732d 6566 6665 6374 2077 6176 6573  ves-effect waves
-00000160: 2d6c 6967 6874 2220 6872 6566 3d22 7b25  -light" href="{%
-00000170: 2075 726c 2027 6372 6561 7465 5f67 726f   url 'create_gro
-00000180: 7570 5f74 7970 6527 2025 7d22 3e0a 2020  up_type' %}">.  
-00000190: 2020 3c69 2063 6c61 7373 3d22 6d61 7465    <i class="mate
-000001a0: 7269 616c 2d69 636f 6e73 2069 636f 6e69  rial-icons iconi
-000001b0: 6679 206c 6566 7422 2064 6174 612d 6963  fy left" data-ic
-000001c0: 6f6e 3d22 6d64 693a 6164 6422 3e3c 2f69  on="mdi:add"></i
-000001d0: 3e0a 2020 2020 7b25 2074 7261 6e73 2022  >.    {% trans "
-000001e0: 4372 6561 7465 2067 726f 7570 2074 7970  Create group typ
-000001f0: 6522 2025 7d0a 2020 3c2f 613e 0a0a 2020  e" %}.  </a>..  
-00000200: 7b25 2072 656e 6465 725f 7461 626c 6520  {% render_table 
-00000210: 6772 6f75 705f 7479 7065 735f 7461 626c  group_types_tabl
-00000220: 6520 257d 0a7b 2520 656e 6462 6c6f 636b  e %}.{% endblock
-00000230: 2025 7d0a                                 %}.
+00000000: 7b25 2065 7874 656e 6473 2022 636f 7265  {% extends "core
+00000010: 2f62 6173 652e 6874 6d6c 2220 257d 0a0a  /base.html" %}..
+00000020: 7b25 206c 6f61 6420 6931 386e 2025 7d0a  {% load i18n %}.
+00000030: 0a7b 2520 626c 6f63 6b20 6272 6f77 7365  .{% block browse
+00000040: 725f 7469 746c 6520 257d 7b25 2062 6c6f  r_title %}{% blo
+00000050: 636b 7472 616e 7320 257d 5468 6520 696e  cktrans %}The in
+00000060: 7669 7465 2066 6561 7475 7265 2069 7320  vite feature is 
+00000070: 6469 7361 626c 6564 7b25 2065 6e64 626c  disabled{% endbl
+00000080: 6f63 6b74 7261 6e73 2025 7d7b 2520 656e  ocktrans %}{% en
+00000090: 6462 6c6f 636b 2025 7d0a 7b25 2062 6c6f  dblock %}.{% blo
+000000a0: 636b 206e 6f5f 7061 6765 5f74 6974 6c65  ck no_page_title
+000000b0: 2025 7d7b 2520 656e 6462 6c6f 636b 2025   %}{% endblock %
+000000c0: 7d0a 0a7b 2520 626c 6f63 6b20 636f 6e74  }..{% block cont
+000000d0: 656e 7420 257d 0a20 203c 6469 7620 636c  ent %}.  <div cl
+000000e0: 6173 733d 2263 6f6e 7461 696e 6572 223e  ass="container">
+000000f0: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
+00000100: 2263 6172 6420 7265 6422 3e0a 2020 2020  "card red">.    
+00000110: 2020 3c64 6976 2063 6c61 7373 3d22 6361    <div class="ca
+00000120: 7264 2d63 6f6e 7465 6e74 2077 6869 7465  rd-content white
+00000130: 2d74 6578 7422 3e0a 2020 2020 2020 2020  -text">.        
+00000140: 3c69 2063 6c61 7373 3d22 6d61 7465 7269  <i class="materi
+00000150: 616c 2d69 636f 6e73 2073 6d61 6c6c 206c  al-icons small l
+00000160: 6566 7422 3e64 6973 6162 6c65 645f 6279  eft">disabled_by
+00000170: 5f64 6566 6175 6c74 3c2f 693e 0a20 2020  _default</i>.   
+00000180: 2020 2020 203c 7370 616e 2063 6c61 7373       <span class
+00000190: 3d22 6361 7264 2d74 6974 6c65 223e 7b25  ="card-title">{%
+000001a0: 2062 6c6f 636b 7472 616e 7320 257d 5468   blocktrans %}Th
+000001b0: 6520 696e 7669 7465 2066 6561 7475 7265  e invite feature
+000001c0: 2069 7320 6469 7361 626c 6564 2e7b 2520   is disabled.{% 
+000001d0: 656e 6462 6c6f 636b 7472 616e 7320 257d  endblocktrans %}
+000001e0: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
+000001f0: 3c70 3e0a 2020 2020 2020 2020 2020 7b25  <p>.          {%
+00000200: 2074 7261 6e73 2022 546f 2065 6e61 626c   trans "To enabl
+00000210: 6520 6974 2c20 7377 6974 6368 206f 6e20  e it, switch on 
+00000220: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
+00000230: 6720 6368 6563 6b62 6f78 2069 6e20 7468  g checkbox in th
+00000240: 6520 6175 7468 656e 7469 6361 7469 6f6e  e authentication
+00000250: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
+00000260: 2220 257d 0a20 2020 2020 2020 2020 203c  " %}.          <
+00000270: 6120 6872 6566 3d22 7b25 2075 726c 2022  a href="{% url "
+00000280: 7072 6566 6572 656e 6365 735f 7369 7465  preferences_site
+00000290: 2220 257d 223e 7b25 2074 7261 6e73 2022  " %}">{% trans "
+000002a0: 7369 7465 2070 7265 6665 7265 6e63 6573  site preferences
+000002b0: 2070 6167 6522 2025 7d3c 2f61 3e2e 0a20   page" %}</a>.. 
+000002c0: 2020 2020 2020 203c 2f70 3e0a 2020 2020         </p>.    
+000002d0: 2020 3c2f 6469 763e 0a20 2020 203c 2f64    </div>.    </d
+000002e0: 6976 3e0a 2020 3c2f 6469 763e 0a7b 2520  iv>.  </div>.{% 
+000002f0: 656e 6462 6c6f 636b 2025 7d0a            endblock %}.
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/index.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/pages/delete.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/pages/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/pages/system_status.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/pages/system_status.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/pages/test_pdf.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/pages/test_pdf.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/announcements.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/announcements.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/avatar_content.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/avatar_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/crud_events.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/crud_events.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/meta.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/meta.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/partials/splash_screen.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/splash_screen.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/perms/assign.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/perms/assign.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/perms/list.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/perms/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/person/create.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/person/edit.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/person/list.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/core/vue_index.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/vue_index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/django_tables2/materialize.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/django_tables2/materialize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/dynamic_preferences/form.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/dynamic_preferences/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/invitations/disabled.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/list.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 {% extends "core/base.html" %}
 
 {% load i18n %}
 
-{% block browser_title %}{% blocktrans %}The invite feature is disabled{% endblocktrans %}{% endblock %}
-{% block no_page_title %}{% endblock %}
+{% block browser_title %}{% blocktrans %}OAuth2 Applications{% endblocktrans %}{% endblock %}
+{% block page_title %}{% blocktrans %}OAuth2 Applications{% endblocktrans %}{% endblock %}
 
 {% block content %}
-  <div class="container">
-    <div class="card red">
-      <div class="card-content white-text">
-        <i class="material-icons small left">disabled_by_default</i>
-        <span class="card-title">{% blocktrans %}The invite feature is disabled.{% endblocktrans %}</span>
-        <p>
-          {% trans "To enable it, switch on the corresponding checkbox in the authentication section of the " %}
-          <a href="{% url "preferences_site" %}">{% trans "site preferences page" %}</a>.
-        </p>
+  <a href="{% url "register_oauth_application" %}" class="btn green waves-effect waves-light">
+    <i class="material-icons iconify left" data-icon="mdi:add"></i>
+    {% blocktrans %}Register new application{% endblocktrans %}
+  </a>
+  <div class="collection">
+    {% for application in applications %}
+      <a class="collection-item avatar" href="{% url "oauth2_application" application.id %}">
+        {% if application.icon %}
+          <img src="{{ application.icon.url }}" alt="{{ application.name }}" class="circle">
+        {% endif %}
+        <span class="title">
+          {{ application.name }}
+        </span>
+      </a>
+      {% empty %}
+      <div class="collection-item flow-text">
+        {% blocktrans %}No applications defined.{% endblocktrans %}
       </div>
-    </div>
+    {% endfor %}
   </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
 {% extends "core/base.html" %} {% load i18n %} {% block browser_title %}{%
-blocktrans %}The invite feature is disabled{% endblocktrans %}{% endblock %} {%
-block no_page_title %}{% endblock %} {% block content %}
-disabled_by_default {% blocktrans %}The invite feature is disabled.{%
-endblocktrans %}
-{% trans "To enable it, switch on the corresponding checkbox in the
-authentication section of the " %} }">{% trans "site preferences page" %}
-.
+blocktrans %}OAuth2 Applications{% endblocktrans %}{% endblock %} {% block
+page_title %}{% blocktrans %}OAuth2 Applications{% endblocktrans %}{% endblock
+%} {% block content %}
+}" class="btn green waves-effect waves-light"> {% blocktrans %}Register new
+application{% endblocktrans %}
+{% for application in applications %} _{_%_ _i_f_ _a_p_p_l_i_c_a_t_i_o_n_._i_c_o_n_ _%_}_ _[_{
+_{_ _a_p_p_l_i_c_a_t_i_o_n_._n_a_m_e_ _}_}_]_{_%_ _e_n_d_i_f_ _%_}_ _{_{_ _a_p_p_l_i_c_a_t_i_o_n_._n_a_m_e_ _}_}_ {% empty %}
+{% blocktrans %}No applications defined.{% endblocktrans %}
+{% endfor %}
 {% endblock %}
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/invitations/enter.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/enter.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/invitations/forms/_invite.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/forms/_invite.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/material/fields/colorfield_colorwidget.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/colorfield_colorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/material/fields/django_select2_select2widget.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/django_select2_select2widget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/oauth2_provider/application/create.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/oauth2_provider/application/detail.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/oauth2_provider/application/edit.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/oauth2_provider/authorize.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/offline.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/offline.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/search/search.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/socialaccount/authentication_error.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/authentication_error.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/socialaccount/connections.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/socialaccount/login.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/socialaccount/login_cancelled.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/login_cancelled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/socialaccount/signup.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/socialaccount/snippets/provider_list.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/base.email` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/base.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/celery_failure.email` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/celery_failure.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/data_checks.email` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/data_checks.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/email.css` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/email.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/invitation.email` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/invitation.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/notification.email` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/notification.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/templated_email/person_changed.email` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/person_changed.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/_wizard_actions.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/_wizard_actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/core/backup_tokens.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/backup_tokens.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/core/login.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/core/otp_required.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/otp_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/core/phone_register.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/phone_register.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/core/setup.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/setup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/core/setup_complete.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/setup_complete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templates/two_factor/profile/disable.html` & `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/profile/disable.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templatetags/data_helpers.py` & `aleksis_core-4.0.0.dev6/aleksis/core/templatetags/data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/templatetags/html_helpers.py` & `aleksis_core-4.0.0.dev6/aleksis/core/templatetags/html_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/tests/browser/test_selenium.py` & `aleksis_core-4.0.0.dev6/aleksis/core/tests/browser/test_selenium.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/tests/mixins/test_registry_object.py` & `aleksis_core-4.0.0.dev6/aleksis/core/tests/mixins/test_registry_object.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/tests/models/test.pdf` & `aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test.pdf`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/tests/models/test_group_sync.py` & `aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_group_sync.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/tests/models/test_notification.py` & `aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/tests/models/test_pdffile.py` & `aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_pdffile.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/tests/regression/test_regression.py` & `aleksis_core-4.0.0.dev6/aleksis/core/tests/regression/test_regression.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/tests/regression/view_oauth.py` & `aleksis_core-4.0.0.dev6/aleksis/core/tests/regression/view_oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/tests/templatetags/test_data_helpers.py` & `aleksis_core-4.0.0.dev6/aleksis/core/tests/templatetags/test_data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/tests/views/test_account.py` & `aleksis_core-4.0.0.dev6/aleksis/core/tests/views/test_account.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/urls.py` & `aleksis_core-4.0.0.dev6/aleksis/core/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,40 +138,27 @@
                     name="person_by_id",
                 ),
                 path(
                     "persons/<int:pk>/edit/",
                     views.EditPersonView.as_view(),
                     name="edit_person_by_id",
                 ),
-                path("persons/<int:id_>/delete/", views.delete_person, name="delete_person_by_id"),
                 path(
                     "persons/<int:pk>/invite/",
                     views.InvitePersonByID.as_view(),
                     name="invite_person_by_id",
                 ),
                 path("groups/", views.groups, name="groups"),
                 path("groups/child_groups/", views.groups_child_groups, name="groups_child_groups"),
                 path("groups/create/", views.edit_group, name="create_group"),
                 path("groups/<int:id_>/", views.group, name="group_by_id"),
                 path("groups/<int:id_>/edit/", views.edit_group, name="edit_group_by_id"),
                 path("groups/<int:id_>/delete/", views.delete_group, name="delete_group_by_id"),
                 path("", views.index, name="index"),
                 path("dashboard/edit/", views.EditDashboardView.as_view(), name="edit_dashboard"),
-                path("groups/group_types/create", views.edit_group_type, name="create_group_type"),
-                path(
-                    "groups/group_types/<int:id_>/delete/",
-                    views.delete_group_type,
-                    name="delete_group_type_by_id",
-                ),
-                path(
-                    "groups/group_types/<int:id_>/edit/",
-                    views.edit_group_type,
-                    name="edit_group_type_by_id",
-                ),
-                path("groups/group_types/", views.group_types, name="group_types"),
                 path("announcements/", views.announcements, name="announcements"),
                 path("announcements/create/", views.announcement_form, name="add_announcement"),
                 path(
                     "announcements/edit/<int:id_>/",
                     views.announcement_form,
                     name="edit_announcement",
                 ),
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/apps.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/apps.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 11018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 7920
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 26
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 18985
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/email.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/email.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 986
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 850
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/notifications.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/notifications.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 3818
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/predicates.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/predicates.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 5801
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 936
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/__pycache__/spdx.cpython-311.pyc` & `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/spdx.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1e9fe065 (Thu Feb 29 15:13:34 2024 UTC)
+moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
 files sz: 125
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/apps.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/auth_helpers.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/auth_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/celery_progress.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/core_helpers.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/email.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/email.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/forms.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/frontend_helpers.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/frontend_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/ldap.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/ldap.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/licenses.json` & `aleksis_core-4.0.0.dev6/aleksis/core/util/licenses.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/messages.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/messages.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/middlewares.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/middlewares.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/model_helpers.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/model_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/notifications.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/notifications.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/pdf.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/predicates.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/predicates.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/sass_helpers.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/sass_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/search.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/util/tables.py` & `aleksis_core-4.0.0.dev6/aleksis/core/util/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/views.py` & `aleksis_core-4.0.0.dev6/aleksis/core/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 from .forms import (
     AccountRegisterForm,
     AnnouncementForm,
     AssignPermissionForm,
     ChildGroupsForm,
     DashboardWidgetOrderFormSet,
     EditGroupForm,
-    EditGroupTypeForm,
     GroupPreferenceForm,
     InvitationCodeForm,
     MaintenanceModeForm,
     OAuthApplicationForm,
     PersonForm,
     PersonPreferenceForm,
     SelectPermissionForm,
@@ -104,15 +103,14 @@
 )
 from .models import (
     Announcement,
     DashboardWidget,
     DashboardWidgetOrder,
     DataCheckResult,
     Group,
-    GroupType,
     OAuthApplication,
     Person,
     PersonInvitation,
 )
 from .registries import (
     group_preferences_registry,
     person_preferences_registry,
@@ -120,15 +118,14 @@
 )
 from .tables import (
     DashboardWidgetTable,
     FullPersonsTable,
     GroupGlobalPermissionTable,
     GroupObjectPermissionTable,
     GroupsTable,
-    GroupTypesTable,
     InvitationsTable,
     PersonsTable,
     UserGlobalPermissionTable,
     UserObjectPermissionTable,
 )
 from .util import messages
 from .util.celery_progress import render_progress_page
@@ -650,98 +647,28 @@
     context["registry_url"] = "preferences_" + registry_name
     context["form"] = form
     context["instance"] = instance
 
     return render(request, "dynamic_preferences/form.html", context)
 
 
-@permission_required("core.delete_person_rule", fn=objectgetter_optional(Person))
-def delete_person(request: HttpRequest, id_: int) -> HttpResponse:
-    """View to delete an person."""
-    person = objectgetter_optional(Person)(request, id_)
-
-    with reversion.create_revision():
-        set_user(request.user)
-        person.save()
-
-    person.delete()
-    messages.success(request, _("The person has been deleted."))
-
-    return redirect("persons")
-
-
 @permission_required("core.delete_group_rule", fn=objectgetter_optional(Group))
 def delete_group(request: HttpRequest, id_: int) -> HttpResponse:
     """View to delete an group."""
     group = objectgetter_optional(Group)(request, id_)
     with reversion.create_revision():
         set_user(request.user)
         group.save()
 
     group.delete()
     messages.success(request, _("The group has been deleted."))
 
     return redirect("groups")
 
 
-@never_cache
-@permission_required("core.change_grouptype_rule", fn=objectgetter_optional(GroupType, None, False))
-def edit_group_type(request: HttpRequest, id_: Optional[int] = None) -> HttpResponse:
-    """View to edit or create a group_type."""
-    context = {}
-
-    group_type = objectgetter_optional(GroupType, None, False)(request, id_)
-    context["group_type"] = group_type
-
-    if id_:
-        # Edit form for existing group_type
-        edit_group_type_form = EditGroupTypeForm(request.POST or None, instance=group_type)
-    else:
-        # Empty form to create a new group_type
-        edit_group_type_form = EditGroupTypeForm(request.POST or None)
-
-    if edit_group_type_form.is_valid():
-        edit_group_type_form.save(commit=True)
-
-        messages.success(request, _("The group type has been saved."))
-
-        return redirect("group_types")
-
-    context["edit_group_type_form"] = edit_group_type_form
-
-    return render(request, "core/group_type/edit.html", context)
-
-
-@pwa_cache
-@permission_required("core.view_grouptypes_rule")
-def group_types(request: HttpRequest) -> HttpResponse:
-    """List view for listing all group types."""
-    context = {}
-
-    # Get all group types
-    group_types = get_objects_for_user(request.user, "core.view_grouptype", GroupType)
-
-    # Build table
-    group_types_table = GroupTypesTable(group_types)
-    RequestConfig(request).configure(group_types_table)
-    context["group_types_table"] = group_types_table
-
-    return render(request, "core/group_type/list.html", context)
-
-
-@permission_required("core.delete_grouptype_rule", fn=objectgetter_optional(GroupType, None, False))
-def delete_group_type(request: HttpRequest, id_: int) -> HttpResponse:
-    """View to delete an group_type."""
-    group_type = objectgetter_optional(GroupType, None, False)(request, id_)
-    group_type.delete()
-    messages.success(request, _("The group type has been deleted."))
-
-    return redirect("group_types")
-
-
 @method_decorator(pwa_cache, name="dispatch")
 class DataCheckView(PermissionRequiredMixin, ListView):
     permission_required = "core.view_datacheckresults_rule"
     model = DataCheckResult
     template_name = "core/data_check/list.html"
     context_object_name = "results"
```

### Comparing `aleksis_core-4.0.0.dev5/aleksis/core/vite.config.js` & `aleksis_core-4.0.0.dev6/aleksis/core/vite.config.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/Makefile` & `aleksis_core-4.0.0.dev6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/2fa.png` & `aleksis_core-4.0.0.dev6/docs/_static/2fa.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/accept_invite.png` & `aleksis_core-4.0.0.dev6/docs/_static/accept_invite.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/create_dashboard_widget.png` & `aleksis_core-4.0.0.dev6/docs/_static/create_dashboard_widget.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/create_social_application.png` & `aleksis_core-4.0.0.dev6/docs/_static/create_social_application.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/dashboard.png` & `aleksis_core-4.0.0.dev6/docs/_static/dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/dashboard_widgets.png` & `aleksis_core-4.0.0.dev6/docs/_static/dashboard_widgets.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/data_checks.png` & `aleksis_core-4.0.0.dev6/docs/_static/data_checks.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/edit_dashboard.png` & `aleksis_core-4.0.0.dev6/docs/_static/edit_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/edit_default_dashboard.png` & `aleksis_core-4.0.0.dev6/docs/_static/edit_default_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/invitations.png` & `aleksis_core-4.0.0.dev6/docs/_static/invitations.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/invite_existing.png` & `aleksis_core-4.0.0.dev6/docs/_static/invite_existing.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/pwa_desktop_chromium.png` & `aleksis_core-4.0.0.dev6/docs/_static/pwa_desktop_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/pwa_mobile_chromium.png` & `aleksis_core-4.0.0.dev6/docs/_static/pwa_mobile_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/pwa_mobile_firefox.png` & `aleksis_core-4.0.0.dev6/docs/_static/pwa_mobile_firefox.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/pwa_mobile_safari.png` & `aleksis_core-4.0.0.dev6/docs/_static/pwa_mobile_safari.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/_static/signup.png` & `aleksis_core-4.0.0.dev6/docs/_static/signup.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/01_core_concepts.rst` & `aleksis_core-4.0.0.dev6/docs/admin/01_core_concepts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/10_install.rst` & `aleksis_core-4.0.0.dev6/docs/admin/10_install.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/15_config_files.rst` & `aleksis_core-4.0.0.dev6/docs/admin/15_config_files.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/16_config_options.rst` & `aleksis_core-4.0.0.dev6/docs/admin/16_config_options.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/17_storage.rst` & `aleksis_core-4.0.0.dev6/docs/admin/17_storage.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/18_mail.rst` & `aleksis_core-4.0.0.dev6/docs/admin/18_mail.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/21_ldap.rst` & `aleksis_core-4.0.0.dev6/docs/admin/21_ldap.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/22_registration.rst` & `aleksis_core-4.0.0.dev6/docs/admin/22_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/23_socialaccounts.rst` & `aleksis_core-4.0.0.dev6/docs/admin/23_socialaccounts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/31_monitoring.rst` & `aleksis_core-4.0.0.dev6/docs/admin/31_monitoring.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/32_tasks.rst` & `aleksis_core-4.0.0.dev6/docs/admin/32_tasks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/33_data_checks.rst` & `aleksis_core-4.0.0.dev6/docs/admin/33_data_checks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/admin/50_dashboard.rst` & `aleksis_core-4.0.0.dev6/docs/admin/50_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/conf.py` & `aleksis_core-4.0.0.dev6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/dev/01_setup.rst` & `aleksis_core-4.0.0.dev6/docs/dev/01_setup.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/dev/02_install_apps.rst` & `aleksis_core-4.0.0.dev6/docs/dev/02_install_apps.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/dev/03_run_tests.rst` & `aleksis_core-4.0.0.dev6/docs/dev/03_run_tests.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/dev/04_materialize_templates.rst` & `aleksis_core-4.0.0.dev6/docs/dev/04_materialize_templates.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/dev/06_merging_app_settings.rst` & `aleksis_core-4.0.0.dev6/docs/dev/06_merging_app_settings.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/dev/10_dashboard_widgets.rst` & `aleksis_core-4.0.0.dev6/docs/dev/10_dashboard_widgets.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/index.rst` & `aleksis_core-4.0.0.dev6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/make.bat` & `aleksis_core-4.0.0.dev6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/ref/core/09_utils.rst` & `aleksis_core-4.0.0.dev6/docs/ref/core/09_utils.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/user/01_registration.rst` & `aleksis_core-4.0.0.dev6/docs/user/01_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/user/02_personal_account.rst` & `aleksis_core-4.0.0.dev6/docs/user/02_personal_account.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/user/10_dashboard.rst` & `aleksis_core-4.0.0.dev6/docs/user/10_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/docs/user/20_pwa.rst` & `aleksis_core-4.0.0.dev6/docs/user/20_pwa.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/pyproject.toml` & `aleksis_core-4.0.0.dev6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-Core"
-version = "4.0.0.dev5"
+version = "4.0.0.dev6"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
```

### Comparing `aleksis_core-4.0.0.dev5/tox.ini` & `aleksis_core-4.0.0.dev6/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev5/PKG-INFO` & `aleksis_core-4.0.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlekSIS-Core
-Version: 4.0.0.dev5
+Version: 4.0.0.dev6
 Summary: AlekSIS (School Information System) — Core
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,digitisation,school apps
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
```

