# Performance budgets

> Last reviewed: 2026-11 · Applies to: web, mobile, games

Set the budget at kickoff, and check it on every release. These are defaults that a project can tighten or loosen, as long as it records the change in its README.

Many users in the Philippines are on mid-range Android phones and mobile data, so test on those conditions, not on a fast laptop on Wi-Fi.

## Web

| Metric | Budget |
|---|---|
| Largest Contentful Paint (LCP) | ≤ 2.5 s on mobile, throttled 4G |
| Interaction to Next Paint (INP) | ≤ 200 ms |
| Cumulative Layout Shift (CLS) | ≤ 0.1 |
| Initial JS (compressed) | ≤ 200 KB |
| Lighthouse performance (mobile) | ≥ 90 |

## Mobile apps

| Metric | Budget |
|---|---|
| Cold start to interactive | ≤ 2 s on a mid-range Android device |
| Install size | Keep as small as practical; review any jump over 20% |
| Smooth scrolling | No visible jank on list screens |

## Games

| Metric | Budget |
|---|---|
| Frame rate | Stable 60 fps (30 fps acceptable on low-end devices if consistent) |
| Load to playable | ≤ 5 s |
| Memory | Stays within the target device's limits with no growth over a session |
