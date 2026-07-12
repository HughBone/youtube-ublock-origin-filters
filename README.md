# youtube-ublock-origin-filters

Paste these into 'My Filters' in ublock origin settings:

```
! 4 video columns instead of 3
www.youtube.com##.ytd-rich-grid-renderer:style(--ytd-rich-grid-items-per-row: 4 !important;)

! Hide shorts
! Hide playable games
! Hide 'Explore more topics'
www.youtube.com##ytd-rich-section-renderer

! Hide already watched videos
www.youtube.com##ytd-rich-item-renderer:has(yt-thumbnail-overlay-progress-bar-view-model)
www.youtube.com##yt-lockup-view-model:has(yt-thumbnail-overlay-progress-bar-view-model)

! Hide Upcoming videos
www.youtube.com##ytd-rich-item-renderer:has(badge-shape:has-text(Upcoming))

! Hide livestream vods
www.youtube.com##ytd-rich-item-renderer:has(span:has-text(Streamed))

! Hide music Mix playlists
www.youtube.com##ytd-rich-item-renderer:has(.ytBadgeShapeText:has-text(Mix))
```
