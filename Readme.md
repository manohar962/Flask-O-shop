# Flask-O-shop
An E-Commerce app built with Python Flask

**Features:**
- Cart, orders, and items feature with a proper order processing system
- Proper user authentication and authorization
- Stripe Payment Integration
- Custom admin panel for order processing and managing items
- Item Search feature
- Bootstrap + custom CSS UI

---

## Prerequisites
- [Python 3.x](https://www.python.org/)
- Stripe API key for Stripe Payment Integration
- [Stripe webhook setup](https://stripe.com/docs/payments/handling-payment-events#install-cli)

---

## How to Run Locally

### 1. Clone the repository
```bash
git clone [https://github.com/manohar962/Flask-O-shop.git](https://github.com/manohar962/Flask-O-shop.git)
cd Flask-O-shop
```

### 2. Set up the Environment
This project uses Pipenv to manage dependencies. Run the following commands to install everything cleanly:
```bash
pip install pipenv
pipenv install
```

### 3. Configure Environment Variables
Create a `.env` file in the root directory and add your secret keys and Stripe credentials:
```text
FLASK_SECRET_KEY=your_secret_key_here
STRIPE_PUBLIC_KEY=your_stripe_public_key
STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
```

### 4. Initialize the Database
*(Note: Adjust this command based on your project's setup, such as using `flask db upgrade` or a custom initialization script).*
```bash
pipenv run python setup_db.py 
```

### 5. Launch the Application
Activate the virtual environment and start the Flask development server:
```bash
pipenv shell
python app.py
```
Once started, open your browser and navigate to http://127.0.0.1:5000/ to view the shop!