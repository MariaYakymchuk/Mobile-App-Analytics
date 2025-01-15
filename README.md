# Mobile-App-Analytics

## Goal:
Analyzing and interpreting user behavior trends.

## Data Description:

### Source:
The data is taken from the **Firebase Analytics** public project: 
`firebase-public-project.analytics_153293282`. This dataset contains events 
that represent user activity within a mobile app.

### Main Characteristics:

#### 1. Time Range:
The time range of **June 12, 2018, to October 3, 2018**, was chosen for analysis because it is the only available period in the dataset. 

This range provides almost four months of data, allowing for the identification of event dynamics and trends. Date filtering was applied to make the queries clear and universal, helping to avoid potential errors when updating or expanding the data.

The sample includes all events within the available period, ensuring maximum representativeness and accuracy of the results. It also allows for a detailed analysis of user behavior in the short term.

#### 2. Event Types:
- **Navigation:** `screen_view`, which shows interactions with screens.
- **User Engagement:** `user_engagement`, reflecting overall activity.
- **Gaming:** 
  - `level_start_quickplay`
  - `level_end_quickplay` (start and end of levels)
  - `post_score` (posting scores).

#### 3. Users:
Users are identified by a unique `user_pseudo_id`, which allows tracking their behavior.

---

### Format:
The data is structured as a table with the following main fields:
- **event_name** — the name of the event.
- **timestamp** — the time when the event occurred.
- **user_pseudo_id** — the unique user identifier.
