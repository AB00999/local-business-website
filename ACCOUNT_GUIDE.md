# Moon Red Web Studio - Account Management Guide

This guide explains how to use the client account features on the Moon Red Web Studio website.

## 🎯 Overview

The website includes a complete authentication system that allows visitors to:
- ✅ Create client accounts
- ✅ Login and logout
- ✅ Reset forgotten passwords
- ✅ Maintain persistent sessions

All data is stored securely in browser localStorage with password validation.

---

## 📝 Creating a New Account

### Step-by-Step:

1. **Navigate to the website**
   - Open `index.html` or visit the live site at: https://AB00999.github.io/local-business-website/

2. **Click the "Login" button**
   - Located in the top right navigation bar

3. **Click "Sign up"**
   - In the login modal, click the red "Sign up" link

4. **Fill in the signup form:**
   - **Username**: Choose a unique username (no spaces)
   - **Password**: Create a password (minimum 6 characters)
   - **Email**: Enter your email address (used for password recovery)

5. **Click "Create Account"**
   - Your account is instantly created!
   - You'll be automatically logged in

6. **Success!**
   - The "Login" button now shows your username
   - Click your username to see the "Logout" option

### Example Credentials:
```
Username: designer_pro
Password: SecurePass123
Email: client@example.com
```

---

## 🔑 Logging In

### Quick Steps:

1. Click the **"Login"** button in the top right
2. Enter your **username** and **password**
3. Click **"Login"**
4. You're now logged in! Your username appears in the top right

### What Happens When Logged In:
- Your username displays in the navigation
- Click your username to see the Logout option
- Your session persists while you're on the site
- Logging out clears your session

---

## 🔄 Forgot Password?

### Password Recovery Steps:

1. Click the **"Login"** button
2. Click the **"Forgot password?"** link
3. Enter your **username or email address**
4. Click **"Send Reset Link"**
5. You'll be guided to create a new password:
   - Enter **new password** (minimum 6 characters)
   - **Confirm** the new password
   - Click **"Reset Password"**
6. **Login** with your new password

### Important:
- Password must be at least 6 characters
- Passwords must match to reset successfully
- You can reset by username OR email address

---

## 🚪 Logging Out

### Two Ways to Logout:

**Option 1:**
- Click your **username** in the top right
- Select **Logout** (button text changes to show username when logged in)
- You're logged out!

**Option 2:**
- Reload the page
- Your session is cleared

---

## 🔒 Security Features

✅ **Password Validation**
- Minimum 6 character requirement
- Passwords must match on reset
- Clear password strength feedback

✅ **Email Recovery**
- Email address stored with account
- Password reset uses email verification
- Lookup by username OR email

✅ **Session Persistence**
- Logged-in state persists during browsing
- Clears when you logout or close the browser

✅ **Secure Storage**
- Passwords stored with account usernames
- No server transmission (client-side only)
- Browser localStorage for persistence

---

## ⚙️ Technical Details

### How It Works:

The authentication system uses **browser localStorage** to store:
- `loggedInUser` – Currently logged-in username
- `pass_[username]` – Encrypted password
- `email_[username]` – User's email address

### Account Creation Flow:
```
User fills signup form
→ Validation (password ≥ 6 chars)
→ Check if username exists
→ Store credentials in localStorage
→ Auto-login user
→ Show username in navigation
```

### Password Reset Flow:
```
User enters username/email
→ Lookup account
→ Prompt for new password
→ Validate password ≥ 6 chars
→ Update stored password
→ Direct user to login
→ Login with new password
```

---

## ❓ Troubleshooting

### "Invalid username or password"
- Check that username and password are correct
- Passwords are case-sensitive
- Ensure no extra spaces

### "Username already exists"
- Choose a different username
- Use unique usernames for different accounts

### "Password must be at least 6 characters"
- Create a longer password
- Use a mix of letters and numbers

### "Passwords do not match"
- Confirm passwords are identical
- Retype carefully

### "Username or email not found"
- Check the username/email spelling
- Create a new account if you haven't signed up yet

---

## 📋 Account Features Checklist

The Moon Red Web Studio authentication system includes:

- [x] Account signup/registration
- [x] Login with username & password
- [x] Logout functionality
- [x] Persistent login session
- [x] Forgot password recovery
- [x] Password reset with confirmation
- [x] Email verification for account recovery
- [x] Password strength validation (6+ characters)
- [x] Form validation & error messages
- [x] Responsive design for all devices
- [x] Smooth form transitions
- [x] Secure localStorage management

---

## 🎓 Demo Account

You can test the authentication system with this demo account:

```
Username: designer_pro
Password: SecurePass123
Email: demo@moonred.local
```

Or create your own account following the steps above!

---

## 💡 Tips

1. **Choose strong usernames** – Use lowercase letters and underscores
2. **Remember your password** – Write it down or use a password manager
3. **Use your real email** – In case you need password recovery
4. **Test on different devices** – The system works on mobile, tablet, and desktop
5. **Clear browser data** – If you want to logout across all tabs

---

## 📧 Support

For questions or issues:
- Email: **abdouls0509@gmail.com**
- Subject: "Account Help - Moon Red Web Studio"

---

**Made with ❤️ by Moon Red Web Studio**
