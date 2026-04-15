# API Documentation

## Endpoints
### Series Intake
- **Description**: Collect, validate and normalize metadata from CDP; attach a runId and timestamp for traceability.
- **Type**: Processing

### Retrieve
- **Description**: Execute retrieve phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Ground
- **Description**: Execute ground phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Recommendation
- **Description**: Recommendation across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Rights Validation
- **Description**: Rights Validation across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Content Classification
- **Description**: Content Classification across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Audience Targeting
- **Description**: Audience Targeting across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Programming Grid
- **Description**: Assemble final payload with status, artifacts, KPIs and audit trail; store to Recommendation Engine; return response JSON for the client.
- **Type**: Processing
