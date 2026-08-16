<div align="center">

  <!-- TOP ANIMATED BADGE -->
  <p align="center">
    <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=700&size=28&pause=1000&color=FF2D20&center=true&vCenter=true&width=700&lines=%E2%9A%A1+AH-PRESS+BACKEND+ENGINE+%E2%9A%A1;THE+MOST+POWERFUL+NEWS+BACKEND;ENGINEERED+FOR+EXTREME+SCALE+%26+SPEED" alt="Typing SVG" />
  </p>

  <!-- RUNNING MARQUEE -->
  <marquee behavior="scroll" direction="left" scrollamount="7" style="background: #1a1a1a; color: #00ffcc; padding: 8px; font-weight: bold; font-family: monospace; border-radius: 5px;">
    🔥 ZERO BOTTLENECK ARCHITECTURE 🚀 15 HYPER-OPTIMIZED TABLES ⚡ NON-BLOCKING ASYNC VISITOR TRACKING 💎 CENTRALIZED MEDIA REUSE ENGINE 🎯 HIGH PRECISION AD MONETIZATION 🔥
  </marquee>

  <br><br>

  <!-- TECH STACK BADGES -->
  <p align="center">
    <img src="https://img.shields.io/badge/PHP-8.3-777BB4?style=for-the-badge&logo=php&logoColor=white" />
    <img src="https://img.shields.io/badge/Laravel-11-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" />
    <img src="https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
    <img src="https://img.shields.io/badge/Redis-Horizon-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
    <img src="https://img.shields.io/badge/Architecture-Clean%20%26%20Decoupled-00C7B7?style=for-the-badge" />
  </p>

</div>

<hr>

### ⚡ AH-PRESS VS TRADITIONAL CMS

| Architecture Metric | Traditional CMS Scripts | AH-PRESS Enterprise Engine |
| :--- | :--- | :--- |
| **Database Structure** | ❌ 40+ Bloated DB Tables | ⚡ 15 Hyper-Optimized Schemas |
| **Visitor Analytics** | ❌ DB Lock on View Count | ⚡ Non-blocking Async Analytics |
| **Storage Handling** | ❌ Duplicate File Uploads | ⚡ Centralized Media Reuse System |
| **Layout Flexibility** | ❌ Hardcoded Frontends | ⚡ Dynamic DB Grid (`grid_span`) |
| **Codebase Quality** | ❌ Messy Monolith Codebase | ⚡ Decoupled Modular Profiles |

<br>

## ⚡ CORE ENGINE ARCHITECTURE

### 🎨 1. Dynamic Homepage Grid System
> Forget static layouts! Content editors control Bootstrap column proportions (`col-md-12`, `col-md-8`, `col-md-4`) directly from the backend via `grid_span`. No frontend redeployment required.

### 🖼️ 2. Centralized Media Storage Engine
> Every asset uploaded is assigned a unique `media_id`. Re-use existing images infinitely across Articles, Profiles, and Advertisements without increasing S3 or Disk storage overhead.

### 📊 3. High-Traffic Guest Analytics
> Zero database locking. Tracks unique readers using IP Address and User Agent hashing via background queues. Handles millions of concurrent hits without breaking a sweat.

### 💰 4. Ad Targeting & Monetization Pipeline
> Inject high-converting ad zones (`ad_zones`) directly into specific categories or layout blocks with precision impression and click-tracking counters.

<br>

## 📂 DATABASE TOPOLOGY (15 SCHEMAS)

<details>
<summary><b>🔥 Click to Expand 15-Table Architecture</b></summary>

<br>

```sql
  1. roles            ➜ Auth Roles (Admin, Journalist, Reader)
  2. users            ➜ Core Credentials (Email/Mobile Auth)
  3. user_profiles    ➜ Nullable Polymorphic Profiles (1:1 Relationship)
  4. categories       ➜ Self-referencing Taxonomy (Categories & Sub-categories)
  5. regions          ➜ Geographic Hierarchy (Divisions & Districts)
  6. tags             ➜ High-speed Content Tagging
  7. articles         ➜ News Engine Core (grid_span, status, breaking_news)
  8. article_tag      ➜ Article-Tag Pivot Table
  9. media            ➜ Centralized Storage Metadata Repository
 10. ad_zones         ➜ Layout Ad Slot Definitions
 11. ads              ➜ Ad Content, Impressions & Click Counters
 12. comments         ➜ Self-referencing Nested Comment Threads
 13. bookmarks        ➜ Reader Saved Articles
 14. system_settings  ➜ Dynamic Global Key-Value Store
 15. article_views    ➜ Non-blocking IP & User-Agent Analytics Engine

```

## 🛠️ QUICK DEPLOYMENT

```bash
# Clone the repository
git clone https://github.com/your-username/AH-PRESS-news-engine.git

# Navigate to project directory
cd AH-PRESS-news-engine

# Install dependencies
composer install

# Environment configuration
cp .env.example .env
php artisan key:generate

# Run Database Migrations & Seeders
php artisan migrate --seed

# Symlink Storage & Start Engine
php artisan storage:link
php artisan serve

```