## Section 7: Review Session Recordings and Command Audit

In this section, we will review the recordings and command audits for the sessions we performed in the previous exercises.

To perform the following exercises, we assigned all users the permissions to access the **Audit space** via the role **global auditors**.

::: pagebreak :::

### 7-1 Accessing the Audit space

1) Login to the Identity Portal if not already connected.

2) Click the **Waffle** button and select **Audit and Reports**.![](images/pam-137.png)

3) Navigate to the **Session Monitoring** section.![](images/pam-138.png)

<x-block class="alert alert-warning"><p>Note we can see the session recordings for all users of this lab here.</p></x-block>

4) In the filter section, type in your username (no need to include the suffix) and press enter: ^^%{metadata:User}^^![](images/pam-139.png)

5) Expand the **Filter** section and ensure only **SIA** is selected as a **Service**.![](images/pam-140.png)

<x-block class="alert alert-warning"><p>If you are using a small screen, close the filter section to make it easier to read.</p></x-block>

::: pagebreak :::

### 7-2 Monitoring Windows sessions

1) In the list, select one of the sessions made to the Windows VM.![](images/pam-141.png)

2) In the **Session details** tab, we can see the Target ID and the connection method (Vaulted or JIT).![](images/pam-142.png)

3) Click on the **Play Recording** button, then review the video recording.![](images/pam-143.png)

<x-block class="alert alert-warning"><p><strong>Note:</strong> If the <strong>Play</strong> <strong>Recording</strong> button isn't yet visible for your RDP sessions, you can access a recording from a prior session. Set the <em>Time range</em> to <strong>30 days</strong>, enter the <em>Session ID</em> ^^<strong>6ca37a57-81c8-468b-b3cf-fdad591ada88</strong>^^, press <strong>Enter</strong> and then <strong>click</strong> on the session to watch the recording.<img src="images/pam-144.png"></p></x-block>

4) Close the window to return to the list.

::: pagebreak :::

### 7-3 Monitoring Linux sessions

1) In the list, select the session to the Linux VM. Notice the risk score assigned due to the configured risky commands rule.![](images/pam-145.png)

2) In the **Session details** tab, we can see the Target ID and the connection method.![](images/pam-146.png)

3) Click on **Commands** to see the list of actions from the session and notice the command that generated the high risk score![](images/pam-147.png)

4) Next, click on **AI Summary,** then **Generate AI summary** to see an analysis of the session by **CORA AI**.![](images/pam-148.png)

5) After a few moments, a summary of the session activities will appear.![](images/pam-149.png)

6) Click on **Play recording**.![](images/pam-150.png)

7) Note that we can navigate the recording via the time bar at the bottom or search for a specific event on the left side.![](images/pam-151.png)

8) Close this view to return to the **Audit** space.

::: pagebreak :::

### 7-4 Monitoring Database sessions

1) Under the **Session monitoring** look for the first database session you connected to in the previous section.![](images/pam-152.png)

2) All the critical pieces of information are visible in **Session details**![](images/pam-153.png)

3) Click on **Commands** to see the commands run during the session.![](images/pam-154.png)

4) Close the window to return to the **Audit** space.

::: pagebreak :::

### 7-5 Monitoring AI Agent Activity

1) Under **Session Monitoring**, look for the latest listed database session, which should appear at the top. Click on it.![](images/pam-155.png)

2) Notice the agent_name for that session, the connection string used and the authentication method.![](images/pam-156.png)

3) Click on **Commands**![](images/pam-157.png)

4) Notice the SQL queries that Le Chat executed through the MCP Connector on behalf of the Identity user.![](images/pam-158.png)

::: pagebreak :::

**This concludes the training lab. Thank you for your participation!**

**The next section includes an optional exercise.**

::: pagebreak :::
