# Wochi

## The Story Behind The Name

"Wochi" (from Kenyan Sheng, meaning watchman) embodies the spirit of community guardianship in everyday Kenyan life. Just as the neighborhood wochi keeps watch over the community, this project keeps watch over financial institutions and their pricing practices.

The name choice reflects our roots in local culture while addressing a universal need for financial oversight. Like the trusted wochi who knows every corner of their territory, this tool examines the details of loan pricing that might otherwise go unnoticed.

## The African Connection: Kwezi

Our project's mission also parallels "Kwezi" (meaning "Star" in Xhosa and Zulu), a South African superhero created by Loyiso Mkize. Both Wochi and Kwezi represent:

- **Illumination**: As Kwezi brings light like a star, Wochi illuminates financial practices
- **Community Protection**: Both serve their communities through vigilance and action
- **Modern African Narrative**: Blending traditional values with contemporary challenges
- **Corporate Responsibility**: Keeping watch over institutional practices

## Project Overview

Wochi analyzes how financial institutions adjust their variable loan rates in response to Monetary Policy Committee (MPC) changes. It serves as a guardian by:

- Analyzing loan documents to extract rate terms
- Tracking historical rate adjustments
- Identifying patterns in bank rate modifications
- Quantifying the impact on borrowers
- Providing transparency in banking practices

## Technical Architecture

### Current Implementation
- **Frontend**: Next.js application
- **Backend**: FastAPI Python server
- **Storage**: MinIO for document management
- **Analysis**:
  - Python scripts for rate analysis
  - LLM integration for document processing
  - Data visualization with D3.js
- **Deployment**: Kamal for production deployment

### Future Implementation (V2)
- Edge computing for enhanced privacy
- Client-side document processing
- Zero-knowledge proof implementations
- End-to-end encryption

## Getting Started

```bash
# Clone repository
git clone https://github.com/ds-ke/wochi.git

# Frontend
cd wochi/frontend
npm install
npm run dev

# Backend
cd ../backend
python -m venv venv
source venv/bin/activate  # or `venv\Scripts\activate` on Windows
pip install -r requirements.txt
uvicorn main:app --reload
```

## Deployment

We use Kamal for zero-downtime deployments:

```bash
# Install Kamal
gem install kamal

# Setup deployment
kamal setup

# Deploy
kamal deploy
```

## Project Structure
```
wochi/
├── frontend/          # Next.js application
├── backend/          # FastAPI server
│   ├── analysis/    # Analysis scripts
│   ├── models/      # Data models
│   └── services/    # Business logic
├── deploy/           # Kamal deployment configs
└── docs/            # Documentation
```

## License

MIT License

---

*"Tunawalinda" (We are watching over them)* - Wochi

*"Ukukhanya kuza ngenkanyezi"* (Light comes from the star) - Inspired by Kwezi

## Roadmap

- [x] V1: Basic implementation with FastAPI and Next.js
- [ ] V2: Edge computing implementation
- [ ] V3: Enhanced privacy features
- [ ] V4: Mobile application