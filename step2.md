<!-- TOP -->
<div class="top">
  <img class="scenario-academy-logo" src="https://datastax-academy.github.io/katapod-shared-assets/images/ds-academy-2023.svg" />
  <div class="scenario-title-section">
    <span class="scenario-title">Start Apache Cassandra™</span>
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

<div class="step-title">Start Cassandra</div>




✅ Switch to the `apache-cassandra-4.1.0/bin` directory.
```
cd /workspace/ds201-lab01/apache-cassandra-4.1.0/bin
```

✅ View the `bin` directory:
```
ls -l
```

✅ Start Cassandra:
```
./cassandra
```

It may take a while for Cassandra to start. 

✅ Run `nodetool` to determine Cassandra's status (you may have to run this command multiple times until Cassandra starts):
```
./nodetool status
```

You should see the status *Up* and state *Normal* - *UN*.

<pre>
Status=Up/Down
|/ State=Normal/Leaving/Joining/Moving
--  Address    Load        Tokens  Owns (effective) ...
UN  127.0.0.1  104.34 KiB  16      100.0%           ...
</pre>

<!-- NAVIGATION -->
<div id="navigation-bottom" class="navigation-bottom">
 <a href='command:katapod.loadPage?[{"step":"step1"}]'
   class="btn btn-dark navigation-bottom-left">⬅️ Back
 </a>
</div>