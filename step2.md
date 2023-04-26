<!-- TOP -->
<div class="top">
  <img class="scenario-academy-logo" src="https://datastax-academy.github.io/katapod-shared-assets/images/ds-academy-2023.svg" />
  <div class="scenario-title-section">
    <span class="scenario-title">Cassandra Query Language (CQL)</span>
    <span class="scenario-subtitle">ℹ️ For technical support, please contact us via <a href="mailto:academy@datastax.com">email</a>.</span>
  </div>
</div>

<!-- NAVIGATION -->
<div id="navigation-bottom" class="navigation-bottom">
 <a href='command:katapod.loadPage?[{"step":"step1"}]'
   class="btn btn-dark navigation-bottom-left">⬅️ Back
 </a>
<span class="step-count"> Step 2 of 2</span>
<a href='command:katapod.loadPage?[{"step":"finish"}]' 
    class="btn btn-dark navigation-top-right">Next ➡️
  </a>
</div>

<!-- CONTENT -->

<div class="step-title">Insert and Load Data</div>


✅ Manually insert a single row into the table using an `INSERT` statement.

|`video_id`                 | `added_date` | `title` |
|---------------------------|--------------|---------|
| `36b8bac0-6260-11ea-ac4c-87a8af4b7ed0` | 2020-03-09 | Foundations of DataStax Enterprise |

<details class="katapod-details">
  <summary>Solution</summary>

```
INSERT INTO videos (video_id, added_date, title)
VALUES (36b8bac0-6260-11ea-ac4c-87a8af4b7ed0, '2020-03-09', 'Foundations of DataStax Enterprise');
```

</details>

✅ Use a `SELECT` statement to retrieve your row from the table.

<details class="katapod-details">
  <summary>Solution</summary>

```
SELECT * from videos;
```

</details>


✅ Insert another row into the table.

|`video_id`                 | `added_date` | `title` |
|---------------------------|--------------|---------|
| `95fe9800-2c2f-11b2-8080-808080808080` | 2020-01-20 | Cassandra Data Modeling |

<details class="katapod-details">
  <summary>Solution</summary>


```
INSERT INTO videos (video_id, added_date, title) 
VALUES (95fe9800-2c2f-11b2-8080-808080808080, '2020-01-20', 'Cassandra Data Modeling');

```

</details>


✅ Retrieve all rows from the table.
```
SELECT * from videos;
```

✅ Delete all previously inserted rows from the table using the `TRUNCATE` statement and verify that the table is empty.

<details class="katapod-details">
  <summary>Solution</summary>

```
TRUNCATE videos;
SELECT * from videos;
```

</details>

✅ Use the `COPY` command to import data into your `videos` table.
```
COPY videos(video_id, added_date, title)
FROM '/workspace/ds201-lab02/data-files/videos.csv'
WITH HEADER=TRUE;
```

✅ Retrieve all rows from the table to verify that the table loaded correctly.
```
SELECT * from videos;
```

<!-- NAVIGATION -->
<div id="navigation-bottom" class="navigation-bottom">
 <a href='command:katapod.loadPage?[{"step":"step1"}]'
   class="btn btn-dark navigation-bottom-left">⬅️ Back
 </a>
 <a href='command:katapod.loadPage?[{"step":"finish"}]' 
    class="btn btn-dark navigation-top-right">Next ➡️
  </a>
</div>