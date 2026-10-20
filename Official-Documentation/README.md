---
title: Official documentation
tags: [documentation, sources, accessibility, testing]
status: verified
updated: 2026-10-19
---

# Official documentation

Platform behavior and accessibility guidance change. These rows are entry points, not copied manuals. Confirm the current page before relying on a feature. Record the version you checked when a decision depends on it.

When a practice page and an official page disagree about a platform feature, the official page for the version you run wins. Update or supersede the practice page afterward.

A platform or a framework belongs on this list. It is not the practice itself. Practices in `Best-Practices/` stay useful for a native app and for a cross-platform app.

Checked as entry points on 2026-10-19.

## Apple platform docs

| Source | Entry |
| --- | --- |
| Apple Developer Documentation | https://developer.apple.com/documentation/ |
| Human Interface Guidelines | https://developer.apple.com/design/human-interface-guidelines/ |
| Requesting access to protected resources | https://developer.apple.com/documentation/uikit/requesting-access-to-protected-resources |
| Accessibility | https://developer.apple.com/documentation/accessibility |

## Android platform docs

| Source | Entry |
| --- | --- |
| Android Developers | https://developer.android.com/docs |
| Permissions on Android | https://developer.android.com/guide/topics/permissions/overview |
| Build accessible apps | https://developer.android.com/guide/topics/ui/accessibility |

The Android permissions overview was dated 2026-10-16 on the page checked 2026-10-19. The accessible-apps guide was dated 2026-04-22 on that same check. Re-open the page before you rely on a permission type or a prompt.

## Mobile accessibility

WCAG is the cross-platform entry. W3C's mobile page says mobile accessibility is covered by existing W3C accessibility standards, including WCAG, and that W3C does not publish a separate mobile standard.

| Source | Entry |
| --- | --- |
| WCAG overview | https://www.w3.org/WAI/standards-guidelines/wcag/ |
| Mobile accessibility at W3C | https://www.w3.org/WAI/standards-guidelines/mobile/ |
| Guidance on Applying WCAG 2.2 to Mobile Applications (WCAG2Mobile) | https://www.w3.org/TR/wcag2mobile-22/ |

WCAG2Mobile was a W3C Group Draft Note dated 6 May 2025 when checked on 2026-10-19. The note says its guidance is informative and does not set requirements. Confirm the current page before treating any sentence in it as stable. The WCAG overview remains the standards entry.

## Mobile testing tools

These are places to confirm a tool's current behavior. The practice of naming a check lives in [Verify on a mobile client, then record](../Best-Practices/04-verify-and-record.md). This list does not choose a test stack.

| Source | Entry |
| --- | --- |
| XCTest | https://developer.apple.com/documentation/xctest |
| Test apps on Android | https://developer.android.com/training/testing |

The Android testing guide was dated 2026-03-05 on the page checked 2026-10-19.

## Sources opened for the 2026-10-19 topic pass

These pages were opened while adding practices 09–208. Confirm the current page before relying on a feature. Dates below are the dates printed on the page when it showed one.

| Source | Entry | Noted on the page |
| --- | --- | --- |
| The activity lifecycle | https://developer.android.com/guide/components/activities/activity-lifecycle | Checked 2026-10-19 |
| Save UI states | https://developer.android.com/topic/libraries/architecture/saving-states | Checked 2026-10-19 |
| Navigation | https://developer.android.com/guide/navigation | Page date 2026-09-23 |
| About deep links | https://developer.android.com/training/app-links | Page date 2026-10-16 |
| Back up user data with Auto Backup | https://developer.android.com/guide/topics/data/autobackup | Checked 2026-10-19 |
| Security tips | https://developer.android.com/privacy-and-security/security-tips | Checked 2026-10-19 |
| Understanding 3.3.1 Error Identification | https://www.w3.org/WAI/WCAG22/Understanding/error-identification.html | Checked 2026-10-19 |
| Understanding 2.5.8 Target Size (Minimum) | https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html | Checked 2026-10-19 |
| Foreground services overview | https://developer.android.com/develop/background-work/services/foreground-services | Page date 2026-10-16 |
| Notification runtime permission | https://developer.android.com/develop/ui/views/notifications/notification-permission | Page date 2026-10-16 |
| Optimize for Doze and App Standby | https://developer.android.com/training/monitoring-device-state/doze-standby | Page date 2026-08-18 |
| Support Direct Boot mode | https://developer.android.com/training/articles/direct-boot | Page date 2026-10-16 |
| Network security configuration | https://developer.android.com/privacy-and-security/security-config | Checked 2026-10-19 |
| Read network state | https://developer.android.com/develop/connectivity/network-ops/reading-network-state | Checked 2026-10-19 |
| Understanding 4.1.2 Name, Role, Value | https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html | Checked 2026-10-19 |
| Understanding 1.1.1 Non-text Content | https://www.w3.org/WAI/WCAG22/Understanding/non-text-content.html | Checked 2026-10-19 |

## How to add a source

Add a row with the official entry URL, the date you checked it, and the decision it supports. Keep AI product docs in the AI knowledge base. Keep warehouse, analytics, store-submission, and CI vendor docs in those repos. Keep language and HTTP specifications that are not specific to a mobile client in the application-development knowledge base.

## Local notes

If you need a short note about a documentation page, add a file next to this README:

- Name it for the topic, not the whole product.
- State the version and the date checked.
- Quote only the minimum needed to support a decision, with the URL.
- Link the note from the practice or lesson that depends on it.
