# 🛒 Multi-Vendor Marketplace

A production-ready multi-vendor marketplace where buyers can browse and purchase products from multiple sellers, vendors can manage their own stores with real-time analytics, and admins have full platform oversight with commission tracking and content moderation.

---

## 🚀 Features

### 👤 Buyer
- Browse and search products across multiple vendors
- Add to cart and checkout securely with **Stripe**
- Order history and tracking

### 🏪 Vendor
- Create and manage your own store
- Add, edit, and remove product listings
- Real-time sales analytics dashboard
- Track orders and revenue

### 🛡️ Admin
- Full platform oversight and user management
- Commission tracking across all vendors
- Content moderation — approve/reject listings
- Revenue and activity reporting

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python · Django |
| Database | PostgreSQL |
| Payments | Stripe |
| Auth | Django Auth (multi-role) |
| API | REST APIs |
| Frontend | HTML · CSS · JavaScript |

---

## ⚙️ Installation & Setup

```bash
# 1. Clone the repository
git clone https://github.com/andriafraderick/multi-vendor-marketplace.git
cd multi-vendor-marketplace

# 2. Create and activate virtual environment
python -m venv venv
source venv/bin/activate        # macOS/Linux
venv\Scripts\activate           # Windows

# 3. Install dependencies
pip install -r requirements.txt

# 4. Set up environment variables
cp .env.example .env
# Edit .env and add your keys:
# SECRET_KEY, DATABASE_URL, STRIPE_PUBLIC_KEY, STRIPE_SECRET_KEY

# 5. Run migrations
python manage.py migrate

# 6. Create superuser (admin)
python manage.py createsuperuser

# 7. Run the development server
python manage.py runserver
```

---

## 🔑 Environment Variables

Create a `.env` file in the root directory:

```env
SECRET_KEY=your_django_secret_key
DEBUG=True
DATABASE_URL=postgresql://user:password@localhost:5432/marketplace_db
STRIPE_PUBLIC_KEY=pk_test_...
STRIPE_SECRET_KEY=sk_test_...
```

---

## 📁 Project Structure

```
multi-vendor-marketplace/
├── marketplace/          # Core app — products, orders, cart
├── vendors/              # Vendor store management & analytics
├── accounts/             # User auth — buyer, vendor, admin roles
├── payments/             # Stripe integration
├── templates/            # HTML templates
├── static/               # CSS, JS, images
├── manage.py
└── requirements.txt
```

---

## 📸 User Roles Overview

```
Admin  ──▶  Platform oversight, commission tracking, moderation
Vendor ──▶  Store management, product listings, analytics
Buyer  ──▶  Browse, cart, Stripe checkout, order tracking
```

---

## 👩‍💻 Author

**Andria Fraderick**
- 🌐 Portfolio: [andriafraderick.github.io](https://andriafraderick.github.io)
- 💼 LinkedIn: [linkedin.com/in/andriafraderick](https://linkedin.com/in/andriafraderick)
- 📧 andriafraderick02@gmail.com
