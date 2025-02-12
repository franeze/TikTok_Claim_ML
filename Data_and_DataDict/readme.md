### Data Understanding  

The dataset used in this project contains various features related to TikTok videos, including user engagement metrics and metadata. Below is a detailed description of each column:  

| Column Name             | Type  | Description  |
|-------------------------|-------|-------------|
| `#`                    | `int` | TikTok-assigned number for videos classified as claims or opinions. |
| `claim_status`         | `obj` | Indicates whether a video is identified as an “opinion” or a “claim.” An “opinion” represents a personal belief, while a “claim” refers to unsourced or unverified information. |
| `video_id`             | `int` | Random identifying number assigned to each published video. |
| `video_duration_sec`   | `int` | Duration of the video in seconds. |
| `video_transcription_text` | `obj` | Transcribed text of the words spoken in the video. |
| `verified_status`      | `obj` | Indicates whether the video's author is a "verified" or "not verified" TikTok user. |
| `author_ban_status`    | `obj` | Status of the author’s account: “active,” “under scrutiny,” or “banned.” |
| `video_view_count`     | `float` | Total number of views the video has received. |
| `video_like_count`     | `float` | Total number of likes the video has received. |
| `video_share_count`    | `float` | Total number of times the video has been shared. |
| `video_download_count` | `float` | Total number of times the video has been downloaded. |
| `video_comment_count`  | `float` | Total number of comments on the video. |

---

