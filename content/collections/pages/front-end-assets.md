---
title: 'Front-end Assets'
updated_by: d73c1391-a10f-4f96-a8d1-30cc427a0b6a
updated_at: 1585308509
id: 18d0418e-1e73-4016-969c-25e862e347cb
---
This starter kit uses Laravel Mix to compile and process CSS & JavaScript assets. 

This means that every time you make changes to CSS or JS, you'll need to re-process your assets. Here's a little demo of how to do that.

> Oh and quick side note, you're gonna need to have your Npm or Yarn dependencies installed before running these commands. Just run `npm i`

## Processing for Development
If you're just wanting to compile the assets once, run `npm run dev`.

Or you can have it watching for changes, and compile when those changes happen. We also have BrowserSync setup so your page will refresh whenever a change happens, just like magic! ✨ `npm run watch`

## Processing for Production
When you run for production, Mix will also minify your styles and it will remove any style rules that aren't being used in your code. `npm run production`