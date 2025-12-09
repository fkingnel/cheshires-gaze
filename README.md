# cheshires-gaze


## preview
<img src='https://github.com/fkingnel/cheshires-gaze/blob/main/gallery/chesiresgazepreview.PNG?raw=true'>

Chashire's Gaze Badge System

Chashire's Gaze is a dynamic badge generator that allows users to create badges with customizable labels, icons, logos, text, and view counters. Each badge has a secure counter that increments on every view. You can also optionally display counts in Roman numerals.

Badges are fully customizable via URL query parameters.

TO DO:
- HOST ON RENDER

| Query Parameter | Type   | Default        | Description                                                                                  | Example                                                                        |
| --------------- | ------ | -------------- | -------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| `username`      | string | `""`           | The username associated with the badge counter.                                              | `fkingnel`                                                                     |
| `key`           | string | `""`           | The secret key for the user/profile to increment/view the count.                             | `a69bcdc3f3f12b37`                                                             |
| `leftItems`     | string | `""`           | Comma-separated sequence for left label: icons, logos, text, or `{count}` for dynamic count. | `knife:custom,{count},https://avatars.githubusercontent.com/u/69657658?v=4,hi` |
| `rightItems`    | string | `""`           | Comma-separated sequence for right label. Same as `leftItems`.                               | `knife:custom,{count},https://avatars.githubusercontent.com/u/69657658?v=4,hi` |
| `height`        | number | `28`           | Height of the badge in pixels.                                                               | `28`                                                                           |
| `labelColors`   | string | `"black,grey"` | Comma-separated colors for left and right labels. Can use named colors or hex codes.         | `black,grey` or `#111,#eee`                                                    |
| `leftLink`      | string | `"#"`          | URL the left label links to.                                                                 | `https://github.com/fkingnel/`                                                 |
| `rightLink`     | string | `"#"`          | URL the right label links to.                                                                | `https://github.com/fkingnel/cheshires-gaze/`                                  |
| `style`         | string | `"flat"`       | Badge style. Options: `flat`, `flat-square`, `plastic`, `for-the-badge`, `circular`.         | `flat-square`                                                                  |
| `roman`         | string | `"false"`      | Optional. Set to `"true"` to display counts as Roman numerals.                               | `true`                                                                         |
