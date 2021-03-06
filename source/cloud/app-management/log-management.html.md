---
title: Log Management
layout: cloud
---

When using Nanobox Cloud, application logs are available both in your dashboard and from the [cloud CLI](/cloud/cli/).

## Unified Log Stream
Just as in Nanobox local, all application logs are aggregated and streamed in a unified log stream. This allows all logs to be viewed in one place. Everything output to stdout and stderr as well as "log_watch'd" files are included in the log stream. For more information read through the [Logs doc](/getting-started/logs/).

## Viewing Logs in Your Dashboard
Logs can be accessed in your app dashboard under the "Logs" tab. There are three types of available logs:

- Streaming
- Historical
- Deploy Logs

![Dashboard Logs](/images/log-management-dashboard.png)

### Streaming Logs
Streaming logs display your app's live log stream. These allow you to see errors in your application as they happen. Each log entry is timestamped and flagged with the service-id and specific log from which it came.

With Streaming logs, only logs entries written after the stream is started are viewable. Any log entries written prior can be viewed in Historical logs.

### Historical Logs
Historical logs contain all of your app's stored log entries. Each log entry is timestamped and flagged with the service-id and specific log from which it came. When viewing historical logs, the entries are loaded 100 at a time. To load more, click the "View More" button and the next 100 entries will be loaded.

### Deploy Logs
Deploy logs are output streams of your app's deploys and builds. They're helpful when troubleshooting failed deploys and builds.

## Viewing Logs Through the CLI
To view the application logs through the CLI, use the the `nanobox cloud log` command. More information is avaialble in the [Cloud CLI log](/cloud/cli/log) doc.