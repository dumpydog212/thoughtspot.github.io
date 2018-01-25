<table cellpadding="4" cellspacing="0" frame="border" border="1" rules="all">
 <colgroup>
    <col style="width:25%" />
    <col style="width:25%" />
    <col style="width:50%" />
 </colgroup>
 <tr>
    <th>Service Task Name</th>
    <th>Key</th>
    <th>Description</th>
 </tr>
 <tr>
    <td><code>falcon.worker</code></td>
    <td><code>falcon_preserve_case</code></td>
    <td>Enables case configuration. The default is false.</td>
 </tr>
 <tr>
    <td><code>infaagent.infaagent</code></td>
    <td><code>agent_max_memory</code></td>
    <td>Sets the max memory for the Agent JVM for ThoughtSpot Data Connect. max_memory is the max memory allowed. 4g is the default value.</td>
 </tr>
 <tr>
    <td><code>infaagent.infaagent</code></td>
    <td><code>bypass_ssl</code></td>
    <td>Allows you to bypass SSL check during ThoughtSpot connection create for,ThoughtSpot Data Connect. It is set to false by default.</td>
 </tr>
 <tr>
    <td><code>infaagent.infaagent</code></td>
    <td><code>max_concurrent_loads</code></td>
    <td>Sets the max number of loads to run concurrently for ThoughtSpot Data,Connect. 4 is the default value.</td>
 </tr>
 <tr>
    <td><code>infaagent.infaagent</code></td>
    <td><code>max_memory</code></td>
    <td>Sets the max memory for the load task for ThoughtSpot Data Connect. 50g is the default.</td>
 </tr>
 <tr>
    <td><code>timely.timely</code></td>
    <td><code>max_scheduled_jobs</code></td>
    <td>Sets the max scheduled jobs (both pinboard and Data Connect) for a cluster. 50 is the default.</td>
 </tr>
</table>