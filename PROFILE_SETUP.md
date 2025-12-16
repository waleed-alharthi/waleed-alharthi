# Gamer-Themed GitHub Profile - Setup Guide

## 🎮 Overview

This profile page features a pixelated gamer theme with auto-refreshing stats and graphics that showcase your coding prowess without exposing repository names or contents.

## ✨ Features Included

### 1. **Pixelated ASCII Art Header**
- Custom "WALEED" ASCII art with "Dev @ Rihal" subtitle
- Animated typing effect showing role and motto

### 2. **Auto-Refreshing Player Stats**
- **GitHub Stats Card**: Shows public contributions, stars, commits, PRs, issues
- **Streak Stats**: Current streak, longest streak, total contributions
- All stats auto-refresh when the page loads

### 3. **Tech Arsenal**
- Dynamic language statistics from actual repositories
- Shows top programming languages used across contributed repos
- Auto-updates based on GitHub activity

### 4. **Achievements (Trophies)**
- Auto-generated achievement badges based on GitHub activity
- Categories: Stars, Commits, PRs, Issues, Followers, etc.

### 5. **Boss Battle Analytics**
- Contribution activity graph with gaming theme
- Visual representation of coding activity over time

### 6. **Contribution Snake Animation**
- Animated snake that "eats" your contributions
- Auto-generates every 12 hours via GitHub Actions
- Supports both light and dark themes

### 7. **Daily Grind (WakaTime Integration)**
- Optional: Shows detailed coding time stats
- Requires WakaTime API key to be set up
- Updates daily automatically

### 8. **Profile View Counter**
- Tracks total profile views
- Gaming-themed badge style

### 9. **Social Links**
- GitHub and LinkedIn badges
- Gaming "GAME STATUS: ONLINE" indicator

### 10. **Animated Footer**
- Waving animation with "GG WP" (Good Game, Well Played)
- Custom gaming quote

## 🚀 What's Auto-Refreshing?

All the following components refresh automatically:

1. **GitHub Stats** - Updates on every page load
2. **Language Stats** - Updates on every page load
3. **Streak Stats** - Updates daily
4. **Trophies** - Updates when achievements change
5. **Activity Graph** - Updates on every page load
6. **Contribution Snake** - Regenerates every 12 hours (via GitHub Actions)
7. **WakaTime Stats** - Updates daily (if API key is configured)
8. **Profile Views** - Updates on every page load

## 🔧 Setup Instructions

### GitHub Actions Workflows

Two workflows have been created:

#### 1. Snake Animation (`snake.yml`)
- **Trigger**: Every 12 hours, on push to main, or manually
- **Action**: Generates the contribution snake animation
- **No setup required**: Uses default GitHub token

#### 2. WakaTime Stats (`waka-readme.yml`)
- **Trigger**: Daily at midnight UTC, or manually
- **Action**: Updates coding time stats in README
- **Setup required**: Add `WAKATIME_API_KEY` to repository secrets

### Optional: WakaTime Setup

If you want to display detailed coding time stats:

1. Sign up at [WakaTime](https://wakatime.com)
2. Install WakaTime plugin in your IDE/editor
3. Get your API key from WakaTime dashboard
4. Add it to GitHub repository secrets:
   - Go to: Settings → Secrets and variables → Actions
   - Click "New repository secret"
   - Name: `WAKATIME_API_KEY`
   - Value: Your WakaTime API key

### Note About Snake Animation

The snake animation will work once the workflow runs. To trigger it immediately:

**Prerequisites**: 
- Ensure GitHub Actions are enabled for your repository (Settings → Actions → General → Allow all actions)

**To run manually**:
1. Go to Actions tab in your repository
2. Select "Generate Snake Animation" workflow
3. Click "Run workflow"

The animation will be available after the first successful run.

## 🎨 Color Scheme

The profile uses a cyberpunk/matrix-inspired color scheme:
- **Primary**: Matrix Green (#00FF41)
- **Background**: Dark Gray (#0D1117)
- **Theme**: Radical (pink/purple accents)

## 📊 Privacy Features

✅ **What's Shown**:
- Total public contributions
- Programming languages used (percentages)
- Contribution counts
- GitHub profile stats (public data)
- Coding time (from WakaTime, if enabled)

❌ **What's NOT Shown**:
- Repository names
- Repository contents
- Private repository information
- Commit messages
- Code snippets
- File names

## 🎯 Customization

You can customize:
- Languages to hide in Tech Arsenal stats (line 47, currently hiding html,css)
- Social links (lines 111-112)
- Gaming quote (line 105)
- Color scheme (change #00FF41 to your preferred color)

## 💡 Tips

1. The profile updates automatically - no manual work needed
2. Snake animation appears after first workflow run
3. WakaTime is optional but adds detailed coding stats
4. All external services are free and reliable
5. Stats don't expose private repository information

## 🎮 Gaming References

- "GG WP" - Good Game, Well Played
- "Player Stats" - Gaming terminology for character statistics
- "Boss Battle Analytics" - Epic battles = epic coding sessions
- "Power Level" - Dragon Ball Z reference for skill level
- "Achievements Unlocked" - Gaming achievement system

---

**Built for**: Dev @ Rihal  
**Purpose**: Showcase technical prowess while maintaining professional privacy  
**Theme**: Retro gaming meets modern development
