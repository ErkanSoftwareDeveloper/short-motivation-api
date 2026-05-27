# Short Motivation API
 
A lightweight REST API that serves random motivational quotes. Built with **FastAPI** and deployed on **Render**.
 
**Live URL:** https://short-motivation-api.onrender.com
 
---
 
## About
 
Short Motivation API is a simple, open-access API that returns a random motivational quote with every request. No authentication required, no rate limits — just hit the endpoint and get inspired.
 
---
 
## Endpoints
 
### `GET /`
 
Health check — confirms the API is running.
 
**Response:**
```json
{
  "message": "Motivation API is running!"
}
```
 
---
 
### `GET /quote`
 
Returns a random motivational quote.
 
**Response:**
```json
{
  "quote": "Discipline equals freedom."
}
```
 
---
 
## Tech Stack
 
| Tool | Purpose |
|------|---------|
| [FastAPI](https://fastapi.tiangolo.com/) | Web framework |
| [Uvicorn](https://www.uvicorn.org/) | ASGI server |
| [Render](https://render.com/) | Cloud deployment |
| Python 3 | Runtime |
 
---
 
## Run Locally
 
**1. Clone the repository**
```bash
git clone https://github.com/ErkanSoftwareDeveloper/short-motivation-api.git
cd short-motivation-api
```
 
**2. Install dependencies**
```bash
pip install -r requirements.txt
```
 
**3. Start the server**
```bash
uvicorn app:app --reload
```
 
The API will be available at `http://127.0.0.1:8000`.
 
---
 
## Project Structure
 
```
short-motivation-api/
├── app.py            # FastAPI app & all endpoints
├── requirements.txt  # Python dependencies
└── README.md
```
 
---
 
## Deployment
 
This project is deployed on **Render** as a free web service. The live API is accessible at:
 
```
https://short-motivation-api.onrender.com/quote
```
 
⚠️ Note: Free tier on Render spins down after inactivity. The first request after idle may take ~30 seconds to respond ⚠️
 
---
 
## License
 
This project is licensed under the [MIT License](LICENSE).
 
