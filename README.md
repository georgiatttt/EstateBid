# EstateBid

EstateBid is a full-stack web application for managing estate sales, with AI-assisted item descriptions and transparent comparable sales analysis.

This project was developed as a **collaborative group project** and represents an end-to-end system spanning frontend, backend, database design, and AI integration.

---

## Project Overview

EstateBid provides a centralized platform for estate sales, allowing sellers to list and manage all items in one place while receiving pricing recommendations supported by visible comparable sales data. The system replaces fragmented workflows with a structured, data-driven approach to inventory management, public listings, and auction pricing.

The application supports multi-item auctions, public bidding, and authenticated seller-only management views with role-based access control.

---

## Key Capabilities

### Auction and Inventory Management
- Create and manage multi item estate auctions
- Configure auction level and item level bidding rules
- Publish public auction pages for bidders

### AI Assisted Item Intelligence
- Generate professional item descriptions from images using vision enabled language models
- Retrieve and store comparable sales data from external marketplaces
- Batch processing to reduce AI cost and latency

### Bidding and Public Views
- Public auction pages for bidders
- Real time bid placement and tracking
- Countdown timers and auction state transitions

### Data and Export
- Structured relational data model for auctions, items, bids, and users
- Excel export for seller reporting and offline workflows

---

## Tech Stack

### Frontend
- React (Vite)
- TailwindCSS + shadcn/ui
- Framer Motion
- Supabase Authentication

### Backend
- FastAPI (Python)
- PostgreSQL (Supabase)
- RESTful API design

### AI and Data
- OpenAI GPT-4o (text and vision)
- Comparable-sales retrieval and storage pipeline

---

## Architecture Highlights

- Clear separation between public auction views and authenticated seller dashboards
- Role-based access enforced via Supabase Auth and Row Level Security (RLS)
- Modular API design for auctions, items, bids, images, and AI services
- Batch-oriented AI workflows to reduce cost and latency

---

## Project Structure (High Level)

```text
EstateBid/
├── backend/            # FastAPI application and API routes
├── front-end/          # React frontend
├── requirements.txt    # Python dependencies
└── .env.example        # Environment variable templates
```

---
## License

MIT

