# Mobile-App-Analytics

## Data Description:

### Source:
The data is taken from the **Firebase Analytics** public project:  
`firebase-public-project.analytics_153293282`.  
This dataset contains events that represent user activity within a mobile app.

---

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
- `event_name` — the name of the event.
- `event_timestamp` — the time when the event occurred.
- `user_pseudo_id` — the unique user identifier.
- `event_params` — parameters providing extra information about the event.

---

## Analysis Methods:

### 1. BigQuery (SQL):
**Purpose:**  
- Collecting, cleaning, and preprocessing large datasets.  
- Executing complex queries to:  
  - Filter data by dates (`event_date`).  
  - Group events (`event_name`).  
  - Calculate session durations (`TIMESTAMP_DIFF`).  
  - Identify returning users.  
- Optimizing queries for quick data retrieval.

---

### 2. Python (Jupyter Notebook):

#### Pandas:
- **For data manipulation** after downloading from BigQuery.  
- **Used for:**  
  - Grouping and aggregating data (e.g., counting events, creating cumulative metrics).  
  - Cleaning data (removing null or extreme values).  
  - **Example:** Analyzing session durations, counting event occurrences.

#### Matplotlib and Seaborn:
- **For creating visualizations** such as:  
  - Line charts (user retention).  
  - Histograms (session duration distribution).  
  - Heatmaps (activity by hour and day of the week).

---

## Results of Using These Methods:
These tools supported the full analytics workflow — from data collection to visualization and reporting.  
BigQuery enabled efficient handling of large datasets, Python allowed in-depth analysis and chart creation.


