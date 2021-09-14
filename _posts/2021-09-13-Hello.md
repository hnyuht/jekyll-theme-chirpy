---
title: SentinelOne Hunting Queries
author: Tony Huynh
date: 2021-09-13 09:50:00 +0600
categories: [Blogging, Tutorial]
tags: [writing]
---

## Welcome!

FileFullName RegExp "Users\\Public\\[^\\\{\}]+$" AND ( EventType IN ( "File Modification" , "File Creation" , "File Deletion" , "File Rename" )  AND (FileFullName EndsWithCIS ".bat" OR FileFullName EndsWithCIS ".cmd" OR FileFullName EndsWithCIS ".dll" OR FileFullName EndsWithCIS ".exe" OR FileFullName EndsWithCIS ".zip" OR FileFullName EndsWithCIS ".ps1" OR FileFullName ContainsCIS ".ht" ))
