# Formspree Setup Guide

## 🚀 **Quick Setup (5 minutes)**

### **Step 1: Create Formspree Account**
1. Go to [formspree.io](https://formspree.io)
2. Click "Get Started" or "Sign Up"
3. Create account with your email

### **Step 2: Create New Form**
1. Click "New Form"
2. Give it a name: "Newsletter Signup"
3. Copy the form ID (looks like: `xpzgkqwe`)

### **Step 3: Update Your HTML**
1. Edit `index.html` in your repository
2. Find this line:
   ```html
   <form id="newsletterForm" action="#" method="POST">
   ```
3. Replace it with:
   ```html
   <form id="newsletterForm" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
4. Replace `YOUR_FORM_ID` with your actual form ID

### **Step 4: Commit Changes**
```bash
git add index.html
git commit -m "Add Formspree email collection"
git push origin main
```

## 📧 **How It Works**

- **Form submissions** go to Formspree
- **You get notified** by email for each signup
- **Spam protection** built-in
- **Free tier**: 50 submissions/month
- **Data export** available

## 🎯 **What You'll Get**

- **Email notifications** for each signup
- **Subscriber list** in Formspree dashboard
- **CSV export** of all subscribers
- **Spam filtering** automatic
- **Analytics** on form submissions

## 🔄 **Testing After Setup**

1. Visit your page: https://vivekbala.github.io/all-time-high-trader/
2. Enter a real email address
3. Submit the form
4. Check your email for Formspree notification
5. Check Formspree dashboard for the submission

## 💰 **Cost**

- **Free**: 50 submissions/month
- **Paid**: $10/month for 1,000 submissions
- **Perfect for starting out!**

## 🚀 **Ready to Set Up?**

Just follow the steps above and your newsletter signup will start collecting real emails from your YouTube viewers!
