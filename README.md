# Chatwoot (chatwoot-com)

Chatwoot is an open-source customer engagement and support suite that unifies email, live-chat, social, and messaging channels into a single shared inbox. Agents, teams, contacts, conversations, and messages are all managed through a REST API surface split across an Application API, a Client API for end-user widgets, and a Platform API for super-admin installation control. Chatwoot is available as self-hostable open-source software and as Chatwoot Cloud.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/apis.yml)

## Tags

- Customer Support
- Customer Engagement
- Shared Inbox
- Live Chat
- Open Source
- Omnichannel
- Help Desk

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## Authentication

Application and Platform API requests authenticate with an `api_access_token` HTTP header (an agent/user token for the Application API, a Platform App token for the Platform API). Client API requests are scoped by an inbox identifier and a contact identifier / pubsub token rather than a static header key. Chatwoot Cloud is served from `https://app.chatwoot.com`; for self-hosted installations substitute your own host.

## APIs

### Chatwoot Application Agents API

Manage agents within an account - list, add, update the role and availability of, and remove agents who staff the shared inbox.

- **Human URL:** [https://developers.chatwoot.com/api-reference/agents](https://developers.chatwoot.com/api-reference/agents)
- **Base URL:** `https://app.chatwoot.com/api/v1/accounts/{account_id}`

#### Tags

- Agents
- Application API

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/agents)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Application Teams API

Create and manage teams and their agent membership so conversations can be routed to the right group of agents.

- **Human URL:** [https://developers.chatwoot.com/api-reference/teams](https://developers.chatwoot.com/api-reference/teams)
- **Base URL:** `https://app.chatwoot.com/api/v1/accounts/{account_id}`

#### Tags

- Teams
- Application API

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/teams)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Application Inboxes API

List, create, update, and delete inboxes across channels (website live-chat, email, and social/messaging), and manage the agents assigned to each inbox.

- **Human URL:** [https://developers.chatwoot.com/api-reference/inboxes](https://developers.chatwoot.com/api-reference/inboxes)
- **Base URL:** `https://app.chatwoot.com/api/v1/accounts/{account_id}`

#### Tags

- Inboxes
- Channels
- Application API

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/inboxes)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Application Contacts API

Manage contacts - create, list, search, filter, update, and delete the people who reach out, plus list a contact's conversations, contactable inboxes, and labels.

- **Human URL:** [https://developers.chatwoot.com/api-reference/contacts](https://developers.chatwoot.com/api-reference/contacts)
- **Base URL:** `https://app.chatwoot.com/api/v1/accounts/{account_id}`

#### Tags

- Contacts
- CRM
- Application API

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/contacts)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Application Conversations API

Create and manage conversations - list with filters, toggle status, assign to agents or teams, update priority, and manage conversation labels and custom attributes.

- **Human URL:** [https://developers.chatwoot.com/api-reference/conversations](https://developers.chatwoot.com/api-reference/conversations)
- **Base URL:** `https://app.chatwoot.com/api/v1/accounts/{account_id}`

#### Tags

- Conversations
- Application API

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/conversations)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Application Messages API

Create, list, and delete messages within a conversation, including outgoing agent replies, private notes, and attachments.

- **Human URL:** [https://developers.chatwoot.com/api-reference/messages](https://developers.chatwoot.com/api-reference/messages)
- **Base URL:** `https://app.chatwoot.com/api/v1/accounts/{account_id}`

#### Tags

- Messages
- Application API

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/messages)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Application Labels API

List the account's labels and read or set the labels applied to individual conversations and contacts for organization and reporting.

- **Human URL:** [https://developers.chatwoot.com/api-reference/labels](https://developers.chatwoot.com/api-reference/labels)
- **Base URL:** `https://app.chatwoot.com/api/v1/accounts/{account_id}`

#### Tags

- Labels
- Application API

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/labels)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Application Custom Attributes API

Define and manage custom attribute definitions for conversations and contacts so installation-specific data can be captured and filtered on.

- **Human URL:** [https://developers.chatwoot.com/api-reference/custom-attributes](https://developers.chatwoot.com/api-reference/custom-attributes)
- **Base URL:** `https://app.chatwoot.com/api/v1/accounts/{account_id}`

#### Tags

- Custom Attributes
- Application API

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/custom-attributes)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Application Canned Responses API

Manage canned responses (saved replies) - list, create, update, and delete the short-code reply templates agents use to answer faster.

- **Human URL:** [https://developers.chatwoot.com/api-reference/canned-responses](https://developers.chatwoot.com/api-reference/canned-responses)
- **Base URL:** `https://app.chatwoot.com/api/v1/accounts/{account_id}`

#### Tags

- Canned Responses
- Application API

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/canned-responses)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Application Automation Rules API

Create and manage automation rules that fire on events (conversation created, updated, message created) to auto-assign, label, and act on conversations from conditions.

- **Human URL:** [https://developers.chatwoot.com/api-reference/automation-rule](https://developers.chatwoot.com/api-reference/automation-rule)
- **Base URL:** `https://app.chatwoot.com/api/v1/accounts/{account_id}`

#### Tags

- Automation
- Rules
- Application API

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/automation-rule)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Application Reports API

Retrieve account-level and agent/team/inbox/label-level metrics - conversation counts, incoming/outgoing volume, resolution and response times, and conversation summary reports.

- **Human URL:** [https://developers.chatwoot.com/api-reference/reports](https://developers.chatwoot.com/api-reference/reports)
- **Base URL:** `https://app.chatwoot.com/api/v1/accounts/{account_id}`

#### Tags

- Reports
- Analytics
- Application API

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/reports)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Client Contacts API

End-user (widget-facing) API to create and update the contact tied to an inbox identifier, returning a pubsub token used to authenticate that contact's subsequent client requests.

- **Human URL:** [https://developers.chatwoot.com/api-reference/client-apis/contacts](https://developers.chatwoot.com/api-reference/client-apis/contacts)
- **Base URL:** `https://app.chatwoot.com/public/api/v1/inboxes/{inbox_identifier}`

#### Tags

- Client API
- Contacts
- Widget

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/client-apis/contacts)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Client Conversations API

End-user API for a contact to create and list their conversations and to toggle status, toggle typing, and update last-seen from within a custom chat interface.

- **Human URL:** [https://developers.chatwoot.com/api-reference/client-apis/conversations](https://developers.chatwoot.com/api-reference/client-apis/conversations)
- **Base URL:** `https://app.chatwoot.com/public/api/v1/inboxes/{inbox_identifier}`

#### Tags

- Client API
- Conversations
- Widget

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/client-apis/conversations)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Client Messages API

End-user API for a contact to create, list, and update messages in their conversation, powering a fully custom chat widget on top of Chatwoot.

- **Human URL:** [https://developers.chatwoot.com/api-reference/client-apis/messages](https://developers.chatwoot.com/api-reference/client-apis/messages)
- **Base URL:** `https://app.chatwoot.com/public/api/v1/inboxes/{inbox_identifier}`

#### Tags

- Client API
- Messages
- Widget

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/client-apis/messages)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Platform Users API

Super-admin API to create, read, update, and delete users across an installation and to obtain a single-sign-on login URL for a user.

- **Human URL:** [https://developers.chatwoot.com/api-reference/platform-apis/users](https://developers.chatwoot.com/api-reference/platform-apis/users)
- **Base URL:** `https://app.chatwoot.com/platform/api/v1`

#### Tags

- Platform API
- Users
- Administration

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/platform-apis/users)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Platform Accounts API

Super-admin API to provision and manage accounts on an installation and to manage the association of users to accounts via account users.

- **Human URL:** [https://developers.chatwoot.com/api-reference/platform-apis/accounts](https://developers.chatwoot.com/api-reference/platform-apis/accounts)
- **Base URL:** `https://app.chatwoot.com/platform/api/v1`

#### Tags

- Platform API
- Accounts
- Administration

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/platform-apis/accounts)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chatwoot Platform Agent Bots API

Super-admin API to create, read, update, and delete agent bots that can be attached to inboxes to power conversational automation.

- **Human URL:** [https://developers.chatwoot.com/api-reference/platform-apis/agentbots](https://developers.chatwoot.com/api-reference/platform-apis/agentbots)
- **Base URL:** `https://app.chatwoot.com/platform/api/v1`

#### Tags

- Platform API
- Agent Bots
- Automation

#### Properties

- [API Reference](https://developers.chatwoot.com/api-reference/platform-apis/agentbots)
- [OpenAPI](openapi/chatwoot-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chatwoot-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chatwoot-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/chatwoot)
- [LinkedIn](https://www.linkedin.com/company/chatwoot)
- [Website](https://www.chatwoot.com)
- [Documentation](https://developers.chatwoot.com)
- [Plans](plans/chatwoot-com-plans-pricing.yml)
- [Rate Limits](rate-limits/chatwoot-com-rate-limits.yml)
- [Fin Ops](finops/chatwoot-com-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
