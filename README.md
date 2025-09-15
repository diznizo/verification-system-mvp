# verification-system-mvp
low cost ,practical build plan for an AI +Hashing+ZKP-powered impact verification system
# Verification System MVP — Low-Cost Build Plan

A practical roadmap for building a next-generation impact verification system powered by:
- AI-assisted checks
- Hashing + perceptual hashing
- Device signing
- Zero-Knowledge Proofs (ZKPs)
- Low-cost, community-powered data capture

---

## 1. Field Data Capture (Zero Cost)
- Use **Google Forms / KoboToolbox** for mobile data collection.
- Fields: Project ID, GPS, photos, videos, timestamps.
- Each submission auto-uploads to Google Drive / Kobo server.

---

## 2. Hashing & Anti-Fraud Layer
- Hash each photo/video locally before upload.
- Use **Perceptual Hashing** (pHash) to catch duplicate or slightly edited photos.
- Store hashes in a public ledger (Google Sheets at first → later blockchain).

---

## 3. Device Identity & Proof
- Every submission tagged with:
  - Device signature (IMEI or app UUID).
  - GPS + timestamp auto-captured.
- Prevents resubmitting the same media from multiple accounts.

---

## 4. Multi-Angle Evidence Protocol
- Require 3+ photos per tree/object:
  - Different angles.
  - With reference object (hand, coin, card).
  - Geo-tagged.
- AI checks for similarity to ensure they are unique trees/objects.

---

## 5. Verification AI (Optional, Low-Cost)
- Free models: Hugging Face / TensorFlow Lite on mobile.
- Classify “tree” vs. “non-tree”.
- Reject invalid or irrelevant photos.

---

## 6. Zero-Knowledge Proofs (Future Upgrade)
- Farmers/orgs don’t share sensitive raw data.
- Instead, submit ZKPs that claims are true (e.g., “I have 1,000 unique trees”).
- Donors trust proofs without raw exposure.

---

## 7. Storage & Ledger
- Start simple: Google Sheets or Airtable as verification log.
- Each entry: Project ID, hash, timestamp, verifier status.
- Later → migrate to blockchain (Polygon/NEAR for low cost).

---

## 8. Verification Workflow
1. Youth/verifier collects data → uploads via Google Form.
2. Script hashes media + logs in verification sheet.
3. AI + human review rejects duplicates/fakes.
4. Approved data = “Verified Impact Unit” (VIU).
5. Ledger records transaction (Google Sheet now, blockchain later).

---

## 9. Cost-Minimized Stack
- **Google Forms** (free).
- **Google Drive** (15GB free).
- **Google Sheets** (free).
- **pHash libraries** (open-source).
- **Python scripts** (free).
- **Hugging Face AI models** (free tiers).
- **Optional**: Airtable free tier for nicer dashboards.

---

## 10. Future Extensions
- IoT sensors for long-term monitoring.
- Drones for random audits.
- Blockchain integration for trustless logging.
- Global API for donors to verify in real time.

---

### ✅ Why This Works
- Prevents duplicate photos → fraud reduction.
- Device signing → no double reporting.
- pHash → detects recycled images.
- Multi-angle protocol → ensures real evidence.
- Start lean (Google tools) → scale to blockchain + ZKPs.

