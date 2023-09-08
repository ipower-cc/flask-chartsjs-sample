# [Flask Charts via Flask-RestX](https://blog.appseed.us/flask-charts-js-and-flask-restx-s92/)

Sample project crafted with `Flask`, `Charts.JS`, and `Flask-RestX` to showcase how to plot different charts **Pie, Line and Bar Charts**. Frontend uses `Bootstrap5` for styling and `Chart.js` for dynamic charts. The dataset is loaded via a custom **Flask CLI** and the project homepage showcases three charts type: `line`, `bar` and `pie`. 

- 👉 [Charts via Flask-RestX](https://flask-charts-via-restx.appseed-srv1.com/) - LIVE Demo
- 👉 Free [support](https://appseed.us/support) via `email` and [Discord](https://discord.gg/fZC6hup).

<br />

> Features:

- ✅ `Up-to-date dependencies`
- ✅ `Stack`: Flask
- ✅ `API`: Flask-RestX
- ✅ `DB Tools`: Flask-SqlAlchemy, SQLite
- ✅ `Charts`: Charts.js

<br />

![Flask Charts via Flask-RestX and Charts.js - provided by AppSeed.us](https://user-images.githubusercontent.com/51070104/164218594-2a0a6a4d-618f-4fb8-90ee-7d4d41088466.jpg)

## ✨ How to use it

> 👉 **Clone Sources** (this repo)

```bash
$ git clone https://github.com/app-generator/blog-sample-flask-charts.git
$ cd blog-sample-flask-charts
```

<br />

> 👉 **Install Modules** using a Virtual Environment

```bash
$ virtualenv env
$ source env/bin/activate
$ pip3 install -r requirements.txt
```

Or for **Windows-based Systems**

```bash
$ virtualenv env
$ .\env\Scripts\activate
$
$ # Install modules - SQLite Database
$ pip3 install -r requirements.txt
```

<br />

> 👉 **Set up the environment**

```bash
$ export FLASK_APP=app.py
$ export FLASK_ENV=development
```

Or for **Windows-based Systems**

```bash
$ # CMD terminal
$ set FLASK_APP=app.py
$ set FLASK_ENV=development
$
$ # Powershell
$ $env:FLASK_APP = ".\app.py"
$ $env:FLASK_ENV = "development"
```

<br />

> 👉 **Load Sample Data** from `data` directory

- `monthly_customers.csv`
- `monthly_sales.csv`
- `product_sales.csv`

```bash
$ flask load-data 
```

<br />

> 👉 **Start the APP**

```bash
$ flask run 
```

<br />

## ✨ Code-base structure

```bash
< PROJECT ROOT >
   |
   |-- app.py            # Create and start the APP object
   |-- api.py            # Simple API node 
   |-- models.py         # app models
   |
   |-- data_loader.py    # Save the data in DB
   |
   |-- templates
   |    |-- index.html   # Simple page styled with BS5 
   |
   |-- static
   |    |-- js/custom.js # Code the Charts
   |
   |-- *******************
```

<br />

> The bootstrap flow

- `app.py` 
  - bundles all resources
  - serve the `index.html`
- `api.py` exposes a simple API using the DB data 
- `templates/index.html`
  - HOMEpage of the project
- `js/custom.js`
  - fetch data exposed by the `API`

<br />

---
[Flask Charts via Flask-RestX](https://blog.appseed.us/flask-charts-js-and-flask-restx-s92/) - provided by [AppSeed](https://appseed.us)
