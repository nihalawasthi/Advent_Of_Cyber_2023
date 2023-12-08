<h1>Scenario</h1>
<p>The backup tapes are corrupted. They can only be restored using a special program, which can only run in MS-DOS. 
Explore AntarctiCrafts’ legacy systems and restore the files! </p>

<h2>Requirements </h2>
<ul>
<li>Start the Machine</li>
<li>Connect with TryHackMe’s VPN or Start the Attackbox</li>
<li>After the Machine starts, Connect with the Remote Machine</li>
<li>If you are on Windows, use Remote Desktop Connection else use rdpclient</li>
</ul>

<h2>Day 5— Tasks Answers</h2>
1. How large (in bytes) is the AC2023.BAK file? <br>
Ans: 12,704<br>
2. What is the name of the backup program?<br>
Ans: BackupMaster3000 <br>
3. What should the correct bytes be in the backup’s file signature to restore the backup properly?<br>
Ans: 41 43 <br>
4. What is the flag after restoring the backup successfully? <br>
Ans: THM{0LD_5CH00L_C00L_d00D}
