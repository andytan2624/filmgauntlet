---
title: Installation
description: 'Install all the things....'
updated_by: d73c1391-a10f-4f96-a8d1-30cc427a0b6a
updated_at: 1585305629
id: 586d4f7c-c6d5-4858-837a-fd2829e04f87
---
Like Statamic, you'll need to have Composer installed before doing anything.

As long as you've got that installed, along with the other requirements, just run through these steps.

**1. Create a new site** by cloning the repo and removing the Gitness
```
git clone git@github.com:doublethreedigital/docs-starter-kit docs-site
cd docs-site
rm -rf .git
composer install
cp .env.example .env && php artisan key:generate
```

**2. Make a new user** - make sure it'a a super so you can login to the CP
```
php please make:user
```

**3. Recompile the CSS** (only if you wanna)
This starter kit uses TailwindCSS and PurgeCSS, meaning it has a build process. 
```
yarn && yarn dev
```

And if you want to do it for production:
```
yarn prod
```

**4. Do your thing!**
If you're using Valet, your site should be good to go at `http://docs-site.test`.

Enjoy!!
