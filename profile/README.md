## flaglogr
Feature Flags, A/B Testing, (error) logging service and system monitoring, focusing on simplicity, ease of use, being lightweight and easy to write and maintain, since **NO AI** is used in the making of this tool.

It is an alternative to tools like Sentry, GrowthBook and LaunchDarkly, with much more limited feature set compared to them

This is why the backend is written in Go using the `gin` framework to enable high throughput at a low memory footprint.
flaglogr uses `gorm` to store its data and thus supports a variety of backends.

## Admin Panel
It also features an Admin Panel allowing you to configure everything via GUI and viewing the metrics and logs generated from your applications, with multi-user support, including roles.

Currently, no `basic auth` is available for flaglogr, only Trusted Header Authentication and OpenID Connect is enabled. PRs welcome!

## SDKs
Since the feature set is very specific, there are specific SDKs for a few languages.
The APIs are designed to be as easy to use as possible, allowing porting to other languages with minimal effort.

**Official SDKs:**
| Language | Repo | Notes |
|----------|------|-------|
| `go` | [flaglogr-go](https://github.com/flaglogr/go) | Works with any webserver framework (and other applications, too) |
| `js` | [flaglogr-go](https://github.com/flaglogr/js) | Works both on server-side and client side and supports the frameworks, too |

More SDKs are coming when I personally need them or people request them (and I have the time to implement them).
