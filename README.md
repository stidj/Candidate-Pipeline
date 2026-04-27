# 🌊 Candidate Pipeline

A lightweight, browser-based recruitment pipeline management tool for tracking candidates through multiple stages. Built with vanilla JavaScript, no backend required.

## 🎯 Features

- **Kanban board** with 8 customizable stages (Sourced → Placed)
- **Candidate management** with full CRUD operations
- **Drag-and-drop** interface for moving candidates between stages
- **Compensation tracking** with fee calculations
- **Calendly integration** to auto-import scheduled events
- **Activity logging** for all candidate interactions
- **Search & filter** by name, role, client, or notes
- **CSV export** for external reporting
- **Dark mode** support
- **Persistent storage** with browser localStorage

## 🚀 Quick Start

Your app is deployed and live at:
```
https://stidj.github.io/Candidate-Pipeline
```

## 🔧 Calendly Integration

To sync Calendly bookings:

1. Get your Personal Access Token at [calendly.com/integrations/api_webhooks](https://calendly.com/integrations/api_webhooks)
2. Click **"↻ Calendly"** button in the app
3. Paste your token and select default stage for new bookings
4. Click **"Sync now"**

The app fetches events from the last 30 days and creates candidates for invitees who aren't already in your pipeline.

## 💾 Data Storage

All data is stored in your browser's localStorage - no server required. Your pipeline is:
- ✅ Private (stays on your device)
- ✅ Always available offline
- ✅ Backed up to localStorage

## 📋 Stages

1. **Sourced** - Passive candidates identified
2. **Outreached** - Initial contact made
3. **Responded** - Candidate replied
4. **Screening** - Phone/initial interview
5. **Submitted** - Sent to client
6. **Interviewing** - In client interviews
7. **Offer** - Offer extended
8. **Placed** - Successfully placed

## 🏷️ Candidate Priorities

- **Hot** (🔴) - High priority, immediate follow-up
- **Warm** (🟡) - Medium priority, normal cadence
- **Cold** (⚪) - Low priority, backlog

## 💰 Fee Calculations

Fees auto-calculate as: `Offer Comp × Fee % / 100`

Or override with a custom fee amount.

## ⌨️ Keyboard Shortcuts

- `Escape` - Close modals
- `Enter` - Save candidate (from text fields)
- Double-click card - Edit candidate

## 🌙 Dark Mode

Automatically uses your system preference.

## 📊 Summary Bar

Real-time stats:
- **Total pipeline** - All candidates
- **Active** - Non-placed candidates
- **Placed** - Successfully placed
- **Projected fees** - Fees from active placements
- **Placed fees** - Collected fees
- **Calendly synced** - Auto-imported candidates

## 🐛 Troubleshooting

**Calendly sync not working:**
- Verify your token is valid at [calendly.com/integrations/api_webhooks](https://calendly.com/integrations/api_webhooks)
- Check browser console for errors (F12)
- Ensure events have invitee email addresses

**Data disappeared:**
- Check if you're in a private/incognito window (uses separate localStorage)
- Try a different browser
- Check if localStorage is enabled in browser settings

---

**Built with ❤️ for recruiting teams** | No signup, no fees, no tracking