Here are clear, practical <meta name="robots"> guidelines for 5 key files in your system—focused on security and proper indexing.

🔐 1. login.php (Login Page)
<meta name="robots" content="noindex, nofollow">

Why:

Prevents the page from appearing on search engines
Avoids exposing login endpoints publicly
🔐 2. register.php (Signup Page)
<meta name="robots" content="noindex, nofollow">

Why:

Registration pages don’t need indexing
Helps reduce spam bot discovery
🔐 3. reset_password.php (Password Reset Page)
<meta name="robots" content="noindex, nofollow, noarchive">

Why:

Highly sensitive page
noarchive prevents cached copies from being stored
🔐 4. dashboard.php (User Dashboard)
<meta name="robots" content="noindex, nofollow, noimageindex">

Why:

Private user data must never appear in search results
noimageindex prevents images from being indexed
🌐 5. index.php (Homepage / Public Page)
<meta name="robots" content="index, follow">

Why:

This is your main public page
You WANT it visible on search engines
🧠 Quick Meaning of Values
index → allow page in search results
noindex → hide page from search results
follow → allow crawling links
nofollow → don’t follow links
noarchive → don’t save cached version
noimageindex → don’t index images
✅ Final Best Practice

Place the tag inside <head>:

<head>
    <meta name="robots" content="noindex, nofollow">
</head>
🔥 Pro Tip

Even with these tags, still:

Use authentication (sessions)
Protect pages on the server side

👉 Because search engine blocking ≠ real security
