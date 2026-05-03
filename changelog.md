# Change Log
This file contains all the notable changes done to the Ballerina MCP package through the releases.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- Support for MCP protocol version `2025-11-25`, with backward compatibility for `2025-06-18`, `2025-03-26`, and `2024-11-05`
- New content types: `AudioContent`, `ResourceLink`; updated `ContentBlock` union
- New types: `BaseMetadata`, `Icon`, `Icons`, `ToolExecution`, `Annotations`, `Resource`, `ResourceLink`
- Task types (`TaskMetadata`, `TaskStatus`, `Task`, `CreateTaskResult`, `ListTasksResult`, `GetTaskResult`, `CancelTaskResult`) per MCP `2025-11-25` spec; service-side task execution not yet supported
- `JsonRpcResultResponse` as spec-aligned alias for the success response record

### Changed
- Extended `ClientCapabilities` and `ServerCapabilities` with new `sampling`, `elicitation`, and `experimental` fields
- Extended `CallToolResult` with richer content blocks (audio, resource links, embedded resources) and optional structured content
- Fixed native-image compatibility for `ContentBlock` array element type handling in `McpServiceMethodHelper`
