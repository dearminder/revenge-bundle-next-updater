# 🚀 Revenge Bundle Updater

A GitHub Pages site that automatically syncs and hosts the latest [Revenge Next](https://github.com/revenge-mod/revenge-bundle-next) bundles daily.

## ⚠️ Warning
> Using custom bundles allows remote code execution. Only use custom bundles from sources you trust.

## 📦 What's This?

This repository automatically fetches the latest production and development bundles from the official Revenge Next repository and hosts them via GitHub Pages. The bundles are updated **once per day** to ensure you always have access to the latest version.

## 🔗 Usage

Set your custom bundle URL in your loader:


Head to Settings > Developer (under the Revenge section).

Tap on the Evaluate JavaScript option.

Paste the link to bundle:

### Production Bundle
>https://dearminder.github.io/revenge-bundle-updater/latest/revenge.bundle
### Development Bundle
>https://dearminder.github.io/revenge-bundle-updater/latest/revenge-development.bundle
## ⚙️ How It Works

1. **Scheduled Sync**: GitHub Actions runs daily at midnight UTC
2. **Fetch Latest**: Downloads the most recent successful build from Revenge Next
3. **Deploy**: Automatically publishes to GitHub Pages
4. **Always Fresh**: You get the latest bundles without manual intervention

## 🛠️ Manual Update

Want to update immediately? Fork the repo and trigger the workflow manually:

1. Go to the [Actions tab](../../actions/workflows/sync.yml)
2. Click "Run workflow"
3. Wait ~1-2 minutes for the update to complete

## 📊 Update Status

Check the [latest workflow run](../../actions) to see when bundles were last updated.

## ⭐ Credits

- [Revenge Mod](https://github.com/revenge-mod) - Original bundle source
- Automated with GitHub Actions

## 📄 License

This is just a deploy tool. All bundle code belongs to the Revenge Mod team.
