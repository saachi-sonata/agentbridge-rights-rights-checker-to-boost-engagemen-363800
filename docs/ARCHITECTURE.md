# Architecture Documentation

## Overview
This RAG implements Rights Rights Checker to boost engagement for Media & Entertainment use cases.

## Components
1. **Series Intake**: Collect, validate and normalize metadata from CDP; attach a runId and timestamp for traceability.
2. **Retrieve**: Execute retrieve phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
3. **Ground**: Execute ground phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
4. **Recommendation**: Recommendation across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
5. **Rights Validation**: Rights Validation across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
6. **Content Classification**: Content Classification across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
7. **Audience Targeting**: Audience Targeting across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
8. **Programming Grid**: Assemble final payload with status, artifacts, KPIs and audit trail; store to Recommendation Engine; return response JSON for the client.

## Data Flow
- Input: Series Intake
- Processing: 8 sequential steps
- Output: Programming Grid
