# ⚠️ [RETIRED / ARCHIVED REPOSITORY]

> ### 🛑 NOTICE: THIS REPOSITORY IS RETIRED (OVER 2 YEARS OLD)
> This codebase, configuration guide, and historical architecture are **deprecated and no longer maintained**. 
>
> 🚀 **Visit the modern, actively maintained repository:**  
> **👉 [https://github.com/promexdotme/laravel-social-gaming](https://github.com/promexdotme/laravel-social-gaming)**
>
> 💬 **Join our official community & verification hub:**  
> **👉 [https://discord.gg/opensource-sports-casino-982859564795957268](https://discord.gg/opensource-sports-casino-982859564795957268**  
> *(All legacy Discord invite links below are expired. Use the link above).*

---

# opensource-casino

Open source slots casino script (formerly-Goldsvet)

This is a legacy laravel casino app, you need to download game packs for it.

You can join our updated Discord at **https://discord.gg/YOUR_NEW_INVITE_LINK** to verify your account and access resources. Games work for both versions (up to v9 so far).

Do not forget to download:  
https://drive.google.com/file/d/1bbRD74BL-f2MOAG4LrBCKlwsYK6qteMj/view  
And add it to your: `storage/app/GeoIP2-City_20201006/` folder.  
The setup assumes regular Laravel setup, with casino folder setup outside your www (or change index).

---

### HISTORICAL SETUP GUIDE (CPANEL SAMPLE)

THIS DOCUMENT SHOWS A SETUP SAMPLE ON A CPANEL SERVER, AND CAN BE REPLICATED ON OTHER SETUPS.

1. Setup your server with Apache, MySQL, PHP 7.1–7.4, Composer, Node.js 16 & PM2.
2. Force Domain SSL.
3. Generate SSL CRT, KEY & BUNDLE. Copy the contents of your CRT/KEY/BUNDLE to files in folder:  
   `casino/PTWebSocket/ssl/`
4. Create a new email & password.
5. Create a new database, grant all privileges.
6. Import the SQL file located in folder `casino/database/migrations/betshopme_8.sql` via phpMyAdmin to the database.  
   *(Extra DB file `experimentalarcadegames.sql` not required unless experimenting with arcade games).*

#### Zip File Uploads
`casino.zip` and `public_html.zip` should be unzipped in the following manner:
* `public_html` → this is your public directory
* `casino` → this goes outside your public folder for security so it becomes your root folder:
  ```text
  /casino
  /public_html
