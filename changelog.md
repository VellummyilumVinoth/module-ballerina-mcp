# Change Log
This file contains all the notable changes done to the Ballerina MCP package through the releases.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- Server-side task execution support: tool calls with a `task` field in `CallToolParams` are executed asynchronously; task lifecycle is tracked per session and accessible via `tasks/list`, `tasks/get`, `tasks/result`, and `tasks/cancel`
