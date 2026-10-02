# Network & privacy

This document describes the intended public network behavior of MJYT v1 at a high level.

## Media requests

MJYT connects to YouTube/Google-owned web and media endpoints as necessary to analyze supported public YouTube URLs, resolve media information, and download the selected media.

MJYT v1 does not expose an account-login or cookie-import workflow for private, members-only, rented/purchased, or other account-bound media.

## Version checks

When **Check new versions** is enabled, MJYT performs an asynchronous lookup of the latest public MJYT GitHub release. This allows the application to compare the installed lineage label with the latest published release and show an in-app notification when a newer release exists.

The setting can be disabled in Options to stop these version lookups.

Version checks do not automatically download or execute an update.

## Local retained state

MJYT retains queue/history state and other application preferences locally so work can survive application restart. Some supported interrupted downloads may also retain local partial/resume state until they complete, are retried cleanly, or are removed by the relevant workflow.

## Logs and reports

User-visible logs and benchmark/download reports are intended for local diagnostics. Before posting logs publicly, review them and remove any media URLs, paths, or other information you do not want to share.

## Accounts and credentials

MJYT v1 is designed around public/anonymous YouTube workflows. Do not provide account credentials to MJYT, and do not post credentials or cookies in public issue reports.
