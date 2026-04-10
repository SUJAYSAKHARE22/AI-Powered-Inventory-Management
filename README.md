# ARIA — AI Inventory Management System

An intelligent, AI-powered inventory management system using Flask + Groq (Llama 3.1).

## Features
- 🤖 **AI Chat Interface** — natural language inventory management via ARIA
- 📦 **Full CRUD** — add, edit, delete products through UI or chat
- 📊 **Real-time Stats** — live dashboard with value, stock alerts
- 🔄 **Stock Management** — add/remove/set stock with transaction history
- 🔍 **Search & Filter** — by name, SKU, supplier, category
- 💾 **SQLite Database** — no external DB needed
- ✨ **Glass UI** — dark theme with glassmorphism design

## Setup

### 1. Install dependencies
```bash
pip install -r requirements.txt
```

### 2. Get a Groq API Key
- Go to https://console.groq.com
- Create a free account and generate an API key

### 3. Run the app
```bash
python app.py
```
Or with your API key as environment variable:
```bash
GROQ_API_KEY=gsk_your_key python app.py
```

### 4. Open in browser
```
http://localhost:5000
```

### 5. Enter API Key in Settings
- Click **Settings** in the sidebar
- Paste your Groq API key
- Click **Save API Key**

## Usage

### AI Chat Examples
- "Add a new product: iPhone 15, SKU ELEC-020, quantity 50, price $999"
- "How many units of Wireless Keyboard do we have?"
- "Remove 10 units from Monitor 27 inch"
- "Show me all low stock items"
- "What's our total inventory value by category?"
- "Delete the Ballpoint Pens product"
- "Set USB-C Hub quantity to 25"

### Manual Management
- Use the **Products** panel to view, edit, delete items
- Use the **Add Product** panel to create new items manually
- Use the **Transactions** panel to view stock history

## Project Structure
```
inventory_ai/
├── app.py              # Flask backend + API routes
├── requirements.txt
├── templates/
│   └── index.html      # Main UI template
├── static/
│   ├── css/style.css   # Glass UI styles
│   └── js/app.js       # Frontend logic
└── instance/
    └── inventory.db    # SQLite database (auto-created)
```
