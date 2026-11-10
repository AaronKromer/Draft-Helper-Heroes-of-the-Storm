# Heroes of the Storm Draft Helper

A small web tool to help you choose heroes during a *Heroes of the Storm* draft.

**Live site:** [hots-drafter.mimmuzzi.workers.dev](https://hots-drafter.mimmuzzi.workers.dev/)

## Features

- Build your allied team, enemy team, and ban list.
- Search heroes and filter the roster by role.
- Select a map and get recommendations for your next hero pick.
- Review each recommendation's score and explanations, based on map ratings, synergies, and counters included in the app.

## How to use

1. Select a map.
2. Use the `Ally`, `Enemy`, and `Ban` buttons to choose which group to add heroes to.
3. Search or filter the roster, then select heroes to add them to the draft. Select an added hero again to remove it.
4. Click **Find the Best Hero** to see recommendations. You can also filter the results by role.

## Run locally

This is a static website and does not require a build step, dependencies, or a local server. Clone or download the repository and open `index.html` directly in your browser.

Alternatively, you can serve the project folder with a local HTTP server. For example, with Python:

```bash
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

## Deployment

Deploy the project folder to a static hosting service, preserving its file structure. The page uses relative paths for portraits in `heroes_profiles/` and icons in `icon/`, so include both folders alongside `index.html`.

## Project structure

- `index.html`: interface, hero data, and draft and recommendation logic.
- `heroes_profiles/`: hero portraits in WebP format.
- `icon/`: role icons and other image assets.
