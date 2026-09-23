# D2C AI Creative Diversity Engine

An n8n workflow that turns a D2C product URL into product intelligence, customer insights, strategic creative angles, and product-consistent static ad concepts using Google Gemini.

## What it does

```text
Product URL
    ↓
Product Page Extraction
    ↓
Product Intelligence
    ↓
Customer Intelligence
    ↓
Creative Territories
    ↓
Creative Concepts
    ↓
Original Product Image
    ↓
AI Static Ad Generation
```

## Core idea

The goal is not to generate hundreds of random ads.

The workflow starts with the actual product and builds different creative directions around different customer motivations, problems, desires, and product proofs.

This creates **creative diversity instead of simple ad variations**.

## Workflow

```text
Product URL
   ↓
Fetch Product Page
   ↓
Extract Product Content
   ↓
Extract Product Image
   ↓
Product Intelligence
   ↓
Customer Intelligence
   ↓
4 Creative Territories
   ↓
Split Territories
   ↓
Attach Original Product Image
   ↓
Gemini Image Generation / Editing
```

## Built With

- n8n
- Google Gemini
- Google AI Studio API
- JavaScript
- HTML extraction

## Current Output

The workflow is designed to produce:

- Structured product information
- Customer motivations and buying insights
- Distinct creative territories
- Product-specific creative concepts
- Static ad concepts based on the original product image

## Product Consistency

The original product image is used as the visual reference for ad generation.

The workflow instructs the image model to preserve:

- Product design
- Shape
- Color
- Material
- Proportions
- Distinctive product details

The objective is to create different advertising concepts without changing the underlying product.

## Setup

### Requirements

- n8n
- Google Gemini API key
- A product URL
- Access to a Gemini model supported by your n8n setup

### Import the workflow

1. Open n8n.
2. Import the workflow JSON from:

```text
workflow/d2c-ai-creative-diversity-engine.json
```

3. Add your own Gemini credentials.
4. Open the Form Trigger.
5. Enter a product URL.
6. Execute the workflow.

## Example Input

```text
https://example.com/products/product-name
```

## Example Creative Structure

A product may generate different territories such as:

```text
ANGLE 01
Customer Problem

ANGLE 02
Product Differentiation

ANGLE 03
Emotional Desire

ANGLE 04
Use Case / Purchase Motivation
```

The actual territories depend on the product and the information available on its page.

## Important

This project does **not** claim to generate or control an internal Meta/Andromeda Entity ID.

The workflow uses an internal creative-diversity framework to create meaningfully different creative concepts.

## Current Scope

This version focuses on:

- Product intelligence
- Customer intelligence
- Creative strategy
- Product-consistent static ad generation

Future versions may add:

- Larger creative batches
- Creative similarity scoring
- Meta Ads performance data
- Creative performance diagnosis
- Automated creative testing loops
- Meta API integrations

## Security

Never commit API keys, access tokens, passwords, or private credentials to this repository.

Use n8n credentials or environment variables for secrets.

## License

MIT License

## Author

Built by Deepak Kumar.

Product & Performance Marketer focused on:

```text
D2C
Product Marketing
Performance Marketing
AI Automation
Creative Strategy
```
