<!-- TOP -->
<div class="top">
  <img class="scenario-academy-logo" src="https://datastax-academy.github.io/katapod-shared-assets/images/ds-academy-2023.svg" />
  <div class="scenario-title-section">
    <span class="scenario-title">Cassandra Query Language (CQL)</span>
    <span class="scenario-subtitle">ℹ️ For technical support, please contact us via <a href="mailto:academy@datastax.com">email</a>.</span>
  </div>
</div>

<!-- NAVIGATION -->
<div id="navigation-top" class="navigation-top">
 <a href='command:katapod.loadPage?[{"step":"intro"}]'
   class="btn btn-dark navigation-top-left">⬅️ Back
 </a>
<span class="step-count"> Step 1 of 2</span>
 <a href='command:katapod.loadPage?[{"step":"step3"}]' 
    class="btn btn-dark navigation-top-right">Next ➡️
  </a>
</div>

<!-- CONTENT -->

<div class="step-title">Create and use a keyspace</div>

Welcome to the KillrVideo company! KillrVideo hired you to build the latest and greatest video sharing application on the Internet. Your task is to ramp up on the domain and become acquainted with Apache Cassandra. To start, you are looking into creating a table schema and to load some data.

The video metadata is made up of:

|Column Name    |Date Type     |
|---------------|--------------|
|video_id       |timeuuid      |
|added_date     |timestamp     |
|title          |text          |



✅ Use `nodetool` to verify that Cassandra is running:
```
cd /workspace/ds201-lab02/apache-cassandra-4.1.0/bin/
./nodetool status 
```

✅ View the downloaded tarball:
```
ls -l
```

✅ Extract tarball:
```
tar xf apache-cassandra-4.1.0-bin.tar.gz
```

The directory should now contain the tarball and the `apache-cassandra-4.1.0` directory

✅ View the directory:
```
ls -l
```

This lab uses a single Cassandra instance. (Subsequent labs will use a multi-node Cassandra cluster.)


<!-- NAVIGATION -->
<div id="navigation-bottom" class="navigation-bottom">
 <a href='command:katapod.loadPage?[{"step":"intro"}]'
   class="btn btn-dark navigation-bottom-left">⬅️ Back
 </a>
 <a href='command:katapod.loadPage?[{"step":"step2"}]'
    class="btn btn-dark navigation-bottom-right">Next ➡️
  </a>
</div>
