# Comparing `tmp/packitos-0.97.0.tar.gz` & `tmp/packitos-0.97.1.tar.gz`

## Comparing `packitos-0.97.0.tar` & `packitos-0.97.1.tar`

### file list

```diff
@@ -1,410 +1,410 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 packitos-0.97.0/.git_archival.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 packitos-0.97.0/.gitattributes
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 packitos-0.97.0/.packit.yaml
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 packitos-0.97.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 packitos-0.97.0/.zuul.yaml
--rw-r--r--   0        0        0    57828 2020-02-02 00:00:00.000000 packitos-0.97.0/CHANGELOG.md
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 packitos-0.97.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 packitos-0.97.0/Containerfile
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 packitos-0.97.0/Containerfile.tests
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 packitos-0.97.0/DCO
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 packitos-0.97.0/LICENSE_HEADER.txt
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 packitos-0.97.0/Makefile
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 packitos-0.97.0/ansible.cfg
--rw-r--r--   0        0        0    13559 2020-02-02 00:00:00.000000 packitos-0.97.0/packit.spec
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 packitos-0.97.0/release-conf.yaml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 packitos-0.97.0/.fmf/version
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 packitos-0.97.0/.github/stale.yml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 packitos-0.97.0/.github/workflows/build-and-push.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 packitos-0.97.0/.github/workflows/check-release-notes.yml
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 packitos-0.97.0/.github/workflows/do_release.yml
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 packitos-0.97.0/.github/workflows/opened-issues-to-the-board.yml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 packitos-0.97.0/.github/workflows/prepare-release.yml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 packitos-0.97.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0  1843517 2020-02-02 00:00:00.000000 packitos-0.97.0/design/logo-packit.sketch
--rw-r--r--   0        0        0   135444 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/hexsticker.png
--rw-r--r--   0        0        0   132230 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-dark.png
--rw-r--r--   0        0        0    75002 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-extended.jpg
--rw-r--r--   0        0        0    48468 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-extended.png
--rw-r--r--   0        0        0    24881 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-extended.svg
--rw-r--r--   0        0        0   106567 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-guideline.pdf
--rw-r--r--   0        0        0    66141 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-no-borders.jpg
--rw-r--r--   0        0        0   143587 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-no-borders.png
--rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-small.png
--rw-r--r--   0        0        0    70268 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-square-small-borders.jpg
--rw-r--r--   0        0        0   150044 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-square-small-borders.png
--rw-r--r--   0        0        0    43972 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-stg-square-bigger-borders.svg
--rw-r--r--   0        0        0   107242 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-stg-square-small-borders.png
--rw-r--r--   0        0        0    43981 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-stg-square-small-borders.svg
--rw-r--r--   0        0        0    28826 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-stg.png
--rw-r--r--   0        0        0    24351 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-stg.svg
--rw-r--r--   0        0        0    18005 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-text.jpg
--rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-text.png
--rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-text.svg
--rw-r--r--   0        0        0   144552 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo-white.png
--rw-r--r--   0        0        0   158074 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo.png
--rw-r--r--   0        0        0    14697 2020-02-02 00:00:00.000000 packitos-0.97.0/design/export/logo.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 packitos-0.97.0/files/install-requirements-git.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 packitos-0.97.0/files/install-requirements-pip.yaml
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 packitos-0.97.0/files/install-requirements-rpms.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 packitos-0.97.0/files/local-tests-requirements.yaml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 packitos-0.97.0/files/packit-testing-farm-prepare-session-recording.yaml
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 packitos-0.97.0/files/packit-testing-farm-prepare.yaml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 packitos-0.97.0/files/zuul-reverse-dep-packit-service.yaml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.97.0/files/zuul-tests-session-recording.yaml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 packitos-0.97.0/files/zuul-tests.yaml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 packitos-0.97.0/files/bash-completion/packit
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/build-rpm-deps.yaml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/centpkg.yaml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/generic-dnf-requirements.yaml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/install-packit-service.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/install-packit.yaml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/ogr.yaml
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/packit-service-requirements.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/project-dir.yaml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/python-compile-deps.yaml
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/requre.yaml
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/rpm-test-deps.yaml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/sandcastle.yaml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 packitos-0.97.0/files/tasks/specfile.yaml
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/actions.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/actions_handler.py
--rw-r--r--   0        0        0    93688 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/api.py
--rw-r--r--   0        0        0    24887 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/base_git.py
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/command_handler.py
--rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/constants.py
--rw-r--r--   0        0        0    20419 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/copr_helper.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/dist_git_instance.py
--rw-r--r--   0        0        0    26575 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/distgit.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/exceptions.py
--rw-r--r--   0        0        0    40197 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/local_project.py
--rw-r--r--   0        0        0    35127 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/patches.py
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/pkgtool.py
--rw-r--r--   0        0        0    29596 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/schema.py
--rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/security.py
--rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/source_git.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/status.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/sync.py
--rw-r--r--   0        0        0    54070 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/upstream.py
--rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/vm_image_build.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/build.py
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/create_update.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/dist_git.py
--rw-r--r--   0        0        0    16593 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/dist_git_init.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/init.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/packit_base.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/prepare_sources.py
--rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/propose_downstream.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/push_updates.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/scan_in_osh.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/source_git.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/source_git_init.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/source_git_status.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/srpm.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/status.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/sync_from_downstream.py
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/types.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/update_dist_git.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/update_source_git.py
--rw-r--r--   0        0        0    13599 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/utils.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/validate_config.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/builds/__init__.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/builds/copr_build.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/builds/in_image_builder.py
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/builds/koji_build.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/builds/local_build.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/cli/builds/mock_build.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/config/__init__.py
--rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/config/aliases.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/config/commands.py
--rw-r--r--   0        0        0    24810 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/config/common_package_config.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/config/config.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/config/job_config.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/config/notifications.py
--rw-r--r--   0        0        0    19870 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/config/package_config.py
--rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/config/package_config_validator.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/config/requirements.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/config/sources.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/data/__init__.py
--rwxr-xr-x   0        0        0     3233 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/data/_packitpatch
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/bodhi.py
--rw-r--r--   0        0        0    10759 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/changelog_helper.py
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/commands.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/decorators.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/extensions.py
--rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/koji_helper.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/logging.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/lookaside.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/monitoring.py
--rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/repo.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/source_script.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/upstream_version.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 packitos-0.97.0/packit/utils/versions.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 packitos-0.97.0/plans/README.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 packitos-0.97.0/plans/full.fmf
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.97.0/plans/git_reference.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.97.0/plans/main.fmf
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.97.0/plans/rpmlint.fmf
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 packitos-0.97.0/plans/session-recording.fmf
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 packitos-0.97.0/plans/smoke.fmf
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/__init__.py
--rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/conftest.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/full.fmf
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/smoke.fmf
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/smoke.sh
--rw-r--r--   0        0        0    22298 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/spellbook.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/copr_config
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/cockpit-ostree/Makefile
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/cockpit-ostree/cockpit-ostree.spec.dg
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/cockpit-ostree/cockpit-ostree.spec.in
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/cockpit-ostree/packit.yaml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/cronie/.cronie.metadata
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/cronie/.gitignore
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/cronie/SOURCES/cronie-1.5.2-restart-on-failure.patch
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/cronie/SOURCES/fix-memory-leaks.patch
--rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/cronie/SOURCES/fix-unsafe-code.patch
--rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/cronie/SPECS/cronie.spec
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/dg-ogr/.packit.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/dg-ogr/README.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/dg-ogr/README.packit
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/dg-ogr/python-ogr.spec
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/dg-ogr/sources
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/dist_git/.packit.yaml
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/dist_git/beer.spec
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/dist_git_with_autochangelog/.packit.yaml
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/dist_git_with_autochangelog/beer.spec
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/edd/.packit.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/edd/LICENSE
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/edd/Makefile
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/edd/README.rst
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/edd/edd
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/edd/edd.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/edd/docs/man.rst
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/empty_changelog/.packit.yaml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/empty_changelog/beer.spec
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/no_version_tag_in_spec/.packit.yaml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/no_version_tag_in_spec/beer.spec
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/no_version_tag_in_spec/source
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/osbuild/.packit.yaml
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/osbuild/__init__.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/osbuild/osbuild.spec
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/osbuild/setup.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/osbuild/sources/test
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/previous/git-diff.patch
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/previous/missing-diff-line.patch
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/previous/unified-diff.patch
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/previous/weird-identical.patch
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/regenerated/git-diff.patch
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/regenerated/missing-diff-line.patch
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/regenerated/unified-diff.patch
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/regenerated/weird-identical.patch
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/rpms/hello/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/rpms/hello/hello.spec
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/src/hello/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/src/hello/.distro/hello.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/patches/src/hello/.distro/source-git.yaml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/rpms/hello/0017-Patch-This..patch
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/rpms/hello/from-git.patch
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/rpms/hello/hello.spec
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/rpms/hello/sources
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/rpms/hello/turn-into-fedora.patch
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/snapd/.packit.yaml
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/snapd/packaging/fedora/fix-spec
--rwxr-xr-x   0        0        0     1866 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/snapd/packaging/fedora/pack-source
--rw-r--r--   0        0        0    18386 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/snapd/packaging/fedora/snapd.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/snapd/packaging/fedora/some-file-to-add
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/snapd/vendor/vendor.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/sourcegit/source_git/ignored_file.txt
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/sourcegit/source_git/.distro/beer.spec
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/sourcegit/source_git/.distro/source-git.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/sourcegit/upstream/big-source-file.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/spec_not_in_root/upstream/.packit.yaml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/spec_not_in_root/upstream/dir_with_spec/beer.spec
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/src/.gitignore
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/src/hello/Makefile
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/src/hello/README.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/src/hello/hello.rs
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/sync_files/a.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/sync_files/b.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/sync_files/c.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/sync_files/example_dir/d.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/sync_files/example_dir/e.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/sync_files/example_dir/f.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/upstream_git/.packit.yaml
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/upstream_git/beer.spec
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/upstream_git_macro_in_source/.packit.yaml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/upstream_git_macro_in_source/beer.spec
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/upstream_git_weird_sources/.packit.yaml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/upstream_git_weird_sources/beer.spec
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/upstream_git_with_multiple_sources/.packit.yaml
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/upstream_git_with_multiple_sources/beer.spec
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/.packit.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/AUDIT
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/BENCHMARKS
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/BUGS
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/COPYING
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/Changelog
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/FAQ
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/INSTALL
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/README
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/README.security
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/REWARD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/SIZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/SPEED
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/TODO
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/TUNING
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/vsftpd.8
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/vsftpd.conf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/vsftpd.conf.5
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/EXAMPLE/example
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/Fedora/vsftpd-generator
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/Fedora/vsftpd.ftpusers
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/Fedora/vsftpd.pam
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/Fedora/vsftpd.service
--rw-r--r--   0        0        0    27817 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/Fedora/vsftpd.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/Fedora/vsftpd.target
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/Fedora/vsftpd.user_list
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/Fedora/vsftpd.xinetd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/Fedora/vsftpd@.service
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/Fedora/vsftpd_conf_migrate.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/RedHat/vsftpd.log
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/data/vsftpd/SECURITY/security
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/functional/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/functional/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/functional/spellbook.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/functional/test_local_build.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/functional/test_prepare_sources.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/functional/test_srpm.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/functional/test_validate_config.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/README.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/bodhi_latest_builds.py
--rw-r--r--   0        0        0    42198 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/bodhi_status_updates.py
--rw-r--r--   0        0        0    15059 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_actions.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_api.py
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_base_git.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_build.py
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_changelog_helper.py
--rw-r--r--   0        0        0    21951 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_copr_build.py
--rw-r--r--   0        0        0    15035 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_create_update.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_distgit.py
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_get_api.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_init.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_local_project.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_pagure.py
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_patches.py
--rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_push_updates.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_security.py
--rw-r--r--   0        0        0    24135 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_source_git.py
--rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_source_git_init.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_source_git_status.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_source_git_synch_push.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_source_git_update_source_git.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_spec.py
--rw-r--r--   0        0        0    21476 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_update.py
--rw-r--r--   0        0        0    20736 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_upstream.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_using_cockpit.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_using_examples.py
--rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_validate_config.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/test_validate_synced_files.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/integration/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/conftest.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_actions.py
--rw-r--r--   0        0        0    20023 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_api.py
--rw-r--r--   0        0        0    34586 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_base_git.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_cli.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_cli_utils.py
--rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_copr_helper.py
--rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_dg.py
--rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_dist_git_init.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_image_builder.py
--rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_iterate_packages.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_koji_build.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_load_authentication.py
--rw-r--r--   0        0        0    34254 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_local_project.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_login_with_kerberos.py
--rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_patches.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_prepare_sources.py
--rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_propose_downstream.py
--rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_security.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_specfile.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_status.py
--rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_sync.py
--rw-r--r--   0        0        0    20147 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_upstream.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/test_utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/config/__init__.py
--rw-r--r--   0        0        0    22698 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/config/test_config.py
--rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/config/test_config_aliases.py
--rw-r--r--   0        0        0    95205 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/config/test_package_config.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/utils/test_changelog_helper.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/utils/test_commands.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/utils/test_decorators.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/utils/test_dist_git_instance.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/utils/test_exceptions.py
--rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/utils/test_koji_helper.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/utils/test_lookaside.py
--rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/utils/test_repo.py
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/utils/test_source_script.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/utils/test_upstream_version.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 packitos-0.97.0/tests/unit/utils/test_versions.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/__init__.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/main.fmf
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_api.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_base_git.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_image_builder.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_local_project.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_repository_cache.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_status.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/testbase.py
--rw-r--r--   0        0        0   513530 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml
--rw-r--r--   0        0        0    53824 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz
--rw-r--r--   0        0        0  1387468 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz
--rw-r--r--   0        0        0   162050 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.packit-dist-gitfnk035np_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0  1425896 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    86697 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml
--rw-r--r--   0        0        0    64940 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.tmp5bwaoc9m_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml
--rw-r--r--   0        0        0    34569 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr_no_merge.yaml
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone2_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0  2668265 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml.tmpgtdjxv_x_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    43243 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.packit-dist-gitzea090jp_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.tmpv3zw6n9v_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0   155977 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.packit-dist-gitl12hm88e_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.tmpyqn3l5sr_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0   152944 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml.tmp9u1xyoyx_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    40654 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_status.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_status.yaml.tmp620nfd0i_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    70501 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml.tmpco60quxn_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.97.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 packitos-0.97.0/LICENSE
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 packitos-0.97.0/README.md
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 packitos-0.97.0/pyproject.toml
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 packitos-0.97.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 packitos-0.97.1/.git_archival.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 packitos-0.97.1/.gitattributes
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 packitos-0.97.1/.packit.yaml
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 packitos-0.97.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 packitos-0.97.1/.zuul.yaml
+-rw-r--r--   0        0        0    57944 2020-02-02 00:00:00.000000 packitos-0.97.1/CHANGELOG.md
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 packitos-0.97.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 packitos-0.97.1/Containerfile
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 packitos-0.97.1/Containerfile.tests
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 packitos-0.97.1/DCO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 packitos-0.97.1/LICENSE_HEADER.txt
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 packitos-0.97.1/Makefile
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 packitos-0.97.1/ansible.cfg
+-rw-r--r--   0        0        0    13650 2020-02-02 00:00:00.000000 packitos-0.97.1/packit.spec
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 packitos-0.97.1/release-conf.yaml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 packitos-0.97.1/.fmf/version
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 packitos-0.97.1/.github/stale.yml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 packitos-0.97.1/.github/workflows/build-and-push.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 packitos-0.97.1/.github/workflows/check-release-notes.yml
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 packitos-0.97.1/.github/workflows/do_release.yml
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 packitos-0.97.1/.github/workflows/opened-issues-to-the-board.yml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 packitos-0.97.1/.github/workflows/prepare-release.yml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 packitos-0.97.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0  1843517 2020-02-02 00:00:00.000000 packitos-0.97.1/design/logo-packit.sketch
+-rw-r--r--   0        0        0   135444 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/hexsticker.png
+-rw-r--r--   0        0        0   132230 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-dark.png
+-rw-r--r--   0        0        0    75002 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-extended.jpg
+-rw-r--r--   0        0        0    48468 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-extended.png
+-rw-r--r--   0        0        0    24881 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-extended.svg
+-rw-r--r--   0        0        0   106567 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-guideline.pdf
+-rw-r--r--   0        0        0    66141 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-no-borders.jpg
+-rw-r--r--   0        0        0   143587 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-no-borders.png
+-rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-small.png
+-rw-r--r--   0        0        0    70268 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-square-small-borders.jpg
+-rw-r--r--   0        0        0   150044 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-square-small-borders.png
+-rw-r--r--   0        0        0    43972 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-stg-square-bigger-borders.svg
+-rw-r--r--   0        0        0   107242 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-stg-square-small-borders.png
+-rw-r--r--   0        0        0    43981 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-stg-square-small-borders.svg
+-rw-r--r--   0        0        0    28826 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-stg.png
+-rw-r--r--   0        0        0    24351 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-stg.svg
+-rw-r--r--   0        0        0    18005 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-text.jpg
+-rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-text.png
+-rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-text.svg
+-rw-r--r--   0        0        0   144552 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo-white.png
+-rw-r--r--   0        0        0   158074 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo.png
+-rw-r--r--   0        0        0    14697 2020-02-02 00:00:00.000000 packitos-0.97.1/design/export/logo.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 packitos-0.97.1/files/install-requirements-git.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 packitos-0.97.1/files/install-requirements-pip.yaml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 packitos-0.97.1/files/install-requirements-rpms.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 packitos-0.97.1/files/local-tests-requirements.yaml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 packitos-0.97.1/files/packit-testing-farm-prepare-session-recording.yaml
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 packitos-0.97.1/files/packit-testing-farm-prepare.yaml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 packitos-0.97.1/files/zuul-reverse-dep-packit-service.yaml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.97.1/files/zuul-tests-session-recording.yaml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 packitos-0.97.1/files/zuul-tests.yaml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 packitos-0.97.1/files/bash-completion/packit
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/build-rpm-deps.yaml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/centpkg.yaml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/generic-dnf-requirements.yaml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/install-packit-service.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/install-packit.yaml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/ogr.yaml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/packit-service-requirements.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/project-dir.yaml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/python-compile-deps.yaml
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/requre.yaml
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/rpm-test-deps.yaml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/sandcastle.yaml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 packitos-0.97.1/files/tasks/specfile.yaml
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/__init__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/actions.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/actions_handler.py
+-rw-r--r--   0        0        0    93688 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/api.py
+-rw-r--r--   0        0        0    24887 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/base_git.py
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/command_handler.py
+-rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/constants.py
+-rw-r--r--   0        0        0    20419 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/copr_helper.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/dist_git_instance.py
+-rw-r--r--   0        0        0    26575 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/distgit.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/exceptions.py
+-rw-r--r--   0        0        0    40197 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/local_project.py
+-rw-r--r--   0        0        0    35127 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/patches.py
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/pkgtool.py
+-rw-r--r--   0        0        0    29596 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/schema.py
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/security.py
+-rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/source_git.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/status.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/sync.py
+-rw-r--r--   0        0        0    54070 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/upstream.py
+-rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/vm_image_build.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/build.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/create_update.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/dist_git.py
+-rw-r--r--   0        0        0    16666 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/dist_git_init.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/init.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/packit_base.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/prepare_sources.py
+-rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/propose_downstream.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/push_updates.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/scan_in_osh.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/source_git.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/source_git_init.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/source_git_status.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/srpm.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/status.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/sync_from_downstream.py
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/types.py
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/update_dist_git.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/update_source_git.py
+-rw-r--r--   0        0        0    13599 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/utils.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/validate_config.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/builds/__init__.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/builds/copr_build.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/builds/in_image_builder.py
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/builds/koji_build.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/builds/local_build.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/cli/builds/mock_build.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/config/__init__.py
+-rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/config/aliases.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/config/commands.py
+-rw-r--r--   0        0        0    24810 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/config/common_package_config.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/config/config.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/config/job_config.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/config/notifications.py
+-rw-r--r--   0        0        0    19870 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/config/package_config.py
+-rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/config/package_config_validator.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/config/requirements.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/config/sources.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/data/__init__.py
+-rwxr-xr-x   0        0        0     3233 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/data/_packitpatch
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/bodhi.py
+-rw-r--r--   0        0        0    10759 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/changelog_helper.py
+-rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/commands.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/decorators.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/extensions.py
+-rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/koji_helper.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/logging.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/lookaside.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/monitoring.py
+-rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/repo.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/source_script.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/upstream_version.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 packitos-0.97.1/packit/utils/versions.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 packitos-0.97.1/plans/README.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 packitos-0.97.1/plans/full.fmf
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.97.1/plans/git_reference.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.97.1/plans/main.fmf
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.97.1/plans/rpmlint.fmf
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 packitos-0.97.1/plans/session-recording.fmf
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 packitos-0.97.1/plans/smoke.fmf
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/__init__.py
+-rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/conftest.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/full.fmf
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/smoke.fmf
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/smoke.sh
+-rw-r--r--   0        0        0    22298 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/spellbook.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/copr_config
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/cockpit-ostree/Makefile
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/cockpit-ostree/cockpit-ostree.spec.dg
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/cockpit-ostree/cockpit-ostree.spec.in
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/cockpit-ostree/packit.yaml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/cronie/.cronie.metadata
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/cronie/.gitignore
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/cronie/SOURCES/cronie-1.5.2-restart-on-failure.patch
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/cronie/SOURCES/fix-memory-leaks.patch
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/cronie/SOURCES/fix-unsafe-code.patch
+-rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/cronie/SPECS/cronie.spec
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/dg-ogr/.packit.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/dg-ogr/README.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/dg-ogr/README.packit
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/dg-ogr/python-ogr.spec
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/dg-ogr/sources
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/dist_git/.packit.yaml
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/dist_git/beer.spec
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/dist_git_with_autochangelog/.packit.yaml
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/dist_git_with_autochangelog/beer.spec
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/edd/.packit.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/edd/LICENSE
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/edd/Makefile
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/edd/README.rst
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/edd/edd
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/edd/edd.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/edd/docs/man.rst
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/empty_changelog/.packit.yaml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/empty_changelog/beer.spec
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/no_version_tag_in_spec/.packit.yaml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/no_version_tag_in_spec/beer.spec
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/no_version_tag_in_spec/source
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/osbuild/.packit.yaml
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/osbuild/__init__.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/osbuild/osbuild.spec
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/osbuild/setup.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/osbuild/sources/test
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/previous/git-diff.patch
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/previous/missing-diff-line.patch
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/previous/unified-diff.patch
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/previous/weird-identical.patch
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/regenerated/git-diff.patch
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/regenerated/missing-diff-line.patch
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/regenerated/unified-diff.patch
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/regenerated/weird-identical.patch
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/rpms/hello/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/rpms/hello/hello.spec
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/src/hello/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/src/hello/.distro/hello.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/patches/src/hello/.distro/source-git.yaml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/rpms/hello/0017-Patch-This..patch
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/rpms/hello/from-git.patch
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/rpms/hello/hello.spec
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/rpms/hello/sources
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/rpms/hello/turn-into-fedora.patch
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/snapd/.packit.yaml
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/snapd/packaging/fedora/fix-spec
+-rwxr-xr-x   0        0        0     1866 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/snapd/packaging/fedora/pack-source
+-rw-r--r--   0        0        0    18386 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/snapd/packaging/fedora/snapd.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/snapd/packaging/fedora/some-file-to-add
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/snapd/vendor/vendor.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/sourcegit/source_git/ignored_file.txt
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/sourcegit/source_git/.distro/beer.spec
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/sourcegit/source_git/.distro/source-git.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/sourcegit/upstream/big-source-file.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/spec_not_in_root/upstream/.packit.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/spec_not_in_root/upstream/dir_with_spec/beer.spec
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/src/.gitignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/src/hello/Makefile
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/src/hello/README.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/src/hello/hello.rs
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/sync_files/a.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/sync_files/b.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/sync_files/c.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/sync_files/example_dir/d.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/sync_files/example_dir/e.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/sync_files/example_dir/f.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/upstream_git/.packit.yaml
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/upstream_git/beer.spec
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/upstream_git_macro_in_source/.packit.yaml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/upstream_git_macro_in_source/beer.spec
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/upstream_git_weird_sources/.packit.yaml
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/upstream_git_weird_sources/beer.spec
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/upstream_git_with_multiple_sources/.packit.yaml
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/upstream_git_with_multiple_sources/beer.spec
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/.packit.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/AUDIT
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/BENCHMARKS
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/BUGS
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/COPYING
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/Changelog
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/FAQ
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/INSTALL
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/README
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/README.security
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/REWARD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/SIZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/SPEED
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/TODO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/TUNING
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/vsftpd.8
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/vsftpd.conf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/vsftpd.conf.5
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/EXAMPLE/example
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/Fedora/vsftpd-generator
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/Fedora/vsftpd.ftpusers
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/Fedora/vsftpd.pam
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/Fedora/vsftpd.service
+-rw-r--r--   0        0        0    27817 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/Fedora/vsftpd.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/Fedora/vsftpd.target
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/Fedora/vsftpd.user_list
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/Fedora/vsftpd.xinetd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/Fedora/vsftpd@.service
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/Fedora/vsftpd_conf_migrate.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/RedHat/vsftpd.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/data/vsftpd/SECURITY/security
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/functional/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/functional/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/functional/spellbook.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/functional/test_local_build.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/functional/test_prepare_sources.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/functional/test_srpm.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/functional/test_validate_config.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/README.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/bodhi_latest_builds.py
+-rw-r--r--   0        0        0    42198 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/bodhi_status_updates.py
+-rw-r--r--   0        0        0    15059 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_actions.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_api.py
+-rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_base_git.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_build.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_changelog_helper.py
+-rw-r--r--   0        0        0    21951 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_copr_build.py
+-rw-r--r--   0        0        0    15035 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_create_update.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_distgit.py
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_get_api.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_init.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_local_project.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_pagure.py
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_patches.py
+-rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_push_updates.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_security.py
+-rw-r--r--   0        0        0    24135 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_source_git.py
+-rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_source_git_init.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_source_git_status.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_source_git_synch_push.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_source_git_update_source_git.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_spec.py
+-rw-r--r--   0        0        0    21476 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_update.py
+-rw-r--r--   0        0        0    20736 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_upstream.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_using_cockpit.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_using_examples.py
+-rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_validate_config.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/test_validate_synced_files.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/integration/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/conftest.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_actions.py
+-rw-r--r--   0        0        0    20023 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_api.py
+-rw-r--r--   0        0        0    34586 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_base_git.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_cli.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_cli_utils.py
+-rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_copr_helper.py
+-rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_dg.py
+-rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_dist_git_init.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_image_builder.py
+-rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_iterate_packages.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_koji_build.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_load_authentication.py
+-rw-r--r--   0        0        0    34254 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_local_project.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_login_with_kerberos.py
+-rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_patches.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_prepare_sources.py
+-rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_propose_downstream.py
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_security.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_specfile.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_status.py
+-rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_sync.py
+-rw-r--r--   0        0        0    20147 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_upstream.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/test_utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/config/__init__.py
+-rw-r--r--   0        0        0    22698 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/config/test_config.py
+-rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/config/test_config_aliases.py
+-rw-r--r--   0        0        0    95205 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/config/test_package_config.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/utils/test_changelog_helper.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/utils/test_commands.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/utils/test_decorators.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/utils/test_dist_git_instance.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/utils/test_exceptions.py
+-rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/utils/test_koji_helper.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/utils/test_lookaside.py
+-rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/utils/test_repo.py
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/utils/test_source_script.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/utils/test_upstream_version.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 packitos-0.97.1/tests/unit/utils/test_versions.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/main.fmf
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_api.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_base_git.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_image_builder.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_local_project.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_repository_cache.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_status.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/testbase.py
+-rw-r--r--   0        0        0   513530 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml
+-rw-r--r--   0        0        0    53824 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz
+-rw-r--r--   0        0        0  1387468 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz
+-rw-r--r--   0        0        0   162050 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.packit-dist-gitfnk035np_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0  1425896 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    86697 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml
+-rw-r--r--   0        0        0    64940 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.tmp5bwaoc9m_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml
+-rw-r--r--   0        0        0    34569 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr_no_merge.yaml
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone2_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0  2668265 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml.tmpgtdjxv_x_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    43243 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.packit-dist-gitzea090jp_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.tmpv3zw6n9v_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0   155977 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.packit-dist-gitl12hm88e_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.tmpyqn3l5sr_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0   152944 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml.tmp9u1xyoyx_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    40654 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_status.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_status.yaml.tmp620nfd0i_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    70501 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml.tmpco60quxn_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.97.1/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 packitos-0.97.1/LICENSE
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 packitos-0.97.1/README.md
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 packitos-0.97.1/pyproject.toml
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 packitos-0.97.1/PKG-INFO
```

### Comparing `packitos-0.97.0/.packit.yaml` & `packitos-0.97.1/.packit.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/.pre-commit-config.yaml` & `packitos-0.97.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/.zuul.yaml` & `packitos-0.97.1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/CHANGELOG.md` & `packitos-0.97.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 0.97.1
+
+- We have fixed the behaviour for `dist-git init` command when `upstream-git-url` argument is specified.
+
 # 0.97.0
 
 - Add a `scan-in-osh` subcommand in the CLI to perform a scan through OpenScanHub. By default, it performs a full scan of the packages and a differential scan can be performed through `--base-srpm` option. (#2301)
 - When running `dist-git init` command from CLI, you can pass a command to specify a git URL of the project. (#2308)
 
 # 0.96.0
```

### Comparing `packitos-0.97.0/CONTRIBUTING.md` & `packitos-0.97.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/DCO` & `packitos-0.97.1/DCO`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/Makefile` & `packitos-0.97.1/Makefile`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit.spec` & `packitos-0.97.1/packit.spec`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 %if 0%{?el9}
 %bcond_with tests
 %else
 %bcond_without tests
 %endif
 
 Name:           packit
-Version:        0.97.0
+Version:        0.97.1
 Release:        1%{?dist}
 Summary:        A tool for integrating upstream projects with Fedora operating system
 
 License:        MIT
 URL:            https://github.com/packit/packit
 Source0:        %{pypi_source packitos}
 BuildArch:      noarch
@@ -75,14 +75,17 @@
 # Epel9 does not tag the license file in pyproject_files as a license. Manually install it in this case
 %if 0%{?el9}
 %license LICENSE
 %endif
 %doc README.md
 
 %changelog
+* Fri May 17 2024 Packit Team <hello@packit.dev> - 0.97.1-1
+- New upstream release 0.97.1
+
 * Fri May 10 2024 Packit Team <hello@packit.dev> - 0.97.0-1
 - New upstream release 0.97.0
 
 * Fri May 03 2024 Packit Team <hello@packit.dev> - 0.96.0-1
 - New upstream release 0.96.0
 
 * Sat Apr 20 2024 Packit Team <hello@packit.dev> - 0.95.0-1
```

### Comparing `packitos-0.97.0/.github/stale.yml` & `packitos-0.97.1/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/.github/workflows/build-and-push.yml` & `packitos-0.97.1/.github/workflows/build-and-push.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/.github/workflows/do_release.yml` & `packitos-0.97.1/.github/workflows/do_release.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/.github/workflows/prepare-release.yml` & `packitos-0.97.1/.github/workflows/prepare-release.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/.github/workflows/pypi-publish.yml` & `packitos-0.97.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/logo-packit.sketch` & `packitos-0.97.1/design/logo-packit.sketch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/hexsticker.png` & `packitos-0.97.1/design/export/hexsticker.png`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-dark.png` & `packitos-0.97.1/design/export/logo-dark.png`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-extended.jpg` & `packitos-0.97.1/design/export/logo-extended.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-extended.png` & `packitos-0.97.1/design/export/logo-extended.png`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-extended.svg` & `packitos-0.97.1/design/export/logo-extended.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-guideline.pdf` & `packitos-0.97.1/design/export/logo-guideline.pdf`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-no-borders.jpg` & `packitos-0.97.1/design/export/logo-no-borders.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-no-borders.png` & `packitos-0.97.1/design/export/logo-no-borders.png`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-small.png` & `packitos-0.97.1/design/export/logo-small.png`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-square-small-borders.jpg` & `packitos-0.97.1/design/export/logo-square-small-borders.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-square-small-borders.png` & `packitos-0.97.1/design/export/logo-square-small-borders.png`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-stg-square-bigger-borders.svg` & `packitos-0.97.1/design/export/logo-stg-square-bigger-borders.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-stg-square-small-borders.png` & `packitos-0.97.1/design/export/logo-stg-square-small-borders.png`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-stg-square-small-borders.svg` & `packitos-0.97.1/design/export/logo-stg-square-small-borders.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-stg.png` & `packitos-0.97.1/design/export/logo-stg.png`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-stg.svg` & `packitos-0.97.1/design/export/logo-stg.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-text.jpg` & `packitos-0.97.1/design/export/logo-text.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-text.png` & `packitos-0.97.1/design/export/logo-text.png`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-text.svg` & `packitos-0.97.1/design/export/logo-text.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo-white.png` & `packitos-0.97.1/design/export/logo-white.png`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo.png` & `packitos-0.97.1/design/export/logo.png`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/design/export/logo.svg` & `packitos-0.97.1/design/export/logo.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/files/local-tests-requirements.yaml` & `packitos-0.97.1/files/local-tests-requirements.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/files/zuul-reverse-dep-packit-service.yaml` & `packitos-0.97.1/files/zuul-reverse-dep-packit-service.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/files/zuul-tests-session-recording.yaml` & `packitos-0.97.1/files/zuul-tests-session-recording.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/files/tasks/packit-service-requirements.yaml` & `packitos-0.97.1/files/tasks/packit-service-requirements.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/files/tasks/rpm-test-deps.yaml` & `packitos-0.97.1/files/tasks/rpm-test-deps.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/actions.py` & `packitos-0.97.1/packit/actions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/actions_handler.py` & `packitos-0.97.1/packit/actions_handler.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/api.py` & `packitos-0.97.1/packit/api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/base_git.py` & `packitos-0.97.1/packit/base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/command_handler.py` & `packitos-0.97.1/packit/command_handler.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/constants.py` & `packitos-0.97.1/packit/constants.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/copr_helper.py` & `packitos-0.97.1/packit/copr_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/dist_git_instance.py` & `packitos-0.97.1/packit/dist_git_instance.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/distgit.py` & `packitos-0.97.1/packit/distgit.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/exceptions.py` & `packitos-0.97.1/packit/exceptions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/local_project.py` & `packitos-0.97.1/packit/local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/patches.py` & `packitos-0.97.1/packit/patches.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/pkgtool.py` & `packitos-0.97.1/packit/pkgtool.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/schema.py` & `packitos-0.97.1/packit/schema.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/security.py` & `packitos-0.97.1/packit/security.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/source_git.py` & `packitos-0.97.1/packit/source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/status.py` & `packitos-0.97.1/packit/status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/sync.py` & `packitos-0.97.1/packit/sync.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/upstream.py` & `packitos-0.97.1/packit/upstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/vm_image_build.py` & `packitos-0.97.1/packit/vm_image_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/build.py` & `packitos-0.97.1/packit/cli/build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/create_update.py` & `packitos-0.97.1/packit/cli/create_update.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/dist_git_init.py` & `packitos-0.97.1/packit/cli/dist_git_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,24 +231,25 @@
     if not (upstream_git_url or upstream_git_url_command):
         click.echo(
             "One of --upstream-git-url or --upstream-git-url-command needs to be specified.",
             err=True,
         )
         return
 
-    click.echo(
-        f"Running the following command to find upstream git URL: {upstream_git_url_command}",
-    )
-    result = commands.run_command(
-        upstream_git_url_command,
-        output=True,
-        cwd=path_or_url.working_dir,
-    )
-    upstream_git_url = result.stdout.strip()
-    click.echo(f"Found the following URL: {upstream_git_url}")
+    if upstream_git_url_command:
+        click.echo(
+            f"Running the following command to find upstream git URL: {upstream_git_url_command}",
+        )
+        result = commands.run_command(
+            upstream_git_url_command,
+            output=True,
+            cwd=path_or_url.working_dir,
+        )
+        upstream_git_url = result.stdout.strip()
+        click.echo(f"Found the following URL: {upstream_git_url}")
 
     DistGitInitializer(
         upstream_git_url=upstream_git_url,
         upstream_tag_template=upstream_tag_template,
         upstream_tag_include=upstream_tag_include,
         upstream_tag_exclude=upstream_tag_exclude,
         version_update_mask=version_update_mask,
```

### Comparing `packitos-0.97.0/packit/cli/init.py` & `packitos-0.97.1/packit/cli/init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/packit_base.py` & `packitos-0.97.1/packit/cli/packit_base.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/prepare_sources.py` & `packitos-0.97.1/packit/cli/prepare_sources.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/propose_downstream.py` & `packitos-0.97.1/packit/cli/propose_downstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/push_updates.py` & `packitos-0.97.1/packit/cli/push_updates.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/scan_in_osh.py` & `packitos-0.97.1/packit/cli/scan_in_osh.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/source_git.py` & `packitos-0.97.1/packit/cli/source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/source_git_init.py` & `packitos-0.97.1/packit/cli/source_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/source_git_status.py` & `packitos-0.97.1/packit/cli/source_git_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/srpm.py` & `packitos-0.97.1/packit/cli/srpm.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/status.py` & `packitos-0.97.1/packit/cli/status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/sync_from_downstream.py` & `packitos-0.97.1/packit/cli/sync_from_downstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/types.py` & `packitos-0.97.1/packit/cli/types.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/update_dist_git.py` & `packitos-0.97.1/packit/cli/update_dist_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/update_source_git.py` & `packitos-0.97.1/packit/cli/update_source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/utils.py` & `packitos-0.97.1/packit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/validate_config.py` & `packitos-0.97.1/packit/cli/validate_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/builds/copr_build.py` & `packitos-0.97.1/packit/cli/builds/copr_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/builds/in_image_builder.py` & `packitos-0.97.1/packit/cli/builds/in_image_builder.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/builds/koji_build.py` & `packitos-0.97.1/packit/cli/builds/koji_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/builds/local_build.py` & `packitos-0.97.1/packit/cli/builds/local_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/cli/builds/mock_build.py` & `packitos-0.97.1/packit/cli/builds/mock_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/config/__init__.py` & `packitos-0.97.1/packit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/config/aliases.py` & `packitos-0.97.1/packit/config/aliases.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/config/common_package_config.py` & `packitos-0.97.1/packit/config/common_package_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/config/config.py` & `packitos-0.97.1/packit/config/config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/config/job_config.py` & `packitos-0.97.1/packit/config/job_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/config/notifications.py` & `packitos-0.97.1/packit/config/notifications.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/config/package_config.py` & `packitos-0.97.1/packit/config/package_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/config/package_config_validator.py` & `packitos-0.97.1/packit/config/package_config_validator.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/config/requirements.py` & `packitos-0.97.1/packit/config/requirements.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/data/_packitpatch` & `packitos-0.97.1/packit/data/_packitpatch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/__init__.py` & `packitos-0.97.1/packit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/bodhi.py` & `packitos-0.97.1/packit/utils/bodhi.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/changelog_helper.py` & `packitos-0.97.1/packit/utils/changelog_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/commands.py` & `packitos-0.97.1/packit/utils/commands.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/decorators.py` & `packitos-0.97.1/packit/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/extensions.py` & `packitos-0.97.1/packit/utils/extensions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/koji_helper.py` & `packitos-0.97.1/packit/utils/koji_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,36 @@
             logger.debug(f"Failed to get changelog of build {nvr} from Koji: {e}")
             return []
         for k, v in headers.items():
             if not isinstance(v, list):
                 headers[k] = [v]
         return list(zip(*[headers[h] for h in requested_headers]))
 
+    def get_builds_in_tag(self, tag: str) -> list[dict]:
+        """
+        Gets list of builds tagged into the specified tag.
+
+        Args:
+            tag: Tag name.
+
+        Returns:
+            List of builds.
+        """
+        try:
+            builds = self.session.listTagged(
+                tag=tag,
+                inherit=False,
+                latest=False,
+                strict=True,
+            )
+        except Exception as e:
+            logger.debug(f"Failed to get builds tagged into {tag} from Koji: {e}")
+            return []
+        return builds
+
     def get_tag_info(self, tag: str) -> Optional[dict]:
         """
         Gets tag information.
 
         Args:
             tag: Koji tag.
```

### Comparing `packitos-0.97.0/packit/utils/logging.py` & `packitos-0.97.1/packit/utils/logging.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/lookaside.py` & `packitos-0.97.1/packit/utils/lookaside.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/monitoring.py` & `packitos-0.97.1/packit/utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/repo.py` & `packitos-0.97.1/packit/utils/repo.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/source_script.py` & `packitos-0.97.1/packit/utils/source_script.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/upstream_version.py` & `packitos-0.97.1/packit/utils/upstream_version.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/packit/utils/versions.py` & `packitos-0.97.1/packit/utils/versions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/plans/full.fmf` & `packitos-0.97.1/plans/full.fmf`

 * *Files 27% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     because: "have the latest builds of ogr and specfile available for upstream test jobs"
     prepare+:
       # enable packit-dev Copr repo to get the latest builds of ogr and specfile
       - how: install
         copr: packit/packit-dev
       # make sure the Copr repo has higher priority than TF Tag Repository
       - how: shell
-        script: dnf -y config-manager --save --setopt="*:packit:packit-dev.priority=5"
+        script: sed -i -n '/^priority=/!p;$apriority=5' /etc/yum.repos.d/*:packit:packit-dev.repo
       # upgrade ogr and specfile in case they are already installed
       - how: shell
         script: dnf -y upgrade python3-ogr python3-specfile
   - when: "distro == rhel-9 or distro == centos-9 or distro == centos-stream-9"
     because: "build and deepdiff are not in EPEL 9"
     prepare+:
       - how: install
```

### Comparing `packitos-0.97.0/plans/session-recording.fmf` & `packitos-0.97.1/plans/session-recording.fmf`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     because: "have the latest builds of ogr and specfile available for upstream test jobs"
     prepare+:
       # enable packit-dev Copr repo to get the latest builds of ogr and specfile
       - how: install
         copr: packit/packit-dev
       # make sure the Copr repo has higher priority than TF Tag Repository
       - how: shell
-        script: dnf -y config-manager --save --setopt="*:packit:packit-dev.priority=5"
+        script: sed -i -n '/^priority=/!p;$apriority=5' /etc/yum.repos.d/*:packit:packit-dev.repo
       # upgrade ogr and specfile in case they are already installed
       - how: shell
         script: dnf -y upgrade python3-ogr python3-specfile
   - when: "distro <= rhel-9 or distro <= centos-9 or distro == centos-stream-8 or distro == centos-stream-9"
     prepare+:
       - how: install
         name: Enable the Copr-repo for Requre
```

### Comparing `packitos-0.97.0/tests/conftest.py` & `packitos-0.97.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/full.fmf` & `packitos-0.97.1/tests/full.fmf`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/spellbook.py` & `packitos-0.97.1/tests/spellbook.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/cockpit-ostree/Makefile` & `packitos-0.97.1/tests/data/cockpit-ostree/Makefile`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/cockpit-ostree/cockpit-ostree.spec.dg` & `packitos-0.97.1/tests/data/cockpit-ostree/cockpit-ostree.spec.dg`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/cockpit-ostree/cockpit-ostree.spec.in` & `packitos-0.97.1/tests/data/cockpit-ostree/cockpit-ostree.spec.in`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch` & `packitos-0.97.1/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/cronie/SOURCES/fix-memory-leaks.patch` & `packitos-0.97.1/tests/data/cronie/SOURCES/fix-memory-leaks.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/cronie/SOURCES/fix-unsafe-code.patch` & `packitos-0.97.1/tests/data/cronie/SOURCES/fix-unsafe-code.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/cronie/SPECS/cronie.spec` & `packitos-0.97.1/tests/data/cronie/SPECS/cronie.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/dg-ogr/.packit.yaml` & `packitos-0.97.1/tests/data/dg-ogr/.packit.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/dg-ogr/python-ogr.spec` & `packitos-0.97.1/tests/data/dg-ogr/python-ogr.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/edd/Makefile` & `packitos-0.97.1/tests/data/edd/Makefile`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/edd/edd.spec` & `packitos-0.97.1/tests/data/edd/edd.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/osbuild/osbuild.spec` & `packitos-0.97.1/tests/data/osbuild/osbuild.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/patches/previous/git-diff.patch` & `packitos-0.97.1/tests/data/patches/previous/git-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/patches/previous/missing-diff-line.patch` & `packitos-0.97.1/tests/data/patches/previous/missing-diff-line.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/patches/previous/unified-diff.patch` & `packitos-0.97.1/tests/data/patches/previous/unified-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/patches/previous/weird-identical.patch` & `packitos-0.97.1/tests/data/patches/previous/weird-identical.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/patches/regenerated/git-diff.patch` & `packitos-0.97.1/tests/data/patches/regenerated/git-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/patches/regenerated/missing-diff-line.patch` & `packitos-0.97.1/tests/data/patches/regenerated/missing-diff-line.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/patches/regenerated/unified-diff.patch` & `packitos-0.97.1/tests/data/patches/regenerated/unified-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/patches/regenerated/weird-identical.patch` & `packitos-0.97.1/tests/data/patches/regenerated/weird-identical.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/rpms/hello/0017-Patch-This..patch` & `packitos-0.97.1/tests/data/rpms/hello/0017-Patch-This..patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/rpms/hello/from-git.patch` & `packitos-0.97.1/tests/data/rpms/hello/from-git.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/snapd/packaging/fedora/fix-spec` & `packitos-0.97.1/tests/data/snapd/packaging/fedora/fix-spec`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/snapd/packaging/fedora/pack-source` & `packitos-0.97.1/tests/data/snapd/packaging/fedora/pack-source`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/snapd/packaging/fedora/snapd.spec` & `packitos-0.97.1/tests/data/snapd/packaging/fedora/snapd.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/snapd/vendor/vendor.json` & `packitos-0.97.1/tests/data/snapd/vendor/vendor.json`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/sourcegit/source_git/.distro/beer.spec` & `packitos-0.97.1/tests/data/sourcegit/source_git/.distro/beer.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/upstream_git/beer.spec` & `packitos-0.97.1/tests/data/upstream_git/beer.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/upstream_git_macro_in_source/beer.spec` & `packitos-0.97.1/tests/data/upstream_git_macro_in_source/beer.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/data/vsftpd/Fedora/vsftpd.spec` & `packitos-0.97.1/tests/data/vsftpd/Fedora/vsftpd.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/functional/spellbook.py` & `packitos-0.97.1/tests/functional/spellbook.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/functional/test_local_build.py` & `packitos-0.97.1/tests/functional/test_local_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/functional/test_prepare_sources.py` & `packitos-0.97.1/tests/functional/test_prepare_sources.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/functional/test_srpm.py` & `packitos-0.97.1/tests/functional/test_srpm.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/bodhi_latest_builds.py` & `packitos-0.97.1/tests/integration/bodhi_latest_builds.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/bodhi_status_updates.py` & `packitos-0.97.1/tests/integration/bodhi_status_updates.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/conftest.py` & `packitos-0.97.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_actions.py` & `packitos-0.97.1/tests/integration/test_actions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_api.py` & `packitos-0.97.1/tests/integration/test_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_base_git.py` & `packitos-0.97.1/tests/integration/test_base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_build.py` & `packitos-0.97.1/tests/integration/test_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_changelog_helper.py` & `packitos-0.97.1/tests/integration/test_changelog_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_copr_build.py` & `packitos-0.97.1/tests/integration/test_copr_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_create_update.py` & `packitos-0.97.1/tests/integration/test_create_update.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_get_api.py` & `packitos-0.97.1/tests/integration/test_get_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_init.py` & `packitos-0.97.1/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_local_project.py` & `packitos-0.97.1/tests/integration/test_local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_pagure.py` & `packitos-0.97.1/tests/integration/test_pagure.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_patches.py` & `packitos-0.97.1/tests/integration/test_patches.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_push_updates.py` & `packitos-0.97.1/tests/integration/test_push_updates.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_security.py` & `packitos-0.97.1/tests/integration/test_security.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_source_git.py` & `packitos-0.97.1/tests/integration/test_source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_source_git_init.py` & `packitos-0.97.1/tests/integration/test_source_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_source_git_status.py` & `packitos-0.97.1/tests/integration/test_source_git_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_source_git_synch_push.py` & `packitos-0.97.1/tests/integration/test_source_git_synch_push.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_source_git_update_source_git.py` & `packitos-0.97.1/tests/integration/test_source_git_update_source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_spec.py` & `packitos-0.97.1/tests/integration/test_spec.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_update.py` & `packitos-0.97.1/tests/integration/test_update.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_upstream.py` & `packitos-0.97.1/tests/integration/test_upstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_using_cockpit.py` & `packitos-0.97.1/tests/integration/test_using_cockpit.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_using_examples.py` & `packitos-0.97.1/tests/integration/test_using_examples.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_validate_config.py` & `packitos-0.97.1/tests/integration/test_validate_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/integration/test_validate_synced_files.py` & `packitos-0.97.1/tests/integration/test_validate_synced_files.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/conftest.py` & `packitos-0.97.1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_actions.py` & `packitos-0.97.1/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_api.py` & `packitos-0.97.1/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_base_git.py` & `packitos-0.97.1/tests/unit/test_base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_cli.py` & `packitos-0.97.1/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_cli_utils.py` & `packitos-0.97.1/tests/unit/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_copr_helper.py` & `packitos-0.97.1/tests/unit/test_copr_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_dg.py` & `packitos-0.97.1/tests/unit/test_dg.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_dist_git_init.py` & `packitos-0.97.1/tests/unit/test_dist_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_image_builder.py` & `packitos-0.97.1/tests/unit/test_image_builder.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_iterate_packages.py` & `packitos-0.97.1/tests/unit/test_iterate_packages.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_koji_build.py` & `packitos-0.97.1/tests/unit/test_koji_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_load_authentication.py` & `packitos-0.97.1/tests/unit/test_load_authentication.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_local_project.py` & `packitos-0.97.1/tests/unit/test_local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_login_with_kerberos.py` & `packitos-0.97.1/tests/unit/test_login_with_kerberos.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_patches.py` & `packitos-0.97.1/tests/unit/test_patches.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_prepare_sources.py` & `packitos-0.97.1/tests/unit/test_prepare_sources.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_propose_downstream.py` & `packitos-0.97.1/tests/unit/test_propose_downstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_security.py` & `packitos-0.97.1/tests/unit/test_security.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_specfile.py` & `packitos-0.97.1/tests/unit/test_specfile.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_status.py` & `packitos-0.97.1/tests/unit/test_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_sync.py` & `packitos-0.97.1/tests/unit/test_sync.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_upstream.py` & `packitos-0.97.1/tests/unit/test_upstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/test_utils.py` & `packitos-0.97.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/config/test_config.py` & `packitos-0.97.1/tests/unit/config/test_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/config/test_config_aliases.py` & `packitos-0.97.1/tests/unit/config/test_config_aliases.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/config/test_package_config.py` & `packitos-0.97.1/tests/unit/config/test_package_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/utils/test_changelog_helper.py` & `packitos-0.97.1/tests/unit/utils/test_changelog_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/utils/test_decorators.py` & `packitos-0.97.1/tests/unit/utils/test_decorators.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/utils/test_dist_git_instance.py` & `packitos-0.97.1/tests/unit/utils/test_dist_git_instance.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/utils/test_koji_helper.py` & `packitos-0.97.1/tests/unit/utils/test_koji_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,41 @@
         assert result == changelog
 
 
 @pytest.mark.parametrize(
     "error",
     [False, True],
 )
+def test_get_builds_in_tag(error):
+    builds = [
+        {
+            "package_name": "python-specfile",
+            "name": "python3-specfile",
+            "version": "0.28.0",
+            "release": "1.fc39",
+        },
+    ]
+
+    def listTagged(*_, **__):
+        if error:
+            raise Exception
+        return builds
+
+    session = flexmock(listTagged=listTagged)
+    result = KojiHelper(session).get_builds_in_tag("f39-build-side-12345")
+    if error:
+        assert result == []
+    else:
+        assert result == builds
+
+
+@pytest.mark.parametrize(
+    "error",
+    [False, True],
+)
 def test_get_tag_info(error):
     info = {"name": "f39-build-side-12345", "id": 12345}
 
     def getBuildConfig(*_, **__):
         if error:
             raise Exception
         return info
```

### Comparing `packitos-0.97.0/tests/unit/utils/test_lookaside.py` & `packitos-0.97.1/tests/unit/utils/test_lookaside.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/utils/test_repo.py` & `packitos-0.97.1/tests/unit/utils/test_repo.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/utils/test_source_script.py` & `packitos-0.97.1/tests/unit/utils/test_source_script.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/utils/test_upstream_version.py` & `packitos-0.97.1/tests/unit/utils/test_upstream_version.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests/unit/utils/test_versions.py` & `packitos-0.97.1/tests/unit/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/README.md` & `packitos-0.97.1/tests_recording/README.md`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_api.py` & `packitos-0.97.1/tests_recording/test_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_base_git.py` & `packitos-0.97.1/tests_recording/test_base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_image_builder.py` & `packitos-0.97.1/tests_recording/test_image_builder.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_local_project.py` & `packitos-0.97.1/tests_recording/test_local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_repository_cache.py` & `packitos-0.97.1/tests_recording/test_repository_cache.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_status.py` & `packitos-0.97.1/tests_recording/test_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/testbase.py` & `packitos-0.97.1/tests_recording/testbase.py`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml` & `packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz` & `packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz` & `packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml` & `packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz` & `packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml` & `packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz` & `packitos-0.97.1/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml` & `packitos-0.97.1/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml` & `packitos-0.97.1/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml` & `packitos-0.97.1/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml` & `packitos-0.97.1/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml` & `packitos-0.97.1/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml` & `packitos-0.97.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml` & `packitos-0.97.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml` & `packitos-0.97.1/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml` & `packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml` & `packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml` & `packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml` & `packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_status.yaml` & `packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_status.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml` & `packitos-0.97.1/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/LICENSE` & `packitos-0.97.1/LICENSE`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/README.md` & `packitos-0.97.1/README.md`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/pyproject.toml` & `packitos-0.97.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packitos-0.97.0/PKG-INFO` & `packitos-0.97.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: packitos
-Version: 0.97.0
+Version: 0.97.1
 Summary: A set of tools to integrate upstream open source projects into Fedora operating system.
 Project-URL: Homepage, https://github.com/packit/packit
 Author-email: Red Hat <user-cont-team@redhat.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: dist-git,fedora,git,packaging,rpm
 Classifier: Development Status :: 4 - Beta
```

