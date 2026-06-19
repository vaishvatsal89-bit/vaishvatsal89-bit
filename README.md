<h1 align="center">Vatsal Tripathi</h1>
<p align="center">
  <strong>B.Tech CSE · Galgotias University</strong><br/>
  Building production-ready full stack applications · Obsessed with clean architecture
</p>
<p align="center">
  <a href="https://linkedin.com/in/vatsal-tripathi-280a55316">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white"/>
  </a>
  <a href="mailto:vaishvatsal89@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-EA4335?style=flat-square&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://instagram.com/vatsal_tripathi77">
    <img src="https://img.shields.io/badge/Instagram-E4405F?style=flat-square&logo=instagram&logoColor=white"/>
  </a>
  <img src="https://komarev.com/ghpvc/?username=vaishvatsal89-bit&style=flat-square&color=6366f1"/>
</p>

What I'm building

Most student projects stop at CRUD with localStorage. I build things that actually run in production — with real payments, real users, and real security constraints to solve.

Right now that means TaskCampus — a peer-to-peer task marketplace for college students. Think Fiverr, but for your hostel block. Post a task, a verified student accepts it, they complete it, you pay via Razorpay — all secured with OTP verification so payment only releases on confirmed completion.


🚀 Featured Project — TaskCampus


"Deliver my notes to Block C Room 214. ₹80."



A live, production-deployed campus marketplace with features most developers treat as "phase 2":

Payment & Financial


🔐 Razorpay live integration with server-side signature verification — the payment amount is verified against Razorpay's API before the task goes live, preventing any client-side manipulation
💰 In-app wallet system — earnings credited on OTP verification, withdrawal requests tracked in DB
🔄 Automatic refund flow when posters cancel unpaid tasks (Razorpay Refund API)


Database Architecture


⚡ Race-condition safe task acceptance using PostgreSQL stored procedures — two students can't accept the same task simultaneously
🕐 Automated task expiry via pg_cron — runs every 5 minutes, marks overdue accepted tasks as expired, sends warnings automatically
🛡️ Row Level Security on every table — users can only access data they're authorized to see
📊 HMAC-SHA256 payment signature verification inside a Supabase Edge Function (TypeScript/Deno)


Real-time & Notifications


🔔 Supabase Realtime subscriptions — new tasks appear on every connected screen instantly without refresh
🔔 Browser push notifications when a new task is posted (Web Notifications API)
💬 In-app chat between poster and doer — real-time via Postgres changes subscription


Security


✅ University email domain enforcement (fake emails verified via Supabase email confirmation)
⚠️ Warning system — doers who miss deadlines or cancel get warnings; 3 strikes = 7-day ban
🔒 OTP brute force protection — attempt counter stored in DB, locked after 10 wrong tries


Stack: React + Vite · Supabase (PostgreSQL, Auth, Realtime, Edge Functions) · TypeScript/Deno · Razorpay · Vercel

🔗 Live: task-campus-three.vercel.app


💻 Tech I actually use

Frontend       React, Vite, JavaScript (ES2022+), CSS3
Backend        Supabase Edge Functions (TypeScript, Deno)
Database       PostgreSQL — RLS, triggers, stored procedures, pg_cron
Auth           Supabase Auth — email confirmation, JWT, session management
Payments       Razorpay — Orders API, Refunds API, signature verification
Realtime       Supabase Realtime — postgres_changes subscriptions
DevOps         Vercel, Git, GitHub
Also know      Node.js, Express, MongoDB, C++


📊 GitHub Stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=vaishvatsal89-bit&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=vaishvatsal89-bit&layout=compact&theme=tokyonight&hide_border=true"/>
</p>
<p align="center">
  <img src="https://streak-stats.demolab.com?user=vaishvatsal89-bit&theme=tokyonight&hide_border=true"/>
</p>

📈 Contribution Activity

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=vaishvatsal89-bit&theme=tokyo-night&hide_border=true"/>
</p>

🏆 Trophies

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=vaishvatsal89-bit&theme=tokyonight&margin-w=8&no-frame=true"/>
</p>

Currently


🎓 B.Tech Computer Science — Galgotias University
🏗️ Scaling TaskCampus to multiple university campuses
📖 Going deep on system design, distributed systems, and backend architecture
🎯 Goal: build things that real people use, at scale
