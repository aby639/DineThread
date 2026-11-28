# Customer menu retest on 28 November 2026

Bibek Rai recorded three checks on the DineThread customer menu. The times below are offsets in the individual recordings. The earlier baseline and revised builds retain their own results.

| Recording | Observation | Evidence |
| --- | --- | --- |
| Keyboard | Whipped Feta & Honey had focus at 0:08. The dish dialog opened and Close had focus at 0:16. After the dialog closed, focus returned to the same dish at 0:18. | [Keyboard frames](keyboard-focus.png) |
| NVDA Speech Viewer | Submitting without a table produced 'Please select your table first' (0:20). Speech Viewer listed Preparing (0:50), Ready (1:01), Served (1:08), the bill acknowledgement (1:19) and Paid (1:35). | [Speech Viewer frames](nvda-speech.png) |
| Chrome zoom | Chrome displayed 200% (0:02). The menu scrolled, the dish dialog exposed Add (0:29), and three portions reached the cart at $16.50 (0:44). The order-status panel displayed the bill acknowledgement (1:14). | [Zoom and dish frames](browser-zoom.png) |

The recordings establish these outcomes for the journeys shown. The zoom recording shows pointer use on Add. Its keyboard focus ring and numerical contrast were not measured. The recordings do not identify the exact application build or installed browser and NVDA versions. The separate download-page screenshot lists NVDA 2026.3.1.

## Original recordings

The group retains the original MP4 files. These SHA-256 hashes identify the recordings from which the public frame excerpts were cropped.

| Recording filename | SHA-256 |
| --- | --- |
| 20261128-0001-33.9049338.mp4 | d9684bfc7a04e18f64dd27f7cfc8097a85dc7bbba99caab62fdf2d999ddf7beb |
| 20261128-0033-21.6871589.mp4 | 99065fe3531c7f9e8b63eeeeb80a45aa257ddbb60192b23a490acd415bc3801d |
| 20261128-0053-52.6791674.mp4 | 491ba76409944b7c9e8218824a5878bc904bcc52020d8f579bcf46d6273d75bb |
