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
</div>

<!-- CONTENT -->

<div class="step-title">Insert and Load Data</div>


✅ Manually insert a single row into the table using `INSERT` statement.
```
INSERT INTO videos (video_id, added_date, title)
VALUES (36b8bac0-6260-11ea-ac4c-87a8af4b7ed0, '2020-03-09', 'Foundations of DataStax Enterprise');
```

✅ Use a `SELECT` statement to retrieve your row from the table.
```
SELECT * from videos;
```

✅ Insert another row into the table.
```
INSERT INTO videos (video_id, added_date, title) 
VALUES (95fe9800-2c2f-11b2-8080-808080808080, '2020-01-20', 'Cassandra Data Modeling');

```

✅ Retrieve all rows from the table.
```
SELECT * from videos;
```

<!-- NAVIGATION -->
<div id="navigation-bottom" class="navigation-bottom">
 <a href='command:katapod.loadPage?[{"step":"step1"}]'
   class="btn btn-dark navigation-bottom-left">⬅️ Back
 </a>
</div>