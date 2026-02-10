# TENUE — Build Plan (Feature Map + MVP + Execution)

---

## 1) The Complete TENUE Feature Map (Full Vision)

This is the entire system, structurally.

---

### Layer 1: Identity Layer

**This is the foundation.**

**Features**
- User accounts (email login)
- Profile page
- Profile photo
- LinkedIn integration
- Friends system

**Purpose**  
Creates persistent identity.

---

### Layer 2: Ownership Layer

**This defines what fragrances a user owns.**

**Features**
- Add fragrance to profile
- Fragrance ownership record
- Verified ownership *(future: NFC / QR)*
- Ownership timestamp
- Village membership

**Purpose**  
Defines identity structure.

---

### Layer 3: Presence Layer (Wear Logging)

**This defines how identity evolves over time.**

**Features**
- Log wear event *(button for MVP)*
- Wear history timeline
- Most worn fragrance
- Presence strength

**Future**
- NFC tap logging
- QR logging

**Purpose**  
Defines identity behavior.

---

### Layer 4: Village Layer (Community)

**This connects users.**

**Features**
- Fragrance page (village)
- List of owners
- List of friends who own it
- Most present members

**Purpose**  
Creates community.

---

### Layer 5: Cultural Layer (Global View)

**This shows macro patterns.**

**Features**
- Most owned fragrances
- Most worn fragrances
- Trending fragrances
- Leaderboard

**Purpose**  
Makes TENUE culturally alive.

---

### Layer 6: Journal Layer

**This creates emotional continuity.**

**Features**
- Wear timeline
- Optional notes
- Ownership timeline

**Purpose**  
Creates narrative.

---

## 2) The MVP (What You ACTUALLY Build First)

Build only these 5 features initially:

1. User account  
2. Add fragrance ownership  
3. Profile page showing owned fragrances  
4. Fragrance page showing owners (village)  
5. Log wear button  

**That’s it.**

No blockchain.  
No NFC yet.  
No AI yet.  

Those come later.

This small system is enough to demonstrate TENUE.

---

## 3) The Actual Screens You Need

Only build these pages:

### Page 1: Login Page
User logs in.

---

### Page 2: Profile Page
Shows:
- username
- owned fragrances
- wear history

Example:

**Archi**

**Owned:**  
- Delina  
- Baccarat Rouge 540  

**Recent wears:**  
- Feb 12 — Delina  
- Feb 10 — BR540  

---

### Page 3: Add Fragrance Page
User selects fragrance from list.  
Click: **“Add to my collection”**

---

### Page 4: Fragrance Page (Village Page)
Example:

**Delina**

**Owners:**  
- Archi  
- Maya  
- Jordan  

---

### Page 5: Log Wear Button
Inside profile or fragrance page:

Button: **“Log wear”**  
Press → logs wear event

---

## 4) Technology Stack (Use This Exact Stack)

Do not overcomplicate this.

- **Frontend:** Next.js  
- **Backend + Database:** Supabase  
- **Hosting:** Vercel  

Simple and powerful.

---

## 5) Database Tables (Minimum Required)

### Users
- id  
- email  
- username  
- created_at  

### Fragrances
- id  
- name  
- brand  
- image_url  

### Ownership
- id  
- user_id  
- fragrance_id  
- created_at  

### WearEvents
- id  
- user_id  
- fragrance_id  
- created_at  

That’s enough.

---

## 6) Build Order (CRITICAL)

Follow this exact order. Do not skip around.

1. Create Supabase project  
2. Create Users table  
3. Create Fragrances table  
4. Create Ownership table  
5. Create WearEvents table  
6. Build login page  
7. Build profile page  
8. Build add fragrance button  
9. Build fragrance village page  
10. Build log wear button  

Now TENUE exists.

---

## 7) What This Looks Like When Done

- User signs up  
- Adds Delina  
- Their profile shows Delina  
- They click **“Log wear”**  
- Wear history appears  
- They click **Delina**  
- They see other Delina owners  

This is already powerful. Everything else is expansion.

---

## 8) What Makes TENUE Special (Mental Model)

TENUE is **not** a perfume database.

TENUE is:

> A network of presence anchored in fragrance ownership.

- Ownership creates structure  
- Wear creates motion  
- Villages create connection  

That’s the system.
