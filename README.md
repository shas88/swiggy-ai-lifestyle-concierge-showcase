# swiggy-ai-lifestyle-concierge-showcase
AI Lifestyle Concierge integrating Food, Instamart and Dineout workflows | Swiggy Builders Club
# AI Lifestyle Concierge

An occasion-driven AI commerce experience built for the **Swiggy Builders Club**.

Instead of making users think in separate services like Food, Instamart, or Dineout, the product is designed around a simpler idea:

> Users think in occasions, not APIs.

A user can start from an intent such as planning dinner or preparing for an evening, and the experience can coordinate the relevant Swiggy services behind the scenes.

## Product Concept

The AI Lifestyle Concierge brings together:

- Swiggy Food
- Swiggy Instamart
- Swiggy Dineout

into one guided experience.

The goal was to explore how conversational AI and external service integrations can reduce friction across multiple commerce journeys.

## My Role

I designed and built the product end-to-end, including:

- Product concept and user flows
- Technical architecture
- Laravel application development
- Swiggy MCP integrations
- OAuth 2.1 + PKCE authentication
- API orchestration
- Cart and booking workflows
- Production deployment
- End-to-end testing
- Demo preparation for Swiggy Builders Club review

## Key Capabilities

### Food

- Restaurant discovery
- Restaurant menu retrieval
- Menu search
- Item customization
- Swiggy cart integration

### Instamart

- Product discovery
- Product recommendations
- Cart updates
- Real cart interaction

### Dineout

- Restaurant discovery
- Restaurant details
- Available slot retrieval
- Guest/date/time selection
- Deal-based table booking

A complete Dineout journey was validated with a real reservation and booking confirmation.

## Architecture

The application uses a Laravel-based product layer with Node.js services handling Swiggy MCP communication.

```text
User
  |
  v
Laravel Application
  |
  | Authenticated Requests
  v
Node.js MCP Client Layer
  |
  | OAuth Access Token
  v
Swiggy MCP Services
  |
  +---- Food
  |
  +---- Instamart
  |
  +---- Dineout
