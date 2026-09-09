# Changelog

## v1.4.0

Consolidated back into a single current version. A `v2` branch and a `v2.0.0` tag existed briefly (module path `github.com/themudhaxk/mudbase-sdk-go/v2`); that work has been folded into this release instead of being kept as a separate major version, since there are no real integrations depending on the old shape yet and a new user should never have to pick "v1 or v2."

What actually changed, carried over from that work:

- Fixed the module path in `go.mod`. It was still the openapi-generator placeholder `github.com/GIT_USER_ID/GIT_REPO_ID`, which meant `go get github.com/themudhaxk/mudbase-sdk-go` would fail Go's module-path validation. Now correctly `github.com/themudhaxk/mudbase-sdk-go` (no `/v2` suffix - this stays a v1.x release, not a major-version bump).
- Model types moved out of the flat repo root into their own `models` package (`models/model_*.go`), matching the folder-based layout the other generated SDKs already use. Import `models` alongside `mudbase` if you reference a type by name.
- Regenerated from the current OpenAPI spec (API version 1.3.13), picking up the latest routes/fields plus generator helper additions (`models/utils.go`, webhook model and response fixes).
- Fixed test file and doc-example import paths that still referenced the placeholder path.

The `v2` branch and `v2.0.0` tag are retired - this repo has exactly one supported install path going forward.

## Earlier versions

See git tags `v1.0.0` through `v1.3.12` for prior release history (regenerated automatically from the OpenAPI spec on each backend change; no hand-written changelog was kept for those).
