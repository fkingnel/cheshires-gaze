# Chashire's Gaze Badge System

Step into Cheshire’s Gaze, where badges are alive. Each one bears a name, a cryptic icon, and a counter that grows as eyes fall upon it. Use text, symbols, and logos to craft your sigil, and even turn the count into Roman numerals for a touch of arcane elegance.

Harness the magic via URL query parameters.

# Preview

## ALPHA LANDING PAGE DEMO
<img src='https://github.com/fkingnel/cheshires-gaze/blob/main/gallery/chesiresgazepreview.PNG?raw=true'>

## EARLY METRICS INTEGRATION DEMO
<img src='https://github.com/fkingnel/cheshires-gaze/blob/main/gallery/chesiresgazepreviewmetrics.PNG?raw=true'>

## PROJECT IS STILL WORK IN PROGRESS AND NOT COMPLETED

TO DO:
- Complete landing page
- Adjust code for Render
- Host on Render
- Complete README documentation

# Query Parameters and Metrics

| Query Parameter / Metric | Type   | Description                                         | Example                                                                                                           |
| ------------------------ | ------ | --------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `username`               | string | User for badge view counter                          | `&username=fkingnel`                                                                                              |
| `key`                    | string | Secret key for profile counter                       | `&key=a69bcdc3f3f12b37`                                                                                           |
| `repo`                   | string | GitHub repo URL (required for GitHub metrics)       | `&repo=https://github.com/fkingnel/cheshires-gaze-badge-system`                                                  |
| `leftItems`              | string | Left label sequence (icons, text, logos, metrics)  | `&leftItems=:stars,Stars`                                                                                         |
| `rightItems`             | string | Right label sequence                                 | `&rightItems=:stars`                                                                                               |
| `height`                 | number | Badge height in px                                   | `&height=28`                                                                                                      |
| `labelColors`            | string | Colors for left and right labels                     | `&labelColors=black,grey`                                                                                         |
| `leftLink`               | string | Link for left label                                  | `&leftLink=https://github.com/fkingnel`                                                                          |
| `rightLink`              | string | Link for right label                                 | `&rightLink=https://github.com/fkingnel/cheshires-gaze-badge-system`                                            |
| `style`                  | string | Badge style (`flat`, `flat-square`, etc.)           | `&style=flat-square`                                                                                               |
| `roman`                  | string | Show counts as Roman numerals                        | `&roman=true`                                                                                                     |
| `:views`                 | metric | Local badge view count                                | `:views`                                                                                                          |
| `:stars`                 | metric | GitHub stars                                         | `:stars`                                                                                                         |
| `:forks`                 | metric | GitHub forks                                         | `:forks`                                                                                                         |
| `:watchers`              | metric | GitHub watchers                                      | `:watchers`                                                                                                      |
| `:open_issues`           | metric | Open issues                                         | `:open_issues`                                                                                                   |
| `:size`                  | metric | Repo size (KB)                                      | `:size`                                                                                                          |
| `:release_count`         | metric | Number of releases                                  | `:release_count`                                                                                                 |
| `:contributors`          | metric | Number of contributors                               | `:contributors`                                                                                                  |
| `:last_commit_age`       | metric | Age of last commit (hours)                           | `:last_commit_age`                                                                                               |


## Fontawesome Icon Integration

Cheshire’s Gaze supports **over 2,000 Font Awesome icons** from the free **Brands** and **Classic** collections. You can use them in your badge via the `leftItems` or `rightItems` query parameters.

- **Usage examples:** `heart:solid`, `star:regular`, `knife:custom`, `github:brands` etc.
- **Custom Icons:** You can also include custom icons by adding them to the `utils/icons` folder. Currently, only a few custom icons are available, but more can be added over time.

Browse available Font Awesome icons here: [Font Awesome Free Brands & Classic](https://fontawesome.com/search?ip=brands%2Cclassic&ic=free-collection)