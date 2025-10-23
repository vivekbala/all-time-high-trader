# EmailJS Setup Guide

## 🔑 **Step 1: Get Your EmailJS Credentials**

### **Find Your Public Key**
1. Go to [emailjs.com](https://emailjs.com) and log in
2. Go to **"Account"** → **"API Keys"**
3. **Copy your Public Key** (looks like: `user_xxxxxxxxxxxxxxxx`)

### **Create Email Service**
1. Go to **"Email Services"** → **"Add New Service"**
2. Choose your email provider:
   - **Gmail**: Select Gmail
   - **Outlook**: Select Outlook
   - **Other**: Select your provider
3. **Follow the setup instructions** for your email provider
4. **Copy your Service ID** (looks like: `service_xxxxxxxx`)

### **Create Email Template**
1. Go to **"Email Templates"** → **"Create New Template"**
2. **Template name**: "Newsletter Signup"
3. **Subject**: "New Newsletter Subscriber"
4. **Content**:
   ```
   New newsletter subscriber: {{from_email}}
   
   Email: {{from_email}}
   Message: {{message}}
   ```
5. **Copy your Template ID** (looks like: `template_xxxxxxxx`)

## 🔧 **Step 2: Update Your Newsletter Page**

### **Edit the Configuration**
1. Open `index.html` in your repository
2. Find these lines:
   ```javascript
   const EMAILJS_PUBLIC_KEY = 'YOUR_PUBLIC_KEY_HERE';
   const EMAILJS_SERVICE_ID = 'YOUR_SERVICE_ID_HERE';
   const EMAILJS_TEMPLATE_ID = 'YOUR_TEMPLATE_ID_HERE';
   ```
3. Replace with your actual values:
   ```javascript
   const EMAILJS_PUBLIC_KEY = 'user_xxxxxxxxxxxxxxxx';
   const EMAILJS_SERVICE_ID = 'service_xxxxxxxx';
   const EMAILJS_TEMPLATE_ID = 'template_xxxxxxxx';
   ```

### **Update Your Email Address**
1. Find this line:
   ```javascript
   to_email: 'YOUR_EMAIL@example.com', // Replace with your email
   ```
2. Replace with your actual email:
   ```javascript
   to_email: 'your-email@gmail.com', // Your actual email
   ```

## 🚀 **Step 3: Deploy Your Changes**

### **Commit and Push**
```bash
git add index.html
git commit -m "Add EmailJS integration"
git push origin main
```

## 🧪 **Step 4: Test Your Integration**

### **Test the Form**
1. Go to: https://vivekbala.github.io/all-time-high-trader/
2. Enter a test email
3. Click "Subscribe Now"
4. Check your email for the notification

### **What You Should See**
- **Success message**: "Thank you for subscribing! Check your email for confirmation."
- **Email notification**: New email in your inbox with subscriber details

## ✅ **What You'll Get**

- **Real email collection** - Subscribers send emails to you
- **Professional notifications** - Get notified of each signup
- **Free forever** - 200 emails/month free
- **Easy management** - All subscribers in your email

## 🎯 **Email Template Example**

Your email template should look like:
```
Subject: New Newsletter Subscriber

New newsletter subscriber: test@example.com

Email: test@example.com
Message: New newsletter subscriber: test@example.com
```

## 🔧 **Troubleshooting**

### **If emails don't arrive:**
- Check your spam folder
- Verify your email service is set up correctly
- Check browser console for errors

### **If you get errors:**
- Make sure all 3 IDs are correct
- Verify your email service is active
- Check that the template exists

### **If the form doesn't work:**
- Check that EmailJS script loaded
- Verify your public key is correct
- Make sure the service is active

## 🚀 **Ready to Go!**

Once configured, your newsletter signup will:
- ✅ **Send real emails** to your inbox
- ✅ **Handle unlimited signups** (200/month free)
- ✅ **Professional notifications** for each subscriber
- ✅ **Easy to manage** - all in your email

Your newsletter can now collect real emails from your YouTube viewers!
