# 🏦 Bank of India

A complete web-based online banking system for Bank of India built with HTML, CSS, JavaScript, PHP, and MySQL. Perfect for college projects!

## Features

### Customer Features
- 🔐 **User Authentication** - Secure login and registration
- 💳 **Account Management** - View balance and account details
- 💰 **Money Transfer** - Transfer funds between accounts
- 📤 **Deposit Funds** - Add money to your account
- 📥 **Withdrawal** - Withdraw money from account
- 📊 **Transaction History** - View all transactions with filters
- 🎨 **Dark Theme UI** - Modern, sleek dark-themed interface

### Admin Features
- 📊 **Dashboard** - System statistics and overview
- 👥 **User Management** - Create, view, and manage user accounts
- 💳 **Transaction Management** - View all system transactions
- ⚙️ **System Management** - Create users, system info
- 📈 **Analytics** - Transaction statistics and summaries

## Technology Stack

- **Frontend:** HTML5, CSS3, JavaScript
- **Backend:** PHP 7+
- **Database:** MySQL/MariaDB
- **Server:** Apache (XAMPP)
- **Theme:** Dark Mode

## System Requirements

- XAMPP (or similar with Apache, PHP, MySQL)
- PHP 7.0 or higher
- MySQL 5.6 or higher
- Modern Web Browser

## Installation & Setup

### Step 1: Download XAMPP
1. Download XAMPP from https://www.apachefriends.org/
2. Install XAMPP on your system
3. Start Apache and MySQL from XAMPP Control Panel

### Step 2: Place Project Files
1. Extract the project folder
2. Move the `banking_management` folder to:
   - **Windows:** `C:\xampp\htdocs\`
   - **Mac:** `/Applications/XAMPP/htdocs/`
   - **Linux:** `/opt/lampp/htdocs/`

### Step 3: Create Database
1. Open phpMyAdmin: http://localhost/phpmyadmin/
2. Create a new database named `banking_db`
3. Click on the `banking_db` database
4. Go to the "Import" tab
5. Select the file `database/banking_db.sql`
6. Click "Go" to import the database

### Step 4: Access the Application

**Customer Portal:**
- URL: `http://localhost/banking_management/`
- Login with demo account:
  - Account Number: `ACC001001`
  - Password: `john123`

**Admin Portal:**
- URL: `http://localhost/banking_management/admin_login.php`
- Login with demo admin:
  - Username: `admin`
  - Password: `admin123`

## Demo Accounts

### Customer Accounts
```
1. Account Number: ACC001001
   Password: john123
   Name: John Doe
   Balance: $5000
   Email: john@example.com

2. Account Number: ACC001002
   Password: jane123
   Name: Jane Smith
   Balance: $3500
   Email: jane@example.com

3. Account Number: ACC001003
   Password: mike123
   Name: Mike Johnson
   Balance: $10000
   Email: mike@example.com
```

### Admin Account
```
Username: admin
Password: admin123
```

## Project Structure

```
banking_management/
├── index.php                 # Customer login page
├── register.php             # User registration
├── dashboard.php            # Customer dashboard
├── transfer.php             # Money transfer page
├── deposit.php              # Deposit page
├── withdrawal.php           # Withdrawal page
├── transactions.php         # Transaction history
├── logout.php               # Logout handler
├── admin_login.php          # Admin login
├── admin_dashboard.php      # Admin dashboard
├── admin_users.php          # User management
├── admin_transactions.php   # Transaction management
├── admin_manage.php         # System management
├── admin_logout.php         # Admin logout
├── css/
│   └── style.css            # Dark theme CSS
├── js/
│   └── script.js            # JavaScript functions
├── database/
│   ├── config.php           # Database configuration
│   └── banking_db.sql       # Database schema & demo data
└── README.md                # This file
```

## Key Features Explanation

### 1. User Registration
- New users can create accounts with personal details
- Account numbers are auto-generated (ACC + 6 digits)
- Passwords are stored securely (MD5 hashing)
- Account types: Savings, Checking, Business

### 2. Login System
- Secure session-based authentication
- Different login for customers and admins
- Password validation
- Session timeout support

### 3. Dashboard
- Real-time balance display
- Account information
- Recent transaction history
- Quick action buttons

### 4. Money Transfer
- Transfer between accounts
- Validation of recipient account
- Insufficient balance checking
- Transaction logging
- Database transactions for consistency

### 5. Transactions
- View all transfers, deposits, withdrawals
- Transaction status (Success, Pending, Failed)
- Transaction history with pagination
- Search functionality
- Detailed transaction information

### 6. Admin Panel
- View all users and their accounts
- Change user account status
- Delete accounts
- Create new accounts manually
- View system statistics
- Manage transactions
- Transaction analytics

## Database Schema

### Users Table
- Stores customer account information
- Fields: full_name, email, phone, balance, account_type, status, etc.

### Transactions Table
- Records all transactions (transfers, deposits, withdrawals)
- Fields: from_account, to_account, amount, type, status, timestamp, etc.

### Admin Users Table
- Stores admin credentials and information
- Fields: username, password, full_name, email, role

## Security Features

✅ SQL Injection Prevention (Prepared statements)
✅ Password Hashing (MD5)
✅ Session Management
✅ Input Validation & Sanitization
✅ XSS Prevention (htmlspecialchars)
✅ Database Transactions for consistency
✅ Error Handling

## Dark Theme Colors

- **Primary:** #00d4ff (Cyan)
- **Secondary:** #ff006e (Pink)
- **Success:** #00d084 (Green)
- **Danger:** #ff4757 (Red)
- **Warning:** #ffa502 (Orange)
- **Background:** #1a1a2e (Dark)

## Troubleshooting

### Database Connection Error
- Check if MySQL is running in XAMPP
- Verify database name is `banking_db`
- Use credentials: root (username), empty password

### Pages Not Loading
- Check if Apache is running
- Verify project is in `htdocs` folder
- Clear browser cache
- Check URL: `http://localhost/banking_management/`

### Login Issues
- Make sure to use provided demo credentials
- Check if database is imported correctly
- Verify no session conflicts

## Future Enhancements

- 💳 Credit/Debit Card Integration
- 📱 Mobile App Version
- 🔔 Email Notifications
- 📊 Advanced Reports & Analytics
- 🔐 Two-Factor Authentication
- 💰 Loan Management
- 📈 Investment Portfolio
- 🌐 Multi-Currency Support

## License

This project is for educational purposes.

## Author

Created for College Projects
Version 1.0

## Support

For issues or questions:
1. Check database connection
2. Verify file permissions
3. Review error logs
4. Check browser console for JavaScript errors

---

**Enjoy using Bank of India!** 🎉

Happy Learning! 📚
