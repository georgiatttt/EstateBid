# EstateBid

EstateBid is a full-stack web application for managing estate sales, with AI-assisted item descriptions and comparable sales analysis.

This project was developed as a **collaborative group project** and represents a complete end-to-end system spanning frontend, backend, database design, and AI integration.

---

## Project Overview

EstateBid provides a centralized platform for estate sales, allowing sellers to list and manage all items in one place while receiving pricing recommendations supported by transparent comparable sales data. The system replaces fragmented workflows with a structured, data-driven approach to inventory management, public listings, and auction pricing.

The system is designed to handle multi-item auctions, public bidding, and seller-only management views with appropriate access controls.

---

## Key Capabilities

- **Auction and Inventory Management**
  - Create and manage multi item estate auctions
  - Configure auction level and item level bidding rules
  - Publish public auction pages for bidders

- **AI Assisted Item Intelligence**
  - Generate professional item descriptions from images using vision enabled LLMs
  - Retrieve and store comparable sales data from external marketplaces
  - Batch processing for cost efficient AI usage

- **Bidding and Public Views**
  - Public auction pages for bidders
  - Real time bid placement and tracking
  - Countdown timers and auction state transitions

- **Data and Export**
  - Structured relational data model for auctions, items, bids, and users
  - Excel export for seller reporting and offline workflows

---

## Tech Stack

**Frontend**
- React (Vite)
- TailwindCSS + shadcn/ui
- Framer Motion
- Supabase Authentication

**Backend**
- FastAPI (Python)
- PostgreSQL (Supabase)
- RESTful API design

**AI & Data**
- OpenAI GPT-4o (text + vision)
- Comparable-sales retrieval and storage pipeline

---

## Architecture Highlights

- Clear separation between public auction views and authenticated seller dashboards
- Role-based access enforced via Supabase Auth and Row Level Security (RLS)
- Modular API design for auctions, items, bids, images, and AI services
- Batch-oriented AI workflows to reduce cost and latency

---
## Project Structure (High Level)

```
EstateBid/
├── backend/            # FastAPI application and API routes
├── front-end/          # React frontend
├── requirements.txt    # Python dependencies
└── .env.example        # Environment variable templates
```

---
## License

MIT
