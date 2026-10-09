# Dollea agent integrations

Public connection configuration and discovery documentation for the official
hosted Dollea Salon and Beauty Coworking services in Munich, Germany.

| Service | Streamable HTTP MCP endpoint | Official registry |
| --- | --- | --- |
| Salon | `https://www.dollea.de/mcp/salon` | [de.dollea/salon](https://registry.modelcontextprotocol.io/v0.1/servers/de.dollea%2Fsalon/versions/latest) |
| Beauty Coworking | `https://coworking.dollea.de/mcp/coworking` | [de.dollea/coworking](https://registry.modelcontextprotocol.io/v0.1/servers/de.dollea%2Fcoworking/versions/latest) |

Clients accepting an `mcpServers` configuration can use [mcp.json](mcp.json).
Public catalog and discovery tools are available anonymously. Account-specific
prices, booking confirmation and private records require the customer's scoped
OAuth authorization with PKCE. Coworking booking permissions follow the normal
customer approval process. Bookings use current, short-lived offers and explicit
consent; repeating an already confirmed offer returns its existing outcome.

Service names, prices, durations, eligible specialists, workspaces, equipment,
availability and promotions are read from the live business records. This package
contains endpoint configuration; agents obtain business data from the current
tools and discovery documents.

| Interface | Live discovery or documentation |
| --- | --- |
| Developer reference, DE/EN/RU | [Dollea for agents](https://www.dollea.de/agents/?language=en) |
| ARD 0.91 | [Publisher manifest](https://dollea.de/.well-known/ard.json) |
| UCP 2026-08-25 | [Business profile](https://dollea.de/.well-known/ucp) |
| UCP booking capability | [Schema and operations](https://dollea.de/ucp/schemas/booking.openapi.json) |
| REST API | [OpenAPI](https://www.dollea.de/api/v1/agents/openapi.json) |
| WebMCP | Native browser tools on the [salon website](https://www.dollea.de/) and [coworking portal](https://coworking.dollea.de/) |
| OAuth discovery | [Authorization server](https://coworking.dollea.de/.well-known/oauth-authorization-server) |

The public release has been tested with the official MCP SDK, native Chromium
WebMCP, isolated salon and rental calendars, current pricing, scoped access,
confirmation replay and the ordinary manual booking workflow.

Maintained by Dollea. Website: https://www.dollea.de/ . Support: info@dollea.de.
