# margdarshak-gwalior
Deterministic-AI Hybrid Engine for Time-Constrained Tourism in Gwalior (AI Synergy Hackathon 2026 - Track 04)
# MargDarshak Gwalior: Beyond the Fort
> **Track 04: Tourism** — *AI Synergy Hackathon 2026 (ABV-IIITM Gwalior)*
> **Solution Architecture:** Deterministic-AI Hybrid Feasibility & Optimization Engine

---

## 🔗 Live Prototype & Artifact Links
* **Live Interactive Web App (Google AI Studio Hosted):**  
  https://margdarshak-gwalior-beyond-the-fort.ai.studio
* **Executable Google Colab Backend:**  
  https://colab.research.google.com/drive/1qNhcJdY6REd99h1jdb7IIy3s4_r9lH4L?usp=sharing
* **Presentation Deck (PDF):** [`MargDarshak_Solution_Presentation.pdf`](./MargDarshak_Solution_Presentation.pdf)
* **System Requirements Specification & SRS (PDF):** [`MargDarshak_Gwalior_Page_3_Solution_Overview_SRS.pdf`](./MargDarshak_Gwalior_Page_3_Solution_Overview_SRS.pdf)

---

## 📌 Problem Diagnosis & Core Engineering Challenge
Time-constrained transit travelers arriving at Gwalior Junction (4–8 hour window) face recurring itinerary breakdowns, arrive at locked gates, and miss authentic regional crafts:
1. **Asynchronous Multi-Agency Off-Days:** Fragmented governance across ASI Bhopal Circle (Friday Fort museum closure), MP State Archaeology (Gujari Mahal closed Mondays), and Scindia Devasthan Trust (Jai Vilas Palace closed Mondays).
2. **Topological Cliff Barrier:** A 100-meter vertical sandstone ridge separates the plain from the fort plateau. Urvai Gate provides the sole vehicular road access, whereas the eastern Gwalior/Hathi Pol approach consists of steep pedestrian stone steps.
3. **Train-Departure Risk:** Static generative LLMs frequently hallucinate transit times, ignore topography, and risk visitors missing scheduled rail connections.

---

## 🏛️ System Architecture: Bounded Hybrid Model
MargDarshak isolates arithmetic and policy enforcement inside a **deterministic constraint solver** while using language models strictly for natural language intent normalization and grounded historical retrieval:

- **Layer 1 (NLP Parser):** Normalizes budget, start time, and mobility toggles.
- **Layer 2 (Deterministic Solver):** Enforces schedule exclusions, stair bypasses, knapsack time bounds, and multi-agency tariffs.
- **Layer 3 (Proximity Embedding):** Automatically matches verified ODOP sandstone sculptors and culinary anchors within 800m.

---

## 🧪 Technical Feasibility Proof: Automated Acceptance Tests (3/3 Passed)
The underlying algorithmic core has been verified in Python 3.11 with an automated test suite operating in `< 5 ms`:
- **TEST 1 (Temporal Feasibility):** Intercepted Monday closure of Gujari Mahal (MP State Archaeology); generated valid alternative route (Tansen Tomb + Man Mandir) in 155 mins. -> **PASS**
- **TEST 2 (Topological & Mobility):** Excluded eastern pedestrian cliff stairs; enforced vehicular routing via Urvai Gate ramp. -> **PASS**
- **TEST 3 (Micro-Merchant Inclusion):** Embedded verified local ODOP sandstone artisans (450m) and 80-year-old culinary anchors in Sarafa Bazaar (150–350m). -> **PASS**

---

## 🚫 Version 1 Scope Boundaries (What V1 Intentionally Does NOT Do)
* **NO Live Ticketing:** Only displays transparent tariff breakdowns; no payment gateway integration.
* **NO Open Merchant Onboarding:** Micro-merchants must be vetted by administrators to protect ODOP authenticity.
* **NO Turn-by-Turn Voice Navigation:** Provides sequenced routing and transit modes, not active GPS turn guidance.
* **NO Open-Ended Historical Generation:** History and site notes are strictly retrieved from verified official documents via RAG.
