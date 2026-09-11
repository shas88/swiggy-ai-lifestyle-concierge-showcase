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

Authentication

The project uses:

OAuth 2.1
PKCE
Secure access-token handling
Authenticated MCP requests

The implementation was designed around Swiggy Builders Club authentication and integration requirements.

Technology Stack
Laravel 12
PHP
JavaScript
Node.js
Model Context Protocol (MCP)
OAuth 2.1 + PKCE
REST / HTTP integrations
Nginx
Linux
Git & GitHub
DigitalOcean
Product Thinking

The central design principle was:

Users should describe what they want to accomplish, while the system coordinates the services required to achieve it.

Example:

"I'm planning a family dinner tonight."

The system can then decide whether the user needs:

Food ordering
Grocery / household items
Restaurant booking
Or a combination of services

This shifts the interface from service selection toward intent-driven orchestration.

Key Engineering Challenges

Some of the interesting technical problems included:

Coordinating multiple external MCP services
Managing authentication across service calls
Maintaining state between user interactions
Refreshing cart state after mutations
Handling different service-specific workflows
Safely separating Laravel product logic from MCP transport logic
Deploying and testing authenticated integrations in production
Live Demo

Live application:
https://concierge.sarshatechnology.com

The source code is maintained in a private repository because the project contains proprietary application logic and protected integration details.

Builders Club

This project was developed as part of the Swiggy Builders Club program.

It is an independent project and does not represent employment by Swiggy.

About Me

I'm Shashwat Asthana, founder of Sarsha Technology and a software engineer / product builder focused on:

SaaS products
Laravel
Applied AI
APIs and integrations
Product architecture
Cloud deployment
Technical product development

GitHub: https://github.com/shas88
Sarsha Technology: https://sarshatechnology.com



> **“It is an independent project and does not represent employment by Swiggy.”**

That's useful because the repository should demonstrate your work without accidentally implying that you worked for Swiggy.

Also, **do not upload source code into this showcase repository later**, even “just a few files.” Keep it purely portfolio-facing.

Once you've committed this README, **pin this repo on your GitHub profile**.

Then we'll create the second showcase for **SmartTask**, which will make the profile suddenly look much less like a ghost town and much more like an actual builder's portfolio. 😄
