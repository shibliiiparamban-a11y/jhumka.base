# Jhumka Base

A simple web app for the Jhumka jewellery business. It keeps purchases, products, expenses, customers and a sales summary in one place, with a light and a dark mode. It works on phones and on desktop.

## What is inside

- **Summary:** total and monthly sales, total and monthly products sold, a six month growth graph and profit.
- **Purchases:** item number, product name, product image, wholesale rate, quantity and bill image.
- **Products:** search, item number, item name, our price, selling price and stock.
- **Expenses:** dropdown type (you can add or remove options), amount, count, total and date.
- **Customers:** name, phone and PIN. Paste a customer message and use "Extract info" to fill the fields.
- **Sales:** record a sale from the Customers tab. It feeds the Summary.
- **Profile:** tap the round button at the top. Enter your name to sign in, and add a profile picture if you like. Your picture, or your first letter if you have none, shows on the button. The page lists the team and recent sign-ins.

## Put it on GitHub Pages

1. Create a new repository on GitHub, for example `jhumka-base`.
2. Upload `index.html` and `README.md` to the root of the repository.
3. Open **Settings, Pages**. Under **Build and deployment** choose **Deploy from a branch**, pick the `main` branch and the `/ (root)` folder, then save.
4. After a minute the app is live at `https://YOUR-USERNAME.github.io/jhumka-base/`.

It is one static file. There is nothing to build or install.

## Demo data

The first time the app opens in a browser it fills itself with demo data: 8 products, 6 customers, six months of purchases, sales and expenses, and three demo teammates on the Profile page. Dates are set relative to today, so the graph always shows a recent trend. Demo entries are marked as samples. Tap **Remove all samples** at the top of any tab to clear them and start with your own books. They are not added again on that device.

## Sign-in on GitHub Pages

The sign-in here is a name saved on the device. It is not a password, and it does not stop anyone who opens the page from seeing the books. Real team logins need a hosted login service such as Firebase Authentication. The Claude hosted version uses each person's Claude account instead, and it only lets invited people in.

## Where the data is saved

On GitHub Pages every entry is saved in the browser of the device you use, so each phone or computer has its own separate books. Clearing the browser data erases them. Photos are kept in the same place and are shrunk to save space.

To share one set of books between several people, the data needs a shared database. The Claude hosted version of this app does that. A hosted database such as Firebase or Supabase can be added to this file later.

## Files

- `index.html` is the whole app: layout, styles and code in one file.

## New in this version
- **Monthly target:** the owner sets an orders target; Summary shows orders left and a progress bar.
- **Month vs last month** comparison with up and down arrows.
- **Payment status** (Paid, Pending, COD) and a "Money to collect" card.
- **Returns and damages** correct stock and profit.
- **Quick add:** same-as-last-time buttons, repeat order, scan QR or barcode, printable QR labels.
- **Product photos** on every product.
- **Roles** (Owner, Manager, Packing staff) and an **activity log**. Hosted version only.
- **Backup and export:** backup file, Excel, CSV, monthly reminder, and import from Google Sheet or a file.

Note: on GitHub Pages everything is saved on each device, so roles and the shared activity log only apply to the hosted version.

## Files in this repository
- `index.html` is the whole app.
- `assets/` holds the logo, favicon and app icons.
- `.nojekyll` tells GitHub Pages to serve the files as they are.
