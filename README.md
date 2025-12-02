# Prompt Engineering Home Assignment

This project contains my (Roi Argaman) solutions to two prompt-engineering tasks:


1. **Classifying customer messages** into
   `support_request`, `sales_inquiry`, `complaint`, `compliment`.
2. **Analyzing a customer conversation** (TV company) and returning a short JSON summary.

Everything is implemented inside the notebook **`prompt_engineer_HA.ipynb`**.

---

## Files

* `prompt_engineer_HA.ipynb` — main notebook
* `prompt_engineer_HA.html` — exported HTML for easy viewing
* `requirements.txt` — Python dependencies
* `.env` — **contains API key (for review only!)**
* `venv/` — pre-built virtual environment (Windows Git Bash)

> ⚠️ **Important:**
> The `.env` and `venv/` folders are included only so the reviewer can run the notebook quickly.
> Please do **not** reuse any API key outside this assignment.

---

## How to Run (Git Bash Only)

### 1. Go to the project folder

```bash
cd "~/OneDrive/OneDrive Documents/GitHub/prompt_engineer_home_assignment"
```

### 2. Activate the provided venv

```bash
source venv/Scripts/activate
```

You should now see:

```
(venv)
```

### 3. Install dependencies (just to be safe)

```bash
pip install -r requirements.txt
```

### 4. Verify your `.env` has a valid API key

Open `.env` and make sure it looks like:

```
OPENAI_API_KEY=your_key_here
```

(Replace the value if needed.)

### 5. Run Jupyter Notebook

```bash
jupyter notebook
```

Then open **`prompt_engineer_HA.ipynb`** and run all cells.

---

## Re-export HTML (optional)

```bash
jupyter nbconvert --to html prompt_engineer_HA.ipynb
```

---

## Notes

* If anything breaks, the easiest fix is to **delete the venv and create a new one**:

  ```bash
  rm -rf venv
  python -m venv venv
  source venv/Scripts/activate
  pip install -r requirements.txt
  ```

* Never commit real API keys in real projects.
  They're included here only for ease of review.