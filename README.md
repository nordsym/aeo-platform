# AEO Platform

*Placeholder name - Product namn under utveckling*

AI-powered search optimization audit tool. Analyzes your website's visibility across Answer Engines (ChatGPT, Claude, Perplexity, Gemini) + traditional SEO + local GEO.

🔗 **Live:** [aeo.nordsym.com](https://aeo.nordsym.com) (Closed Beta)

## 🎯 What It Does

**Input:** Your domain  
**Output:** Complete visibility audit with scores for:
- **AEO (Answer Engine Optimization)** - AI chatbot visibility
- **SEO (Search Engine Optimization)** - Traditional Google rankings
- **GEO (Generative Engine Optimization)** - AI-generated answer placement

**The Balance:** All three matter. Pure AEO without SEO/GEO = incomplete strategy.

## ✨ Free Audit Flow

1. **Submit Domain** - Enter website URL
2. **Email Capture** - Intercept modal (theater mode)
3. **Live Analysis** - DataForSEO crawl + GPT-4o-mini analysis
4. **Personalized Report** - Email with scores + recommendations (Swedish)
5. **Consultation Offer** - Upgrade to implementation services

## 🏗️ Architecture

**Single-File SaaS Pattern:**
- **Frontend:** 51KB HTML (vanilla JS + Tailwind)
- **Backend:** n8n workflows
  - Audit trigger webhook
  - DataForSEO integration
  - GPT-4o-mini report generation
  - Email delivery (HTML formatted)
- **Lead Management:** Airtable + Slack notifications
- **Contact Forms:** Formspree

### Tech Stack
```
Frontend:  Vanilla JS, Tailwind CSS, Canvas animations
Backend:   n8n Cloud (nordsym.app.n8n.cloud)
SEO API:   DataForSEO (crawl + analysis)
AI:        GPT-4o-mini (Swedish audit reports)
Emails:    n8n Email nodes (HTML templates)
Forms:     Formspree (pricing/contact)
Hosting:   GitHub Pages → aeo.nordsym.com
```

## 🎨 Design System

**Visual Identity:**
- **Dark Mode:** Starfall canvas animation (Nord cyan/purple)
- **Light Mode:** Grid pattern background
- **AI Logos:** Rotating pulse (ChatGPT, Claude, Perplexity, Gemini, Grok)
- **Typography:** System fonts (performance first)

**Brand Elements:**
- Hero badge: "CLOSED BETA"
- CTA: Theatre mode reveal
- Nord palette: Cyan (#88C0D0) + Purple accents

## 💳 Pricing Model (Lead Gen)

**Free Audit:**
- One-time domain analysis
- Email report (Swedish)
- Basic recommendations

**Paid Plans (Positioning only - leads to custom consulting):**
- **Starter:** 1,999 SEK/mån - Self-service tools
- **Growth:** 4,999 SEK/mån - Managed optimization (HIGHLIGHTED)
- **Enterprise:** Custom - White-glove implementation

**Reality:** Free audit → Discovery call → 60-120k SEK custom projects

## 🚀 User Flow

1. **Landing Page** - Hero form (domain input)
2. **Submit** - Theatre mode reveal
3. **Email Capture** - Intercept modal (required for report)
4. **Processing** - n8n triggers DataForSEO + GPT analysis
5. **Report Delivered** - HTML email with scores + next steps
6. **Slack Notification** - Internal lead tracking
7. **Airtable Save** - CRM entry for follow-up

## 📊 Technical Implementation

### DataForSEO Integration
- **Crawl Trigger:** n8n webhook (`/webhook/aeo-audit-trigger`)
- **Result Webhook:** n8n listener (`/webhook/aeo-audit-results`)
- **Cost:** ~4 SEK per audit (OnPage crawl)

### GPT-4o-mini Report Generation
- **System Prompt:** Swedish AEO/SEO/GEO expert
- **Temperature:** 0.3 (consistency)
- **Output:** Structured audit with scores + actionable recommendations
- **Language:** Svenska (target market)

### Lead Management
- **Airtable:** Domain, email, timestamp, audit status
- **Slack:** Real-time notifications (audit start + completion)
- **Follow-up:** Manual outreach within 24h

## 🧠 Strategic Positioning

### Why AEO + SEO + GEO?

**AEO alone = incomplete:**
- Answer Engines use traditional search signals
- Local GEO critical for Swedish businesses
- Balanced strategy = sustainable visibility

**Free audit = Trust builder:**
- Shows immediate value
- Demonstrates expertise
- Converts to consulting (60-120k SEK projects)

### Competitive Advantage
- **First-mover:** AEO still emerging in Sweden
- **AI-native:** Built by AI automation experts
- **Proven delivery:** Guldkant Portal case study

## 🔗 Links

- **Live Site:** https://aeo.nordsym.com
- **NordSym:** https://nordsym.com
- **Support:** info@nordsym.se
- **DataForSEO:** API integration (OnPage tasks)

## 🛠️ Development

### Local Testing
```bash
# Clone repo
git clone https://github.com/nordsym/aeo-platform.git
cd aeo-platform

# Open index.html in browser
# No build step required (single-file architecture)
```

### Backend Setup
n8n workflows required:
1. `/webhook/aeo-audit-trigger` - Domain submission handler
2. `/webhook/aeo-audit-results` - DataForSEO callback receiver
3. Email delivery workflow (Swedish HTML templates)
4. Slack notification workflow

## 📈 Business Model

**Lead Generation Engine:**
1. Free audit reveals optimization gaps
2. Email report shows potential improvements
3. Discovery call converts to custom project
4. 60-120k SEK implementation contracts
5. Optional: 2-5k SEK/mån ongoing optimization

**Current Status:**
- Live: Closed Beta (aeo.nordsym.com)
- Leads: 1 genuine lead (early validation)
- Goal: Lead engine > Direct SaaS revenue

---

**Built by NordSym AB** | Stockholm | 559535-5768  
**Architecture:** Single-File Lead Magnet | **Stack:** Vanilla JS + n8n + DataForSEO + GPT-4o
