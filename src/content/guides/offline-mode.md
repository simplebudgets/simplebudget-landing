---
title: Working Offline
description: How simpleTracker's offline-first architecture keeps you productive without internet.
product: simpletracker
category: features
order: 6
---

simpleTracker is built offline-first — your notes and tasks are always available, even when you don't have internet.

## How It Works

When you create, edit, or delete a note or task offline:

1. The change is saved locally to your device immediately
2. It's added to a background sync queue (stored in IndexedDB)
3. When connectivity returns, all queued changes are synced to the server automatically

You don't need to do anything — it just works.

## What Works Offline

- ✅ Viewing all your notes and tasks
- ✅ Creating new notes and tasks
- ✅ Editing existing items
- ✅ Completing/uncompleting tasks and subtasks
- ✅ Deleting items

## What Requires Internet

- ❌ Sharing notes or projects (these need real-time sync)
- ❌ First-time login
- ❌ Seeing changes made by collaborators on shared items

## Sync Indicators

simpleTracker shows you when you have pending changes waiting to sync. Once connectivity is restored, syncing happens automatically via:

- The browser's `online` event
- A 30-second background heartbeat check
- When you switch back to the app (visibility change)

## Lie-fi Detection

Sometimes your phone shows "connected" but can't actually reach anything (common on weak WiFi or congested cellular). simpleTracker detects this by pinging the actual backend — not just trusting `navigator.onLine` — so you'll always know your true connectivity status.

## Tips

- Non-shared items always work offline — plan around this if you're about to go somewhere without service
- The app caches your data locally, so it loads instantly even on slow connections
- If you see a pending sync count, don't worry — it will resolve automatically when you're back online
