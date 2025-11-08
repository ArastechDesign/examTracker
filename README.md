# Exam Tracker

A beautiful, customizable exam progress tracker built with Cloudflare Workers + KV. Features an iOS-inspired liquid glass design and admin panel for easy management.

## ✨ Features

- 🎨 Beautiful iOS liquid glass design
- 🔐 Admin panel to manage exams
- 📊 Real-time progress tracking
- 🔍 Search and filter functionality
- 📍 Exam locations
- 💾 Data stored in Cloudflare KV
- 🚀 **Deploy in 5 minutes!**
- 🌍 Open source - anyone can install their own
- 💰 **FREE** on Cloudflare Workers

## 🚀 Quick Deploy

See [DEPLOY.md](DEPLOY.md) for step-by-step instructions.

**TL;DR:**
```bash
npm install
npx wrangler login
npx wrangler kv namespace create "EXAM_DATA"
# Update wrangler.toml with KV ID and password
npx wrangler deploy
```

## Demo

**Live Demo:** https://exam-tracker.asrulmunir.workers.dev
**Admin Panel:** https://exam-tracker.asrulmunir.workers.dev/admin
(Password: changeme123)

## Usage

## Usage

### Public View
Visit your deployed URL to see the exam tracker.

### Admin Panel
1. Go to `/admin`
2. Login with your admin password
3. Configure title and description
4. Add/edit/delete exams
5. Save changes

## Configuration

### Change Admin Password
Edit `wrangler.toml`:
```toml
[vars]
ADMIN_PASSWORD = "your-new-password"
```

Then redeploy:
```bash
npx wrangler deploy
```

## Exam Data Format

```json
{
  "code": "EXAM001",
  "name": "Mathematics Paper 1",
  "date": "2025-12-01",
  "time": "08:15",
  "endTime": "10:15",
  "category": "Core"
}
```

## Customization

- Change colors in the CSS gradient
- Modify the liquid glass effect
- Add custom categories
- Adjust auto-refresh interval

## License

MIT - Feel free to use for your own exam tracking needs!

## Support

For issues or questions, please open an issue on GitHub.
