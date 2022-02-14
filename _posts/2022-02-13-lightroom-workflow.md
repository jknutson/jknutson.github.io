---
layout: post
title:  "Lightroom Workflow"
date:   2022-02-13 08:00:00 -0600
tags:   photography
author: John Knutson
---

It's not as efficient or straighforward as I'd like, but it works with Adobe's Lightroom products and meets my needs.
<!--snippet-->

## High Level Workflow

1. Import Photos [from SD card, HDD, etc.] to Lightroom
2. Lightroom syncs photos to Adobe cloud
3. Lightroom Classic syncs photos to local (NAS) storage
4. NAS syncs to BackBlaze B2 cloud

## Particular Settings

### Lightroom Cloud

* uncheck "store a copy of all photos at specified location"

### Lightroom Classic

* check "Specify location for Lightroom’s synced images"
  * location: `/Volumes/media/Pictures/Lightroom`
  * `/Volumes/media` is a mounted network share
* check "Use subfolders formatted by date"
  * format: `2022/2022-02-07`

## Detailed Workflow

1. Import photos [from SD card, HDD, etc.] to Lightroom Cloud
2. Photos sync to Adobe Creative Cloud storage
3. Lightroom Classic syncs photos to “Local” (NAS) storage
4. NAS syncs to BackBlaze B2
    * http://truenas.local/ui/data-protection
    * "Cloud Sync Task"
    * `/mnt/squire/media/Pictures` -> `/Pictures`
    * TODO: update to sync path to eliminate nested Pictures

## Sharing / Portfolio

### Adobe Portfolio

<p><a href="https://portfolio.john-knutson.com">portfolio.john-knutson.com</a></p>
