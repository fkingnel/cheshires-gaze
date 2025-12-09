# cheshires-gaze 

## PROJECT IS STILL WORK IN PROGRESS AND NOT COMPLETED

TO DO:
- Complete landing page
- Adjust code for Render
- Host on Render
- Complete README documentation

## Preview
<img src='https://github.com/fkingnel/cheshires-gaze/blob/main/gallery/chesiresgazepreview.PNG?raw=true'>

## Chashire's Gaze Badge System

Step into Cheshire’s Gaze, where badges are alive. Each one bears a name, a cryptic icon, and a counter that grows as eyes fall upon it. Use text, symbols, and logos to craft your sigil, and even turn the count into Roman numerals for a touch of arcane elegance.

Harness the magic via URL query parameters.

## Query Parameters and Features
| Query Parameter | Type   | Description                                                                                                           | Example                                                                                                           |
| --------------- | ------ | --------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `username`      | string | The username associated with the badge counter. Optional if you do not want use the tracking feature                                                                    | `&username=fkingnel`                                                                                              |
| `key`           | string | The secret key for the user/profile to increment/view the count. Optional if you do not want use the tracking feature                                                    | `&key=XXXXXXXXXXXXXXXX`                                                                                           |
| `leftItems`     | string | Comma-separated sequence for the left label. Can include **icons** (`heart:solid`), **logos** (image URLs), **text**, and `{count}` for dynamic counter placement. | `&leftItems=knife:custom,github:brands,{count},https://avatars.githubusercontent.com/u/69657658?v=4,hi`                        |
| `rightItems`    | string | Comma-separated sequence for the right label. Same as `leftItems`. Supports icons, logos, text, and `{count}`.       | `&rightItems=star:regular,heart:solid,{count},https://avatars.githubusercontent.com/u/69657658?v=4,viewers`                   |
| `height`        | number | Height of the badge in pixels.                                                                                        | `&height=28`                                                                                                      |
| `labelColors`   | string | Comma-separated colors for left and right labels. Can use named colors or hex codes.                                  | `&labelColors=black,grey`                                                                                         |
| `leftLink`      | string | URL the left label links to.                                                                                          | `&leftLink=https://github.com/fkingnel/`                                                                         |
| `rightLink`     | string | URL the right label links to.                                                                                         | `&rightLink=https://github.com/fkingnel/cheshires-gaze/`                                                         |
| `style`         | string | Badge style. Options: `flat`, `flat-square`, `plastic`, `for-the-badge`, `circular`.                                  | `&style=flat-square`                                                                                               |
| `roman`         | string | Optional. Set to `"true"` to display counts as Roman numerals.                                                        | `&roman=true`                                                                                                     |


### fontawesome integration

Cheshire’s Gaze supports **over 2,000 Font Awesome icons** from the free **Brands** and **Classic** collections. You can use them in your badge via the `leftItems` or `rightItems` query parameters.

- **Usage examples:** `heart:solid`, `star:regular`, `knife:custom`, `github:brands` etc.
- **Custom Icons:** You can also include custom icons by adding them to the `utils/icons` folder. Currently, only a few custom icons are available, but more can be added over time.

Browse available Font Awesome icons here: [Font Awesome Free Brands & Classic](https://fontawesome.com/search?ip=brands%2Cclassic&ic=free-collection)