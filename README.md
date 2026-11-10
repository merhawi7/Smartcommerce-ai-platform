# SmartCommerce AI

An e-commerce platform concept with real-time event tracking, product recommendations and a business dashboard.

**Live demo:** https://YOUR-USERNAME.github.io/smartcommerce-ai/

## What the demo shows

- Storefront where every click (search, product view, add to cart, purchase) creates an event
- Event pipeline view: API, Pub/Sub, consumer, BigQuery
- Admin dashboard: revenue, orders, active shoppers, conversion, abandoned carts, top products, live activity
- Recommendations ("shoppers also viewed") and simple rule-based business insights
- Keyword-based shopping assistant

## Current status

The demo is a **front-end prototype**. Traffic, pipeline stages and dashboard numbers are **simulated in the browser**. It is not yet connected to Google Cloud, and the recommendations are co-view counts, not Vertex AI.

## Event schema

```json
{
  "eventId": "EVT-10001",
  "userId": "USER-102",
  "eventType": "PRODUCT_VIEW",
  "productId": "PROD-501",
  "timestamp": "2026-11-10T18:00:00Z"
}
```

## Planned architecture

React + TypeScript, Java 21 + Spring Boot, Cloud SQL (PostgreSQL), Redis, Google Cloud Pub/Sub, BigQuery, Vertex AI, Cloud Run.

## Roadmap

1. Java backend, database, authentication
2. E-commerce frontend and shopping cart
3. Customer tracking and event collection
4. Pub/Sub streaming and BigQuery analytics
5. AI recommendations and shopping assistant
6. GCP deployment, monitoring and testing

## Run locally

Open `index.html` in any browser. No build step needed.
