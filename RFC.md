# RFC: Unified Streaming Usage API

## Abstract

This RFC proposes a standardized API for retrieving personal usage data from streaming platforms. The goal is to empower users with visibility into their own viewing habits, enabling better subscription decisions, screen time awareness, and third-party tooling. The API is designed to be provider-agnostic, privacy-respecting, and extensible.

## Motivation

Streaming services have little incentive to expose usage analytics to end users. Most platforms offer only minimal watch history, if any, and none provide structured, exportable data. This opacity undermines user agency and makes it difficult to:

- Audit personal or household viewing behavior
- Optimize subscription costs
- Build parental controls or screen time dashboards
- Conduct academic or market research

## Definitions

- **Viewing Session**: A discrete period of content playback, including start time, duration, and completion status.
- **Content Metadata**: Title, genre, runtime, provider, and region availability.
- **User Profile**: Subscription status, device types, and household context.

## API Schema Overview

Endpoints (suggested):
- `GET /viewing-history`
- `GET /session-summary`
- `GET /content-metadata`
- `GET /provider-status`

Authentication:
- OAuth2 or token-based access
- Explicit user consent required

## Use Cases

- Personal dashboards for subscription optimization
- Household screen time audits
- Research into media consumption patterns
- Integration with budgeting or wellness apps

## Privacy Considerations

- Data minimization: Only user-authorized data is exposed
- Local-first design: Encourage client-side processing
- Opt-in sharing: No third-party access without consent

## Future Extensions

- Real-time session tracking
- Integration with smart TVs or media centers
- Provider compliance scoring
- Federation across open-source tools
