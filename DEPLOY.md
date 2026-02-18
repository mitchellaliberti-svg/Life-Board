# My Life Dashboard — Vercel Deployment Guide

## What's in this folder
A React web app with Budget, Journal, and Daily (AI news/trivia) tabs.
Designed to be added to your iPhone home screen as a PWA.

---

## Step 1 — Upload to GitHub

1. Go to **github.com** and sign in (or create a free account)
2. Click the **+** icon → **New repository**
3. Name it `my-life-dashboard`, keep it Public, click **Create repository**
4. On the next page, click **uploading an existing file**
5. Drag the entire contents of this folder into the upload area
   *(make sure to include the `src/` and `public/` folders)*
6. Click **Commit changes**

---

## Step 2 — Deploy on Vercel

1. Go to **vercel.com** and sign in with your GitHub account
2. Click **Add New → Project**
3. Find and select your `my-life-dashboard` repo
4. Under **Framework Preset**, select **Create React App**
5. Click **Deploy**
6. Wait ~60 seconds — you'll get a live URL like `my-life-dashboard.vercel.app`

> If you see a 404, go to Vercel → your project → Settings → General
> and confirm Output Directory is set to `build`

---

## Step 3 — Add to iPhone Home Screen

1. Open the Vercel URL in **Safari** on your iPhone
2. Tap the **Share** button (box with arrow at the bottom)
3. Scroll down and tap **Add to Home Screen**
4. Name it **My Life** → tap **Add**

It will appear on your home screen and open fullscreen like a native app! ✓

---

## Step 4 — Set up the Daily tab

The Daily tab needs an Anthropic API key to generate news/trivia.

1. Go to **console.anthropic.com** on your computer
2. Sign up for a free account
3. Go to **API Keys** → **Create Key**
4. Copy the key (starts with `sk-ant-`)
5. Open your app, go to the **Daily** tab, and paste the key

The key is stored only on your device. New users get free credits to start.

---

## Your data
All budget and journal data is saved in your browser's localStorage.
It persists between sessions on the same device/browser.
