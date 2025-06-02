# Finance Manager - Django Edition

Finance Manager is a comprehensive personal finance application built with Django and MongoDB. It helps users track expenses, manage investments, and analyze financial data in a modern, intuitive interface.

## Key Features

- 💸 **Expense Tracking**: Record and categorize expenses
- 📈 **Investment Management**: Track stock investments with buy/sell prices
- 💰 **Profit/Loss Calculation**: Automatic calculation of investment performance
- 🗂️ **Database Explorer**: View and manage financial data
- 📊 **Investment Summaries**: Grouped performance reports by stock
- 🧹 **Data Management**: One-click clearing of expenses or investments

## Technology Stack

### Backend
- **Django 4.2**: Python web framework
- **Djongo**: MongoDB connector for Django
- **MongoDB**: NoSQL database for flexible data storage

### Frontend
- **HTML5/CSS3**: Responsive design with modern UI
- **JavaScript**: Interactive elements and form handling
- **CSS Gradients**: Modern aesthetic with dark theme

## Installation Guide

### Prerequisites
- Python 3.8+
- MongoDB installed locally
- Pip package manager

### Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/finance-manager-django.git
   cd finance-manager-django
   ```

2. Create and activate virtual environment:
   ```bash
   python -m venv venv
   # Linux/MacOS:
   source venv/bin/activate
   # Windows:
   venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Apply migrations:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. Start MongoDB service (make sure it's running)

6. Start development server:
   ```bash
   python manage.py runserver
   ```

7. Access the application at:
   ```
   http://localhost:8000
   ```

## Usage Guide

### Adding Expenses
1. Go to "Add Expense" section
2. Enter category, amount, and date
3. Click "Submit Expense"

### Adding Investments
1. Go to "Add Investment" section
2. Enter stock symbol, buy/sell prices, quantity, and tax paid
3. Click "Submit Investment"

### Viewing Reports
1. Go to "Investment Summary" section
2. Click "Load Summary" to see profit/loss breakdown
3. Use "Database Explorer" to view raw expense/investment data

## Project Structure

```
finance_manager/
├── finance_manager/          # Django project configuration
├── finance_app/              # Main application module
│   ├── migrations/           # Database migrations
│   ├── templates/            # HTML templates
│   ├── models.py             # Data models
│   ├── views.py              # Application logic
│   └── urls.py               # App-specific routes
├── static/                   # Static assets
│   └── finance_app/
│       ├── script.js         # Client-side JavaScript
│       └── style.css         # Custom styles
├── manage.py                 # Django management script
└── requirements.txt          # Python dependencies
```

## API Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/add_expense/` | POST | Add new expense |
| `/add_investment/` | POST | Add new investment |
| `/view_investment_summary/` | GET | Get investment summary |
| `/dump_expenses/` | GET | Get all expenses |
| `/dump_investments/` | GET | Get all investments |
| `/clear_expenses/` | POST | Clear all expenses |
| `/clear_investments/` | POST | Clear all investments |



## Future Enhancements

- [ ] User authentication system
- [ ] Data visualization charts
- [ ] Monthly budget planning
- [ ] CSV import/export functionality
- [ ] Email notifications and reports
- [ ] Mobile application integration

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Create a new Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For support or questions, please open an issue on our [GitHub repository](https://github.com/yourusername/finance-manager-django/issues).

---

**Developed with ❤️ using Django and MongoDB**  
[![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)](https://www.djangoproject.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
