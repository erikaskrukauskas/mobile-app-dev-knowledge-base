---
title: Best practices index
tags: [practices, index, mobile]
status: verified
updated: 2026-10-19
---

# Best practices

These pages are the stable mobile-application rules. Lessons in `Lessons-Learned/` are evidence from real work on a mobile client. When a lesson holds beyond the original project, fold the reusable part into a page here and link the lesson to that page.

A general application rule — architecture that any client could use, a public HTTP API, a shared state rule, or application security that does not depend on the device — lives in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base). Link that page. Do not restate it here.

| Guide | Use it when |
| --- | --- |
| [Consult before a mobile design choice](01-consult-before-design.md) | About to choose navigation, a screen contract, lifecycle behavior, offline state, or a device security boundary |
| [Specify the screen and done](02-specify-screen-and-done.md) | Writing the change a mobile client must make |
| [Compare before choosing](03-compare-before-choosing.md) | Choosing navigation, a screen contract, or where mobile state lives |
| [Verify on a mobile client, then record](04-verify-and-record.md) | Deciding the work is done, or saving a lesson |
| [Practice versus project](05-practice-versus-project.md) | Deciding whether a decision belongs in this repo |
| [Mobile application security](06-mobile-application-security.md) | Handling platform permissions, data on the device, or secrets |
| [Mobile accessibility](07-mobile-accessibility.md) | Naming what a person must be able to perceive, operate, and understand on a phone |
| [Write findable pages](08-write-findable-pages.md) | Adding a page a later search should find |
| [Save state before process death](09-save-before-process-death.md) | The person expects a screen to look the same when they switch away and come back. The system may destroy the process while they are gone. |
| [A dismissed screen starts clean](10-clean-start-after-dismissal.md) | When a person finishes a screen, or removes the app from the recent-apps list, they expect a later visit to start clean. |
| [Keep input across a configuration change](11-keep-state-across-configuration-change.md) | Rotation, resizing, and multi-window are not a new visit. The person expects the same input and the same place in the task. |
| [Release work when the app is not visible](12-release-work-when-backgrounded.md) | A screen that keeps a camera, a location stream, or a playback session running after the person has left spends the device and can surprise them. |
| [Resume the same task](13-resume-the-same-task.md) | Coming back after a call or a home press is a continuation, not a new session, unless the person dismissed the screen. |
| [Do not start a new flow in the background](14-no-new-flow-from-background.md) | A process that is not in front of the person should not open a new screen over whatever they are doing now. |
| [A failed restore opens a safe screen](15-safe-screen-when-restore-fails.md) | Saved state can be missing, too old, or from a screen that no longer exists. |
| [Keep process-death state small](16-small-saved-state.md) | The bundle that survives process death is for a small key, not for the whole record. |
| [Back returns to the previous place](17-back-returns-to-previous.md) | Back means the person returns to the place they came from, in an order they can predict. |
| [Name the destinations and how they connect](18-destination-map.md) | A mobile client needs an explicit list of screens and the moves between them. A pile of buttons is not that list. |
| [A deep link has a fallback screen](19-deep-link-fallback.md) | A link can name a screen or a record that is gone, private, or not loaded yet. |
| [An unverified link is not the caller's identity](20-unverified-link-is-not-identity.md) | A custom scheme or an unverified web link can be claimed by more than one app, and the system may ask the person to choose. |
| [Prefer a verified association for your own links](21-verified-app-link.md) | A link to your own site should open your app without asking the person to pick from a list, once the association is verified. |
| [Each top-level section keeps its place](22-each-section-keeps-its-place.md) | Switching top-level sections and coming back should show the place the person left, not the root of that section every time. |
| [Say when up and back differ](23-up-and-back.md) | Back follows the path the person took. Up goes to the parent in the structure. They are the same only when the path and the parent match. |
| [Back does not silently drop unsaved input](24-back-keeps-unsaved-input.md) | The system back gesture can pop a screen that still holds what the person typed. |
| [Returning from another app restores the screen](25-external-return-restores-screen.md) | A share sheet, a browser, or a payment app sends the person away and then back. |
| [Dismissing a modal is an explicit choice](26-modal-dismiss-is-explicit.md) | A sheet or dialog sits on top of a task. Dismissing it can discard a choice or commit one. |
| [Show the age of offline data](27-show-data-age-when-offline.md) | A screen that shows a stored copy while the network is absent can look current when it is not. |
| [User work is not cache](28-user-work-is-not-cache.md) | Cache is disposable. A draft, a photo they took, or a message they have not sent is not disposable. |
| [An offline command applies once](29-offline-command-applies-once.md) | A command queued while offline can be sent twice when the network returns, or sent again after the app restarts. |
| [Sign-out clears private local data](30-sign-out-clears-private-data.md) | A later person who opens the app on the same device should not see the previous person's private cache, drafts, or tokens. |
| [External storage is untrusted](31-external-storage-is-untrusted.md) | Storage the person can remove, or that other apps can read, is not a private store. |
| [Private files stay in app storage](32-private-files-stay-in-app-storage.md) | Files that only this app should read belong in storage the platform keeps private to the app. |
| [Exclude secrets from backup](33-exclude-secrets-from-backup.md) | A platform backup can copy app files to the person's account. A token in those files leaves the device. |
| [Backup is not the only copy](34-backup-is-not-the-only-copy.md) | Backup runs only when the device is idle, on a network, and under a size limit. It can fail or never run. |
| [Cache is not the record](35-cache-is-not-the-record.md) | A cache directory is excluded from backup and may be cleared. It cannot be the only place a record exists. |
| [Sharing stored data with other apps is explicit](36-exported-store-is-explicit.md) | A store that other apps can read is a published surface. The default is that they cannot. |
| [Validate data that arrives from outside](37-validate-data-from-outside.md) | Files, links, shares, and network responses are input. They can be the wrong shape or hostile. |
| [A local store failure is visible](38-local-store-failure-is-visible.md) | A full disk, a locked store, or a migration failure can leave a screen with nothing to show. |
| [Name an input error in text](39-name-the-input-error-in-text.md) | Color, a shake, or a redisplayed form does not tell someone what failed. |
| [Point an error at the field](40-name-the-field-that-failed.md) | A banner that says something failed does not say which field to fix. |
| [A network failure says what still works](41-network-failure-names-what-remains.md) | A failed request is not the same as an empty screen, and it is not the same as a loss of local data. |
| [A denied permission is explained in text](42-permission-failure-is-text.md) | A system dialog can close and leave the screen looking unchanged. The person may not know the action was refused. |
| [Do not only redisplay the screen after a failure](43-do-not-only-redisplay-the-screen.md) | Putting the same screen back with no change hides the failure. |
| [Request the smallest permission](44-smallest-permission.md) | A permission is access to restricted data or a restricted action. Extra access is extra harm if the app is misused. |
| [Recheck a permission before each use](45-recheck-before-each-use.md) | A grant can be removed in system settings while the app is installed. |
| [Do not depend on permission groups staying put](46-permission-group-is-not-stable.md) | Platforms group related permissions in the prompt. The grouping can change. |
| [The permission prompt matches a decision the person can understand](47-explain-the-permission-decision.md) | A prompt that does not say what is being allowed is not a decision. |
| [Ask for a permission at the action](48-ask-at-the-action.md) | A prompt at first launch asks for access the person has not tried to use. |
| [Access while the app is hidden is a separate decision](49-special-access-is-separate.md) | Using the camera, microphone, or location while the person is looking at the screen is not the same decision as using them while the app is hidden. |
| [A permanent denial has a way forward](50-permanent-denial-path.md) | After a person denies a prompt enough times, the platform may stop showing it. |
| [Do not hand permission-only data to another app](51-do-not-leak-permission-data.md) | Data the app can read only because it holds a permission is still restricted. |
| [Do not log personal data on the device](52-do-not-log-personal-data.md) | Device logs can be read by other software and often survive longer than the screen that wrote them. |
| [Web content is another trust boundary](53-web-content-is-another-trust-boundary.md) | A view that renders remote pages can run script. That is a different trust boundary from the rest of the app. |
| [Use protected transport on networks you do not control](54-https-on-networks-you-do-not-control.md) | Phones join networks the person does not control. A cleartext call on that network is readable. |
| [An SMS is not an authenticated command](55-sms-is-not-an-authenticated-command.md) | A text message can be spoofed, and other apps that can read messages can see it. |
| [Keep as little personal data on the device as the screen needs](56-minimize-personal-data-on-the-device.md) | A copy on the device is a copy that backup, logs, and the next user of the phone can expose. |
| [Do not use a phone identifier as the account id](57-do-not-use-a-phone-identifier.md) | A phone number or a hardware identifier is tied to the person and to the device. It is a poor account key and a privacy leak. |
| [A third-party component gets no unexplained personal data](58-third-parties-get-no-unexplained-data.md) | An analytics, advertising, or support library runs inside the app and can receive what you pass it. |
| [Store a token, not the password](59-store-a-token-not-the-password.md) | A password saved on the device is the person's credential for other places too. |
| [Do not share secrets over a local network socket](60-do-not-use-a-local-socket-for-secrets.md) | A port on the device can be reached by other apps. It is not a private channel. |
| [Clear a web view that showed sensitive content](61-clear-sensitive-web-cache.md) | A web view can keep files for pages it showed, including pages that contained private data. |
| [A script bridge is only for trusted pages](62-script-bridge-only-for-trusted-pages.md) | A bridge lets page script call into the app. That is app-level power. |
| [Keep on-device tokens short-lived](63-short-lived-tokens.md) | A token on the device will be copied if the device is. A long-lived token makes that copy useful. |
| [Limit repeated authentication attempts on the device](64-limit-authentication-attempts.md) | A screen that accepts unlimited password or code attempts helps someone who holds the unlocked phone. |
| [Make touch targets large enough or far enough apart](65-target-size-or-spacing.md) | Small controls placed against each other are easy to hit by mistake. |
| [Enlarged text still operates the screen](66-enlarged-text-still-operates.md) | A person who enlarges text still has to reach every control and read every name. |
| [Honor reduced motion](67-reduced-motion.md) | Motion that explains a change can also make a person sick or hide the change. |
| [Audio has a text alternative](68-captions-for-audio.md) | A video or a voice clip that carries information leaves out anyone who cannot hear it in that moment. |
| [Focus order follows the task](69-focus-order.md) | A screen reader and a keyboard move focus in an order. A random order hides the task. |
| [The accessible name matches the visible label](70-label-matches-visible-text.md) | A button that shows Save and is spoken as Button can be reached, but not understood. |
| [An error is announced](71-error-is-announced.md) | A text error that appears away from the current focus can be invisible to a screen reader. |
| [A status icon also has text](72-status-icons-have-text.md) | A color or an icon that means failed, waiting, or done is invisible to someone who cannot see that color. |
| [The whole flow works with assistive technology](73-flows-work-with-assistive-tech.md) | A labeled button is not a flow. The person has to start, finish, and recover. |
| [Contrast is part of the screen contract](74-contrast-is-part-of-the-screen.md) | Text that is visible on a designer's monitor can disappear in sunlight or for someone with low vision. |
| [A time limit can be extended or is explained](75-time-limits-can-be-extended.md) | A code entry or a session that expires while a person is still working fails people who need more time. |
| [A complex gesture has a simple alternative](76-gesture-has-a-simple-alternative.md) | A swipe, a long-press, or a multi-finger gesture is invisible and may be impossible. |
| [The keyboard does not cover the focused field](77-keyboard-does-not-cover-the-field.md) | A software keyboard can sit on top of the field the person is typing into, and on top of the error under it. |
| [System bars do not cover the controls](78-safe-area-keeps-controls-reachable.md) | A notch, a status bar, a navigation bar, or a home indicator can cover a control placed at the edge. |
| [An empty screen says why it is empty](79-empty-state-says-why.md) | An empty list can mean the person has no items, the filter excluded them, or the load failed. |
| [A loading screen says it is waiting](80-loading-state-says-waiting.md) | A blank screen while data loads looks like a crash or an empty account. |
| [Keep what the person typed when validation fails](81-preserve-input-when-validation-fails.md) | Clearing a form after a validation error makes them type it again, and they may not remember it. |
| [A destructive action confirms on the device](82-destructive-action-confirms.md) | Delete, send, and pay are hard to undo. A single stray tap should not complete them. |
| [One account's local data is not another's](83-accounts-do-not-share-local-data.md) | Two accounts on one phone can share a process. Their drafts and tokens must not. |
| [A draft survives process death](84-draft-survives-process-death.md) | A draft is user work. Process death is normal while they are in another app. |
| [A notification opens the screen that holds the state](85-notification-opens-the-state.md) | A notification is a hint that something changed. The state lives in the app. |
| [Notification permission is its own decision](86-notification-permission-is-separate.md) | Being allowed to run the app is not the same as being allowed to interrupt the person. |
| [A badge matches the unread state](87-badge-matches-unread-state.md) | A badge that stays after the person has read the item teaches them to ignore it. |
| [Share only what the screen allows](88-share-out-only-what-the-screen-allows.md) | The system share sheet sends data to another app. The person may not see every field that goes with it. |
| [An incoming share is validated before it is stored](89-incoming-share-is-validated.md) | Another app can share a file the person did not expect, of a type or size you do not handle. |
| [Picking one item does not need the whole library](90-one-item-does-not-need-the-library.md) | Ongoing access to every photo, contact, or file is a larger decision than choosing one item. |
| [Precise location is a separate, narrower need](91-precise-location-only-when-needed.md) | A nearby-store feature and a turn-by-turn feature do not need the same precision. |
| [Do sensitive work on the device when the server does not need the data](92-prefer-on-device-for-sensitive-work.md) | Sending personal data to a server creates a copy the screen may not need. |
| [Query local structured stores with parameters](93-parameterized-local-queries.md) | A local database is still a database. Building a query by gluing text from a link or a search box is injection. |
| [A release build limits logs](94-release-build-limits-logs.md) | A debug log that is useful on a desk is a leak on a person's phone. |
| [Test lifecycle on a device or emulator](95-test-lifecycle-on-a-device.md) | A host unit test does not rotate the device or kill the process. |
| [Test offline with the network off](96-test-offline-with-network-off.md) | A mock that returns an error is not the same as a phone with no network. |
| [Test with the platform assistive technology](97-test-with-assistive-technology.md) | An automated contrast check does not prove a screen reader can finish the task. |
| [Test backup and restore](98-test-backup-and-restore.md) | Backup rules that were never restored are a guess. |
| [Test the missing deep link](99-test-the-missing-deep-link.md) | The happy link is the easy check. The missing record is the one that crashes. |
| [Test a configuration change in the middle of input](100-test-configuration-change.md) | Rotation is the check people skip because the simulator is already in portrait. |
| [Multi-window keeps the screen's state](101-multi-window-keeps-state.md) | Split screen is a configuration change the person can do without meaning to restart the task. |
| [The first screen does not ask for sensitive access](102-first-screen-asks-for-nothing-sensitive.md) | The first screen is where the person decides whether to stay. A permission prompt is a poor greeting. |
| [Process-death memory holds a key, not the record](103-saved-state-holds-a-key.md) | The small save that survives process death is slow to write and limited in size. |
| [The first screen does not wait on a permission](104-first-screen-does-not-wait-on-a-permission.md) | Blocking the first frame on a permission dialog hides the product behind a decision the person cannot judge yet. |
| [Punctuation in input is data, not a command](105-input-punctuation-is-data.md) | Search boxes and names contain apostrophes, quotes, and characters that are special in a query language. |
| [Script in a web view stays off until a screen needs it](106-script-stays-off-until-needed.md) | Script is how a page reaches for app power. The default in the platform guidance is off. |
| [Backup is not a save button](107-backup-does-not-run-as-a-save-button.md) | The platform backup may skip an app that is in the foreground, and it runs on a schedule, not when the person taps Save. |
| [A restore can finish before the first launch](108-restore-before-first-launch.md) | On a new device, restored files can appear before the person has opened the app. First-launch code that assumes empty storage will wipe or misread that data. |
| [Ongoing work the person is not watching is still visible](109-ongoing-work-is-visible.md) | Work that continues while the person is in another app has to be obvious. A hidden task that holds the radio or the microphone is not. |
| [The person can stop ongoing work](110-person-can-stop-ongoing-work.md) | A task that keeps running after they leave needs a way for them to end it. |
| [Do not stay awake just to avoid being treated as idle](111-do-not-stay-awake-to-look-busy.md) | Holding a visible ongoing task so the system will not treat the app as idle drains the battery for no task the person asked for. |
| [Background sync may wait until the device is idle-awake](112-background-sync-may-wait.md) | A phone that is still, unplugged, and dark defers network and jobs. A sync started then does not have to finish then. |
| [An urgent push is for an alert the person will see](113-urgent-push-is-for-a-visible-alert.md) | Waking the device for a message that only refreshes a cache spends the battery and trains them to ignore alerts. |
| [A battery exemption is a rare, named exception](114-battery-exemption-is-rare.md) | Asking the person to ignore battery limits so the app can sync is not a default setup step. |
| [The app recovers when the device leaves idle](115-recover-when-the-device-wakes.md) | After a long idle period, the next open should look like a normal open, not a crash or a wiped draft. |
| [Private data waits until the device is unlocked](116-private-data-waits-for-unlock.md) | After a restart, the device can be on while the lock screen is still up. Storage that needs the person's credential is not available yet. |
| [Work before unlock is a small, explicit component](117-before-unlock-work-is-explicit.md) | The whole app should not run on a locked device. A clock alarm or an accessibility service sometimes must. |
| [Check that alerts are allowed before you send one](118-check-before-you-notify.md) | A grant from last month may have been turned off in system settings. |
| [Dismissing an alert prompt is not allow or deny](119-dismissing-the-prompt-is-not-a-choice.md) | Swiping a permission dialog away is not the same as refusing, and it is not the same as agreeing. |
| [A new install cannot notify until the person allows it](120-a-new-install-cannot-notify-yet.md) | Installing the app is not permission to interrupt them. |
| [A playback notice is not a promotional alert](121-playback-notice-is-not-a-promotion.md) | The notice that says audio is playing is part of that task. A marketing alert is a different decision. |
| [A grant to alert is not a grant to alert often](122-use-alerts-sparingly-after-a-grant.md) | People can see how many alerts an app sends, and they can revoke the grant. |
| [Cleartext network access stays off](123-cleartext-stays-off.md) | An unencrypted call is easy to add by accident when a URL changes. |
| [A certificate pin needs a way to rotate](124-a-pin-needs-a-rotation-plan.md) | A pin that only matches today's key strands every installed app when the key changes. |
| [Debug trust settings do not ship](125-debug-certificates-do-not-ship.md) | A certificate added so a developer can inspect traffic must not be trusted by the build people install. |
| [A sensitive call trusts a named set of authorities](126-sensitive-calls-trust-a-named-set.md) | Trusting every certificate on the device includes ones the person, or someone with the device, added. |
| [A captive portal is not a reachable server](127-captive-portal-is-not-your-server.md) | The phone can be joined to a network and still be stuck on a sign-in page. That is not a successful call to your server, and it is not proof the person has no account. |
| [A large transfer respects a metered network](128-large-transfer-respects-a-metered-network.md) | A photo backup or a dataset download on a metered link can cost the person money. |
| [A connected network is not a successful response](129-a-network-object-is-not-success.md) | Seeing that Wi-Fi is associated does not mean your server answered. |
| [Work that can wait is scheduled](130-waiting-work-is-scheduled.md) | Starting a large job the moment any network appears fights the radio and the battery limits. |
| [A custom control exposes its name, role, and value](131-custom-control-exposes-name-role-and-value.md) | A control drawn as a picture is invisible to a screen reader unless the platform is told what it is. |
| [A control's state is available, not only its label](132-a-control-state-is-part-of-the-name.md) | A switch that only says Notifications can be on or off. The label alone hides which. |
| [Focus location is exposed to assistive technology](133-focus-itself-is-exposed.md) | People navigating by switch or keyboard need to know which control has focus. |
| [A decorative image is skipped by assistive technology](134-decorative-images-are-skipped.md) | A flourish that is announced as an image makes the screen longer without adding meaning. |
| [A meaningful image has equivalent text](135-a-meaningful-image-has-an-equivalent-text.md) | A photo, chart, or icon that carries information needs text that carries the same information, not the file name. |
| [A media clip has a name before it plays](136-a-media-clip-has-a-name.md) | A play button on an unnamed clip does not say what will play. |
| [A human-check has more than one sense](137-a-captcha-has-another-sense.md) | A check that is only a picture leaves out anyone who cannot see that picture. |
| [An icon button is named for its action](138-an-icon-button-is-named-for-its-action.md) | A button whose accessible name is the image file name, or button, does not say what will happen. |
| [A slider or progress control exposes its value](139-a-value-control-exposes-the-value.md) | A slider the person can move, or a progress indicator they are waiting on, has a value. A silent graphic does not. |
| [An expandable section exposes whether it is open](140-an-expandable-section-exposes-expanded.md) | A row that opens more content is a state, not only a tap target. |
| [A dialog announces itself and returns focus](141-a-dialog-announces-itself.md) | A sheet that appears without moving focus is invisible to a screen reader. When it closes, focus should not fall on a random control. |
| [A live update is announced when it changes the task](142-a-live-update-is-announced-when-it-matters.md) | A new message or a finished upload can appear away from the focused control. |
| [Ongoing work names why it is allowed to continue](143-ongoing-work-names-its-reason.md) | Platforms ask you to declare the kind of ongoing work. The reason is also how you know when to stop. |
| [Do not promote a background job into ongoing work](144-do-not-promote-idle-work-to-ongoing.md) | A sync that was fine to defer should not be relabeled as a user-visible task so it can start while the app is in the background. |
| [If the system stops a long task, say so](145-a-stopped-task-says-it-stopped.md) | Some platforms limit how long ongoing work may run. The person should not think it is still going. |
| [A silent heartbeat is not a user alarm](146-a-silent-heartbeat-is-not-an-alarm.md) | An alarm the person created, such as a wake-up time, is allowed to fire. A timer whose only job is to wake the app is not that alarm. |
| [A push that alerts carries its text](147-a-push-carries-its-text.md) | Waking the device and then fetching the message body forces another network call at the worst time. |
| [Test the app on an idle device](148-test-the-idle-device.md) | A test on a plugged-in, awake phone never sees deferred jobs. |
| [Do not hold a private always-on connection](149-do-not-hold-your-own-always-on-connection.md) | One socket per app, kept open forever, is a battery cost. It also dies under idle restrictions. |
| [An idle deferral is not an error banner](150-idle-deferral-is-not-an-error-banner.md) | The person did nothing wrong when the system waits to sync. |
| [Waiting work may run when the device is charging](151-charging-may-run-waiting-work.md) | Plugging in is one of the moments the system lets waiting jobs run. The person should not have to babysit that. |
| [Read private storage only after unlock](152-ask-unlock-before-private-reads.md) | A restart can deliver a boot event before the person has unlocked the phone. |
| [Test a reboot that stays locked](153-test-the-locked-reboot.md) | A test that unlocks immediately never sees the before-unlock path. |
| [Tokens are not copied into before-unlock storage](154-tokens-are-not-copied-before-unlock.md) | Moving a token so an alarm can see it also leaves the token available before the person unlocks the phone. |
| [The default store is the one that needs unlock](155-the-default-store-needs-unlock.md) | The convenient default is the private store that appears after unlock. The before-unlock store is the special case. |
| [A group of fields has a name](156-a-group-of-fields-has-a-name.md) | Three radio options without a group name are three unrelated buttons. |
| [The selected section exposes that it is selected](157-a-selected-tab-exposes-selected.md) | A row of sections that all look like buttons hides which one is current. |
| [An invalid field exposes an invalid state](158-an-invalid-field-exposes-invalid.md) | Error text next to a field can be missed if the field itself does not carry the invalid state. |
| [Unknown progress says working, not a percent](159-progress-that-is-unknown-says-working.md) | A bar that creeps with no real measurement lies. A bar with no text is silent. |
| [Chart text matches the chart](160-chart-text-matches-the-chart.md) | A chart alternative that says chart of sales does not give the numbers. |
| [A link's name says where it goes](161-link-purpose-is-in-the-name.md) | A control named here or this does not say what will open. |
| [Binding traffic to one network is explicit](162-binding-traffic-to-one-network-is-explicit.md) | Forcing all traffic onto one network can need a separate permission and can surprise the person when that network drops. |
| [Listen for network changes instead of polling](163-listen-for-network-changes.md) | Polling connectivity keeps the device awake and still misses fast changes. |
| [A restored app may already allow alerts](164-a-restored-app-may-already-allow-alerts.md) | A backup from a phone where they allowed alerts can arrive on a new phone with that choice already made. |
| [A previous alert denial still holds after an upgrade](165-a-denial-of-alerts-sticks-across-upgrade.md) | An operating-system upgrade should not quietly turn alerts back on after the person turned them off. |
| [A battery exemption lives in their settings](166-exemption-lives-in-their-settings.md) | The list of apps allowed to ignore battery limits is the person's list. |
| [An ordinary refresh uses ordinary priority](167-ordinary-refresh-uses-ordinary-priority.md) | Marking every sync urgent makes urgent meaningless and wakes the device all day. |
| [Idle alarms are rare](168-rate-limit-idle-alarms.md) | A loop of exact alarms while the device is idle is a battery bug, and the platform will coalesce it anyway. |
| [Standby means they have not been using the app](169-standby-means-they-have-not-used-the-app.md) | An app they have not opened, and that is not doing a task they expect, will be treated as idle. |
| [A call-style notice is only for a call](170-a-calling-style-notice-is-only-for-a-call.md) | Platforms exempt some call-style notices from the ordinary alert permission. That exemption is not a costume for other messages. |
| [A stopped transfer says what was kept](171-partial-result-of-a-stopped-transfer-is-named.md) | Stopping a long upload or download can leave a partial file. The screen has to say whether that partial file is usable. |
| [The visible ongoing status carries no secrets](172-visible-status-carries-no-secrets.md) | A status-bar notice is visible on a locked phone in many cases, and it is visible to someone looking over a shoulder. |
| [Opening the ongoing status opens that task](173-opening-the-status-opens-the-task.md) | Tapping the notice for a recording or a download should land on that task, not on the home screen. |
| [Two ongoing tasks have two statuses](174-two-ongoing-tasks-have-two-statuses.md) | One generic ongoing notice for two different jobs hides which one is running and which stop button does what. |
| [A finished task clears its status](175-a-finished-task-clears-its-status.md) | A notice that still says recording after they pressed stop teaches them not to trust the status. |
| [Losing the network mid-task is a named state](176-network-loss-mid-task-is-a-named-state.md) | A transfer or a call that loses the network is not the same as the person pressing stop. |
| [A late callback does not update a screen that is gone](177-do-not-trust-a-callback-after-the-screen-is-gone.md) | A response can arrive after the person has left the screen or after the process has a new screen in its place. |
| [Stop listening when the screen closes](178-unsubscribe-when-the-screen-closes.md) | A listener that outlives the screen keeps the device working and can update the wrong generation of the screen. |
| [The metered warning comes before the bytes move](179-a-metered-warning-is-before-the-bytes.md) | Asking after a large upload has started does not give them the choice. |
| [A tunnel is not proof your server answered](180-vpn-or-private-dns-is-still-not-your-server.md) | A VPN or a private DNS setting can be up while your server is down, or the tunnel can be the thing that failed. |
| [A pin failure has a screen, not a crash](181-pin-failure-has-a-screen.md) | A pin that no longer matches is a connectivity failure. The person cannot fix a certificate. |
| [The release check does not trust the debug proxy](182-a-debug-proxy-is-not-in-the-release-check.md) | A test that only passes because a debug certificate is installed is not a test of the build people get. |
| [A custom authority is named, not global](183-custom-trust-is-named.md) | Trusting a company or self-signed authority for one host should not make that authority valid for every host. |
| [The locked device does not show private records](184-locked-screen-hides-private-records.md) | A notification or a widget that renders a private record on the lock screen publishes it before unlock. |
| [A reboot does not throw away local work](185-reboot-does-not-sign-them-out-of-local-work.md) | Unlocking after a reboot is not a new account and not a reason to drop drafts that were in the private store. |
| [An accessibility helper that runs before unlock stays limited](186-accessibility-service-before-unlock-is-limited.md) | An accessibility service is one of the few reasons to run before unlock. That does not entitle it to the mailbox. |
| [A changed count is announced when it is the point](187-announce-the-new-count.md) | A badge that changes from one to two while they are on the screen can be the whole point of the screen, or it can be noise. |
| [A pressed or selected control exposes that state](188-a-pressed-control-exposes-pressed.md) | A toggle that only changes color is the color-only problem again, and a screen reader never hears it. |
| [A form error exposes which fields are invalid](189-form-errors-expose-which-fields.md) | A summary that says two errors is not enough if the fields themselves do not carry the invalid state. |
| [An image of words is also text](190-images-of-text-are-text.md) | A picture of a sentence cannot be enlarged, copied, or read reliably. |
| [A map has a text list of the places that matter](191-a-map-has-a-text-list.md) | A map pin the person cannot see is a place they cannot choose. |
| [A test image is identified without spoiling it](192-test-images-do-not-leak-the-answer.md) | Some images are the question. A description that gives the answer makes the question pointless, and no description makes it impossible. |
| [Do not poll for a job the scheduler owns](193-do-not-poll-for-a-job-the-scheduler-owns.md) | Waking the app every minute to see if the network is back undoes the idle restrictions. |
| [A timer they set is allowed to be exact](194-a-user-visible-timer-is-allowed-to-be-exact.md) | A cooking timer or a reminder they just created is a promise about a clock time. |
| [A refresh on open is honest about age](195-sync-on-open-is-honest-about-age.md) | Opening the app is when deferred work may finally run. The first paint might still be the stored copy. |
| [Do not chain urgent wakes](196-do-not-chain-urgent-wakes.md) | One urgent alert that fetches more data and then sends another urgent message keeps the device awake. |
| [Do not fight the idle bucket](197-standby-buckets-are-not-a-tuning-knob.md) | Trying to stay in the most active bucket is the same mistake as asking for a battery exemption. |
| [Test standby separately from device idle](198-test-standby-separately-from-doze.md) | The whole device being asleep and this app being unused are different restrictions. |
| [A dismissed prompt does not lock the feature](199-a-permission-dialog-swipe-does-not-lock-them-out.md) | Treating a swipe-away as a permanent denial sends them to settings for a choice they never made. |
| [Alerts and the in-app screen are allowed to diverge](200-alerts-and-the-in-app-screen-can-diverge.md) | Turning off alerts is not deleting the data. |
| [Ongoing work usually starts from a tap](201-foreground-work-from-a-tap-is-the-usual-start.md) | The usual reason ongoing work is allowed is that the person just asked for it. |
| [The stop control on the status really stops the work](202-the-status-stop-control-is-real.md) | A stop action that only dismisses the notice and leaves the microphone on is a lie. |
| [A crash does not leave a lying status](203-a-crash-clears-a-stale-ongoing-status.md) | If the process dies, a status that still says live is worse than no status. |
| [Encryption at rest still unlocks for the person](204-encrypted-at-rest-is-not-hidden-from-the-user.md) | Storage encrypted until unlock is not a second password you invented. It unlocks when they unlock the device. |
| [Another user on the device is another unlock](205-a-second-user-on-the-device-is-another-unlock.md) | Some devices have more than one user. Their credential stores are not yours to read while they are locked. |
| [The idle check and the locked check are part of done](206-document-the-idle-and-locked-checks.md) | A feature that syncs, alerts, or stores private data is not done when it works on an awake, unlocked developer phone. |
| [Say which network facts the screen uses](207-say-which-network-facts-the-screen-uses.md) | Connected, metered, captive, and validated are different facts. A screen that says offline for all of them hides the choice. |
| [Review alerts against the current grant](208-review-alerts-against-the-grant.md) | An alert feature that was only tested while notifications were on misses the default-off install. |

Pages 09 through 208 are `tested` because the official page named on each one was opened on 2026-10-19. They become `verified` only after the check named on the page is run on a mobile client.

Search before adding another topic. If a page already answers the question, edit that page.
