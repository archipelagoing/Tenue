# TENUE ; who is your fragrance?
## Verified Fragrance Ownership and Presence Network

TENUE is a platform that transforms luxury fragrance from a private object into a persistent, visible, and social identity layer.

Users register the exact fragrances they own, log when they wear them, and connect with others through shared ownership. Each fragrance forms its own network ("village"), and each wear event contributes to a living map of fragrance presence.

TENUE enables identity to persist through scent.

---

# Core Principles

TENUE is built on three fundamental signals:

### Ownership
Permanent record of which fragrances a user owns.

Ownership is binary. You either own a fragrance or you do not.

Ownership defines identity structure.

---

### Presence
Temporal record of when a fragrance is worn.

Presence evolves over time through wear logging.

Presence defines identity continuity.

---

### Village
Community formed by shared ownership of a specific fragrance.

Each fragrance automatically forms its own network of owners.

Villages define identity adjacency.

---

# System Overview

TENUE consists of five core subsystems:

- Identity System
- Ownership System
- Presence (Wear Logging) System
- Village System
- Cultural Intelligence System

---

# Feature Breakdown

## Identity System

Provides persistent user identity.

Features:

- Email authentication
- User profile
- Username
- Profile photo (optional)
- LinkedIn integration (optional)
- Friend system (future expansion)

Purpose:

Creates persistent identity surface.

---

## Ownership System

Tracks exact fragrance possession.

Features:

- Add fragrance to profile
- Ownership record creation
- Ownership timestamp
- Verified ownership (future: NFC / QR)
- Automatic village assignment

Ownership records are permanent.

---

## Presence System (Wear Logging)

Tracks fragrance usage over time.

Features:

- Log wear event
- Wear history timeline
- Most worn fragrances
- Presence strength calculation

Future integration:

- NFC tap logging
- QR scan logging

Presence transforms ownership into living identity.

---

## Village System

Each fragrance forms its own community.

Village page includes:

- Fragrance information
- Owner list
- Ownership count
- Presence activity

Villages are generated dynamically.

---

## Cultural Intelligence System

Tracks fragrance presence across all users.

Features:

- Most owned fragrances
- Most worn fragrances
- Trending fragrances
- Presence momentum detection

Creates real-time cultural map of fragrance presence.

---

## Journal System

Tracks relationship between user and fragrance over time.

Features:

- Wear timeline
- Ownership timeline
- Optional notes
- Usage frequency

Creates narrative continuity.

---

# NFC / QR Integration Model (Future)

First tap or scan:

- Registers ownership
- Creates ownership certificate
- Assigns village membership

Subsequent taps or scans:

- Logs wear event
- Updates presence timeline
- Updates cultural intelligence layer

MVP simulates this interaction via software button.

---

# Technology Stack

## Frontend

- Next.js
- React
- TypeScript
- TailwindCSS

Purpose:

- User interface
- Client-side interaction
- State management

Hosted on:

- Vercel

---

## Backend

- Supabase

Provides:

- PostgreSQL database
- Authentication
- API layer
- Row-level security

Supabase functions as backend-as-a-service.

---

## Database

PostgreSQL via Supabase.

Stores:

- Users
- Fragrances
- Ownership records
- Wear events
- Friend relationships

---

## Authentication

Supabase Auth

Supports:

- Email login
- Session management
- OAuth (future expansion)

---

## Infrastructure

- Frontend: Vercel
- Backend: Supabase
- Database: PostgreSQL

Fully serverless architecture.

---

# Database Schema

## Users

Stores identity.

Fields:

- id (uuid, primary key)
- email (text, unique)
- username (text)
- profile_photo_url (text)
- linkedin_url (text)
- created_at (timestamp)

---

## Fragrances

Stores fragrance objects.

Fields:

- id (uuid, primary key)
- name (text)
- brand (text)
- image_url (text)
- fragrantica_url (text)
- created_at (timestamp)

---

## Ownership

Stores permanent ownership records.

Fields:

- id (uuid, primary key)
- user_id (uuid, foreign key)
- fragrance_id (uuid, foreign key)
- verified (boolean)
- created_at (timestamp)

---

## WearEvents

Stores wear logging events.

Fields:

- id (uuid, primary key)
- user_id (uuid, foreign key)
- fragrance_id (uuid, foreign key)
- created_at (timestamp)

---

## Friends (Future Expansion)

Stores friend relationships.

Fields:

- id (uuid, primary key)
- requester_id (uuid)
- receiver_id (uuid)
- status (pending, accepted)
- created_at (timestamp)

---

# Core API Operations

## Register User

Creates new user identity.

---

## Add Ownership

Creates ownership record and assigns village membership.

---

## Log Wear Event

Creates presence record and updates journal timeline.

---

## Fetch Profile

Returns:

- Ownership records
- Wear history
- Village memberships

---

## Fetch Fragrance Village

Returns:

- Owner list
- Ownership count
- Presence activity

---

# Core Pages

## Login Page

Handles authentication.

---

## Profile Page

Displays:

- Owned fragrances
- Wear timeline
- Village memberships

---

## Fragrance Page (Village Page)

Displays:

- Fragrance information
- Owner list
- Village activity

---

## Add Fragrance Page

Allows users to register ownership.

---

## Journal Page

Displays wear history timeline.

---

# Presence Model

Presence weight derived from wear frequency.

Example:

presence_weight = log(1 + wear_count)

This prevents runaway scaling while preserving relative strength.

Presence weight powers:

- Cultural rankings
- Identity strength
- Village activity

---

# Deployment

Frontend:

- Deploy using Vercel

Backend and database:

- Supabase

No dedicated backend server required.

Fully serverless deployment.

---

# MVP Scope

Minimum viable TENUE includes:

- User authentication
- Add fragrance ownership
- Profile page
- Fragrance village page
- Wear logging button
- Wear history timeline

Hardware integration not required for MVP.

---

# Future Expansion

Planned features:

- NFC ownership verification
- QR ownership verification
- Blockchain ownership certificates
- AI cultural intelligence modeling
- Recommendation systems

These extend the ownership-presence model.

---

# Vision

TENUE creates a persistent identity layer anchored in fragrance ownership.

Ownership defines structure.

Presence defines continuity.

Villages define connection.

TENUE transforms fragrance into shared cultural presence.
