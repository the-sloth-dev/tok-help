# Tok Help

Public support and feedback for **Tok**, an experimental private peer-to-peer messenger for Android.

- [Report a bug](https://github.com/the-sloth-dev/tok-help/issues/new?template=bug_report.yml)
- [Request a feature](https://github.com/the-sloth-dev/tok-help/issues/new?template=feature_request.yml)
- [Other issue or question](https://github.com/the-sloth-dev/tok-help/issues/new?template=other_issue.yml)
- [Search existing issues](https://github.com/the-sloth-dev/tok-help/issues)

Search open and closed issues for your symptom, platform or version before creating a report. If a matching issue exists, add your reproducible observations there. Submission requires a GitHub account. **Reports, comments and attachments are public.**

This repository contains support instructions and issue forms. The application and website source repositories remain private. This is not a source release or a download repository. No app binaries or diagnostic exports are included.

## What to include

For bugs, provide the affected area, app version/build (or website page and browser/version), device/OS, exact reproduction steps, expected behavior and actual behavior. Do not assume that an online indicator proves delivery. For connection problems, note whether each device used Wi-Fi or mobile data, without posting network addresses or contact identities.

For feature requests, describe the problem, requested behavior and alternatives considered. Use the other-issue form for setup questions, documentation problems or feedback that does not fit a bug or feature request.

## Basic connection checks

Open Tok on both phones and check internet access. Review the contact request and compare the shared connection code through a trusted channel before approval. Keep both apps open for a first message test and check its delivery status. On Android, background reception depends on Stay available, notification permission, battery settings and force-stop restrictions. Delivery and calls remain best effort; Tok is experimental and has not received an independent security audit.

For more detail, open **Settings → Advanced → Connection diagnostics** in Tok and run connection checks. A connected relay does not prove the other phone is reachable. Retry connection may deliver queued traffic. Do not delete contacts or reinstall as a first troubleshooting step: that can remove local data.

## Optional diagnostic attachments

1. Reproduce the problem and note the steps and network type. For call problems, note which device placed or answered the call without including personal contact names.
2. Open **Settings → Advanced → Private app log**. After a call, inspect **Call setup timings** and **Call quality** if relevant.
3. Choose **Export sanitized log** (the export icon) and save the readable JSON file. Connection diagnostics also offers **Copy sanitized report**.
4. Open and review the file yourself. Inspect screenshots too. Remove credentials, app passwords, keys, private messages, personal information, addresses, contact identifiers and invitation links/QR codes. If unsure, omit the attachment.
5. Manually attach only a reviewed, sanitized copy to the GitHub form. Never place diagnostic content in URL parameters.

Nothing is uploaded automatically. GitHub issue submissions and attachments have their own logging and privacy behavior; see [GitHub's privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement). Do not post confidential security details here; no private reporting channel is advertised in this repository.

## Maintaining the tracker

Keep Issues enabled and preserve the `bug`, `enhancement` and `question` labels. The default branch contains `.github/ISSUE_TEMPLATE/bug_report.yml`, `feature_request.yml`, `other_issue.yml` and `config.yml`. These JSON-formatted YAML files use GitHub's native issue-form schema; blank issues are disabled. Required fields and optional attachments should stay consistent with the report descriptions. Keep the matching form copies and reporting links in the private website repository synchronized.

This tracker needs no backend, authentication token, Actions workflow or access to the private app repository. Do not commit private source, binaries, logs, backups, credentials or signing material here.
