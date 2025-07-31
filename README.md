
---

````markdown
# 🏡 California Housing Price Prediction

A machine learning web app that predicts house prices based on California housing data.  
Built with Flask, Dockerized, and deployed to the cloud using **Render** with a **CI/CD pipeline powered by GitHub Actions**.

---

## 🚀 Live Demo

👉 [Try the App](https://californiahousing-2.onrender.com)

---

## 📸 Screenshot

![App Screenshot](screenshot.png) <!-- Replace with your actual screenshot file -->

---

## 🛠️ Tech Stack

- **Frontend**: HTML/CSS (Flask Templates)
- **Backend**: Python, Flask
- **Machine Learning**: scikit-learn
- **Containerization**: Docker
- **CI/CD**: GitHub Actions
- **Deployment**: Render

---

## 📦 Features

- Predicts house prices from given features
- Uses trained regression model on California Housing dataset
- Responsive UI
- Dockerized for consistent deployment
- Auto-deployment with GitHub Actions

---

## 🐳 Docker Usage

To run locally with Docker:

```bash
# Build image
docker build -t california-housing .

# Run container
docker run -p 5000:5000 california-housing
````

---

## 🔁 CI/CD Pipeline

* On every `push` to GitHub:

  * Docker image is built
  * Render is triggered via API to redeploy the app
* Managed via GitHub Actions (`.github/workflows/deploy.yaml`)

---

## 📁 Project Structure

```
.
├── app.py
├── Dockerfile
├── requirements.txt
├── .github/
│   └── workflows/
│       └── deploy.yaml
├── templates/
│   └── index.html
├── static/
│   └── style.css
└── model.pkl
```

---

## 💻 Local Development (without Docker)

```bash
# Install dependencies
pip install -r requirements.txt

# Run the app
python app.py
```

Then go to `http://localhost:5000`.

---

## 🔐 Secrets & Deployment

Add the following secrets in your GitHub repository under **Settings > Secrets**:

* `RENDER_API_KEY`: Your Render API key
* `RENDER_SERVICE_ID`: Your Render service ID

These are used by the GitHub Actions pipeline to trigger deployment.

---

## 📊 ML Model

* Dataset: California Housing Dataset (from `sklearn.datasets`)
* Model: Linear Regression
* Preprocessing: Feature scaling (optional)

---

## 📃 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙌 Acknowledgments

* [scikit-learn](https://scikit-learn.org/)
* [Flask](https://flask.palletsprojects.com/)
* [Render](https://render.com/)
* [GitHub Actions](https://github.com/features/actions)

```

---